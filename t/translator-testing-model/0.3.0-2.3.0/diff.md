# Comparing `tmp/translator_testing_model-0.3.0.tar.gz` & `tmp/translator_testing_model-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "translator_testing_model-0.3.0.tar", max compression
+gzip compressed data, was "translator_testing_model-2.3.0.tar", max compression
```

## Comparing `translator_testing_model-0.3.0.tar` & `translator_testing_model-2.3.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1080 2024-03-18 19:38:54.622938 translator_testing_model-0.3.0/LICENSE
--rw-r--r--   0        0        0     2191 2024-03-18 19:38:54.622938 translator_testing_model-0.3.0/README.md
--rw-r--r--   0        0        0    21407 2024-03-18 19:38:54.622938 translator_testing_model-0.3.0/project/excel/translator_testing_model.xlsx
--rw-r--r--   0        0        0     8777 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/project/graphql/translator_testing_model.graphql
--rw-r--r--   0        0        0     6223 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/project/jsonld/translator_testing_model.context.jsonld
--rw-r--r--   0        0        0   100554 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/project/jsonld/translator_testing_model.jsonld
--rw-r--r--   0        0        0    82474 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/project/jsonschema/translator_testing_model.schema.json
--rw-r--r--   0        0        0    83194 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/project/owl/translator_testing_model.owl.ttl
--rw-r--r--   0        0        0      228 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/project/prefixmap/translator_testing_model.yaml
--rw-r--r--   0        0        0    11468 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/project/protobuf/translator_testing_model.proto
--rw-r--r--   0        0        0    72116 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/project/shacl/translator_testing_model.shacl.ttl
--rw-r--r--   0        0        0    10041 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/project/shex/translator_testing_model.shex
--rw-r--r--   0        0        0    15252 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/project/sqlschema/translator_testing_model.sql
--rw-r--r--   0        0        0      992 2024-03-18 19:39:07.270959 translator_testing_model-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      709 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/src/data/examples/Bad-AcceptanceTestAsset-001.yaml
--rw-r--r--   0        0        0      496 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/src/data/examples/Bad-AcceptanceTestCase-001.yaml
--rw-r--r--   0        0        0      332 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/src/data/examples/Bad-TestAsset-001.yaml
--rw-r--r--   0        0        0      390 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/src/data/examples/Bad-TestAsset-002.yaml
--rw-r--r--   0        0        0      391 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/src/data/examples/Bad-TestAsset-003.yaml
--rw-r--r--   0        0        0      391 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/src/data/examples/Bad-TestAsset-004.yaml
--rw-r--r--   0        0        0      391 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/src/data/examples/Bad-TestAsset-005.yaml
--rw-r--r--   0        0        0      399 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/src/data/examples/Bad-TestAsset-006.yaml
--rw-r--r--   0        0        0     1405 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/src/data/examples/Bad-TestCase-001.yaml
--rw-r--r--   0        0        0      508 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/src/data/examples/Bad-TestCaseSpecification-001.yaml
--rw-r--r--   0        0        0      829 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/src/data/examples/Bad-TestEntity-001.yaml
--rw-r--r--   0        0        0      816 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/src/data/examples/Bad-TestEntity-002.yaml-uriorcurie_should_fail_but_does_not
--rw-r--r--   0        0        0      554 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/src/data/examples/Bad-TestMetadata-001.yaml
--rw-r--r--   0        0        0      636 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/src/data/examples/Bad-TestSuite-001.yaml
--rw-r--r--   0        0        0      959 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/src/data/examples/Good-AcceptanceTestAsset-001.yaml
--rw-r--r--   0        0        0      829 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/src/data/examples/Good-AcceptanceTestCase-001.yaml
--rw-r--r--   0        0        0      358 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/src/data/examples/Good-TestAsset-001.json
--rw-r--r--   0        0        0     1642 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/src/data/examples/Good-TestAsset-001.yaml
--rw-r--r--   0        0        0      585 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/src/data/examples/Good-TestCase-001.json
--rw-r--r--   0        0        0     1786 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/src/data/examples/Good-TestCase-001.yaml
--rw-r--r--   0        0        0      529 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/src/data/examples/Good-TestCaseSpecification-001.yaml
--rw-r--r--   0        0        0      782 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/src/data/examples/Good-TestEntity-Complete.yaml
--rw-r--r--   0        0        0      144 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/src/data/examples/Good-TestEntity-Missing_Description_OK.yaml
--rw-r--r--   0        0        0      133 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/src/data/examples/Good-TestEntity-Missing_Name_OK.yaml
--rw-r--r--   0        0        0      506 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/src/data/examples/Good-TestMetadata-001.yaml
--rw-r--r--   0        0        0      637 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/src/data/examples/Good-TestSuite-001.yaml
--rw-r--r--   0        0        0      828 2024-03-18 19:38:54.626937 translator_testing_model-0.3.0/src/data/examples/SampleTestAssetList.json
--rw-r--r--   0        0        0      243 2024-03-18 19:38:54.630937 translator_testing_model-0.3.0/src/translator_testing_model/README.md
--rw-r--r--   0        0        0     3313 2024-03-18 19:38:54.630937 translator_testing_model-0.3.0/src/translator_testing_model/adaptor/test_case_generator.py
--rw-r--r--   0        0        0     2299 2024-03-18 19:38:54.630937 translator_testing_model-0.3.0/src/translator_testing_model/adaptor/testrunner.py
--rw-r--r--   0        0        0      270 2024-03-18 19:38:54.630937 translator_testing_model-0.3.0/src/translator_testing_model/datamodel/README.md
--rw-r--r--   0        0        0    49677 2024-03-18 19:38:54.630937 translator_testing_model-0.3.0/src/translator_testing_model/datamodel/pydanticmodel.py
--rw-r--r--   0        0        0    49370 2024-03-18 19:38:54.630937 translator_testing_model-0.3.0/src/translator_testing_model/datamodel/pydanticmodel_v2.py
--rw-r--r--   0        0        0    72360 2024-03-18 19:38:54.630937 translator_testing_model-0.3.0/src/translator_testing_model/datamodel/translator_testing_model.py
--rw-r--r--   0        0        0      124 2024-03-18 19:38:54.630937 translator_testing_model-0.3.0/src/translator_testing_model/schema/README.md
--rw-r--r--   0        0        0    27665 2024-03-18 19:38:54.630937 translator_testing_model-0.3.0/src/translator_testing_model/schema/translator_testing_model.yaml
--rw-r--r--   0        0        0     3038 2024-03-18 19:38:54.630937 translator_testing_model-0.3.0/src/translator_testing_model/scripts/GitHub_issue_parser.py
--rw-r--r--   0        0        0    11983 2024-03-18 19:38:54.630937 translator_testing_model-0.3.0/src/translator_testing_model/scripts/generate_suite_for_demo.py
--rw-r--r--   0        0        0     3536 2024-03-18 19:38:54.630937 translator_testing_model-0.3.0/src/translator_testing_model/scripts/test_suite_generator.py
--rw-r--r--   0        0        0     2989 1970-01-01 00:00:00.000000 translator_testing_model-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-03-18 19:40:32.656137 translator_testing_model-2.3.0/LICENSE
+-rw-r--r--   0        0        0     2191 2024-03-18 19:40:32.656137 translator_testing_model-2.3.0/README.md
+-rw-r--r--   0        0        0    21223 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/project/excel/translator_testing_model.xlsx
+-rw-r--r--   0        0        0     8135 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/project/graphql/translator_testing_model.graphql
+-rw-r--r--   0        0        0     6223 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/project/jsonld/translator_testing_model.context.jsonld
+-rw-r--r--   0        0        0    99507 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/project/jsonld/translator_testing_model.jsonld
+-rw-r--r--   0        0        0    79264 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/project/jsonschema/translator_testing_model.schema.json
+-rw-r--r--   0        0        0    81158 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/project/owl/translator_testing_model.owl.ttl
+-rw-r--r--   0        0        0      228 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/project/prefixmap/translator_testing_model.yaml
+-rw-r--r--   0        0        0    10811 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/project/protobuf/translator_testing_model.proto
+-rw-r--r--   0        0        0    68537 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/project/shacl/translator_testing_model.shacl.ttl
+-rw-r--r--   0        0        0     9703 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/project/shex/translator_testing_model.shex
+-rw-r--r--   0        0        0    14640 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/project/sqlschema/translator_testing_model.sql
+-rw-r--r--   0        0        0      992 2024-03-18 19:40:56.772001 translator_testing_model-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0      709 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Bad-AcceptanceTestAsset-001.yaml
+-rw-r--r--   0        0        0      496 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Bad-AcceptanceTestCase-001.yaml
+-rw-r--r--   0        0        0      332 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Bad-TestAsset-001.yaml
+-rw-r--r--   0        0        0      390 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Bad-TestAsset-002.yaml
+-rw-r--r--   0        0        0      391 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Bad-TestAsset-003.yaml
+-rw-r--r--   0        0        0      391 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Bad-TestAsset-004.yaml
+-rw-r--r--   0        0        0      391 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Bad-TestAsset-005.yaml
+-rw-r--r--   0        0        0      399 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Bad-TestAsset-006.yaml
+-rw-r--r--   0        0        0     1405 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Bad-TestCase-001.yaml
+-rw-r--r--   0        0        0      508 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Bad-TestCaseSpecification-001.yaml
+-rw-r--r--   0        0        0      829 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Bad-TestEntity-001.yaml
+-rw-r--r--   0        0        0      816 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Bad-TestEntity-002.yaml-uriorcurie_should_fail_but_does_not
+-rw-r--r--   0        0        0      554 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Bad-TestMetadata-001.yaml
+-rw-r--r--   0        0        0      636 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Bad-TestSuite-001.yaml
+-rw-r--r--   0        0        0      959 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Good-AcceptanceTestAsset-001.yaml
+-rw-r--r--   0        0        0      829 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Good-AcceptanceTestCase-001.yaml
+-rw-r--r--   0        0        0      358 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Good-TestAsset-001.json
+-rw-r--r--   0        0        0     1642 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Good-TestAsset-001.yaml
+-rw-r--r--   0        0        0      585 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Good-TestCase-001.json
+-rw-r--r--   0        0        0     1786 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Good-TestCase-001.yaml
+-rw-r--r--   0        0        0      529 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Good-TestCaseSpecification-001.yaml
+-rw-r--r--   0        0        0      782 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Good-TestEntity-Complete.yaml
+-rw-r--r--   0        0        0      144 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Good-TestEntity-Missing_Description_OK.yaml
+-rw-r--r--   0        0        0      133 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Good-TestEntity-Missing_Name_OK.yaml
+-rw-r--r--   0        0        0      506 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Good-TestMetadata-001.yaml
+-rw-r--r--   0        0        0      637 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Good-TestSuite-001.yaml
+-rw-r--r--   0        0        0      828 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/SampleTestAssetList.json
+-rw-r--r--   0        0        0      243 2024-03-18 19:40:32.664137 translator_testing_model-2.3.0/src/translator_testing_model/README.md
+-rw-r--r--   0        0        0     3313 2024-03-18 19:40:32.664137 translator_testing_model-2.3.0/src/translator_testing_model/adaptor/test_case_generator.py
+-rw-r--r--   0        0        0     2299 2024-03-18 19:40:32.664137 translator_testing_model-2.3.0/src/translator_testing_model/adaptor/testrunner.py
+-rw-r--r--   0        0        0      270 2024-03-18 19:40:32.664137 translator_testing_model-2.3.0/src/translator_testing_model/datamodel/README.md
+-rw-r--r--   0        0        0    47412 2024-03-18 19:40:32.664137 translator_testing_model-2.3.0/src/translator_testing_model/datamodel/pydanticmodel.py
+-rw-r--r--   0        0        0    47105 2024-03-18 19:40:32.664137 translator_testing_model-2.3.0/src/translator_testing_model/datamodel/pydanticmodel_v2.py
+-rw-r--r--   0        0        0    70932 2024-03-18 19:40:32.664137 translator_testing_model-2.3.0/src/translator_testing_model/datamodel/translator_testing_model.py
+-rw-r--r--   0        0        0      124 2024-03-18 19:40:32.664137 translator_testing_model-2.3.0/src/translator_testing_model/schema/README.md
+-rw-r--r--   0        0        0    27461 2024-03-18 19:40:32.664137 translator_testing_model-2.3.0/src/translator_testing_model/schema/translator_testing_model.yaml
+-rw-r--r--   0        0        0     3038 2024-03-18 19:40:32.664137 translator_testing_model-2.3.0/src/translator_testing_model/scripts/GitHub_issue_parser.py
+-rw-r--r--   0        0        0    12807 2024-03-18 19:40:32.664137 translator_testing_model-2.3.0/src/translator_testing_model/scripts/generate_suite_for_demo.py
+-rw-r--r--   0        0        0     3536 2024-03-18 19:40:32.664137 translator_testing_model-2.3.0/src/translator_testing_model/scripts/test_suite_generator.py
+-rw-r--r--   0        0        0     2989 1970-01-01 00:00:00.000000 translator_testing_model-2.3.0/PKG-INFO
```

### Comparing `translator_testing_model-0.3.0/LICENSE` & `translator_testing_model-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `translator_testing_model-0.3.0/README.md` & `translator_testing_model-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `translator_testing_model-0.3.0/project/excel/translator_testing_model.xlsx` & `translator_testing_model-2.3.0/project/excel/translator_testing_model.xlsx`

 * *Files 14% similar despite different names*

```diff
@@ -1,1338 +1,1327 @@
-00000000: 504b 0304 1400 0000 0800 8b8a 6f58 465a  PK..........oXFZ
+00000000: 504b 0304 1400 0000 0800 5263 7258 465a  PK........RcrXFZ
 00000010: c10c 8200 0000 b100 0000 1000 0000 646f  ..............do
 00000020: 6350 726f 7073 2f61 7070 2e78 6d6c 4d8e  cProps/app.xmlM.
 00000030: 4d0b c230 1044 ff4a e9dd 6e55 f020 3120  M..0.D.J..nU. 1 
 00000040: d4a3 e0c9 7b48 3736 9064 4376 85fc 7c53  ....{H76.dCv..|S
 00000050: c18f db3c de30 8cba 15ca 58c4 2377 3586  ...<.0....X.#w5.
 00000060: c4a7 7e11 c947 00b6 0b46 c343 d3a9 1947  ..~..G...F.C...G
 00000070: 251a 6958 1e40 ce79 8b13 d967 c424 b01b  %.iX.@.y...g.$..
 00000080: c703 6015 4c33 ce9b fc1d ecb5 3ae7 1cbc  ..`.L3......:...
 00000090: 35e2 29e9 abb7 8598 9c74 976a 3128 f897  5.)......t.j1(..
 000000a0: 6bf3 8e85 d7bc 1fb6 6ff9 6105 bf93 fa05  k.......o.a.....
-000000b0: 504b 0304 1400 0000 0800 8b8a 6f58 5fea  PK..........oX_.
-000000c0: 0ffc ec00 0000 cb01 0000 1100 0000 646f  ..............do
+000000b0: 504b 0304 1400 0000 0800 5263 7258 6a72  PK........RcrXjr
+000000c0: 2c18 ed00 0000 cb01 0000 1100 0000 646f  ,.............do
 000000d0: 6350 726f 7073 2f63 6f72 652e 786d 6c95  cProps/core.xml.
-000000e0: 91c1 6ac3 300c 865f a5f8 9ec8 4946 0fc6  ..j.0.._....IF..
-000000f0: f5a5 63a7 0d06 2b6c ec66 6cb5 358b 6363  ..c...+l.fl.5.cc
-00000100: 6b24 7dfb 2559 9b76 6c97 812f d6ff e993  k$}.%Y.vl../....
-00000110: 8ca5 89c2 8484 cf29 444c e430 af06 df76  .......)DL.0...v
-00000120: 5998 b861 47a2 2800 b239 a2d7 b91c 896e  Y..aG.(..9.....n
-00000130: 0cf7 2179 4de3 351d 206a f3a1 0f08 35e7  ..!yM.5. j....5.
-00000140: 6bf0 48da 6ad2 3009 8bb8 18d9 5969 cda2  k.H.j.0.....Yi..
-00000150: 8c9f a99d 05d6 00b6 e8b1 a30c 5559 c195  ............UY..
-00000160: 254c 3eff d930 270b 3964 b750 7ddf 977d  %L>..0'.9d.P}..}
-00000170: 3373 e346 15bc 3d3d becc cb17 aecb a43b  3s.F..==.......;
-00000180: 834c 496b 8449 a829 2435 bd28 9e86 56c2  .LIk.I.)$5.(..V.
-00000190: 4d51 9e67 7f17 d0ae c609 824e 1137 ec92  MQ.g.......N.7..
-000001a0: bc36 dbfb dd03 5335 afef 0ade 14d5 7ac7  .6....S5......z.
-000001b0: b9a8 a7f3 3eb9 7ef4 5f85 3e58 b777 ff34  ....>.~._.>X.w.4
-000001c0: 3637 c68b 4049 f8f5 6fea 0b50 4b03 0414  67..@I..o..PK...
-000001d0: 0000 0008 008b 8a6f 5899 5c9c 2310 0600  .......oX.\.#...
-000001e0: 009c 2700 0013 0000 0078 6c2f 7468 656d  ..'......xl/them
-000001f0: 652f 7468 656d 6531 2e78 6d6c ed5a 5b73  e/theme1.xml.Z[s
-00000200: da38 147e efaf d078 67f6 6d0b c636 81b6  .8.~...xg.m..6..
-00000210: b413 7369 76db b499 84ed 4e1f 8511 588d  ..siv.....N...X.
-00000220: 6c79 6491 847f bf47 3610 cb96 0ded 924d  lyd....G6......M
-00000230: ba9b 3c04 2ce9 fbce 4547 e7e8 3879 f3ee  ..<.,...EG..8y..
-00000240: 2e62 e886 8894 f278 60d9 2fdb d6bb b72f  .b.....x`./..../
-00000250: dee0 5732 2411 4130 19a7 aff0 c00a a54c  ..W2$.A0.......L
-00000260: 5eb5 5a69 00c3 387d c913 12c3 dc82 8b08  ^.Zi..8}........
-00000270: 4b78 14cb d65c e05b 1a2f 23d6 eab4 dbdd  Kx...\.[./#.....
-00000280: 5684 696c a118 4764 607d 5e2c 6840 d054  V.il..Gd`}^,h@.T
-00000290: 515a 6f5f 20b4 e51f 33f8 15cb 548d 65a3  QZo_ ...3...T.e.
-000002a0: 0113 5741 26b9 88b4 f2f9 6cc5 fcda de3e  ..WA&.....l....>
-000002b0: 65cf e93a 1d32 816e 301b 5820 7fce 6fa7  e..:.2.n0.X ..o.
-000002c0: e44e 5a88 e154 c2c4 c06a 673f 566b c7d1  .NZ..T...jg?Vk..
-000002d0: d248 8082 c97d 9405 ba49 f6a3 d315 0832  .H...}...I.....2
-000002e0: 0d3b 3a9d 58ce 767c f6c4 ed9f 8cca da74  .;:.X.v|.......t
-000002f0: 346d 1ae0 e3f1 7838 b6cb d28b 701c 04e0  4m....x8....p...
-00000300: 51bb 9ec2 9df4 6cbf a441 09b4 a369 d064  Q.....l..A...i.d
-00000310: d8f6 daae 91a6 aa8d 534f d3f7 7ddf eb9b  ........SO..}...
-00000320: 689c 0a8d 5b4f d36b 77dd d38e 89c6 add0  h...[O.kw.......
-00000330: 780d bef1 4f87 c3ae 89c6 abd0 74eb 6926  x...O.......t.i&
-00000340: 27fd ae6b a4e9 1668 4246 e3eb 7a12 15b5  '..k...hBF..z...
-00000350: e540 d320 0058 7076 d6cc d203 965e 29fa  .@. .Xpv.....^).
-00000360: 7594 1ad9 1dbb dd41 5cf0 58ee 3989 11fe  u......A\.X.9...
-00000370: c6c5 04d6 69d2 1996 3446 729d 9005 0e00  ....i...4Fr.....
-00000380: 37c4 d14c 507c af41 b68a e0c2 92d2 5c90  7..LP|.A......\.
-00000390: d6cf 29b5 501a 089a c881 f547 8221 c5dc  ..).P......G.!..
-000003a0: affd f597 bbc9 a433 7a9d 7d3a ce6b 947f  .......3z.}:.k..
-000003b0: 69ab 01a7 edbb 9bcf 93fc 73e8 e49f a793  i.........s.....
-000003c0: d74d 42ce 70bc 2c09 f1fb 235b 6187 276e  .MB.p.,...#[a.'n
-000003d0: 3b13 723a 1c67 427c cff6 f691 a525 32cf  ;.r:.gB|.....%2.
-000003e0: eff9 0aeb 4e3c 671f 5696 b05d cfcf e49e  ....N<g.V..]....
-000003f0: 8c72 23bb ddf6 587d f64f 476e 23d7 a9c0  .r#...X}.OGn#...
-00000400: b322 d794 4624 459f c82d bae4 1138 b549  ."..F$E..-...8.I
-00000410: 0d32 133f 089d 8698 6a50 1c02 a409 3196  .2.?....jP....1.
-00000420: a186 f8b4 c6ac 11e0 137d b7be 08c8 df8d  .........}......
-00000430: 88f7 ab6f 9a3d 57a1 5849 da84 f810 461a  ...o.=W.XI....F.
-00000440: e29c 73e6 73d1 6cfb 07a5 46d1 f655 bcdc  ..s.s.l...F..U..
-00000450: a397 5815 0197 18df 34aa 352c c5d6 7895  ..X.....4.5,..x.
-00000460: c0f1 ad9c 3c1d 1312 cd94 0b06 4186 9724  ....<.......A..$
-00000470: 2612 a939 7e4d 4813 fe2b a5da fe9c d340  &..9~MH..+.....@
-00000480: f094 2f24 fa4a 918f 69b3 23a7 7426 cde8  ../$.J..i.#.t&..
-00000490: 331a c146 af1b 7587 68d2 3c7a fe05 f99c  3..F..u.h.<z....
-000004a0: 350a 1c91 1b1d 0267 1bb3 4621 8469 bbf0  5......g..F!.i..
-000004b0: 1eaf 248e 9aad c211 2b42 3e62 1936 1a72  ..$.....+B>b.6.r
-000004c0: b516 81b6 71a9 8460 5a12 c6d1 784e d2b4  ....q..`Z...xN..
-000004d0: 11fc 59ac 3593 3e60 c8ec cd91 75ce d691  ..Y.5.>`....u...
-000004e0: 0e11 925e 3742 3e62 ce8b 9011 bf1e 8638  ...^7B>b.......8
-000004f0: 4a9a eda2 7158 04fd 9e5e c349 c1e8 82cb  J...qX...^.I....
-00000500: 66fd b87e 86d5 336c 2c8e f747 d417 4ae4  f..~..3l,..G..J.
-00000510: 0f26 a73f e932 3407 a39a 5909 bd84 566a  .&.?.24...Y...Vj
-00000520: 9faa 8734 3ea8 1e32 0a05 f1b9 1e3e e57a  ...4>..2.....>.z
-00000530: 780a 3796 c6bc 50ae 827b 01ff d1da 37c2  x.7...P..{....7.
-00000540: abf8 82c0 397f 2e7d cfa5 efb9 f43d a1d2  ....9..}.....=..
-00000550: b737 237d 67c1 d38b 5bde 466e 5bc4 fbae  .7#}g...[.Fn[...
-00000560: 31da d734 2e28 6357 72cd c8c7 54af 9329  1..4.(cWr...T..)
-00000570: d839 9fc0 ecfd 683e 9ef1 edfa d924 84af  .9....h>.....$..
-00000580: 9a59 2d23 1690 4b81 b341 24b8 fc8b caf0  .Y-#..K..A$.....
-00000590: 2ac4 09e8 645b 2509 cb54 d365 378a 129e  *...d[%..T.e7...
-000005a0: 421b 6ee9 53f5 4a95 d7e5 afb9 28b8 3c5b  B.n.S.J.....(.<[
-000005b0: e4e9 afa1 743e 2ccf f93c 5fe7 b4cd 0b33  ....t>,..<_....3
-000005c0: 43b7 724b eab6 94be b526 384a f4b1 cc70  C.rK.....&8J...p
-000005d0: 4e1e cb0c 3b67 3c92 1db6 77a0 1d35 fbf6  N...;g<...w..5..
-000005e0: 5d76 e423 a530 5397 43b8 1a42 be03 6dba  ]v.#.0S.C..B..m.
-000005f0: 9ddc 3a38 9e98 91b9 0ad3 5290 6fc3 f9e9  ..:8......R.o...
-00000600: c578 1ae2 39d9 04b9 7d98 576d e7d8 d1d1  .x..9...}.Wm....
-00000610: fbe7 c151 b0a3 ef3c 961d c788 f2a2 21ee  ...Q...<......!.
-00000620: a186 98cf c343 8779 7b5f 9867 95c6 5034  .....C.y{_.g..P4
-00000630: 146d 6cac 242c 46b7 60b8 d7f1 2c14 e064  .ml.$,F.`...,..d
-00000640: 602d a007 83af 5102 f252 5560 315b c603  `-....Q..RU`1[..
-00000650: 2b90 a27c 4c8c 45e8 70e7 975c 5fe3 d192  +..|L.E.p..\_...
-00000660: e3db a665 b56e af29 7719 6d22 5239 c269  ...e.n.)w.m"R9.i
-00000670: 9813 67ab cade 65b1 c155 1dcf 555b f2b0  ..g...e..U..U[..
-00000680: be6a 3db4 154e cffe 59ad c89f 0c11 4e16  .j=..N..Y.....N.
-00000690: 0b12 4863 9417 a64a a2f3 1953 bee7 2b49  ..Hc...J...S..+I
-000006a0: c455 38bf 4533 b612 9718 bce3 e6c7 714e  .U8.E3........qN
-000006b0: 53b8 1276 b60f 0232 b9bb 39a9 7a65 3167  S..v...2..9.ze1g
-000006c0: a6f2 df2d 0c09 2c5b 8859 12e2 4d5d edd5  ...-..,[.Y..M]..
-000006d0: e79b 9cae 7a22 76fa 9777 c160 f2fd 70c9  ....z"v..w.`..p.
-000006e0: 470f e53b e75f f45d 43ae 7ef6 dde3 fa6e  G..;._.]C.~....n
-000006f0: 933b 484c 9c79 c511 0174 4502 2395 1c06  .;HL.y...tE.#...
-00000700: 1617 32e4 50ee 9290 0613 01cd 94c9 44f0  ..2.P.........D.
-00000710: 0282 64a6 1c80 98fa 0bbd f20c b929 15ce  ..d..........)..
-00000720: ad3e 397f 452c 8386 4e5e d225 1214 8ab0  .>9.E,..N^.%....
-00000730: 0c05 2117 72e3 efef 936a 778c d7fa 2c81  ..!.r....jw...,.
-00000740: 6d84 5432 64d5 17ca 4389 c13d 3372 43d8  m.T2d...C..=3rC.
-00000750: 5425 f3ae da26 0b85 dbe2 54cd bb1a be26  T%...&....T....&
-00000760: 604b c37a 6e9d 2d27 ffdb 5ed4 3db4 173d  `K.zn.-'..^.=..=
-00000770: 46f3 a399 e01e b387 739b 7ab8 c245 acff  F.......s.z..E..
-00000780: 58d6 1ef9 32df 3970 db3a de03 5ee6 132c  X...2.9p.:..^..,
-00000790: 43a4 7ec1 7d8a 8a80 11ab 62be baaf 4ff9  C.~.}.....b...O.
-000007a0: 259c 3bb4 7bf1 8120 9bfc d6db a4f6 dde0  %.;.{.. ........
-000007b0: 0c7c d4ab 5aa5 642b 113f 4b07 7c1f 9206  .|..Z.d+.?K.|...
-000007c0: 638c 5bf4 345f 8f14 62ad a6b1 adc6 da31  c.[.4_..b......1
-000007d0: 0c79 8058 f30c a166 38df 8745 9a1a 33d5  .y.X...f8..E..3.
-000007e0: 8bac 398d 0a6f 41d5 40e5 3fdb d40d 68f6  ..9..oA.@.?...h.
-000007f0: 0d34 1c91 055e 3199 b636 a3e4 4e0a 3cdc  .4...^1..6..N.<.
-00000800: feef 0db0 c2c4 8ee1 ed8b bf01 504b 0304  ............PK..
-00000810: 1400 0000 0800 8b8a 6f58 0f95 4d33 4801  ........oX..M3H.
-00000820: 0000 4902 0000 1800 0000 786c 2f77 6f72  ..I.......xl/wor
-00000830: 6b73 6865 6574 732f 7368 6565 7431 2e78  ksheets/sheet1.x
-00000840: 6d6c 7552 db4e c330 0cfd 952a 1fb0 7448  mluR.N.0...*..tH
-00000850: 5c34 b595 d810 8207 a469 13f0 9cb5 6e1b  \4.......i....n.
-00000860: 2d89 4be2 aef0 f738 ed6e 3cf0 14fb c4e7  -.K....8.n<.....
-00000870: f8d8 4936 a0df 8716 8092 6f6b 5cc8 454b  ..I6......ok\.EK
-00000880: d42d a40c 650b 5685 1976 e0f8 a646 6f15  .-..e.V..v...Fo.
-00000890: 71ea 1b19 3a0f aa1a 49d6 c89b 34bd 9356  q...:...I...4..V
-000008a0: 6927 8a6c c4d6 bec8 b027 a31d ac7d 127a  i'.l.....'...}.z
-000008b0: 6b95 ff59 82c1 2117 7371 0236 ba69 6904  k..Y..!.sq.6.ii.
-000008c0: 6491 75aa 812d d07b c704 4ee5 59a7 d216  d.u..-.{..N.Y...
-000008d0: 5cd0 e812 0f75 2e1e e78b e5c4 182b 3e34  \....u.......+>4
-000008e0: 0ce1 2a4e e230 3bc4 7d4c 5eab 5ca4 d113  ..*N.0;.}L^.\...
-000008f0: 1828 294a 283e 0eb0 0263 a212 3bf9 3a8a  .()J(>...c..;.:.
-00000900: 8a4b d3c8 bc8e 4ff2 cfe3 fc6c 6fa7 02ac  .K....O....lo...
-00000910: d07c ea8a da5c 3c88 a482 5af5 8636 38bc  .|...\<...Z..68.
-00000920: c071 a6db 8bc5 2745 aac8 3c0e 898f c316  .q....'E..<.....
-00000930: 5919 83d8 920b b58b 4bda 9267 5c73 272a  Y.......K..g\s'*
-00000940: 3ae5 9505 029f 4962 1b11 94e5 91b4 fc8f  :.....Ib........
-00000950: 7450 a687 bf04 c91d 4f63 4c16 e28a df94  tP......OcL.....
-00000960: 6fb4 0b89 819a 85d2 d93d 1bf5 93e7 2921  o........=....)!
-00000970: ecc6 27d9 2111 da31 6cf9 a9c1 c702 beaf  ..'.!..1l.......
-00000980: 11e9 9cc4 9d9d 7f4f f10b 504b 0304 1400  .......O..PK....
-00000990: 0000 0800 8b8a 6f58 0f95 4d33 4801 0000  ......oX..M3H...
-000009a0: 4902 0000 1800 0000 786c 2f77 6f72 6b73  I.......xl/works
-000009b0: 6865 6574 732f 7368 6565 7432 2e78 6d6c  heets/sheet2.xml
-000009c0: 7552 db4e c330 0cfd 952a 1fb0 7448 5c34  uR.N.0...*..tH\4
-000009d0: b595 d810 8207 a469 13f0 9cb5 6e1b 2d89  .......i....n.-.
-000009e0: 4be2 aef0 f738 ed6e 3cf0 14fb c4e7 f8d8  K....8.n<.......
-000009f0: 4936 a0df 8716 8092 6f6b 5cc8 454b d42d  I6......ok\.EK.-
-00000a00: a40c 650b 5685 1976 e0f8 a646 6f15 71ea  ..e.V..v...Fo.q.
-00000a10: 1b19 3a0f aa1a 49d6 c89b 34bd 9356 6927  ..:...I...4..Vi'
-00000a20: 8a6c c4d6 bec8 b027 a31d ac7d 127a 6b95  .l.....'...}.zk.
-00000a30: ff59 82c1 2117 7371 0236 ba69 6904 6491  .Y..!.sq.6.ii.d.
-00000a40: 75aa 812d d07b c704 4ee5 59a7 d216 5cd0  u..-.{..N.Y...\.
-00000a50: e812 0f75 2e1e e78b e5c4 182b 3e34 0ce1  ...u.......+>4..
-00000a60: 2a4e e230 3bc4 7d4c 5eab 5ca4 d113 1828  *N.0;.}L^.\....(
-00000a70: 294a 283e 0eb0 0263 a212 3bf9 3a8a 8a4b  )J(>...c..;.:..K
-00000a80: d3c8 bc8e 4ff2 cfe3 fc6c 6fa7 02ac d07c  ....O....lo....|
-00000a90: ea8a da5c 3c88 a482 5af5 8636 38bc c071  ...\<...Z..68..q
-00000aa0: a6db 8bc5 2745 aac8 3c0e 898f c316 5919  ....'E..<.....Y.
-00000ab0: 83d8 920b b58b 4bda 9267 5c73 272a 3ae5  ......K..g\s'*:.
-00000ac0: 9505 029f 4962 1b11 94e5 91b4 fc8f 7450  ....Ib........tP
-00000ad0: a687 bf04 c91d 4f63 4c16 e28a df94 6fb4  ......OcL.....o.
-00000ae0: 0b89 819a 85d2 d93d 1bf5 93e7 2921 ecc6  .......=....)!..
-00000af0: 27d9 2111 da31 6cf9 a9c1 c702 beaf 11e9  '.!..1l.........
-00000b00: 9cc4 9d9d 7f4f f10b 504b 0304 1400 0000  .....O..PK......
-00000b10: 0800 8b8a 6f58 b111 5547 4002 0000 7805  ....oX..UG@...x.
-00000b20: 0000 1800 0000 786c 2f77 6f72 6b73 6865  ......xl/workshe
-00000b30: 6574 732f 7368 6565 7433 2e78 6d6c bd54  ets/sheet3.xml.T
-00000b40: db6e db30 0cfd 15c3 cf41 9d04 eb05 8163  .n.0.....A.....c
-00000b50: 2097 a629 b000 5d93 768f 0363 33b1 1659   ..)..].v..c3..Y
-00000b60: f424 ba5e ff7e 949d a617 2479 dc8b 2d1e  .$.^.~....$y..-.
-00000b70: f150 3c12 c9b8 26bb 7339 2207 7f0b 6ddc  .P<...&.s9"...m.
-00000b80: 30cc 99cb 4114 b934 c702 dc05 9568 6467  0...A..4.....hdg
-00000b90: 43b6 0016 d36e 2357 5a84 ac21 153a ea77  C....n#WZ..!.:.w
-00000ba0: bb57 5101 ca84 49dc 600f 3689 a962 ad0c  .WQ...I.`.6..b..
-00000bb0: 3ed8 c055 4501 f675 8c9a ea61 d80b df80  >..UE..u...a....
-00000bc0: 47b5 cdb9 01a2 242e 618b 4be4 a752 0862  G.....$.a.K..R.b
-00000bd0: 4687 3899 2ad0 3845 26b0 b819 86a3 de60  F.8.*.8E&......`
-00000be0: de32 1a8f 6785 b5fb b00e bc98 35d1 ce1b  .2..g.......5...
-00000bf0: f7d9 30ec fa9c 5063 ca3e 04c8 ef05 27a8  ..0...Pc.>....'.
-00000c00: b58f 2499 fcd9 070d df0f f5cc 8feb b7f0  ..$.............
-00000c10: b346 bfa4 b706 8713 d23f 55c6 f930 bc09  .F.......?U..0..
-00000c20: 830c 3750 697e a47a 8e7b 4d97 ef29 4e81  ..7Pi~.z.{M..)N.
-00000c30: 2189 2dd5 81f5 6293 38f5 0b7f a438 2ae3  !.-...b.8....8*.
-00000c40: 2f69 c956 7025 2771 c2e8 f897 a3ca a618  /i.Vp%'q........
-00000c50: 472c 8978 384a f7b4 f159 9a88 418b e628  G,.x8J...Y..A..(
-00000c60: 7372 9649 ebdf d8dc cd11 e6f4 2c13 8c21  sr.I........,..!
-00000c70: 067f bbee 08f7 f614 5765 47bc 67a7 bc0d  ........WeG.g...
-00000c80: 14c7 32bb 3be5 9fa1 4bad 2a7d 5647 68f3  ..2.;...K.*}VGh.
-00000c90: 9382 60fb 4544 24ef f656 0ced 4366 f27d  ..`.ED$..V..Cf.}
-00000ca0: 06ad b256 7390 5265 2458 3ffc ba75 28ae  ...Vs.Re$X?..u(.
-00000cb0: fe60 d4eb 7ebb b9bc be92 82cb a99e 5a2a  .`..~.........Z*
-00000cc0: a754 1b5f 9c0d 706f ca8a 17e8 9cf4 c001  .T._..po........
-00000cd0: bcb5 96ec 4710 b4f4 cf58 83d9 353d c3af  ....G....X..5=..
-00000ce0: a5e0 5a39 9693 7d6f 561a 7a49 b85c dc76  ..Z9..}oV.zI.\.v
-00000cf0: 968b a7c7 59e7 4ef1 bc5a 3f39 b433 c46c  ....Y.N..Z?9.3.l
-00000d00: 0de9 aeb3 1a4d 569d b114 48be 002b a605  .....MV...H..+..
-00000d10: e334 30d9 1542 d159 c973 7a8d df29 6d04  .40..B.Y.sz..)m.
-00000d20: 8471 7488 1b47 9fc5 9d12 3be9 0f26 ff4f  .qt..G....;..&.O
-00000d30: ec28 4db1 6490 82f7 b9b7 ca64 b2ec 1aeb  .(M.d......d....
-00000d40: 4705 8695 2fcd 9766 fbbc 9c2f 806b 2792  G.../..f.../.k'.
-00000d50: 5cd3 56c9 236b dcc8 1b77 2fae a5af 6ddb  \.V.#k...w/...m.
-00000d60: e2ad c154 3609 ae89 998a 6699 cb64 44eb  ...T6.....f..dD.
-00000d70: 1d64 7f43 c407 c38f 98c3 b04d fe01 504b  .d.C.......M..PK
-00000d80: 0304 1400 0000 0800 8b8a 6f58 e7b3 5928  ..........oX..Y(
-00000d90: fe02 0000 f009 0000 1800 0000 786c 2f77  ............xl/w
-00000da0: 6f72 6b73 6865 6574 732f 7368 6565 7434  orksheets/sheet4
-00000db0: 2e78 6d6c bd56 db72 da30 10fd 158f 9f99  .xml.V.r.0......
-00000dc0: 1898 e632 8cf1 0c09 4993 26a4 34d7 b62f  ...2....I.&.4../
-00000dd0: 1e61 2fa0 224b 8eb4 8e93 bfef ca04 9266  .a/."K.........f
-00000de0: 24e0 a94f 96d6 3a67 2f5a ed6e 5c2b bd30  $..O..:g/Z.n\+.0
-00000df0: 7300 0c5e 0a21 4d3f 9c23 96bd 2832 d91c  s..^.!M?.#..(2..
-00000e00: 0a66 f654 0992 fe4c 952e 18d2 56cf 2253  .f.T...L....V."S
-00000e10: 6a60 7903 2a44 d46d b70f a282 7119 2671  j`y.*D.m....q.&q
-00000e20: 231b eb24 5615 0a2e 61ac 0353 1505 d3af  #..$V...a..S....
-00000e30: c720 54dd 0f3b e14a 70c3 6773 6c04 5112  . T..;.Jp.gsl.Q.
-00000e40: 976c 06b7 80f7 2501 681b ad79 725e 8034  .l....%.h..yr^.4
-00000e50: 5cc9 40c3 b41f 0e3a bdc1 6009 698e 3c70  \.@....:..`.i.<p
-00000e60: a8cd 8775 60bd 9928 b5b0 9b8b bc1f b6ad  ...u`..(........
-00000e70: 5120 2043 cbc1 e8f3 0c27 2084 a522 539e  Q  C.....' .."S.
-00000e80: de58 c377 ad16 f971 bda2 3f6b 0240 f64d  .X.w...q..?k.@.M
-00000e90: 9881 1325 1e79 8ef3 7e78 1406 394c 5925  ...%.y..~x..9LY%
-00000ea0: f046 d5e7 f0e6 d4fe bb89 4386 2c89 b5aa  .F........C.,...
-00000eb0: 036d bd4d e2cc 2eac 4a3a c8a5 8dd2 2d6a  .m.M....J:....-j
-00000ec0: 9273 d284 0997 6585 29cf e308 c90a 2b8b  .s....e.).....+.
-00000ed0: b237 ccf1 668c 6405 3850 279b 5119 4398  .7..f.d.8P'.Q.C.
-00000ee0: 29fd ea40 0e7d 48ba fe9c 5ba0 dbce d3ed  )..@.}H...[.....
-00000ef0: 388f ad67 3e24 a593 372c 5fb7 803c bace  8..g>$..7,_..<..
-00000f00: b7c0 3604 e6c2 0765 c6a8 8c33 9b6b 0ed8  ..6....e...3.k..
-00000f10: 371f eca9 6282 4f39 68e3 405d fa50 f052  7...b.O9h.@].P.R
-00000f20: 525a 439e 2e0d 7640 af7c 5004 43c1 34a6  RZC...v@.|P.C.4.
-00000f30: 7205 66e4 4319 aa07 1279 961a 7806 cdd1  r.f.C....y..x...
-00000f40: 159a 6b7f b6a5 cf1d 07e0 bb0f 50d3 2b4d  ..k.........P.+M
-00000f50: 1752 d5ae 508e 377a 468f 1a34 c8cc e5dd  .R..P.7zF..4....
-00000f60: 0f1f 5257 5282 26df 10b9 9cb9 6ee2 66a3  ..RWR.&.....n.f.
-00000f70: d202 90e5 f4d6 1dc0 5b1f 70c2 1589 16e9  ........[.p.....
-00000f80: 2a01 f274 fd44 1c34 77db 684c 35f9 4329  *..t.D.4w.hL5.C)
-00000f90: 9132 6333 63cd aa1d 5cf7 bb72 e55c 2f8b  .2c3c...\..r.\/.
-00000fa0: e746 ba87 6d74 6a67 cb1e 77a4 dacd b09f  .F..mtjg..w.....
-00000fb0: de7c 7495 925f bed3 9e1a f2db 773e 0793  .|t.._......w>..
-00000fc0: 695e 7a0a c1c0 5bfd 917d cebc 883a c7aa  i^z...[..}...:..
-00000fd0: 1d2d 5b89 4db2 07f2 386f ea8c 0932 5549  .-[.M...8o...2UI
-00000fe0: 22eb 869f 7fad dadb 55b7 77d5 697f 39da  ".......U.w.i.9.
-00000ff0: 3f3c a096 3757 f550 ab72 480f cbb6 c746  ?<..7W.P.rH....F
-00001000: 7061 5bc1 088c a136 bc16 9e6a adf4 4721  pa[....6...j..G!
-00001010: 13d4 c28f 0593 8ba6 6de3 6b49 72c1 0d92  ........m.kIr...
-00001020: 663b 1e54 8275 9230 6395 0113 4885 01d2  f;.T.u.0c...H...
-00001030: 9880 a675 37ba 1cb7 56e5 3440 a582 19d0  ...u7...V.4@....
-00001040: 53e3 592b 5312 354d 0e4d ca5b 675a 76e8  S.Y+S.5M.M.[gZv.
-00001050: a08d 08b4 1260 5aef 852a 8ca3 b58e 38fa  .....`Z..*....8.
-00001060: d751 9fe3 a36e 6ff4 ff1c 3fa7 dedf ba52  .Q...no...?....R
-00001070: 75eb 5ae1 a02c 05b9 3111 5bec fe24 30cb  u.Z..,..1.[..$0.
-00001080: 4968 c4f4 8cd3 cd0a 98d2 c5b6 f70e 699c  Ih............i.
-00001090: d0cb c962 b941 5536 964c 14a2 2a9a e59c  ...b.AU6.L..*...
-000010a0: 2632 d0f6 00fd 9f2a 85eb 8d9d 6cd6 435e  &2.....*....l.C^
-000010b0: f217 504b 0304 1400 0000 0800 8b8a 6f58  ..PK..........oX
-000010c0: 2511 6947 cd03 0000 0c0f 0000 1800 0000  %.iG............
-000010d0: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
-000010e0: 6565 7435 2e78 6d6c bd57 5d73 da3a 10fd  eet5.xml.W]s.:..
-000010f0: 2b1e 3f7b 6a60 6ed3 0e03 cc40 9226 344d  +.?{j`n....@.&4M
-00001100: 6f6e d292 dbbe 7884 b580 8a2c b95a 1927  on....x....,.Z.'
-00001110: fffe aecc 4772 1909 3a79 e009 69c5 591d  ....Gr..:y..i.Y.
-00001120: ad57 6757 bd5a 9b25 2e00 6cf4 5448 85fd  .WgW.Z.%..l.TH..
-00001130: 7861 6dd9 4d53 cc17 5030 7ca7 4b50 b432  xam.MS..P0|.KP.2
-00001140: d3a6 6096 a666 9e62 6980 f106 54c8 b4d3  ..`..f.bi...T...
-00001150: 6a9d a505 132a 1ef4 1adb 9d19 f474 65a5  j....*.......te.
-00001160: 5070 6722 ac8a 8299 e711 485d f7e3 76bc  Ppg"......H]..v.
-00001170: 35dc 8bf9 c236 8674 d02b d91c 1ec0 7e2f  5....6.t.+....~/
-00001180: 0940 d374 e787 8b02 140a ad22 03b3 7e3c  .@.t......."..~<
-00001190: 6c77 8737 6b48 f397 8980 1a5f 8d23 779a  lw.7kH....._.#w.
-000011a0: a9d6 4b37 19f3 7edc 72a4 4042 6e9d 0f46  ..K7..~.r.@Bn..F
-000011b0: 3f2b 3807 299d 2ba2 f27b e335 7ed9 d521  ?+8.).+..{.5~..!
-000011c0: 5f8f b7ee 3f35 0120 7e53 8670 aee5 a3e0  _...?5. ~S.p....
-000011d0: 76d1 8f3f c611 8719 aba4 bdd7 f535 6c0e  v..?.........5l.
-000011e0: f5fe 85e2 05b3 6cd0 33ba 8e8c 3bed a097  ......l.3...;...
-000011f0: bb81 db92 fe28 948b d283 3564 17b4 931d  .....(....5d....
-00001200: 1415 daac 6488 1967 167a a925 2e6e 25cd  ....d..g.z.%.n%.
-00001210: 37c8 d171 24a8 9530 5a51 e4ac c7c1 79c8  7..q$..0ZQ....y.
-00001220: 01e6 8210 6226 f2ec 7705 e822 e681 5f04  ....b&..w..".._.
-00001230: e1d6 0835 a7cd ad79 f6e0 2e43 382e ccfa  ...5...y...C8...
-00001240: f378 409f 4220 a6b0 0693 09d5 e4a5 cc72  .x@.B .........r
-00001250: ad72 287d c7bd 0ab9 80a7 92f6 059e 1940  .r(}...........@
-00001260: fa7c 1ee8 7508 6a75 9949 5881 f480 c621  .|..u.ju.IX....!
-00001270: 10c5 d43c 674a 73df 57fd 1c42 296d 013d  ...<gJs.W..B)m.=
-00001280: 809b 1040 a8b2 b299 e01e cc97 c318 c50a  ...@............
-00001290: 1fb5 dbc3 a89c d274 aebd 9ffc 6b08 49fa  .......t....k.I.
-000012a0: c185 03fa 79fe 7d1c 17e0 7a17 4292 1e05  ....y.}...z.B...
-000012b0: c3f2 cf11 5060 affb 23b0 0381 7908 a635  ....P`..#...y..5
-000012c0: a2ce 050b dc86 6fe1 d462 92ee 2d18 5fa6  ......o..b..-._.
-000012d0: 7c3f 7a01 d684 3dd0 49f0 0290 3c64 02b1  |?z...=.I...<d..
-000012e0: f205 e631 a810 5450 4860 f20c e9ee 1861  ...1..TPH`.....a
-000012f0: 7da1 f937 9c6d d9aa ed01 fc08 016a 92f9  }..7.m.......j..
-00001300: 6ca9 74ed 0be5 cf83 27a3 aa00 0648 513c  l.t.....'....HQ<
-00001310: c861 50ba 4da5 1469 1282 b524 84be 4f31  .aP.M..i...$..O1
-00001320: 0c8a 77b3 6d01 9691 ea33 1f32 a8da 53a1  ..w.m....3.2..S.
-00001330: c9b4 ccb6 39c0 b3dd 2df1 f909 caf7 d60f  ....9...-.......
-00001340: 56d3 5f94 1619 4397 1d3b b7c6 e72c a8e9  V._...C..;...,..
-00001350: fbce 761a 7fd8 5f50 eeb7 fef4 9f73 0bea  ..v..._P.....s..
-00001360: fe9e af3f a416 ac05 5e49 1906 ab40 404c  ...?....^I...@@L
-00001370: 86c1 02c0 0173 23ca 8024 0c83 75c0 b2fd  .....s#..$..u...
-00001380: 144c a909 d976 36eb aec4 25db 840e cd1b  .L...v6...%.....
-00001390: c5c1 28d7 9522 6767 f1fe d2b6 531a 75ba  ..(.."gg....S.u.
-000013a0: a376 ebaf 8fef 3f9c 51f7 b4d0 f585 d1e5  .v....?.Q.......
-000013b0: 055d 31d7 6935 86b1 2b0a b780 481d ddce  .]1.i5..+...H...
-000013c0: 7869 8c36 af8d 4c52 3738 924c 2d9b 0ed0  xi.6..LR78.L-...
-000013d0: 3e97 6497 022d edec 2a7a 2559 7b10 7358  >.d..-..*z%Y{.sX
-000013e0: 25b9 48dc dd48 4aa3 79dc 4b77 8bbd f4ff  %.H..HJ.y.Kw....
-000013f0: 0c43 8c2f 3bdd cbd3 3116 2aa7 d618 8127  .C./;...1.*....'
-00001400: 1c36 a3b7 90be ea74 af4e 4a5a 561c b2b9  .6.....t.NJZV...
-00001410: d63c 81a7 f564 cade c47c dce9 8e4f c77c  .<...d...|...O.|
-00001420: 232f c9fa 2abf 85ef a4d3 9d9c 8e6f ce2a  #/..*........o.*
-00001430: 048c a8a7 8b2c 6587 c5e4 dbed cd5d b2ed  .....,e......]..
-00001440: 1422 ab75 3407 2a22 224f a8a3 b586 5e55  .".u4.*""O....^U
-00001450: 8d94 bbdb 99b8 0719 4d64 64b4 044c 5e6a  ........Mdd..L^j
-00001460: f05b 0efe d8e9 3e9e eee0 d7f4 2e4a bee8  .[....>......J..
-00001470: 3af9 aaed b02c 251d 632a 8ff0 de33 e0fa  :....,%.c*...3..
-00001480: 9578 cbcc 5c90 5449 9891 52b5 de7d a0a7  .x..\.TI..R..}..
-00001490: 9659 bfba d613 eacd 1b26 536d ad2e 9ae1  .Y.......&Sm....
-000014a0: 825e ab60 dc1f 687d a6a9 a3de 4edc ab6f  .^.`..h}....N..o
-000014b0: f700 1efc 0750 4b03 0414 0000 0008 008b  .....PK.........
-000014c0: 8a6f 58e7 b359 28fe 0200 00f0 0900 0018  .oX..Y(.........
-000014d0: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
-000014e0: 2f73 6865 6574 362e 786d 6cbd 56db 72da  /sheet6.xml.V.r.
-000014f0: 3010 fd15 8f9f 9918 98e6 328c f10c 0949  0.........2....I
-00001500: 9326 a434 d7b6 2f1e 612f a022 4b8e b48e  .&.4../.a/."K...
-00001510: 93bf efca 0492 6624 e0a9 4f96 d63a 672f  ......f$..O..:g/
-00001520: 5aed 6e5c 2bbd 3073 000c 5e0a 214d 3f9c  Z.n\+.0s..^.!M?.
-00001530: 2396 bd28 32d9 1c0a 66f6 5409 92fe 4c95  #..(2...f.T...L.
-00001540: 2e18 d256 cf22 536a 6079 032a 44d4 6db7  ...V."Sj`y.*D.m.
-00001550: 0fa2 8271 1926 7123 1beb 2456 150a 2e61  ...q.&q#..$V...a
-00001560: ac03 5315 05d3 afc7 2054 dd0f 3be1 4a70  ..S..... T..;.Jp
-00001570: c367 736c 0451 1297 6c06 b780 f725 0168  .gsl.Q..l....%.h
-00001580: 1bad 7972 5e80 345c c940 c3b4 1f0e 3abd  ..yr^.4\.@....:.
-00001590: c160 0969 8e3c 70a8 cd87 7560 bd99 28b5  .`.i.<p...u`..(.
-000015a0: b09b 8bbc 1fb6 ad51 2020 43cb c1e8 f30c  .......Q  C.....
-000015b0: 2720 84a5 2253 9ede 58c3 77ad 16f9 71bd  ' .."S..X.w...q.
-000015c0: a23f 6b02 40f6 4d98 8113 251e 798e f37e  .?k.@.M...%.y..~
-000015d0: 7814 0639 4c59 25f0 46d5 e7f0 e6d4 febb  x..9LY%.F.......
-000015e0: 8943 862c 89b5 aa03 6dbd 4de2 cc2e ac4a  .C.,....m.M....J
-000015f0: 3ac8 a58d d22d 6a92 73d2 8409 9765 8529  :....-j.s....e.)
-00001600: cfe3 08c9 0a2b 8bb2 37cc f166 8c64 0538  .....+..7..f.d.8
-00001610: 5027 9b51 1943 9829 fdea 400e 7d48 bafe  P'.Q.C.)..@.}H..
-00001620: 9c5b a0db ced3 ed38 8fad 673e 24a5 9337  .[.....8..g>$..7
-00001630: 2c5f b780 3cba ceb7 c036 04e6 c207 65c6  ,_..<....6....e.
-00001640: a88c 339b 6b0e d837 1fec a962 824f 3968  ..3.k..7...b.O9h
-00001650: e340 5dfa 50f0 5252 5a43 9e2e 0d76 40af  .@].P.RRZC...v@.
-00001660: 7c50 0443 c134 a672 0566 e443 19aa 0712  |P.C.4.r.f.C....
-00001670: 7996 1a78 06cd d115 9a6b 7fb6 a5cf 1d07  y..x.....k......
-00001680: e0bb 0f50 d32b 4d17 52d5 ae50 8e37 7a46  ...P.+M.R..P.7zF
-00001690: 8f1a 34c8 cce5 dd0f 1f52 5752 8226 df10  ..4......RWR.&..
-000016a0: b99c b96e e266 a3d2 0290 e5f4 d61d c05b  ...n.f.........[
-000016b0: 1f70 c215 8916 e92a 01f2 74fd 441c 3477  .p.....*..t.D.4w
-000016c0: db68 4c35 f943 2991 3263 3363 cdaa 1d5c  .hL5.C).2c3c...\
-000016d0: f7bb 72e5 5c2f 8be7 46ba 876d 746a 67cb  ..r.\/..F..mtjg.
-000016e0: 1e77 a4da cdb0 9fde 7c74 9592 5fbe d39e  .w......|t.._...
-000016f0: 1af2 db77 3e07 9369 5e7a 0ac1 c05b fd91  ...w>..i^z...[..
-00001700: 7dce bc88 3ac7 aa1d 2d5b 894d b207 f238  }...:...-[.M...8
-00001710: 6fea 8c09 3255 4922 eb86 9f7f adda db55  o...2UI".......U
-00001720: b777 d569 7f39 da3f 3ca0 9637 57f5 50ab  .w.i.9.?<..7W.P.
-00001730: 7248 0fcb b6c7 4670 615b c108 8ca1 36bc  rH....Fpa[....6.
-00001740: 169e 6aad f447 2113 d4c2 8f05 938b a66d  ..j..G!........m
-00001750: e36b 4972 c10d 9266 3b1e 5482 7592 3063  .kIr...f;.T.u.0c
-00001760: 9501 1348 8501 d298 80a6 7537 ba1c b756  ...H......u7...V
-00001770: e534 40a5 8219 d053 e359 2b53 1235 4d0e  .4@....S.Y+S.5M.
-00001780: 4dca 5b67 5a76 e8a0 8d08 b412 605a ef85  M.[gZv......`Z..
-00001790: 2a8c a3b5 8e38 fad7 519f e3a3 6e6f f4ff  *....8..Q...no..
-000017a0: 1c3f a7de dfba 5275 eb5a e1a0 2c05 b931  .?....Ru.Z..,..1
-000017b0: 115b ecfe 2430 cb49 68c4 f48c d3cd 0a98  .[..$0.Ih.......
-000017c0: d2c5 b6f7 0e69 9cd0 cbc9 62b9 4155 3696  .....i....b.AU6.
-000017d0: 4c14 a22a 9ae5 9c26 32d0 f600 fd9f 2a85  L..*...&2.....*.
-000017e0: eb8d 9d6c d643 5ef2 1750 4b03 0414 0000  ...l.C^..PK.....
-000017f0: 0008 008b 8a6f 5864 2f60 5f58 0100 00a8  .....oXd/`_X....
-00001800: 0200 0018 0000 0078 6c2f 776f 726b 7368  .......xl/worksh
-00001810: 6565 7473 2f73 6865 6574 372e 786d 6c75  eets/sheet7.xmlu
-00001820: 52db 4ec3 300c fd95 2a1f b074 485c 34b5  R.N.0...*..tH\4.
-00001830: 95d8 2604 0f48 d326 e039 6bdd 365a 1297  ..&..H.&.9k.6Z..
-00001840: c4a3 f0f7 38ed 2e20 6d4f b19d 738e 7d9c  ....8.. mO..s.}.
-00001850: 643d fa5d 6801 28f9 b6c6 855c b444 dd4c  d=.]h.(....\.D.L
-00001860: ca50 b660 5598 6007 8e6f 6af4 5611 a7be  .P.`U.`..oj.V...
-00001870: 91a1 f3a0 aa81 648d bc49 d33b 6995 76a2  ......d..I.;i.v.
-00001880: c886 daca 1719 eec9 6807 2b9f 84bd b5ca  ........h.+.....
-00001890: ffcc c160 9f8b a938 16d6 ba69 6928 c822  ...`...8...ii(."
-000018a0: eb54 031b a0b7 8e09 9cca 934e a52d b8a0  .T.........N.-..
-000018b0: d125 1eea 5c3c 4e67 cb91 3120 de35 f4e1  .%..\<Ng..1 .5..
-000018c0: 4f9c 4433 5bc4 5d4c 5eaa 5ca4 7126 3050  O.D3[.]L^.\.q&0P
-000018d0: 5294 507c 7cc1 028c 894a 3cc9 e741 549c  R.P||....J<..AT.
-000018e0: 9b46 e6df f828 ff34 f8e7 f1b6 2ac0 02cd  .F...(.4....*...
-000018f0: 87ae a8cd c583 482a a8d5 ded0 1afb 6738  ......H*......g8
-00001900: 78ba 3d8f b854 a48a cc63 9ff8 68b6 c8ca  x.=..T...c..h...
-00001910: 18c4 960c d42e 2e69 439e eb9a 3b51 a1ab  .......iC...;Q..
-00001920: 4c12 f78f 992c 0fe8 f935 b453 162e e017  L....,...5.S....
-00001930: d7f0 1584 d2eb 2e2e e302 6d79 8d46 aa09  ..........my.F..
-00001940: fff1 920d 1db7 343a 8c2f f8aa 7ca3 5d48  ......4:./..|.]H
-00001950: 0cd4 ac93 4eee 790f 7e5c c998 1076 c38b  ....N.y.~\...v..
-00001960: 6f91 08ed 10b6 fc93 c047 00df d788 744a  o........G....tJ
-00001970: e293 9c3e 67f1 0b50 4b03 0414 0000 0008  ...>g..PK.......
-00001980: 008b 8a6f 5855 85c6 84f8 0200 003f 0a00  ...oXU.......?..
-00001990: 0018 0000 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
-000019a0: 7473 2f73 6865 6574 382e 786d 6cbd 56db  ts/sheet8.xml.V.
-000019b0: 72da 3010 fd15 c6cf 4e0c 4c73 19c6 30c3  r.0.....N.Ls..0.
-000019c0: 9db4 a1a5 81a4 8f1e 212f 5845 961c 691d  ........!/XE..i.
-000019d0: 9abf efca 2424 cdd8 61ca 032f 20ad 7476  ....$$..a../ .tv
-000019e0: cf91 b4eb 0db7 da6c 6c02 80b5 3fa9 54b6  .......ll...?.T.
-000019f0: ed25 8859 2b08 2c4f 2065 f65c 67a0 6865  .%.Y+.,O e.\g.he
-00001a00: a54d ca90 a666 1dd8 cc00 8b0b 502a 8366  .M...f......P*.f
-00001a10: bd7e 19a4 4c28 af13 16b6 99e9 843a 4729  .~..L(.......:G)
-00001a20: 14cc 4ccd e669 cacc 730f a4de b6bd 86f7  ..L..i..s.......
-00001a30: 6ab8 13eb 040b 43d0 0933 b686 39e0 7d46  j.....C..3..9.}F
-00001a40: 009a 067b 3fb1 4841 59a1 55cd c0aa ed75  ...{?.HAY.U....u
-00001a50: 1bad d90e 51ec 7810 b0b5 efc6 3527 66a9  ....Q.x.....5'f.
-00001a60: f5c6 4d6e e2b6 5777 9c40 0247 e782 d1df  ..Mn..Ww.@.G....
-00001a70: 13f4 414a e789 983c be38 f5de 823a e4fb  ..AJ...<.8...:..
-00001a80: f1ab fb51 a19f e82d 9985 be96 bf44 8c49  ...Q...-.....D.I
-00001a90: dbbb f66a 31ac 582e f14e 6f27 f0a2 e9e2  ...j1.X..No'....
-00001aa0: 8de2 8021 eb84 466f 6bc6 89ed 84dc 0d5c  ...!..Fok......\
-00001ab0: 48da 2894 3ba4 391a b20b 8a84 1d04 8b11  H.(.;.9.........
-00001ac0: a8a7 3040 62e1 6c01 7fc1 f4aa 308f 3998  ..0@b.l.....0.9.
-00001ad0: e708 9f33 2841 f53f 8dc4 ac05 b425 b041  ...3(A.?.....%.A
-00001ae0: 158c ae9e 6b15 0b77 a065 c061 653c c332  ....k..w.e.ae<.2
-00001af0: 1121 a499 6458 c674 5485 e43a cdb4 0255  .!..dX.tT..:...U
-00001b00: 4a74 fca9 3e4e 9715 e9e5 6f28 6ebe 043e  Jt..>N....o(n..>
-00001b10: 390c b73a 37bc 0c7b 7318 4ba7 150b 4e7a  9..:7..{s.K...Nz
-00001b20: 23c5 d232 1f5f ffc7 8788 4b3c 7c3b ec41  #..2._....K<|;.A
-00001b30: a82c c772 f4ed 61b4 c995 0213 d143 41a1  .,.r..a......CA.
-00001b40: d665 7730 ad72 521a f27b d5ee 8a23 fa51  .ew0.rR..{...#.Q
-00001b50: b53f 06cb 8dc8 dc4b 2c81 cd2a 95b1 8f22  .?.....K,..*..."
-00001b60: 024a cfd7 9cdf e56b 4cbf 0f4c 0afa 77ef  .J.....kL..L..w.
-00001b70: bcc6 75ae c8d9 a5f7 7169 5f43 9aad 6ea3  ..u.....qi_C..n.
-00001b80: fee5 fae2 ea92 ea4a a2b7 03a3 b381 de2a  .......J.......*
-00001b90: 5783 0ac3 8dbb 8429 584b a56e 6f1c 1aa3  W......)XK.no...
-00001ba0: cd7b 2393 5426 7b92 a94d 511a 5d52 b73d  .{#.T&{..MQ.]R.=
-00001bb0: 292c 5264 5782 73c9 1a1d 2f86 279f 0bdf  ),RdW.s.../.'...
-00001bc0: dd91 9f19 1d7b 61b0 5f0c 837f 1956 31ee  .....{a._....V1.
-00001bd0: 355b bdd3 3146 fa62 a03d 86e7 b0d9 1a9e  5[..1F.b.=......
-00001be0: 8e27 3d41 29b4 a16c b3fe 8eb3 8f89 0188  .'=A)..l........
-00001bf0: 129d f9b1 c9d7 d1ce 1a19 6620 8a85 054a  ..........f ...J
-00001c00: 9162 e10c f5d9 1a14 1ca3 71d4 6c8d 4ea7  .b........q.l.N.
-00001c10: f118 86e3 666b 7c3a 865d ce21 43a6 382c  ....fk|:.].!C.8,
-00001c20: dc13 ef81 e209 f50c 9b62 f633 670a 0532  .........b.3g..2
-00001c30: 57d1 9de1 1839 9366 6b72 3a39 f3e9 d09f  W....9.fkr:9....
-00001c40: 4fef ef46 fe58 e024 5fde 5b30 2380 78c9  O..F.X.$_.[0#.x.
-00001c50: f8c6 5f74 fb8b 9dc2 2929 f417 8629 4b5f  .._t....))...)K_
-00001c60: 486d 16c0 52df 0974 25e9 56f3 42c0 e762  Hm..R..t%.V.B..b
-00001c70: 3f18 ecae b122 bf6b 4145 4cc2 8a6a 58fd  ?....".kAEL..jX.
-00001c80: fc8a da13 b3eb 5476 13d4 5941 7fa9 1175  ......Tv..YA...u
-00001c90: 5a0c 136a f0c0 b80d b4be d21a f713 d729  Z..j...........)
-00001ca0: ed7b c6ce 5f50 4b03 0414 0000 0008 008b  .{.._PK.........
-00001cb0: 8a6f 5855 85c6 84f8 0200 003f 0a00 0018  .oXU.......?....
-00001cc0: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
-00001cd0: 2f73 6865 6574 392e 786d 6cbd 56db 72da  /sheet9.xml.V.r.
-00001ce0: 3010 fd15 c6cf 4e0c 4c73 19c6 30c3 9db4  0.....N.Ls..0...
-00001cf0: a1a5 81a4 8f1e 212f 5845 961c 691d 9abf  ......!/XE..i...
-00001d00: efca 2424 cdd8 61ca 032f 20ad 7476 cf91  ..$$..a../ .tv..
-00001d10: b4eb 0db7 da6c 6c02 80b5 3fa9 54b6 ed25  .....ll...?.T..%
-00001d20: 8859 2b08 2c4f 2065 f65c 67a0 6865 a54d  .Y+.,O e.\g.he.M
-00001d30: ca90 a666 1dd8 cc00 8b0b 502a 8366 bd7e  ...f......P*.f.~
-00001d40: 19a4 4c28 af13 16b6 99e9 843a 4729 14cc  ..L(.......:G)..
-00001d50: 4ccd e669 cacc 730f a4de b6bd 86f7 6ab8  L..i..s.......j.
-00001d60: 13eb 040b 43d0 0933 b686 39e0 7d46 009a  ....C..3..9.}F..
-00001d70: 067b 3fb1 4841 59a1 55cd c0aa ed75 1bad  .{?.HAY.U....u..
-00001d80: d90e 51ec 7810 b0b5 efc6 3527 66a9 f5c6  ..Q.x.....5'f...
-00001d90: 4d6e e2b6 5777 9c40 0247 e782 d1df 13f4  Mn..Ww.@.G......
-00001da0: 414a e789 983c be38 f5de 823a e4fb f1ab  AJ...<.8...:....
-00001db0: fb51 a19f e82d 9985 be96 bf44 8c49 dbbb  .Q...-.....D.I..
-00001dc0: f66a 31ac 582e f14e 6f27 f0a2 e9e2 8de2  .j1.X..No'......
-00001dd0: 8021 eb84 466f 6bc6 89ed 84dc 0d5c 48da  .!..Fok......\H.
-00001de0: 2894 3ba4 391a b20b 8a84 1d04 8b11 a8a7  (.;.9...........
-00001df0: 3040 62e1 6c01 7fc1 f4aa 308f 3998 e708  0@b.l.....0.9...
-00001e00: 9f33 2841 f53f 8dc4 ac05 b425 b041 158c  .3(A.?.....%.A..
-00001e10: ae9e 6b15 0b77 a065 c061 653c c332 1121  ..k..w.e.ae<.2.!
-00001e20: a499 6458 c674 5485 e43a cdb4 0255 4a74  ..dX.tT..:...UJt
-00001e30: fca9 3e4e 9715 e9e5 6f28 6ebe 043e 390c  ..>N....o(n..>9.
-00001e40: b73a 37bc 0c7b 7318 4ba7 150b 4e7a 23c5  .:7..{s.K...Nz#.
-00001e50: d232 1f5f ffc7 8788 4b3c 7c3b ec41 a82c  .2._....K<|;.A.,
-00001e60: c772 f4ed 61b4 c995 0213 d143 41a1 d665  .r..a......CA..e
-00001e70: 7730 ad72 521a f27b d5ee 8a23 fa51 b53f  w0.rR..{...#.Q.?
-00001e80: 06cb 8dc8 dc4b 2c81 cd2a 95b1 8f22 024a  .....K,..*...".J
-00001e90: cfd7 9cdf e56b 4cbf 0f4c 0afa 77ef bcc6  .....kL..L..w...
-00001ea0: 75ae c8d9 a5f7 7169 5f43 9aad 6ea3 fee5  u.....qi_C..n...
-00001eb0: fae2 ea92 ea4a a2b7 03a3 b381 de2a 5783  .....J.......*W.
-00001ec0: 0ac3 8dbb 8429 584b a56e 6f1c 1aa3 cd7b  .....)XK.no....{
-00001ed0: 2393 5426 7b92 a94d 511a 5d52 b73d 292c  #.T&{..MQ.]R.=),
-00001ee0: 5264 5782 73c9 1a1d 2f86 279f 0bdf dd91  RdW.s.../.'.....
-00001ef0: 9f19 1d7b 61b0 5f0c 837f 1956 31ee 355b  ...{a._....V1.5[
-00001f00: bdd3 3146 fa62 a03d 86e7 b0d9 1a9e 8e27  ..1F.b.=.......'
-00001f10: 3d41 29b4 a16c b3fe 8eb3 8f89 0188 129d  =A)..l..........
-00001f20: f9b1 c9d7 d1ce 1a19 6620 8a85 054a 9162  ........f ...J.b
-00001f30: e10c f5d9 1a14 1ca3 71d4 6c8d 4ea7 f118  ........q.l.N...
-00001f40: 86e3 666b 7c3a 865d ce21 43a6 382c dc13  ..fk|:.].!C.8,..
-00001f50: ef81 e209 f50c 9b62 f633 670a 0532 57d1  .......b.3g..2W.
-00001f60: 9de1 1839 9366 6b72 3a39 f3e9 d09f 4fef  ...9.fkr:9....O.
-00001f70: ef46 fe58 e024 5fde 5b30 2380 78c9 f8c6  .F.X.$_.[0#.x...
-00001f80: 5f74 fb8b 9dc2 2929 f417 8629 4b5f 486d  _t....))...)K_Hm
-00001f90: 16c0 52df 0974 25e9 56f3 42c0 e762 3f18  ..R..t%.V.B..b?.
-00001fa0: ecae b122 bf6b 4145 4cc2 8a6a 58fd fc8a  ...".kAEL..jX...
-00001fb0: da13 b3eb 5476 13d4 5941 7fa9 1175 5a0c  ....Tv..YA...uZ.
-00001fc0: 136a f0c0 b80d b4be d21a f713 d729 ed7b  .j...........).{
-00001fd0: c6ce 5f50 4b03 0414 0000 0008 008b 8a6f  .._PK..........o
-00001fe0: 5855 85c6 84f8 0200 003f 0a00 0019 0000  XU.......?......
-00001ff0: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
-00002000: 6865 6574 3130 2e78 6d6c bd56 db72 da30  heet10.xml.V.r.0
-00002010: 10fd 15c6 cf4e 0c4c 7319 c630 c39d b4a1  .....N.Ls..0....
-00002020: a581 a48f 1e21 2f58 4596 1c69 1d9a bfef  .....!/XE..i....
-00002030: ca24 24cd d861 ca03 2f20 ad74 76cf 91b4  .$$..a../ .tv...
-00002040: eb0d b7da 6c6c 0280 b53f a954 b6ed 2588  ....ll...?.T..%.
-00002050: 592b 082c 4f20 65f6 5c67 a068 65a5 4dca  Y+.,O e.\g.he.M.
-00002060: 90a6 661d d8cc 008b 0b50 2a83 66bd 7e19  ..f......P*.f.~.
-00002070: a44c 28af 1316 b699 e984 3a47 2914 cc4c  .L(.......:G)..L
-00002080: cde6 69ca cc73 0fa4 deb6 bd86 f76a b813  ..i..s.......j..
-00002090: eb04 0b43 d009 33b6 8639 e07d 4600 9a06  ...C..3..9.}F...
-000020a0: 7b3f b148 4159 a155 cdc0 aaed 751b add9  {?.HAY.U....u...
-000020b0: 0e51 ec78 10b0 b5ef c635 2766 a9f5 c64d  .Q.x.....5'f...M
-000020c0: 6ee2 b657 779c 4002 47e7 82d1 df13 f441  n..Ww.@.G......A
-000020d0: 4ae7 8998 3cbe 38f5 de82 3ae4 fbf1 abfb  J...<.8...:.....
-000020e0: 51a1 9fe8 2d99 85be 96bf 448c 49db bbf6  Q...-.....D.I...
-000020f0: 6a31 ac58 2ef1 4e6f 27f0 a2e9 e28d e280  j1.X..No'.......
-00002100: 21eb 8446 6f6b c689 ed84 dc0d 5c48 da28  !..Fok......\H.(
-00002110: 943b a439 1ab2 0b8a 841d 048b 11a8 a730  .;.9...........0
-00002120: 4062 e16c 017f c1f4 aa30 8f39 98e7 089f  @b.l.....0.9....
-00002130: 3328 41f5 3f8d c4ac 05b4 25b0 4115 8cae  3(A.?.....%.A...
-00002140: 9e6b 150b 77a0 65c0 6165 3cc3 3211 21a4  .k..w.e.ae<.2.!.
-00002150: 9964 58c6 7454 85e4 3acd b402 554a 74fc  .dX.tT..:...UJt.
-00002160: a93e 4e97 15e9 e56f 286e be04 3e39 0cb7  .>N....o(n..>9..
-00002170: 3a37 bc0c 7b73 184b a715 0b4e 7a23 c5d2  :7..{s.K...Nz#..
-00002180: 321f 5fff c787 884b 3c7c 3bec 41a8 2cc7  2._....K<|;.A.,.
-00002190: 72f4 ed61 b4c9 9502 13d1 4341 a1d6 6577  r..a......CA..ew
-000021a0: 30ad 7252 1af2 7bd5 ee8a 23fa 51b5 3f06  0.rR..{...#.Q.?.
-000021b0: cb8d c8dc 4b2c 81cd 2a95 b18f 2202 4acf  ....K,..*...".J.
-000021c0: d79c dfe5 6b4c bf0f 4c0a fa77 efbc c675  ....kL..L..w...u
-000021d0: aec8 d9a5 f771 695f 439a ad6e a3fe e5fa  .....qi_C..n....
-000021e0: e2ea 92ea 4aa2 b703 a3b3 81de 2a57 830a  ....J.......*W..
-000021f0: c38d bb84 2958 4ba5 6e6f 1c1a a3cd 7b23  ....)XK.no....{#
-00002200: 9354 267b 92a9 4d51 1a5d 52b7 3d29 2c52  .T&{..MQ.]R.=),R
-00002210: 6457 8273 c91a 1d2f 8627 9f0b dfdd 919f  dW.s.../.'......
-00002220: 191d 7b61 b05f 0c83 7f19 5631 ee35 5bbd  ..{a._....V1.5[.
-00002230: d331 46fa 62a0 3d86 e7b0 d91a 9e8e 273d  .1F.b.=.......'=
-00002240: 4129 b4a1 6cb3 fe8e b38f 8901 8812 9df9  A)..l...........
-00002250: b1c9 d7d1 ce1a 1966 208a 8505 4a91 62e1  .......f ...J.b.
-00002260: 0cf5 d91a 141c a371 d46c 8d4e a7f1 1886  .......q.l.N....
-00002270: e366 6b7c 3a86 5dce 2143 a638 2cdc 13ef  .fk|:.].!C.8,...
-00002280: 81e2 09f5 0c9b 62f6 3367 0a05 3257 d19d  ......b.3g..2W..
-00002290: e118 3993 666b 723a 39f3 e9d0 9f4f efef  ..9.fkr:9....O..
-000022a0: 46fe 58e0 245f de5b 3023 8078 c9f8 c65f  F.X.$_.[0#.x..._
-000022b0: 74fb 8b9d c229 29f4 1786 294b 5f48 6d16  t....))...)K_Hm.
-000022c0: c052 df09 7425 e956 f342 c0e7 623f 18ec  .R..t%.V.B..b?..
-000022d0: aeb1 22bf 6b41 454c c28a 6a58 fdfc 8ada  ..".kAEL..jX....
-000022e0: 13b3 eb54 7613 d459 417f a911 755a 0c13  ...Tv..YA...uZ..
-000022f0: 6af0 c0b8 0db4 bed2 1af7 13d7 29ed 7bc6  j...........).{.
-00002300: ce5f 504b 0304 1400 0000 0800 8b8a 6f58  ._PK..........oX
-00002310: 3013 165e 0d03 0000 b30a 0000 1900 0000  0..^............
-00002320: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
-00002330: 6565 7431 312e 786d 6cbd 5651 53db 300c  eet11.xml.VQS.0.
-00002340: fe2b bd3c 67a4 f406 e37a 69ef a005 5a46  .+.<g....zi...ZF
-00002350: 3728 657b ccb9 8eda 7875 accc 56e8 f8f7  7(e{....xu..V...
-00002360: 9353 288c 4bca 8d87 beb4 b6ec 4ffa 3e5b  .S(.K.......O.>[
-00002370: 5614 afd1 ae5c 0640 ad3f b936 ae17 6444  V....\.@.?.6..dD
-00002380: 4537 8a9c cc20 17ee 000b 30bc b240 9b0b  E7... ....0..@..
-00002390: e2a9 5d46 aeb0 20d2 0a94 eba8 d36e 1f47  ..]F.. ......n.G
-000023a0: b950 26e8 c795 edc6 f663 2c49 2b03 37b6  .P&......c,I+.7.
-000023b0: e5ca 3c17 f6f1 0c34 ae7b c161 f06c 98aa  ..<....4.{.a.l..
-000023c0: 6546 9521 eac7 8558 c21d d07d c100 9e46  eF.!...X...}...F
-000023d0: 5b3f a9ca c138 85a6 6561 d10b 4e0f bbd3  [?...8..ea..N...
-000023e0: 0da2 daf1 43c1 dabd 1ab7 bc98 39e2 ca4f  ....C.......9..O
-000023f0: c669 2f68 7b4e a041 9277 21f8 ef01 06a0  .i/h{N.A.w!.....
-00002400: b5f7 c44c 7e3f 390d 5e82 7ae4 ebf1 b3fb  ...L~?9.^.z.....
-00002410: 8b4a 3fd3 9b0b 0703 d43f 554a 592f 3809  .J?......?UJY/8.
-00002420: 5a29 2c44 a969 8aeb 113c 693a 7aa1 3814  Z),D.i...<i:z.8.
-00002430: 24fa b1c5 75cb 7ab1 fd58 fa81 0fc9 1b95  $...u.z..X......
-00002440: f187 7447 96ed 8a23 519f ac28 54f2 00d6  ..tG...#Q..(T...
-00002450: 6b8e 2362 2a7e 2192 4fc0 b326 e05c 219b  k.#b*~!.O..&.\!.
-00002460: 563b a083 c698 e028 01f3 5083 1936 617e  V;.....(..P..6a~
-00002470: 9760 1f13 7a2c a006 75be 3392 700e c8d5  .`..z,..u.3.p...
-00002480: c02e 9a60 9c6e 124d aafc 25d6 012f 779f  ...`.n.M..%../w.
-00002490: 2641 5e68 4175 4c47 4d48 8979 8106 4c2d  &A^hAuLGMH.y..L-
-000024a0: d1f1 4e7d 9213 24c1 f92f a8b2 ad06 7ef5  ..N}..$../....~.
-000024b0: 3edc 6169 651d f6eb fb58 3ead 5449 d69b  >.aie....X>.TI..
-000024c0: 1891 d7f9 b8fe 1f1f 2aad f130 79df 8332  ........*..0y..2
-000024d0: 4549 f5e8 6fef a36d 690c d884 1385 9459  EI..o..mi......Y
-000024e0: d6dd c1f7 2627 b521 6f9a 7637 1cd1 6dd3  ....&'.!o.v7..m.
-000024f0: fe14 9cb4 aaa0 fa27 366d 5426 de8a 88b8  .......'6mT&....
-00002500: 243c d799 4d8d 48f9 f787 d08a ff7d 9eb7  $<..M.H......}..
-00002510: 2496 869d 1d07 6f97 9eeb d6a0 d31d 1cb6  $.....o.........
-00002520: 3f9f 1c7d 39e6 5a96 e17a 68b1 18e2 daf8  ?..}9.Z..zh.....
-00002530: ba57 19c6 fe12 26e0 1c97 d7ad f1dc 5ab4  .W....&.......Z.
-00002540: af8d 4273 693e d3c2 acaa 72ec 1f75 2fd0  ..Bsi>....r..u/.
-00002550: ca11 47f6 65bf d4e2 b01f a4f0 104a 15fa  ..G.e........J..
-00002560: 3b0a 0b8b 6910 47db c538 fa97 6113 e361  ;...i.G..8..a..a
-00002570: a73b dc1f 63e2 af14 b98f f0bc ec74 2ff7  .;..c........t/.
-00002580: c793 5350 2bb4 fcda 5cb8 e11c 5266 0192  ..SP+...\...Rf..
-00002590: 0c8b 30b5 e532 d958 132b 2c24 a972 c04f  ..0..2.X.+,$.r.O
-000025a0: a45a f844 f869 0906 3ea2 71d4 e98e f6a7  .Z.D.i..>.q.....
-000025b0: f123 0cc7 9dee 787f 0c4f a584 8284 9130  .#....x..O.....0
-000025c0: f329 7e06 4666 dca7 acaa d96d 290c 2912  .)~.Ff.....m).).
-000025d0: bea2 7bc3 47e4 5c75 ba57 fb93 7337 390f  ..{.G.\u.W..s79.
-000025e0: ef26 f7d3 8bf0 52d1 a89c df3b b017 00e9  .&....R....;....
-000025f0: 5cc8 5538 3b1d cc36 0a27 ac30 9c59 611c  \.U8;..6.'.0.Ya.
-00002600: 7f21 d1ce 40e4 a117 e84b d235 ca4a c06e  .!..@....K.5.J.n
-00002610: b16f 0c6e d3cc b1df a5e2 22a6 61c1 35ac  .o.n......".a.5.
-00002620: 7df0 855b 22bb e98e 3613 c2a2 a23f 4722  }..["...6....?G"
-00002630: ccab 61c6 4d25 58bf 81d7 1788 b49d f8ee  ..a.M%X.........
-00002640: 6cdb a7f6 ff02 504b 0304 1400 0000 0800  l.....PK........
-00002650: 8b8a 6f58 5585 c684 f802 0000 3f0a 0000  ..oXU.......?...
-00002660: 1900 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
-00002670: 732f 7368 6565 7431 322e 786d 6cbd 56db  s/sheet12.xml.V.
-00002680: 72da 3010 fd15 c6cf 4e0c 4c73 19c6 30c3  r.0.....N.Ls..0.
-00002690: 9db4 a1a5 81a4 8f1e 212f 5845 961c 691d  ........!/XE..i.
-000026a0: 9abf efca 2424 cdd8 61ca 032f 20ad 7476  ....$$..a../ .tv
-000026b0: cf91 b4eb 0db7 da6c 6c02 80b5 3fa9 54b6  .......ll...?.T.
-000026c0: ed25 8859 2b08 2c4f 2065 f65c 67a0 6865  .%.Y+.,O e.\g.he
-000026d0: a54d ca90 a666 1dd8 cc00 8b0b 502a 8366  .M...f......P*.f
-000026e0: bd7e 19a4 4c28 af13 16b6 99e9 843a 4729  .~..L(.......:G)
-000026f0: 14cc 4ccd e669 cacc 730f a4de b6bd 86f7  ..L..i..s.......
-00002700: 6ab8 13eb 040b 43d0 0933 b686 39e0 7d46  j.....C..3..9.}F
-00002710: 009a 067b 3fb1 4841 59a1 55cd c0aa ed75  ...{?.HAY.U....u
-00002720: 1bad d90e 51ec 7810 b0b5 efc6 3527 66a9  ....Q.x.....5'f.
-00002730: f5c6 4d6e e2b6 5777 9c40 0247 e782 d1df  ..Mn..Ww.@.G....
-00002740: 13f4 414a e789 983c be38 f5de 823a e4fb  ..AJ...<.8...:..
-00002750: f1ab fb51 a19f e82d 9985 be96 bf44 8c49  ...Q...-.....D.I
-00002760: dbbb f66a 31ac 582e f14e 6f27 f0a2 e9e2  ...j1.X..No'....
-00002770: 8de2 8021 eb84 466f 6bc6 89ed 84dc 0d5c  ...!..Fok......\
-00002780: 48da 2894 3ba4 391a b20b 8a84 1d04 8b11  H.(.;.9.........
-00002790: a8a7 3040 62e1 6c01 7fc1 f4aa 308f 3998  ..0@b.l.....0.9.
-000027a0: e708 9f33 2841 f53f 8dc4 ac05 b425 b041  ...3(A.?.....%.A
-000027b0: 158c ae9e 6b15 0b77 a065 c061 653c c332  ....k..w.e.ae<.2
-000027c0: 1121 a499 6458 c674 5485 e43a cdb4 0255  .!..dX.tT..:...U
-000027d0: 4a74 fca9 3e4e 9715 e9e5 6f28 6ebe 043e  Jt..>N....o(n..>
-000027e0: 390c b73a 37bc 0c7b 7318 4ba7 150b 4e7a  9..:7..{s.K...Nz
-000027f0: 23c5 d232 1f5f ffc7 8788 4b3c 7c3b ec41  #..2._....K<|;.A
-00002800: a82c c772 f4ed 61b4 c995 0213 d143 41a1  .,.r..a......CA.
-00002810: d665 7730 ad72 521a f27b d5ee 8a23 fa51  .ew0.rR..{...#.Q
-00002820: b53f 06cb 8dc8 dc4b 2c81 cd2a 95b1 8f22  .?.....K,..*..."
-00002830: 024a cfd7 9cdf e56b 4cbf 0f4c 0afa 77ef  .J.....kL..L..w.
-00002840: bcc6 75ae c8d9 a5f7 7169 5f43 9aad 6ea3  ..u.....qi_C..n.
-00002850: fee5 fae2 ea92 ea4a a2b7 03a3 b381 de2a  .......J.......*
-00002860: 5783 0ac3 8dbb 8429 584b a56e 6f1c 1aa3  W......)XK.no...
-00002870: cd7b 2393 5426 7b92 a94d 511a 5d52 b73d  .{#.T&{..MQ.]R.=
-00002880: 292c 5264 5782 73c9 1a1d 2f86 279f 0bdf  ),RdW.s.../.'...
-00002890: dd91 9f19 1d7b 61b0 5f0c 837f 1956 31ee  .....{a._....V1.
-000028a0: 355b bdd3 3146 fa62 a03d 86e7 b0d9 1a9e  5[..1F.b.=......
-000028b0: 8e27 3d41 29b4 a16c b3fe 8eb3 8f89 0188  .'=A)..l........
-000028c0: 129d f9b1 c9d7 d1ce 1a19 6620 8a85 054a  ..........f ...J
-000028d0: 9162 e10c f5d9 1a14 1ca3 71d4 6c8d 4ea7  .b........q.l.N.
-000028e0: f118 86e3 666b 7c3a 865d ce21 43a6 382c  ....fk|:.].!C.8,
-000028f0: dc13 ef81 e209 f50c 9b62 f633 670a 0532  .........b.3g..2
-00002900: 57d1 9de1 1839 9366 6b72 3a39 f3e9 d09f  W....9.fkr:9....
-00002910: 4fef ef46 fe58 e024 5fde 5b30 2380 78c9  O..F.X.$_.[0#.x.
-00002920: f8c6 5f74 fb8b 9dc2 2929 f417 8629 4b5f  .._t....))...)K_
-00002930: 486d 16c0 52df 0974 25e9 56f3 42c0 e762  Hm..R..t%.V.B..b
-00002940: 3f18 ecae b122 bf6b 4145 4cc2 8a6a 58fd  ?....".kAEL..jX.
-00002950: fc8a da13 b3eb 5476 13d4 5941 7fa9 1175  ......Tv..YA...u
-00002960: 5a0c 136a f0c0 b80d b4be d21a f713 d729  Z..j...........)
-00002970: ed7b c6ce 5f50 4b03 0414 0000 0008 008b  .{.._PK.........
-00002980: 8a6f 5855 85c6 84f8 0200 003f 0a00 0019  .oXU.......?....
-00002990: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
-000029a0: 2f73 6865 6574 3133 2e78 6d6c bd56 db72  /sheet13.xml.V.r
-000029b0: da30 10fd 15c6 cf4e 0c4c 7319 c630 c39d  .0.....N.Ls..0..
-000029c0: b4a1 a581 a48f 1e21 2f58 4596 1c69 1d9a  .......!/XE..i..
-000029d0: bfef ca24 24cd d861 ca03 2f20 ad74 76cf  ...$$..a../ .tv.
-000029e0: 91b4 eb0d b7da 6c6c 0280 b53f a954 b6ed  ......ll...?.T..
-000029f0: 2588 592b 082c 4f20 65f6 5c67 a068 65a5  %.Y+.,O e.\g.he.
-00002a00: 4dca 90a6 661d d8cc 008b 0b50 2a83 66bd  M...f......P*.f.
-00002a10: 7e19 a44c 28af 1316 b699 e984 3a47 2914  ~..L(.......:G).
-00002a20: cc4c cde6 69ca cc73 0fa4 deb6 bd86 f76a  .L..i..s.......j
-00002a30: b813 eb04 0b43 d009 33b6 8639 e07d 4600  .....C..3..9.}F.
-00002a40: 9a06 7b3f b148 4159 a155 cdc0 aaed 751b  ..{?.HAY.U....u.
-00002a50: add9 0e51 ec78 10b0 b5ef c635 2766 a9f5  ...Q.x.....5'f..
-00002a60: c64d 6ee2 b657 779c 4002 47e7 82d1 df13  .Mn..Ww.@.G.....
-00002a70: f441 4ae7 8998 3cbe 38f5 de82 3ae4 fbf1  .AJ...<.8...:...
-00002a80: abfb 51a1 9fe8 2d99 85be 96bf 448c 49db  ..Q...-.....D.I.
-00002a90: bbf6 6a31 ac58 2ef1 4e6f 27f0 a2e9 e28d  ..j1.X..No'.....
-00002aa0: e280 21eb 8446 6f6b c689 ed84 dc0d 5c48  ..!..Fok......\H
-00002ab0: da28 943b a439 1ab2 0b8a 841d 048b 11a8  .(.;.9..........
-00002ac0: a730 4062 e16c 017f c1f4 aa30 8f39 98e7  .0@b.l.....0.9..
-00002ad0: 089f 3328 41f5 3f8d c4ac 05b4 25b0 4115  ..3(A.?.....%.A.
-00002ae0: 8cae 9e6b 150b 77a0 65c0 6165 3cc3 3211  ...k..w.e.ae<.2.
-00002af0: 21a4 9964 58c6 7454 85e4 3acd b402 554a  !..dX.tT..:...UJ
-00002b00: 74fc a93e 4e97 15e9 e56f 286e be04 3e39  t..>N....o(n..>9
-00002b10: 0cb7 3a37 bc0c 7b73 184b a715 0b4e 7a23  ..:7..{s.K...Nz#
-00002b20: c5d2 321f 5fff c787 884b 3c7c 3bec 41a8  ..2._....K<|;.A.
-00002b30: 2cc7 72f4 ed61 b4c9 9502 13d1 4341 a1d6  ,.r..a......CA..
-00002b40: 6577 30ad 7252 1af2 7bd5 ee8a 23fa 51b5  ew0.rR..{...#.Q.
-00002b50: 3f06 cb8d c8dc 4b2c 81cd 2a95 b18f 2202  ?.....K,..*...".
-00002b60: 4acf d79c dfe5 6b4c bf0f 4c0a fa77 efbc  J.....kL..L..w..
-00002b70: c675 aec8 d9a5 f771 695f 439a ad6e a3fe  .u.....qi_C..n..
-00002b80: e5fa e2ea 92ea 4aa2 b703 a3b3 81de 2a57  ......J.......*W
-00002b90: 830a c38d bb84 2958 4ba5 6e6f 1c1a a3cd  ......)XK.no....
-00002ba0: 7b23 9354 267b 92a9 4d51 1a5d 52b7 3d29  {#.T&{..MQ.]R.=)
-00002bb0: 2c52 6457 8273 c91a 1d2f 8627 9f0b dfdd  ,RdW.s.../.'....
-00002bc0: 919f 191d 7b61 b05f 0c83 7f19 5631 ee35  ....{a._....V1.5
-00002bd0: 5bbd d331 46fa 62a0 3d86 e7b0 d91a 9e8e  [..1F.b.=.......
-00002be0: 273d 4129 b4a1 6cb3 fe8e b38f 8901 8812  '=A)..l.........
-00002bf0: 9df9 b1c9 d7d1 ce1a 1966 208a 8505 4a91  .........f ...J.
-00002c00: 62e1 0cf5 d91a 141c a371 d46c 8d4e a7f1  b........q.l.N..
-00002c10: 1886 e366 6b7c 3a86 5dce 2143 a638 2cdc  ...fk|:.].!C.8,.
-00002c20: 13ef 81e2 09f5 0c9b 62f6 3367 0a05 3257  ........b.3g..2W
-00002c30: d19d e118 3993 666b 723a 39f3 e9d0 9f4f  ....9.fkr:9....O
-00002c40: efef 46fe 58e0 245f de5b 3023 8078 c9f8  ..F.X.$_.[0#.x..
-00002c50: c65f 74fb 8b9d c229 29f4 1786 294b 5f48  ._t....))...)K_H
-00002c60: 6d16 c052 df09 7425 e956 f342 c0e7 623f  m..R..t%.V.B..b?
-00002c70: 18ec aeb1 22bf 6b41 454c c28a 6a58 fdfc  ....".kAEL..jX..
-00002c80: 8ada 13b3 eb54 7613 d459 417f a911 755a  .....Tv..YA...uZ
-00002c90: 0c13 6af0 c0b8 0db4 bed2 1af7 13d7 29ed  ..j...........).
-00002ca0: 7bc6 ce5f 504b 0304 1400 0000 0800 8b8a  {.._PK..........
-00002cb0: 6f58 2359 55fc e301 0000 0704 0000 1900  oX#YU...........
-00002cc0: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
-00002cd0: 7368 6565 7431 342e 786d 6c8d 536d 6fda  sheet14.xml.Smo.
-00002ce0: 3010 fe2b 913f 5735 54eb 8b50 12a9 40d1  0..+.?W5T..P..@.
-00002cf0: 3a8d ad2a 1bd3 3e21 935c 8885 e3cb eccb  :..*..>!.\......
-00002d00: b2fe fb9d 13a0 a081 b44f be7b fcdc e37b  .........O.{...{
-00002d10: 73dc a2db fa12 80a2 3f95 b13e 1125 513d  s.......?..>.%Q=
-00002d20: 92d2 6725 54ca 5f63 0d96 6f0a 7495 2276  ..g%T._c..o.t."v
-00002d30: dd46 fada 81ca bba0 cac8 9bc1 e04e 564a  .F...........NVJ
-00002d40: 5b91 c61d f6e2 d218 1b32 dac2 8b8b 7c53  [........2....|S
-00002d50: 55ca bd8d c160 9b88 a1d8 03af 7a53 5207  U....`......zSR.
-00002d60: c834 aed5 0616 40df 6b0e 6057 1e74 725d  .4....@.k.`W.tr]
-00002d70: 81f5 1a6d e4a0 48c4 e370 34eb 233a c652  ...m..H..p4.#:.R
-00002d80: 43eb 8fec 2814 b346 dc06 e739 4fc4 20e4  C...(..F...9O. .
-00002d90: 0406 320a 128a 8fdf 3001 6382 1267 f26b  ..2.....0.c..g.k
-00002da0: 272a de1f 0d91 c7f6 5e7e d6d5 cfe9 ad95  '*......^~......
-00002db0: 8709 9a1f 3aa7 3211 0f22 caa1 508d a157  ....:.2.."..P..W
-00002dc0: 6c3f c2ae a6db f714 a78a 541a 3b6c 2317  l?........T.;l#.
-00002dd0: 8a4d e32c 18e1 4926 6a1b 9ab4 20c7 b8e6  .M.,..I&j... ...
-00002de0: 9728 25f0 b4ca 3966 5568 032b 8399 2274  .(%...9fUh.+.."t
-00002df0: b124 ce29 3064 b653 18ff a742 3fb7 3302  .$.)0d.S...B?.3.
-00002e00: 934b 023a 3fc3 9e5e 625b 55c1 19fe d325  .K.:?..^b[U....%
-00002e10: 7e0e 3e73 ba0e f338 1336 bb58 95da f853  ~.>s...8.6.X...S
-00002e20: bee4 9eee 07d5 3739 14bd 5446 f3c9 ea3e  ......79..TF...>
-00002e30: cab0 b1d4 37fd f46a 3ff8 f1cd 683c 1c7c  ....7..j?...h<.|
-00002e40: 78b8 bdbf e365 28b1 9d3a aca7 d8da b038  x....e(..:.....8
-00002e50: 1df0 6ceb 86e6 e03d efe7 017c 720e dd31  ..l....=...|r..1
-00002e60: a80c eff6 d828 bbed f699 de6a c68d f6c4  .....(.....j....
-00002e70: 2f87 fe37 460d 53f1 6db1 bcfa f938 ff7c  /..7F.S.m....8.|
-00002e80: f569 f1f5 8b88 e5e1 2696 a7e9 fd03 f8fe  .i......&.......
-00002e90: 83cc 95db 68ae cb40 c165 0dae ef79 cd5c  ....h..@.e...y.\
-00002ea0: bf71 bd43 5877 09ac 9108 abce 2cf9 a382  .q.CXw......,...
-00002eb0: 0b04 be2f 10e9 e084 8d3f fcfd f42f 504b  .../.....?.../PK
-00002ec0: 0304 1400 0000 0800 8b8a 6f58 bc72 e0e6  ..........oX.r..
-00002ed0: ff01 0000 8104 0000 1900 0000 786c 2f77  ............xl/w
-00002ee0: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
-00002ef0: 352e 786d 6c7d 54db 6edb 300c fd15 43cf  5.xml}T.n.0...C.
-00002f00: 4195 14eb 0581 63a0 49da a5c0 0214 2dda  A.....c.I.....-.
-00002f10: 3d16 8a4c c742 749b 44cf ebdf 8fb2 9334  =..L.Bt.D......4
-00002f20: dd92 3c59 3ce2 2179 44d2 79eb c226 d600  ..<Y<.!yD.y..&..
-00002f30: 98fd 31da c609 ab11 fd98 f328 6b30 225e  ..1........(k0"^
-00002f40: 380f 966e 2a17 8c40 32c3 9a47 1f40 941d  8..n*..@2..G.@..
-00002f50: c968 7e39 1c5e 7323 9465 45de 614f a1c8  .h~9.^s#.eE.aO..
-00002f60: 5d83 5a59 780a 596c 8c11 e163 0ada b513  ].ZYx.Yl...c....
-00002f70: 3662 3be0 59ad 6bec 005e e45e ace1 05f0  6b;.Y.k..^.^....
-00002f80: d513 814c be8f 532a 0336 2a67 b300 d584  ...L..S*.6*g....
-00002f90: dd8d c68b 9ed1 79bc 2968 e3c1 394b 6256  ......y.)h..9KbV
-00002fa0: ce6d 92f1 584e d830 d504 1a24 a610 823e  .m..XN.0...$...>
-00002fb0: bf61 065a a748 54c9 af6d 50f6 9934 310f  .a.Z.HT..mP..41.
-00002fc0: cfbb f00f 9d7e 2a6f 2522 cc9c fea9 4aac  .....~*o%"....J.
-00002fd0: 27ec 9665 2554 a2d1 f8ec da05 6c35 5d7d  '..e%T......l5]}
-00002fe0: 9638 1728 8a3c b836 0b49 6c91 cb74 4829  .8.(.<.6.Il..tH)
-00002ff0: c951 d9f4 482f 1808 5794 090b 8488 ef06  .Q..H/..W.......
-00003000: 5094 c4cb 3952 29e9 82cb 2d71 7a96 e821  P...9R)...-qz..!
-00003010: 4467 8ff1 6667 7992 34c5 23ac f959 566c  Dg..fgy.4.#..YVl
-00003020: 14c2 7bf4 2055 a5a4 484f 7c24 c6fd a918  ..{. U..HO|$....
-00003030: aa3c e2fd 70ca db0a 0347 fcbf 9ff2 2f21  .<..p....G..../!
-00003040: caa0 fc89 a216 2785 89f5 3f0f c1a9 77bb  ......'...?...w.
-00003050: 81e8 9b99 5af3 26b4 2a3b c931 93ae b1d8  ....Z.&.*;.1....
-00003060: 37f7 ebd5 6ec0 a697 e3e9 68f8 edf6 eae6  7...n.....h.....
-00003070: 9a86 ae76 ed3c 383f 77ad 4d03 da01 8fd6  ...v.<8?w.M.....
-00003080: 37b8 8418 690f f6e0 7d08 2e1c 8242 d30e  7...i...}....B..
-00003090: 4db5 b09b 6e6f f0c3 13ae 5544 ca9c f6b3  M...no....UD....
-000030a0: d162 54b0 3bad 0733 d245 2dd1 831f b40c  .bT.;..3.E-.....
-000030b0: af7e b004 590b 4b9e 4ab2 9cef 7d73 feb5  .~..Y.K.J...}s..
-000030c0: e0ff 80d8 afe6 5284 b522 a51a 2a12 3abc  ......R.."..*.:.
-000030d0: b8a1 010f fdac f706 3adf 95b4 7288 ce74  ........:...r..t
-000030e0: c79a 7e11 1092 03dd 57ce e1de 48bb b6ff  ..~.....W...H...
-000030f0: eb14 7f01 504b 0304 1400 0000 0800 8b8a  ....PK..........
-00003100: 6f58 bc72 e0e6 ff01 0000 8104 0000 1900  oX.r............
-00003110: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
-00003120: 7368 6565 7431 362e 786d 6c7d 54db 6edb  sheet16.xml}T.n.
-00003130: 300c fd15 43cf 4195 14eb 0581 63a0 49da  0...C.A.....c.I.
-00003140: a5c0 0214 2dda 3d16 8a4c c742 749b 44cf  ....-.=..L.Bt.D.
-00003150: ebdf 8fb2 9334 dd92 3c59 3ce2 2179 44d2  .....4..<Y<.!yD.
-00003160: 79eb c226 d600 98fd 31da c609 ab11 fd98  y..&....1.......
-00003170: f328 6b30 225e 380f 966e 2a17 8c40 32c3  .(k0"^8..n*..@2.
-00003180: 9a47 1f40 941d c968 7e39 1c5e 7323 9465  .G.@...h~9.^s#.e
-00003190: 45de 614f a1c8 5d83 5a59 780a 596c 8c11  E.aO..].ZYx.Yl..
-000031a0: e163 0ada b513 3662 3be0 59ad 6bec 005e  .c....6b;.Y.k..^
-000031b0: e45e ace1 05f0 d513 814c be8f 532a 0336  .^.......L..S*.6
-000031c0: 2a67 b300 d584 dd8d c68b 9ed1 79bc 2968  *g..........y.)h
-000031d0: e3c1 394b 6256 ce6d 92f1 584e d830 d504  ..9KbV.m..XN.0..
-000031e0: 1a24 a610 823e bf61 065a a748 54c9 af6d  .$...>.a.Z.HT..m
-000031f0: 50f6 9934 310f cfbb f00f 9d7e 2a6f 2522  P..41......~*o%"
-00003200: cc9c fea9 4aac 27ec 9665 2554 a2d1 f8ec  ....J.'..e%T....
-00003210: da05 6c35 5d7d 9638 1728 8a3c b836 0b49  ..l5]}.8.(.<.6.I
-00003220: 6c91 cb74 4829 c951 d9f4 482f 1808 5794  l..tH).Q..H/..W.
-00003230: 090b 8488 ef06 5094 c4cb 3952 29e9 82cb  ......P...9R)...
-00003240: 2d71 7a96 e821 4467 8ff1 6667 7992 34c5  -qz..!Dg..fgy.4.
-00003250: 23ac f959 566c 14c2 7bf4 2055 a5a4 484f  #..YVl..{. U..HO
-00003260: 7c24 c6fd a918 aa3c e2fd 70ca db0a 0347  |$.....<..p....G
-00003270: fcbf 9ff2 2f21 caa0 fc89 a216 2785 89f5  ..../!......'...
-00003280: 3f0f c1a9 77bb 81e8 9b99 5af3 26b4 2a3b  ?...w.....Z.&.*;
-00003290: c931 93ae b1d8 37f7 ebd5 6ec0 a697 e3e9  .1....7...n.....
-000032a0: 68f8 edf6 eae6 9a86 ae76 ed3c 383f 77ad  h........v.<8?w.
-000032b0: 4d03 da01 8fd6 37b8 8418 690f f6e0 7d08  M.....7...i...}.
-000032c0: 2e1c 8242 d30e 4db5 b09b 6e6f f0c3 13ae  ...B..M...no....
-000032d0: 5544 ca9c f6b3 d162 54b0 3bad 0733 d245  UD.....bT.;..3.E
-000032e0: 2dd1 831f b40c af7e b004 590b 4b9e 4ab2  -......~..Y.K.J.
-000032f0: 9cef 7d73 feb5 e0ff 80d8 afe6 5284 b522  ..}s........R.."
-00003300: a51a 2a12 3abc b8a1 010f fdac f706 3adf  ..*.:.........:.
-00003310: 95b4 7288 ce74 c79a 7e11 1092 03dd 57ce  ..r..t..~.....W.
-00003320: e1de 48bb b6ff eb14 7f01 504b 0304 1400  ..H.......PK....
-00003330: 0000 0800 8b8a 6f58 953b a42f 1101 0000  ......oX.;./....
-00003340: c801 0000 1900 0000 786c 2f77 6f72 6b73  ........xl/works
-00003350: 6865 6574 732f 7368 6565 7431 372e 786d  heets/sheet17.xm
-00003360: 6c4d 51cb 6ec3 2010 fc15 8b0f 084e a53e  lMQ.n. ......N.>
-00003370: 14d9 96d2 5455 7ba8 14a5 6a7b c6f1 da46  ....TU{...j{...F
-00003380: 0196 c2ba 6eff be80 6327 2776 7677 8619  ....n...c''vvw..
-00003390: 2846 7427 df03 50f6 ab95 f125 eb89 ec86  (Ft'..P....%....
-000033a0: 737f ec41 0bbf 420b 264c 5a74 5a50 80ae  s..A..B.&LZtZP..
-000033b0: e3de 3a10 4d22 69c5 6ff2 fc8e 6b21 0dab  ..:.M"i.o...k!..
-000033c0: 8ad4 dbbb aac0 8194 34b0 7799 1fb4 16ee  ........4.w.....
-000033d0: ef11 148e 255b b3b9 7190 5d4f a9c1 abc2  ....%[..q.]O....
-000033e0: 8a0e de81 3e6c 2004 c817 9d46 6a30 5ea2  ....>l ....Fj0^.
-000033f0: c91c b425 dbae 37db 8991 363e 258c feaa  ...%..7...6>%...
-00003400: ce62 981a f114 c16b 53b2 3c7a 0205 478a  .b.....kS.<z..G.
-00003410: 1222 1c3f b003 a5a2 5270 f27d 1665 974b  .".?....Rp.}.e.K
-00003420: 23f3 ba9e e59f 53fe 60af 161e 76a8 be64  #.....S.`...v..d
-00003430: 437d c91e 58d6 402b 0645 071c 5fe0 9ce9  C}..X.@+.E.._...
-00003440: f662 f149 9098 13be 09d7 49e3 3305 6dd8  .b.I......I.3.m.
-00003450: ca57 f761 cf4d 9409 10da f422 3512 a14e  .W.a.M....."5..N
-00003460: 651f 5e1a 5c5c 08f3 1691 1610 2d2f 9f57  e.^.\\......-/.W
-00003470: fd03 504b 0304 1400 0000 0800 8b8a 6f58  ..PK..........oX
-00003480: bc72 e0e6 ff01 0000 8104 0000 1900 0000  .r..............
-00003490: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
-000034a0: 6565 7431 382e 786d 6c7d 54db 6edb 300c  eet18.xml}T.n.0.
-000034b0: fd15 43cf 4195 14eb 0581 63a0 49da a5c0  ..C.A.....c.I...
-000034c0: 0214 2dda 3d16 8a4c c742 749b 44cf ebdf  ..-.=..L.Bt.D...
-000034d0: 8fb2 9334 dd92 3c59 3ce2 2179 44d2 79eb  ...4..<Y<.!yD.y.
-000034e0: c226 d600 98fd 31da c609 ab11 fd98 f328  .&....1........(
-000034f0: 6b30 225e 380f 966e 2a17 8c40 32c3 9a47  k0"^8..n*..@2..G
-00003500: 1f40 941d c968 7e39 1c5e 7323 9465 45de  .@...h~9.^s#.eE.
-00003510: 614f a1c8 5d83 5a59 780a 596c 8c11 e163  aO..].ZYx.Yl...c
-00003520: 0ada b513 3662 3be0 59ad 6bec 005e e45e  ....6b;.Y.k..^.^
-00003530: ace1 05f0 d513 814c be8f 532a 0336 2a67  .......L..S*.6*g
-00003540: b300 d584 dd8d c68b 9ed1 79bc 2968 e3c1  ..........y.)h..
-00003550: 394b 6256 ce6d 92f1 584e d830 d504 1a24  9KbV.m..XN.0...$
-00003560: a610 823e bf61 065a a748 54c9 af6d 50f6  ...>.a.Z.HT..mP.
-00003570: 9934 310f cfbb f00f 9d7e 2a6f 2522 cc9c  .41......~*o%"..
-00003580: fea9 4aac 27ec 9665 2554 a2d1 f8ec da05  ..J.'..e%T......
-00003590: 6c35 5d7d 9638 1728 8a3c b836 0b49 6c91  l5]}.8.(.<.6.Il.
-000035a0: cb74 4829 c951 d9f4 482f 1808 5794 090b  .tH).Q..H/..W...
-000035b0: 8488 ef06 5094 c4cb 3952 29e9 82cb 2d71  ....P...9R)...-q
-000035c0: 7a96 e821 4467 8ff1 6667 7992 34c5 23ac  z..!Dg..fgy.4.#.
-000035d0: f959 566c 14c2 7bf4 2055 a5a4 484f 7c24  .YVl..{. U..HO|$
-000035e0: c6fd a918 aa3c e2fd 70ca db0a 0347 fcbf  .....<..p....G..
-000035f0: 9ff2 2f21 caa0 fc89 a216 2785 89f5 3f0f  ../!......'...?.
-00003600: c1a9 77bb 81e8 9b99 5af3 26b4 2a3b c931  ..w.....Z.&.*;.1
-00003610: 93ae b1d8 37f7 ebd5 6ec0 a697 e3e9 68f8  ....7...n.....h.
-00003620: edf6 eae6 9a86 ae76 ed3c 383f 77ad 4d03  .......v.<8?w.M.
-00003630: da01 8fd6 37b8 8418 690f f6e0 7d08 2e1c  ....7...i...}...
-00003640: 8242 d30e 4db5 b09b 6e6f f0c3 13ae 5544  .B..M...no....UD
-00003650: ca9c f6b3 d162 54b0 3bad 0733 d245 2dd1  .....bT.;..3.E-.
-00003660: 831f b40c af7e b004 590b 4b9e 4ab2 9cef  .....~..Y.K.J...
-00003670: 7d73 feb5 e0ff 80d8 afe6 5284 b522 a51a  }s........R.."..
-00003680: 2a12 3abc b8a1 010f fdac f706 3adf 95b4  *.:.........:...
-00003690: 7288 ce74 c79a 7e11 1092 03dd 57ce e1de  r..t..~.....W...
-000036a0: 48bb b6ff eb14 7f01 504b 0304 1400 0000  H.......PK......
-000036b0: 0800 8b8a 6f58 bc72 e0e6 ff01 0000 8104  ....oX.r........
-000036c0: 0000 1900 0000 786c 2f77 6f72 6b73 6865  ......xl/workshe
-000036d0: 6574 732f 7368 6565 7431 392e 786d 6c7d  ets/sheet19.xml}
-000036e0: 54db 6edb 300c fd15 43cf 4195 14eb 0581  T.n.0...C.A.....
-000036f0: 63a0 49da a5c0 0214 2dda 3d16 8a4c c742  c.I.....-.=..L.B
-00003700: 749b 44cf ebdf 8fb2 9334 dd92 3c59 3ce2  t.D......4..<Y<.
-00003710: 2179 44d2 79eb c226 d600 98fd 31da c609  !yD.y..&....1...
-00003720: ab11 fd98 f328 6b30 225e 380f 966e 2a17  .....(k0"^8..n*.
-00003730: 8c40 32c3 9a47 1f40 941d c968 7e39 1c5e  .@2..G.@...h~9.^
-00003740: 7323 9465 45de 614f a1c8 5d83 5a59 780a  s#.eE.aO..].ZYx.
-00003750: 596c 8c11 e163 0ada b513 3662 3be0 59ad  Yl...c....6b;.Y.
-00003760: 6bec 005e e45e ace1 05f0 d513 814c be8f  k..^.^.......L..
-00003770: 532a 0336 2a67 b300 d584 dd8d c68b 9ed1  S*.6*g..........
-00003780: 79bc 2968 e3c1 394b 6256 ce6d 92f1 584e  y.)h..9KbV.m..XN
-00003790: d830 d504 1a24 a610 823e bf61 065a a748  .0...$...>.a.Z.H
-000037a0: 54c9 af6d 50f6 9934 310f cfbb f00f 9d7e  T..mP..41......~
-000037b0: 2a6f 2522 cc9c fea9 4aac 27ec 9665 2554  *o%"....J.'..e%T
-000037c0: a2d1 f8ec da05 6c35 5d7d 9638 1728 8a3c  ......l5]}.8.(.<
-000037d0: b836 0b49 6c91 cb74 4829 c951 d9f4 482f  .6.Il..tH).Q..H/
-000037e0: 1808 5794 090b 8488 ef06 5094 c4cb 3952  ..W.......P...9R
-000037f0: 29e9 82cb 2d71 7a96 e821 4467 8ff1 6667  )...-qz..!Dg..fg
-00003800: 7992 34c5 23ac f959 566c 14c2 7bf4 2055  y.4.#..YVl..{. U
-00003810: a5a4 484f 7c24 c6fd a918 aa3c e2fd 70ca  ..HO|$.....<..p.
-00003820: db0a 0347 fcbf 9ff2 2f21 caa0 fc89 a216  ...G..../!......
-00003830: 2785 89f5 3f0f c1a9 77bb 81e8 9b99 5af3  '...?...w.....Z.
-00003840: 26b4 2a3b c931 93ae b1d8 37f7 ebd5 6ec0  &.*;.1....7...n.
-00003850: a697 e3e9 68f8 edf6 eae6 9a86 ae76 ed3c  ....h........v.<
-00003860: 383f 77ad 4d03 da01 8fd6 37b8 8418 690f  8?w.M.....7...i.
-00003870: f6e0 7d08 2e1c 8242 d30e 4db5 b09b 6e6f  ..}....B..M...no
-00003880: f0c3 13ae 5544 ca9c f6b3 d162 54b0 3bad  ....UD.....bT.;.
-00003890: 0733 d245 2dd1 831f b40c af7e b004 590b  .3.E-......~..Y.
-000038a0: 4b9e 4ab2 9cef 7d73 feb5 e0ff 80d8 afe6  K.J...}s........
-000038b0: 5284 b522 a51a 2a12 3abc b8a1 010f fdac  R.."..*.:.......
-000038c0: f706 3adf 95b4 7288 ce74 c79a 7e11 1092  ..:...r..t..~...
-000038d0: 03dd 57ce e1de 48bb b6ff eb14 7f01 504b  ..W...H.......PK
-000038e0: 0304 1400 0000 0800 8b8a 6f58 4f5c d595  ..........oXO\..
-000038f0: 6901 0000 e702 0000 1900 0000 786c 2f77  i...........xl/w
-00003900: 6f72 6b73 6865 6574 732f 7368 6565 7432  orksheets/sheet2
-00003910: 302e 786d 6c75 52d9 4ec3 400c fc95 683f  0.xmluR.N.@...h?
-00003920: 806d 9138 5425 91e8 81e0 01a9 6a05 3c56  .m.8T%......j.<V
-00003930: dbc4 4956 dd23 785d 027f 8f37 3d85 daa7  ..IV.#x]...7=...
-00003940: d8de 99b1 3d71 da79 dc84 0680 921f 6b5c  ....=q.y......k\
-00003950: c844 43d4 8ea4 0c45 0356 851b df82 e397  .DC....E.V......
-00003960: caa3 55c4 29d6 32b4 08aa ec49 d6c8 dbc1  ..U.).2....I....
-00003970: e05e 5aa5 9dc8 d3be 36c7 3cf5 5b32 dac1  .^Z.....6.<.[2..
-00003980: 1c93 b0b5 56e1 ef18 8cef 3231 1487 c242  ....V.....21...B
-00003990: d70d f505 99a7 adaa 6109 f4de 3281 5379  ........a...2.Sy
-000039a0: d429 b505 17b4 7709 4295 89a7 e168 b663  .)....w.B....h.c
-000039b0: f488 0f0d 5d38 8b93 b8cc dafb 4d4c 5ecb  ....]8......ML^.
-000039c0: 4c0c e24c 60a0 a028 a1f8 f30d 1330 262a  L..L`..(.....0&*
-000039d0: f124 5f7b 5171 6a1a 99e7 f141 feb9 df9f  .$_{Qqj....A....
-000039e0: c75b ab00 136f 3e75 494d 261e 4552 42a5  .[...o>uIM&.ERB.
-000039f0: b686 16be 7b81 fd4e 77a7 11a7 8a54 9ea2  ....{..Nw....T..
-00003a00: ef12 8ccb e669 1183 d892 81da 4593 9684  .....i......E...
-00003a10: 5cd7 dc89 7282 402b dcba 55ab 5059 20c0  \...r.@+..U.PY .
-00003a20: 904a e281 e2b3 2cf6 f4f1 35ba 2e2f a027  .J....,...5../.'
-00003a30: d7d0 8e3b 5cc0 4faf e14b 0805 ea36 7a79  ...;\.O..K...6zy
-00003a40: 8136 bbba 93aa ff2d 21d9 8f83 c93b 83e2  .6.....-!....;..
-00003a50: 01bc 29ac b50b 8981 8a75 0637 0f6c 23ee  ..)......u.7.l#.
-00003a60: 1cdd 25e4 dbfe 60d6 9ec8 db3e 6cf8 1001  ..%...`....>l...
-00003a70: 2380 df2b efe9 98c4 3f7a bced fc0f 504b  #..+....?z....PK
-00003a80: 0304 1400 0000 0800 8b8a 6f58 7d51 27cc  ..........oX}Q'.
-00003a90: ea01 0000 4504 0000 1900 0000 786c 2f77  ....E.......xl/w
-00003aa0: 6f72 6b73 6865 6574 732f 7368 6565 7432  orksheets/sheet2
-00003ab0: 312e 786d 6c85 544d 6fdb 300c fd2b 86ce  1.xml.TMo.0..+..
-00003ac0: 4395 14eb 0702 c7c0 92b4 5d0f 058a 166b  C.........]....k
-00003ad0: 8f81 62d3 b110 59d2 447a 5eff fd28 3949  ..b...Y.Dz^..(9I
-00003ae0: 132c d92e 36f9 c447 3d9a a4f3 de85 0d36  .,..6..G=......6
-00003af0: 0094 fd6e 8dc5 a968 88fc 444a 2c1b 6815  ...n...h..DJ,.h.
-00003b00: 5e38 0f96 4f6a 175a 45ec 86b5 441f 4055  ^8..Oj.ZE...D.@U
-00003b10: 89d4 1a79 391a 5dcb 5669 2b8a 3c61 cfa1  ...y9.].Vi+.<a..
-00003b20: c85d 4746 5b78 0e19 766d abc2 c70c 8ceb  .]GF[x..vm......
-00003b30: a762 2c76 c08b 5e37 9400 59e4 5ead e115  .b,v..^7..Y.^...
-00003b40: e887 6702 bb72 9fa7 d22d 58d4 ce66 01ea  ..g..r...-X..f..
-00003b50: a9f8 369e 3c0c 8c14 f1a6 a1c7 033b 8bc5  ..6.<........;..
-00003b60: ac9c db44 e7b1 9a8a 51d4 0406 4a8a 2914  ...D....Q...J.).
-00003b70: bf7e c11c 8c89 9958 c9cf 6d52 f179 6964  .~.....X..mR.yid
-00003b80: 1eda bbf4 f7a9 7e96 b752 0873 67de 7545  ......~..R.sg.uE
-00003b90: cd54 dc8a ac82 5a75 865e 5cff 1db6 355d  .T....Zu.^\...5]
-00003ba0: 7d4a 5c28 5245 1e5c 9f85 586c 9197 d188  }J\(RE.\..Xl....
-00003bb0: 5772 a0b6 f123 bd52 605c f34d 5410 202d  Wr...#.R`\.MT. -
-00003bc0: b1d3 044b 5de5 9258 4a3c 90e5 9638 fb27  ...K]..XJ<...8.'
-00003bd0: b164 6d27 48f3 ff92 9601 906b 38c1 5d9c  .dm'H......k8.].
-00003be0: e39e 9477 772e daaa f694 b2fb 73f1 1560  ...ww.......s..`
-00003bf0: 19b4 8f6d 3b41 7b38 5b90 5ae3 71bc e44f  ...m;A{8[.Z.q..O
-00003c00: bfeb e7d0 8b8a 9f6f ca68 7e73 76cc 4ad7  .......o.h~sv.J.
-00003c10: 591a 7a73 7cb4 9b8f f9e5 643e 1e7d bdbd  Y.zs|.....d>.}..
-00003c20: bab9 e699 695c bf08 ce2f 5c6f e37c 25e0  ....i\.../\o.|%.
-00003c30: d1fa 8e9e 0091 c778 0fde 85e0 c221 a80c  .......x.....!..
-00003c40: afc0 cc28 bb49 634f 1f9e 71a3 91f8 e6b8  ...(.IcO..q.....
-00003c50: 5e9d 51e3 42a4 9e78 8508 d597 64d7 4a9b  ^.Q.B..x....d.J.
-00003c60: 9d8d 1bed 3d54 2297 7b42 2e8f 55ff 05e0  ....=T".{B..U...
-00003c70: b05e 4f2a ac35 976b a0e6 6a47 1737 3ca4  .^O*.5.k..jG.7<.
-00003c80: 6198 d7c1 21e7 93ae 9523 726d 321b 5e73  a...!....#rm2.^s
-00003c90: 0831 80cf 6be7 68ef c47d d9ff 398a 3f50  .1..k.h..}..9.?P
-00003ca0: 4b03 0414 0000 0008 008b 8a6f 58d4 5695  K..........oX.V.
-00003cb0: de87 0100 008f 0300 0019 0000 0078 6c2f  .............xl/
-00003cc0: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
-00003cd0: 3232 2e78 6d6c 7d93 db4e c330 0c86 5fa5  22.xml}..N.0.._.
-00003ce0: ca03 900d 8983 a6b6 128c c3b8 409a 8680  ............@...
-00003cf0: cb29 6bdd 3622 87e2 7814 de1e a73b 8050  .)k.6"..x....;.P
-00003d00: cb55 6dc7 9fe3 3f76 d3ce e35b 6800 28f9  .Um...?v...[h.(.
-00003d10: b4c6 854c 3444 ed4c ca50 3460 5538 f12d  ...L4D.L.P4`U8.-
-00003d20: 383e a93c 5a45 ec62 2d43 8ba0 ca1e b246  8>.<ZE.b-C.....F
-00003d30: 9e4e 26e7 d22a ed44 9ef6 b125 e6a9 df92  .N&..*.D...%....
-00003d40: d10e 9698 84ad b50a bfae c1f8 2e13 5371  ..............Sq
-00003d50: 08ac 74dd 501f 9079 daaa 1a9e 809e 5b06  ..t.P..y......[.
-00003d60: d895 c73a a5b6 e082 f62e 41a8 3271 359d  ...:......A.2q5.
-00003d70: 2d76 449f f1a2 a10b bfec 248a d978 ff16  -vD.......$..x..
-00003d80: 9d87 3213 93d8 1318 2828 9650 fcf9 8039  ..2.....((.P...9
-00003d90: 1813 2b71 27ef fba2 e2e7 d248 feb6 0fe5  ..+q'......H....
-00003da0: ef7a fddc de46 0598 7bf3 aa4b 6a32 7129  .z...F..{..Kj2q)
-00003db0: 9212 2ab5 35b4 f2dd 02f6 9ace 7e5a bc51  ..*.5.......~Z.Q
-00003dc0: a4f2 147d 9760 149b a745 34e2 959c a85d  ...}.`...E4....]
-00003dd0: 7ca4 2742 8e6b be89 7282 406b dc3a 07b8  |.'B.k..r.@k.:..
-00003de0: 76ca 422a 89bb 8967 b2d8 b3d7 ffb2 e048  v.B*...g.......H
-00003df0: 9386 3000 ceff 050b d6b5 4608 2c65 08be  ..0.......F.,e..
-00003e00: 1985 7942 8194 6d07 a0db 3148 9703 d977  ..yB..m...1H...w
-00003e10: 63d9 230f 713f 965f 4228 50b7 71e6 03d8  c.#.q?._B(P.q...
-00003e20: 6254 89aa ff28 973c b7c3 32ec 0619 17f5  bT...(.<..2.....
-00003e30: 5161 ad5d 480c 545c 6772 72c1 e3c6 dde4  Qa.]H.T\grr.....
-00003e40: 770e f9b6 5fec 8d27 f2b6 371b fe61 0063  w..._..'..7..a.c
-00003e50: 029f 57de d3d1 899b 77fc 07f3 6f50 4b03  ..W.....w...oPK.
-00003e60: 0414 0000 0008 008b 8a6f 58c4 ce01 8a6c  .........oX....l
-00003e70: 0100 000f 0300 0019 0000 0078 6c2f 776f  ...........xl/wo
-00003e80: 726b 7368 6565 7473 2f73 6865 6574 3233  rksheets/sheet23
-00003e90: 2e78 6d6c 7553 db6e 8330 0cfd 1594 0f58  .xmluS.n.0.....X
-00003ea0: e8a4 5d54 01d2 daae da1e 2655 adb6 3d56  ..]T......&U..=V
-00003eb0: 2918 889a 0b4b dcb1 fdfd 1ce8 4d13 3c61  )....K......M.<a
-00003ec0: 3be7 1cfb 3821 69ad dbfb 1a00 a31f ad8c  ;...8!i.........
-00003ed0: 4f59 8dd8 4c39 f779 0d5a f81b db80 a193  OY..L9.y.Z......
-00003ee0: d23a 2d90 5257 71df 3810 4547 d28a dfc6  .:-.RWq.8.EG....
-00003ef0: f13d d742 1a96 255d 6de5 b2c4 1e50 4903  .=.B..%]m....PI.
-00003f00: 2b17 f983 d6c2 fdce 40d9 3665 1376 2aac  +.......@.6e.v*.
-00003f10: 6555 6357 e059 d288 0a36 80ef 0d11 28e5  eUcW.Y...6....(.
-00003f20: 679d 426a 305e 5a13 3928 53f6 3499 2e7b  g.Bj0^Z.9(S.4..{
-00003f30: 4687 f890 d0fa ab38 0a66 76d6 ee43 f25a  F......8.fv..C.Z
-00003f40: a42c 0e33 8182 1c83 84a0 cf37 cc41 a9a0  .,.3.......7.A..
-00003f50: 4493 7c1d 45d9 a569 605e c727 f965 e79f  D.|.E..i`^.'.e..
-00003f60: c6db 090f 73ab 3e65 8175 ca1e 5954 4029  ....s.>e.u..YT@)
-00003f70: 0e0a d7b6 7d81 a3a7 bbcb 880b 8122 4b9c  ....}........"K.
-00003f80: 6d23 17cc 6649 1e82 d092 80d2 8425 6dd0  m#..fI.......%m.
-00003f90: 515d 5227 cc10 3c6e 736a b195 45c2 9126  Q]R'..<nsj..E..&
-00003fa0: 0975 9e1f 79b3 315e b3f7 03f0 f918 7c50  .u..y.1^......|P
-00003fb0: 7c31 8636 42c3 00fe 790c 5f80 cf9d 6cc2  |1.6B...y._...l.
-00003fc0: ce07 68cb 51ef a2fa 6782 d3de 4e97 d12f  ..h.Q...g...N../
-00003fd0: 323c 9437 e12a 697c a4a0 249d f8e6 81d6  2<.7.*i|..$.....
-00003fe0: edfa cdf7 09da a67b 583b 8b68 7517 d6f4  .......{X;.hu...
-00003ff0: 60c1 0500 9d97 d6e2 3909 377f fe07 b23f  `.......9.7....?
-00004000: 504b 0304 1400 0000 0800 8b8a 6f58 1b56  PK..........oX.V
-00004010: 7ebc 9c01 0000 0d04 0000 1900 0000 786c  ~.............xl
-00004020: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
-00004030: 7432 342e 786d 6c7d 94db 6adc 3010 865f  t24.xml}..j.0.._
-00004040: c5e8 01a2 4da1 0782 6d68 364d 9386 4248  ....M...mh6M..BH
-00004050: 687a 59b4 f6d8 162b 69d4 d16c 9cbe 7d25  hzY....+i..l..}%
-00004060: ef21 2948 bdf2 ccf8 ff46 33e6 97eb 1969  .!)H.....F3....i
-00004070: 1b26 00ae 5eac 71a1 1113 b3bf 9032 7413  .&..^.q......2t.
-00004080: 5815 ced0 838b 6f06 24ab 38a6 34ca e009  X.....o.$.8.4...
-00004090: 54bf 40d6 c877 abd5 0769 9576 a2ad 97da  T.@..w...i.v....
-000040a0: 3db5 35ee d868 07f7 5485 9db5 8afe 5c82  =.5..h..T.....\.
-000040b0: c1b9 11e7 e258 78d0 e3c4 4b41 b6b5 5723  .....Xx...KA..W#
-000040c0: 3c02 fff0 1188 a93c f5e9 b505 1734 ba8a  <......<.....4..
-000040d0: 6068 c4e7 f38b bb3d b128 9e34 cce1 4d5c  `h.....=.(.4..M\
-000040e0: a565 3688 db94 dcf6 8d58 a599 c040 c7a9  .e6......X...@..
-000040f0: 858a 8f67 5883 31a9 539c e4f7 a1a9 783d  ...gX.1.S.....x=
-00004100: 3491 6fe3 63fb eb65 ff38 de46 0558 a3f9  4.o.c..e.8.F.X..
-00004110: a97b 9e1a f149 543d 0c6a 67f8 01e7 1b38  .{...IT=.jg....8
-00004120: ecf4 fe75 c42b c5aa ad09 e78a d2b2 6ddd  ...u.+........m.
-00004130: a520 1d19 85da a58f f4c8 14eb 3a9e c4ad  . ..........:...
-00004140: 5704 8e7f f96d 2d39 8e91 8ab2 3b40 9725  W....m-9....;@.%
-00004150: c802 8dd0 e7a1 7509 52a4 4624 9741 aefe  ......u.R.F$.A..
-00004160: 83bc 64f4 5f4a fa9d 0bd0 1170 86b9 2e31  ..d._J.....p...1
-00004170: 1b86 8cfc 6b49 aead 277c d66e cc40 3745  ....kI..'|.n.@7E
-00004180: a8cf a86f 4b6a a76c 6ea4 6f25 7d0f a123  ...oKj.ln.o%}..#
-00004190: ed93 e332 d85d 0963 3586 7ff5 32ba e668  ...2.].c5...2..h
-000041a0: c5bd 8dd2 35f9 ae68 d42e 5406 86d8 6775  ....5..h..T...gu
-000041b0: f631 9a8d f6be db27 8c7e b956 1b64 46bb  .1.....'.~.V.dF.
-000041c0: 8453 bcae 4049 10df 0f88 7c4a 92ef 4f7f  .S..@I....|J..O.
-000041d0: 80f6 2f50 4b03 0414 0000 0008 008b 8a6f  ../PK..........o
-000041e0: 58d2 05f1 4652 0200 0047 0a00 000d 0000  X...FR...G......
-000041f0: 0078 6c2f 7374 796c 6573 2e78 6d6c dd56  .xl/styles.xml.V
-00004200: db8a db30 10fd 15e3 0fa8 9398 9ab8 2479  ...0..........$y
-00004210: a821 5068 cbc2 ee43 5fe5 584e 04ba b8b2  .!Ph...C_.XN....
-00004220: bc24 fdfa 6a24 e7b6 9be3 52fa 569b e099  .$..j$....R.V...
-00004230: 393a 3367 a431 ceaa 7727 c99f 0f9c bbe4  9:3g.1..w'......
-00004240: a8a4 eed7 e9c1 b9ee 5396 f5bb 0357 acff  ........S....W..
-00004250: 603a ae3d d21a ab98 f3ae dd67 7d67 396b  `:.=.......g}g9k
-00004260: 7a22 2999 2d66 b322 534c e874 b3d2 83da  z").-f."SL.t....
-00004270: 2ad7 273b 3368 b74e 6769 926d 56ad d1d7  *.';3h.Ngi.mV...
-00004280: d03c 8d01 bf96 299e bc32 b94e 2b26 456d  .<....)..2.N+&Em
-00004290: 455c cc94 90a7 185f 84c8 ce48 6313 e7d5  E\....._...Hc...
-000042a0: 70a2 53a8 ff15 17cc 4797 a48e b994 d0c6  p.S.....G.......
-000042b0: 8668 16cb 8447 ef13 0b29 2f2a 1669 0c6c  .h...G...)/*.i.l
-000042c0: 561d 738e 5bbd f54e 2485 e87b 6cb4 5f4e  V.s.[..N$..{l._N
-000042d0: 9d57 b1b7 ec34 5f7c 4c6f 18e1 e1cb d4c6  .W...4_|Lo......
-000042e0: 36dc deb5 1b43 9b95 e4ad 2386 15fb 4330  6....C....#...C0
-000042f0: 9ce9 e851 1be7 8c22 ab11 6c6f 348b 4ace  ...Q..."..lo4.J.
-00004300: b4d1 f0b9 775c ca67 3aaf 1fed 5d81 639b  ....w\.g:...].c.
-00004310: c48d ffd2 843d a78e cfa6 5735 9a31 cde8  .....=....W5.1..
-00004320: 5081 db74 31f9 bfe7 edc4 ab71 9f07 df90  P..t1......q....
-00004330: 0efe cfc1 38fe 6479 2b8e c13f b66f 045c  ....8.dy+..?.o.\
-00004340: 6a07 2577 e52f d184 4665 9d7e a711 9437  j.%w./..Fe.~...7
-00004350: 39ea 4148 27f4 e81d 44d3 70fd be3b 9fdf  9.AH'...D.p..;..
-00004360: b1da 0ff9 5d01 bfaa e12d 1ba4 7bb9 80eb  ....]....-..{...
-00004370: f46a 7fe3 8d18 5479 59f5 448d 8dab aef6  .j....TyY.D.....
-00004380: 573a ca79 719d 535f 4ce8 861f 7953 8dae  W:.yq.S_L...yS..
-00004390: ddd7 c14c bce1 cb8e 5760 bc85 b6e1 0210  ...L....W`......
-000043a0: 6445 1040 04c2 5a50 0664 451e acf5 3ff6  dE.@..ZP.dE...?.
-000043b0: b5c4 7d45 102a 5c3e 8696 98b5 c4ac c87b  ..}E.*\>.......{
-000043c0: 0855 e186 b500 abf4 1768 b92c f3bc 28e0  .U.......h.,..(.
-000043d0: f656 d563 1915 dcc3 a2a0 1f48 0815 1207  .V.c.......H....
-000043e0: d6a2 6a7f bbf3 1303 3031 367f 980d 78ca  ..j.....016...x.
-000043f0: 9363 035b 9e18 51d8 f2c4 ce13 04f6 9038  .c.[..Q........8
-00004400: 6509 0600 d622 0e3c 1438 5124 02d4 a251  e....".<.8Q$...Q
-00004410: 03ac 3ca7 7386 0ae1 6b3e 0195 2584 6848  ..<.s...k>..%.hH
-00004420: c1f4 1605 daa8 826e 705e f025 caf3 b204  .......np^.%....
-00004430: 1081 4046 9e43 885e d809 08ca 2021 10ca  ..@F.C.^.... !..
-00004440: f3f8 217d f33d cbce dfb9 ecfa d771 f31b  ..!}.=.......q..
-00004450: 504b 0304 1400 0000 0800 8b8a 6f58 b747  PK..........oX.G
-00004460: eb8a c000 0000 1602 0000 0b00 0000 5f72  .............._r
-00004470: 656c 732f 2e72 656c 739d 924b 6e02 310c  els/.rels..Kn.1.
-00004480: 40af 1265 5f4c a9c4 0231 acd8 b043 880b  @..e_L...1...C..
-00004490: b889 e7a3 99c4 9163 c4f4 f68d d8c0 2068  .......c...... h
-000044a0: 114b ff9e 9e2d af0f 34a0 761c 73db a56c  .K...-..4.v.s..l
-000044b0: c630 c45c d956 35ad 00b2 6b29 609e 71a2  .0.\.V5...k)`.q.
-000044c0: 582a 354b 402d a134 90d0 f5d8 102c e6f3  X*5K@-.4.....,..
-000044d0: 25c8 2dc3 6ed6 b74c 73fc 49f4 0a91 ebba  %.-.n..Ls.I.....
-000044e0: 73b4 6577 0a14 f501 f8ae c39a 234a 435a  s.ew........#JCZ
-000044f0: d971 8033 4bff cddc cf0a d49a 9daf acec  .q.3K...........
-00004500: fca7 35f0 a6cc f3f5 2090 a247 4570 2cf4  ..5..... ..GEp,.
-00004510: 91a4 4c8b 7694 af3e 9edd bea4 f3a5 6362  ..L.v..>......cb
-00004520: b478 dfe8 fff3 d0a8 143d f9bf 9d30 a589  .x.......=...0..
-00004530: d2d7 4509 266f b0f9 0550 4b03 0414 0000  ..E.&o...PK.....
-00004540: 0008 008b 8a6f 5821 0fd9 4c7b 0200 00e5  .....oX!..L{....
-00004550: 0800 000f 0000 0078 6c2f 776f 726b 626f  .......xl/workbo
-00004560: 6f6b 2e78 6d6c 8d96 6d4f db30 1080 ff4a  ok.xml..mO.0...J
-00004570: 951f b034 8196 1751 24d6 3240 6cb4 2388  ...4...Q$.2@l.#.
-00004580: ef57 e7d2 9c70 ecc8 76e8 c6af 9f9d 5048  .W...p..v.....PH
-00004590: ebcc dba7 d467 ebe9 5dfc 9c9d 8bad 542f  .....g..].....T/
-000045a0: 6b29 5f46 bf2a 2ef4 b99a 45a5 31f5 791c  k)_F.*....E.1.y.
-000045b0: 6b56 6205 fa8b ac51 d8b9 42aa 0a8c 1daa  kVb....Q..B.....
-000045c0: 4d2c 8b82 182e 246b 2a14 264e c7e3 69ac  M,....$k*.&N..i.
-000045d0: 9083 2129 7449 b58e 3ada ffb0 74ad 1072  ..!)tI..:...t..r
-000045e0: 5d22 9a8a 77a8 0a48 4497 17bb cc56 6a14  ]"..w..HD....Vj.
-000045f0: f747 d220 73ff e4a2 2ef2 4cb8 d59f 0bdc  .G. s.....L.....
-00004600: 70f4 4a9a d6c4 c9fc 9e45 ed6f 8ed1 a822  p.J......E.o..."
-00004610: 4115 bd61 3e8b c6d1 4897 727b 2b15 bd49  A..a>...H.r{+..I
-00004620: 6180 674c 49ce 6751 d24d 3ca3 32c4 bc70  a.gLI.gQ.M<.2..p
-00004630: e6d2 7c82 b56e 2306 d68f aee6 5934 1d5b  ..|..n#.....Y4.[
-00004640: 6041 4a9b 7645 cb07 9be4 2bda c5dd a831  `AJ.vE....+....1
-00004650: f21b 7183 6a01 066f 946c 6a12 9b16 63cb  ..q.j..o.lj...c.
-00004660: 887b 75b4 af62 f71c 09a8 7016 3da1 36d7  .{u..b....p.=.6.
-00004670: c2d8 7256 a06c c462 5c42 76c1 5dde 2567  ..rV.l.b\Bv.].%g
-00004680: 2cb5 57aa 3a27 3ba1 eef2 8edf 67fd 6c80  ,.W.:';.....g.l.
-00004690: 5341 7b84 3440 483d 82cb e607 1ac8 c140  SA{.4@H=.......@
-000046a0: 0f72 1480 1c0d 42ae b446 d323 1c07 08c7  .r....B..F.#....
-000046b0: 1ee1 8a31 ac0d 0886 43ac 4980 3519 cce6  ...1....C.I.5...
-000046c0: 3adf e062 bfa4 6900 32f5 202b 854c 8a9c  :..b..i.2. +.L..
-000046d0: 9c9c 3dc8 4900 7232 98c9 1c34 f600 a701  ..=.I.r2...4....
-000046e0: c0e9 3f5e cb01 ea2c 803a 1b52 c549 07ad  ..?^...,.:.R.I..
-000046f0: c83e 2c19 87c4 1b7b b8b9 ac6a 4e7f c92c  .>,....{...jN..,
-00004700: 095a ec6b 7c2f e496 a3dd b21b 0575 f900  .Z.k|/.......u..
-00004710: afb4 69cf 9f21 7448 efc4 f77b 29f0 56d6  ..i..!tH...{).V.
-00004720: 43a0 90e2 c9b0 e359 4306 b31a 99ed 3906  C......YC.....9.
-00004730: 076a 2421 e313 5ff9 0f60 9f11 323d f155  .j$!.._..`..2=.U
-00004740: dff7 c3a3 8594 4f7c e7bf a260 6505 ea65  ......O|...`e..e
-00004750: 1016 523f f1dd cf6c 5a39 a85c ef9b e261  ..R?...lZ9.\...a
-00004760: 430d 91f8 1df1 b99f 1e29 d40f 89df 108e  C........)......
-00004770: f1d8 0881 6a2e 4541 9b46 1dee 681a ea89  ....j.EA.F..h...
-00004780: d4ef 899d 658f a81b de3f bfd2 503f a47e  ....e....?..P?.~
-00004790: 3fbc a796 a1d6 0719 050f f7e1 d37d d998  ?............}..
-000047a0: bad9 cb26 647e 3a6c 7e57 d2ea 3edb 3b97  ...&d~:l~W..>.;.
-000047b0: d390 f269 a77c bcbb 0373 2c48 60fe 6099  ...i.|...s,H`.`.
-000047c0: da4d d81b 99d9 cf01 f7e8 1afb 78e2 76a9  .M..........x.v.
-000047d0: 6838 9fdb d852 7c97 907f 5caa bb2f 82cb  h8...R|...\../..
-000047e0: 3f50 4b03 0414 0000 0008 008b 8a6f 5872  ?PK..........oXr
-000047f0: 967e 9137 0100 0039 0f00 001a 0000 0078  .~.7...9.......x
-00004800: 6c2f 5f72 656c 732f 776f 726b 626f 6f6b  l/_rels/workbook
-00004810: 2e78 6d6c 2e72 656c 73cd d741 8e82 3014  .xml.rels..A..0.
-00004820: c6f1 ab90 1ec0 f2aa a24e c495 1bb7 132f  .........N...../
-00004830: d0e0 1388 4049 dbc9 e8ed 87c8 023f 328b  ....@I.......?2.
-00004840: d998 792b d212 1eff 45f3 0bec 3fb9 b1b1  ..y+....E...?...
-00004850: 765d a8ea 3e24 f7b6 e942 aeaa 18fb 0fad  v]..>$...B......
-00004860: 4351 716b c3c2 f5dc 0d77 aece b736 0e4b  CQqk.....w...6.K
-00004870: 5fea de16 375b b236 699a 69ff 3a43 1df6  _...7[.6i.i.:C..
-00004880: af33 93f3 a3e7 bf4c 74d7 6b5d f0d1 155f  .3.....Lt.k]..._
-00004890: 2d77 f197 c1fa dbf9 5ba8 98a3 4ace d697  -w......[...J...
-000048a0: 1c73 a5ef cdb4 1df4 f342 8b61 b24a 4e97  .s.......B.a.JN.
-000048b0: 5cf9 d385 54a2 ffbb c840 9111 50b4 84a2  \...T....@..P...
-000048c0: a580 a215 14ad 0414 ada1 682d a028 83a2  ..........h-.(..
-000048d0: 4c40 d106 8a36 028a b650 b415 50b4 83a2  L@...6...P..P...
-000048e0: 9d80 224a 91c8 5442 d38c 6d09 6e13 c24d  .."J..TB..m.n..M
-000048f0: 12e4 26a4 9b24 d84d 8837 49d0 9b90 6f92  ..&..$.M.7I...o.
-00004900: e037 21e0 2441 7042 c249 82e1 8488 9304  .7!.$ApB.I......
-00004910: c509 1927 098e 1b74 dc48 70dc a0e3 4682  ...'...t.Hp...F.
-00004920: e366 f601 2ec1 7183 8e1b 098e 1b74 dcbc  .f....q......t..
-00004930: d5f1 101f 0d87 2968 5c63 c05b d18e c3b3  ......)h\c.[....
-00004940: 3cbd ffb9 1c37 6747 7864 5ac3 9ff2 e107  <....7gGxdZ.....
-00004950: 504b 0304 1400 0000 0800 8b8a 6f58 8b1a  PK..........oX..
-00004960: e4a4 7101 0000 3510 0000 1300 0000 5b43  ..q...5.......[C
-00004970: 6f6e 7465 6e74 5f54 7970 6573 5d2e 786d  ontent_Types].xm
-00004980: 6ccd 98cb 6ec2 3010 457f 25ca 1611 63b7  l...n.0.E.%...c.
-00004990: a50f 019b b6db 9645 7fc0 4d26 c4c2 2f79  .......E..M&../y
-000049a0: 0c85 bfaf 130a 522b ca43 54ea 6c62 259e  ......R+.CT.lb%.
-000049b0: b9f7 c623 1d29 19bd ad3d 60b6 32da e238  ...#.)...=`.2..8
-000049c0: 6f62 f40f 8c61 d980 9158 380f 36ed d42e  ob...a...X8.6...
-000049d0: 1819 d36d 9831 2fcb b99c 0113 83c1 9095  ...m.1/.........
-000049e0: ce46 b0b1 1f5b 8d7c 327a 825a 2e74 cc9e  .F...[.|2z.Z.t..
-000049f0: 57e9 312a 67c7 7900 8d79 f6b8 296c bdc6  W.1*g.y..y..)l..
-00004a00: b9f4 5eab 52c6 b4cf 96b6 fae1 d2ff 7228  ..^.R.........r(
-00004a10: 5267 5783 8df2 d84b 0579 c6f6 5a74 5bbf  RgW....K.y..Zt[.
-00004a20: 3a6c 1b5f 9710 82aa 209b ca10 5fa4 4965  :l._.... ..._.Ie
-00004a30: 6ca5 19c6 b506 2c0e 6bec 49e9 ea5a 9550  l.....,.k.I..Z.P
-00004a40: b972 6152 4b81 3e80 acb0 0188 4617 1bd1  .raRK.>.....F...
-00004a50: de11 eb98 0e19 3657 7e71 804e e6a0 632a  ......6W~q.N..c*
-00004a60: 9d06 e731 4d2d c0f9 7edb b1b4 dd7d 9f84  ...1M-..~....}..
-00004a70: 2044 75e4 2577 9649 fbe2 3784 76e2 1554   Du.%w.I..7.v..T
-00004a80: a79a a713 fe70 61de cd04 59b7 5c7e ccdf  .....pa...Y.\~..
-00004a90: e7bc d33f 3788 a012 e48a 4a90 6b2a 416e  ...?7.....J.k*An
-00004aa0: a804 1952 0972 4b25 c81d 9520 f754 82f0  ...R.rK%... .T..
-00004ab0: 0199 2464 d8ca c9c0 9593 a12b 2783 574e  ..$d.......+'.WN
-00004ac0: 86af 9c0c 6039 19c2 7232 88e5 6418 2bc8  ....`9..r2..d.+.
-00004ad0: 3056 9061 ac20 c358 4186 b1e2 5f19 fbee  0V.a. .XA..._...
-00004ae0: dcfc afbf 62db b530 52d9 5d00 d6fd 2d98  ....b..0R.]...-.
-00004af0: 7c02 504b 0102 1403 1400 0000 0800 8b8a  |.PK............
-00004b00: 6f58 465a c10c 8200 0000 b100 0000 1000  oXFZ............
-00004b10: 0000 0000 0000 0000 0000 8001 0000 0000  ................
-00004b20: 646f 6350 726f 7073 2f61 7070 2e78 6d6c  docProps/app.xml
-00004b30: 504b 0102 1403 1400 0000 0800 8b8a 6f58  PK............oX
-00004b40: 5fea 0ffc ec00 0000 cb01 0000 1100 0000  _...............
-00004b50: 0000 0000 0000 0000 8001 b000 0000 646f  ..............do
-00004b60: 6350 726f 7073 2f63 6f72 652e 786d 6c50  cProps/core.xmlP
-00004b70: 4b01 0214 0314 0000 0008 008b 8a6f 5899  K............oX.
-00004b80: 5c9c 2310 0600 009c 2700 0013 0000 0000  \.#.....'.......
-00004b90: 0000 0000 0000 0080 01cb 0100 0078 6c2f  .............xl/
-00004ba0: 7468 656d 652f 7468 656d 6531 2e78 6d6c  theme/theme1.xml
-00004bb0: 504b 0102 1403 1400 0000 0800 8b8a 6f58  PK............oX
-00004bc0: 0f95 4d33 4801 0000 4902 0000 1800 0000  ..M3H...I.......
-00004bd0: 0000 0000 0000 0000 8081 0c08 0000 786c  ..............xl
-00004be0: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
-00004bf0: 7431 2e78 6d6c 504b 0102 1403 1400 0000  t1.xmlPK........
-00004c00: 0800 8b8a 6f58 0f95 4d33 4801 0000 4902  ....oX..M3H...I.
-00004c10: 0000 1800 0000 0000 0000 0000 0000 8081  ................
-00004c20: 8a09 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
-00004c30: 732f 7368 6565 7432 2e78 6d6c 504b 0102  s/sheet2.xmlPK..
-00004c40: 1403 1400 0000 0800 8b8a 6f58 b111 5547  ..........oX..UG
-00004c50: 4002 0000 7805 0000 1800 0000 0000 0000  @...x...........
-00004c60: 0000 0000 8081 080b 0000 786c 2f77 6f72  ..........xl/wor
-00004c70: 6b73 6865 6574 732f 7368 6565 7433 2e78  ksheets/sheet3.x
-00004c80: 6d6c 504b 0102 1403 1400 0000 0800 8b8a  mlPK............
-00004c90: 6f58 e7b3 5928 fe02 0000 f009 0000 1800  oX..Y(..........
-00004ca0: 0000 0000 0000 0000 0000 8081 7e0d 0000  ............~...
-00004cb0: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
-00004cc0: 6565 7434 2e78 6d6c 504b 0102 1403 1400  eet4.xmlPK......
-00004cd0: 0000 0800 8b8a 6f58 2511 6947 cd03 0000  ......oX%.iG....
-00004ce0: 0c0f 0000 1800 0000 0000 0000 0000 0000  ................
-00004cf0: 8081 b210 0000 786c 2f77 6f72 6b73 6865  ......xl/workshe
-00004d00: 6574 732f 7368 6565 7435 2e78 6d6c 504b  ets/sheet5.xmlPK
-00004d10: 0102 1403 1400 0000 0800 8b8a 6f58 e7b3  ............oX..
-00004d20: 5928 fe02 0000 f009 0000 1800 0000 0000  Y(..............
-00004d30: 0000 0000 0000 8081 b514 0000 786c 2f77  ............xl/w
-00004d40: 6f72 6b73 6865 6574 732f 7368 6565 7436  orksheets/sheet6
-00004d50: 2e78 6d6c 504b 0102 1403 1400 0000 0800  .xmlPK..........
-00004d60: 8b8a 6f58 642f 605f 5801 0000 a802 0000  ..oXd/`_X.......
-00004d70: 1800 0000 0000 0000 0000 0000 8081 e917  ................
-00004d80: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
-00004d90: 7368 6565 7437 2e78 6d6c 504b 0102 1403  sheet7.xmlPK....
-00004da0: 1400 0000 0800 8b8a 6f58 5585 c684 f802  ........oXU.....
-00004db0: 0000 3f0a 0000 1800 0000 0000 0000 0000  ..?.............
-00004dc0: 0000 8081 7719 0000 786c 2f77 6f72 6b73  ....w...xl/works
-00004dd0: 6865 6574 732f 7368 6565 7438 2e78 6d6c  heets/sheet8.xml
-00004de0: 504b 0102 1403 1400 0000 0800 8b8a 6f58  PK............oX
-00004df0: 5585 c684 f802 0000 3f0a 0000 1800 0000  U.......?.......
-00004e00: 0000 0000 0000 0000 8081 a51c 0000 786c  ..............xl
-00004e10: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
-00004e20: 7439 2e78 6d6c 504b 0102 1403 1400 0000  t9.xmlPK........
-00004e30: 0800 8b8a 6f58 5585 c684 f802 0000 3f0a  ....oXU.......?.
-00004e40: 0000 1900 0000 0000 0000 0000 0000 8081  ................
-00004e50: d31f 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
-00004e60: 732f 7368 6565 7431 302e 786d 6c50 4b01  s/sheet10.xmlPK.
-00004e70: 0214 0314 0000 0008 008b 8a6f 5830 1316  ...........oX0..
-00004e80: 5e0d 0300 00b3 0a00 0019 0000 0000 0000  ^...............
-00004e90: 0000 0000 0080 8102 2300 0078 6c2f 776f  ........#..xl/wo
-00004ea0: 726b 7368 6565 7473 2f73 6865 6574 3131  rksheets/sheet11
-00004eb0: 2e78 6d6c 504b 0102 1403 1400 0000 0800  .xmlPK..........
-00004ec0: 8b8a 6f58 5585 c684 f802 0000 3f0a 0000  ..oXU.......?...
-00004ed0: 1900 0000 0000 0000 0000 0000 8081 4626  ..............F&
-00004ee0: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
-00004ef0: 7368 6565 7431 322e 786d 6c50 4b01 0214  sheet12.xmlPK...
-00004f00: 0314 0000 0008 008b 8a6f 5855 85c6 84f8  .........oXU....
-00004f10: 0200 003f 0a00 0019 0000 0000 0000 0000  ...?............
-00004f20: 0000 0080 8175 2900 0078 6c2f 776f 726b  .....u)..xl/work
-00004f30: 7368 6565 7473 2f73 6865 6574 3133 2e78  sheets/sheet13.x
-00004f40: 6d6c 504b 0102 1403 1400 0000 0800 8b8a  mlPK............
-00004f50: 6f58 2359 55fc e301 0000 0704 0000 1900  oX#YU...........
-00004f60: 0000 0000 0000 0000 0000 8081 a42c 0000  .............,..
-00004f70: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
-00004f80: 6565 7431 342e 786d 6c50 4b01 0214 0314  eet14.xmlPK.....
-00004f90: 0000 0008 008b 8a6f 58bc 72e0 e6ff 0100  .......oX.r.....
-00004fa0: 0081 0400 0019 0000 0000 0000 0000 0000  ................
-00004fb0: 0080 81be 2e00 0078 6c2f 776f 726b 7368  .......xl/worksh
-00004fc0: 6565 7473 2f73 6865 6574 3135 2e78 6d6c  eets/sheet15.xml
-00004fd0: 504b 0102 1403 1400 0000 0800 8b8a 6f58  PK............oX
-00004fe0: bc72 e0e6 ff01 0000 8104 0000 1900 0000  .r..............
-00004ff0: 0000 0000 0000 0000 8081 f430 0000 786c  ...........0..xl
-00005000: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
-00005010: 7431 362e 786d 6c50 4b01 0214 0314 0000  t16.xmlPK.......
-00005020: 0008 008b 8a6f 5895 3ba4 2f11 0100 00c8  .....oX.;./.....
-00005030: 0100 0019 0000 0000 0000 0000 0000 0080  ................
-00005040: 812a 3300 0078 6c2f 776f 726b 7368 6565  .*3..xl/workshee
-00005050: 7473 2f73 6865 6574 3137 2e78 6d6c 504b  ts/sheet17.xmlPK
-00005060: 0102 1403 1400 0000 0800 8b8a 6f58 bc72  ............oX.r
-00005070: e0e6 ff01 0000 8104 0000 1900 0000 0000  ................
-00005080: 0000 0000 0000 8081 7234 0000 786c 2f77  ........r4..xl/w
-00005090: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
-000050a0: 382e 786d 6c50 4b01 0214 0314 0000 0008  8.xmlPK.........
-000050b0: 008b 8a6f 58bc 72e0 e6ff 0100 0081 0400  ...oX.r.........
-000050c0: 0019 0000 0000 0000 0000 0000 0080 81a8  ................
-000050d0: 3600 0078 6c2f 776f 726b 7368 6565 7473  6..xl/worksheets
-000050e0: 2f73 6865 6574 3139 2e78 6d6c 504b 0102  /sheet19.xmlPK..
-000050f0: 1403 1400 0000 0800 8b8a 6f58 4f5c d595  ..........oXO\..
-00005100: 6901 0000 e702 0000 1900 0000 0000 0000  i...............
-00005110: 0000 0000 8081 de38 0000 786c 2f77 6f72  .......8..xl/wor
-00005120: 6b73 6865 6574 732f 7368 6565 7432 302e  ksheets/sheet20.
-00005130: 786d 6c50 4b01 0214 0314 0000 0008 008b  xmlPK...........
-00005140: 8a6f 587d 5127 ccea 0100 0045 0400 0019  .oX}Q'.....E....
-00005150: 0000 0000 0000 0000 0000 0080 817e 3a00  .............~:.
-00005160: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
-00005170: 6865 6574 3231 2e78 6d6c 504b 0102 1403  heet21.xmlPK....
-00005180: 1400 0000 0800 8b8a 6f58 d456 95de 8701  ........oX.V....
-00005190: 0000 8f03 0000 1900 0000 0000 0000 0000  ................
-000051a0: 0000 8081 9f3c 0000 786c 2f77 6f72 6b73  .....<..xl/works
-000051b0: 6865 6574 732f 7368 6565 7432 322e 786d  heets/sheet22.xm
-000051c0: 6c50 4b01 0214 0314 0000 0008 008b 8a6f  lPK............o
-000051d0: 58c4 ce01 8a6c 0100 000f 0300 0019 0000  X....l..........
-000051e0: 0000 0000 0000 0000 0080 815d 3e00 0078  ...........]>..x
-000051f0: 6c2f 776f 726b 7368 6565 7473 2f73 6865  l/worksheets/she
-00005200: 6574 3233 2e78 6d6c 504b 0102 1403 1400  et23.xmlPK......
-00005210: 0000 0800 8b8a 6f58 1b56 7ebc 9c01 0000  ......oX.V~.....
-00005220: 0d04 0000 1900 0000 0000 0000 0000 0000  ................
-00005230: 8081 0040 0000 786c 2f77 6f72 6b73 6865  ...@..xl/workshe
-00005240: 6574 732f 7368 6565 7432 342e 786d 6c50  ets/sheet24.xmlP
-00005250: 4b01 0214 0314 0000 0008 008b 8a6f 58d2  K............oX.
-00005260: 05f1 4652 0200 0047 0a00 000d 0000 0000  ..FR...G........
-00005270: 0000 0000 0000 0080 01d3 4100 0078 6c2f  ..........A..xl/
-00005280: 7374 796c 6573 2e78 6d6c 504b 0102 1403  styles.xmlPK....
-00005290: 1400 0000 0800 8b8a 6f58 b747 eb8a c000  ........oX.G....
-000052a0: 0000 1602 0000 0b00 0000 0000 0000 0000  ................
-000052b0: 0000 8001 5044 0000 5f72 656c 732f 2e72  ....PD.._rels/.r
-000052c0: 656c 7350 4b01 0214 0314 0000 0008 008b  elsPK...........
-000052d0: 8a6f 5821 0fd9 4c7b 0200 00e5 0800 000f  .oX!..L{........
-000052e0: 0000 0000 0000 0000 0000 0080 0139 4500  .............9E.
-000052f0: 0078 6c2f 776f 726b 626f 6f6b 2e78 6d6c  .xl/workbook.xml
-00005300: 504b 0102 1403 1400 0000 0800 8b8a 6f58  PK............oX
-00005310: 7296 7e91 3701 0000 390f 0000 1a00 0000  r.~.7...9.......
-00005320: 0000 0000 0000 0000 8001 e147 0000 786c  ...........G..xl
-00005330: 2f5f 7265 6c73 2f77 6f72 6b62 6f6f 6b2e  /_rels/workbook.
-00005340: 786d 6c2e 7265 6c73 504b 0102 1403 1400  xml.relsPK......
-00005350: 0000 0800 8b8a 6f58 8b1a e4a4 7101 0000  ......oX....q...
-00005360: 3510 0000 1300 0000 0000 0000 0000 0000  5...............
-00005370: 8001 5049 0000 5b43 6f6e 7465 6e74 5f54  ..PI..[Content_T
-00005380: 7970 6573 5d2e 786d 6c50 4b05 0600 0000  ypes].xmlPK.....
-00005390: 0020 0020 0097 0800 00f2 4a00 0000 00    . . ......J....
+000000e0: 91c1 4ec3 300c 865f 65ea bd75 d3a0 0aa2  ..N.0.._e..u....
+000000f0: ac17 1027 9090 9804 e216 25de 16ad 49a3  ...'......%...I.
+00000100: c4a8 dddb d396 ad1b 820b c7f8 fffc d956  ...............V
+00000110: a40e 4277 115f 6217 3092 c5b4 1a5c eb93  ..Bw._b.0....\..
+00000120: d061 9ded 8982 0048 7a8f 4ea5 6224 fc18  .a.....Hz.N.b$..
+00000130: 6ebb e814 8dcf b883 a0f4 41ed 10aa b2ac  n.........A.....
+00000140: c121 29a3 48c1 24cc c362 cc4e 4aa3 1765  .!).H.$..b.NJ..e
+00000150: f88c ed2c 301a b045 879e 12b0 82c1 8525  ...,0..E.......%
+00000160: 8c2e fdd9 3027 0b39 24bb 507d df17 3d9f  ....0'.9$.P}..=.
+00000170: b971 2306 efcf 4faf f3f2 b9f5 8994 d798  .q#...O.........
+00000180: 35d2 68a1 232a ea62 335d 148e 432b e1aa  5.h.#*.b3]..C+..
+00000190: 284f b3bf 0b68 56e3 0441 c780 ebec 9cbc  (O...hV..A......
+000001a0: f1fb 87cd 63d6 5465 7593 973c 67b7 1b76  ....c.Teu..<g..v
+000001b0: 27aa 5a70 fe31 b97e f45f 84ae 3376 6bff  '.Zp.1.~._..3vk.
+000001c0: 69ac af8c 6741 23e1 d7bf 355f 504b 0304  i...gA#...5_PK..
+000001d0: 1400 0000 0800 5263 7258 995c 9c23 1006  ......RcrX.\.#..
+000001e0: 0000 9c27 0000 1300 0000 786c 2f74 6865  ...'......xl/the
+000001f0: 6d65 2f74 6865 6d65 312e 786d 6ced 5a5b  me/theme1.xml.Z[
+00000200: 73da 3814 7eef afd0 7867 f66d 0bc6 3681  s.8.~...xg.m..6.
+00000210: b6b4 1373 6976 dbb4 9984 ed4e 1f85 1158  ...siv.....N...X
+00000220: 8d6c 7964 9184 7fbf 4736 10cb 960d ed92  .lyd....G6......
+00000230: 4dba 9b3c 042c e9fb ce45 47e7 e838 79f3  M..<.,...EG..8y.
+00000240: ee2e 62e8 8688 94f2 7860 d92f dbd6 bbb7  ..b.....x`./....
+00000250: 2fde e057 3224 1141 3019 a7af f0c0 0aa5  /..W2$.A0.......
+00000260: 4c5e b55a 6900 c338 7dc9 1312 c3dc 828b  L^.Zi..8}.......
+00000270: 084b 7814 cbd6 5ce0 5b1a 2f23 d6ea b4db  .Kx...\.[./#....
+00000280: dd56 8469 6ca1 1847 6460 7d5e 2c68 40d0  .V.il..Gd`}^,h@.
+00000290: 5451 5a6f 5f20 b4e5 1f33 f815 cb54 8d65  TQZo_ ...3...T.e
+000002a0: a301 1357 4126 b988 b4f2 f96c c5fc dade  ...WA&.....l....
+000002b0: 3e65 cfe9 3a1d 3281 6e30 1b58 207f ce6f  >e..:.2.n0.X ..o
+000002c0: a7e4 4e5a 88e1 54c2 c4c0 6a67 3f56 6bc7  ..NZ..T...jg?Vk.
+000002d0: d1d2 4880 82c9 7d94 05ba 49f6 a3d3 1508  ..H...}...I.....
+000002e0: 320d 3b3a 9d58 ce76 7cf6 c4ed 9f8c cada  2.;:.X.v|.......
+000002f0: 7434 6d1a e0e3 f178 38b6 cbd2 8b70 1c04  t4m....x8....p..
+00000300: e051 bb9e c29d f46c bfa4 4109 b4a3 69d0  .Q.....l..A...i.
+00000310: 64d8 f6da ae91 a6aa 8d53 4fd3 f77d dfeb  d........SO..}..
+00000320: 9b68 9c0a 8d5b 4fd3 6b77 ddd3 8e89 c6ad  .h...[O.kw......
+00000330: d078 0dbe f14f 87c3 ae89 c6ab d074 eb69  .x...O.......t.i
+00000340: 2627 fdae 6ba4 e916 6842 46e3 eb7a 1215  &'..k...hBF..z..
+00000350: b5e5 40d3 2000 5870 76d6 ccd2 0396 5e29  ..@. .Xpv.....^)
+00000360: fa75 941a d91d bbdd 415c f058 ee39 8911  .u......A\.X.9..
+00000370: fec6 c504 d669 d219 9634 4672 9d90 050e  .....i...4Fr....
+00000380: 0037 c4d1 4c50 7caf 41b6 8ae0 c292 d25c  .7..LP|.A......\
+00000390: 90d6 cf29 b550 1a08 9ac8 81f5 4782 21c5  ...).P......G.!.
+000003a0: dcaf fdf5 97bb c9a4 337a 9d7d 3ace 6b94  ........3z.}:.k.
+000003b0: 7f69 ab01 a7ed bb9b cf93 fc73 e8e4 9fa7  .i.........s....
+000003c0: 93d7 4d42 ce70 bc2c 09f1 fb23 5b61 8727  ..MB.p.,...#[a.'
+000003d0: 6e3b 1372 3a1c 6742 7ccf f6f6 91a5 2532  n;.r:.gB|.....%2
+000003e0: cfef f90a eb4e 3c67 1f56 96b0 5dcf cfe4  .....N<g.V..]...
+000003f0: 9e8c 7223 bbdd f658 7df6 4f47 6e23 d7a9  ..r#...X}.OGn#..
+00000400: c0b3 22d7 9446 2445 9fc8 2dba e411 38b5  .."..F$E..-...8.
+00000410: 490d 3213 3f08 9d86 986a 501c 02a4 0931  I.2.?....jP....1
+00000420: 96a1 86f8 b4c6 ac11 e013 7db7 be08 c8df  ..........}.....
+00000430: 8d88 f7ab 6f9a 3d57 a158 49da 84f8 1046  ....o.=W.XI....F
+00000440: 1ae2 9c73 e673 d16c fb07 a546 d1f6 55bc  ...s.s.l...F..U.
+00000450: dca3 9758 1501 9718 df34 aa35 2cc5 d678  ...X.....4.5,..x
+00000460: 95c0 f1ad 9c3c 1d13 12cd 940b 0641 8697  .....<.......A..
+00000470: 2426 12a9 397e 4d48 13fe 2ba5 dafe 9cd3  $&..9~MH..+.....
+00000480: 40f0 942f 24fa 4a91 8f69 b323 a774 26cd  @../$.J..i.#.t&.
+00000490: e833 1ac1 46af 1b75 8768 d23c 7afe 05f9  .3..F..u.h.<z...
+000004a0: 9c35 0a1c 911b 1d02 671b b346 2184 69bb  .5......g..F!.i.
+000004b0: f01e af24 8e9a adc2 112b 423e 6219 361a  ...$.....+B>b.6.
+000004c0: 72b5 1681 b671 a984 605a 12c6 d178 4ed2  r....q..`Z...xN.
+000004d0: b411 fc59 ac35 933e 60c8 eccd 9175 ced6  ...Y.5.>`....u..
+000004e0: 910e 1192 5e37 423e 62ce 8b90 11bf 1e86  ....^7B>b.......
+000004f0: 384a 9aed a271 5804 fd9e 5ec3 49c1 e882  8J...qX...^.I...
+00000500: cb66 fdb8 7e86 d533 6c2c 8ef7 47d4 174a  .f..~..3l,..G..J
+00000510: e40f 26a7 3fe9 3234 07a3 9a59 09bd 8456  ..&.?.24...Y...V
+00000520: 6a9f aa87 343e a81e 320a 05f1 b91e 3ee5  j...4>..2.....>.
+00000530: 7a78 0a37 96c6 bc50 ae82 7b01 ffd1 da37  zx.7...P..{....7
+00000540: c2ab f882 c039 7f2e 7dcf a5ef b9f4 3da1  .....9..}.....=.
+00000550: d2b7 3723 7d67 c1d3 8b5b de46 6e5b c4fb  ..7#}g...[.Fn[..
+00000560: ae31 dad7 342e 2863 5772 cdc8 c754 af93  .1..4.(cWr...T..
+00000570: 29d8 399f c0ec fd68 3e9e f1ed fad9 2484  ).9....h>.....$.
+00000580: af9a 592d 2316 904b 81b3 4124 b8fc 8bca  ..Y-#..K..A$....
+00000590: f02a c409 e864 5b25 09cb 54d3 6537 8a12  .*...d[%..T.e7..
+000005a0: 9e42 1b6e e953 f54a 95d7 e5af b928 b83c  .B.n.S.J.....(.<
+000005b0: 5be4 e9af a174 3e2c cff9 3c5f e7b4 cd0b  [....t>,..<_....
+000005c0: 3343 b772 4bea b694 beb5 2638 4af4 b1cc  3C.rK.....&8J...
+000005d0: 704e 1ecb 0c3b 673c 921d b677 a01d 35fb  pN...;g<...w..5.
+000005e0: f65d 76e4 23a5 3053 9743 b81a 42be 036d  .]v.#.0S.C..B..m
+000005f0: ba9d dc3a 389e 9891 b90a d352 906f c3f9  ...:8......R.o..
+00000600: e9c5 781a e239 d904 b97d 9857 6de7 d8d1  ..x..9...}.Wm...
+00000610: d1fb e7c1 51b0 a3ef 3c96 1dc7 88f2 a221  ....Q...<......!
+00000620: eea1 8698 cfc3 4387 797b 5f98 6795 c650  ......C.y{_.g..P
+00000630: 3414 6d6c ac24 2c46 b760 b8d7 f12c 14e0  4.ml.$,F.`...,..
+00000640: 6460 2da0 0783 af51 02f2 5255 6031 5bc6  d`-....Q..RU`1[.
+00000650: 032b 90a2 7c4c 8c45 e870 e797 5c5f e3d1  .+..|L.E.p..\_..
+00000660: 92e3 dba6 65b5 6eaf 2977 196d 2252 39c2  ....e.n.)w.m"R9.
+00000670: 6998 1367 abca de65 b1c1 551d cf55 5bf2  i..g...e..U..U[.
+00000680: b0be 6a3d b415 4ecf fe59 adc8 9f0c 114e  ..j=..N..Y.....N
+00000690: 160b 1248 6394 17a6 4aa2 f319 53be e72b  ...Hc...J...S..+
+000006a0: 49c4 5538 bf45 33b6 1297 18bc e3e6 c771  I.U8.E3........q
+000006b0: 4e53 b812 76b6 0f02 32b9 bb39 a97a 6531  NS..v...2..9.ze1
+000006c0: 67a6 f2df 2d0c 092c 5b88 5912 e24d 5ded  g...-..,[.Y..M].
+000006d0: d5e7 9b9c ae7a 2276 fa97 77c1 60f2 fd70  .....z"v..w.`..p
+000006e0: c947 0fe5 3be7 5ff4 5d43 ae7e f6dd e3fa  .G..;._.]C.~....
+000006f0: 6e93 3b48 4c9c 79c5 1101 7445 0223 951c  n.;HL.y...tE.#..
+00000700: 0616 1732 e450 ee92 9006 1301 cd94 c944  ...2.P.........D
+00000710: f002 8264 a61c 8098 fa0b bdf2 0cb9 2915  ...d..........).
+00000720: cead 3e39 7f45 2c83 864e 5ed2 2512 148a  ..>9.E,..N^.%...
+00000730: b00c 0521 1772 e3ef ef93 6a77 8cd7 fa2c  ...!.r....jw...,
+00000740: 816d 8454 3264 d517 ca43 89c1 3d33 7243  .m.T2d...C..=3rC
+00000750: d854 25f3 aeda 260b 85db e254 cdbb 1abe  .T%...&....T....
+00000760: 2660 4bc3 7a6e 9d2d 27ff db5e d43d b417  &`K.zn.-'..^.=..
+00000770: 3d46 f3a3 99e0 1eb3 8773 9b7a b8c2 45ac  =F.......s.z..E.
+00000780: ff58 d61e f932 df39 70db 3ade 035e e613  .X...2.9p.:..^..
+00000790: 2c43 a47e c17d 8a8a 8011 ab62 beba af4f  ,C.~.}.....b...O
+000007a0: f925 9c3b b47b f181 209b fcd6 dba4 f6dd  .%.;.{.. .......
+000007b0: e00c 7cd4 ab5a a564 2b11 3f4b 077c 1f92  ..|..Z.d+.?K.|..
+000007c0: 0663 8c5b f434 5f8f 1462 ada6 b1ad c6da  .c.[.4_..b......
+000007d0: 310c 7980 58f3 0ca1 6638 df87 459a 1a33  1.y.X...f8..E..3
+000007e0: d58b ac39 8d0a 6f41 d540 e53f dbd4 0d68  ...9..oA.@.?...h
+000007f0: f60d 341c 9105 5e31 99b6 36a3 e44e 0a3c  ..4...^1..6..N.<
+00000800: dcfe ef0d b0c2 c48e e1ed 8bbf 0150 4b03  .............PK.
+00000810: 0414 0000 0008 0052 6372 580f 954d 3348  .......RcrX..M3H
+00000820: 0100 0049 0200 0018 0000 0078 6c2f 776f  ...I.......xl/wo
+00000830: 726b 7368 6565 7473 2f73 6865 6574 312e  rksheets/sheet1.
+00000840: 786d 6c75 52db 4ec3 300c fd95 2a1f b074  xmluR.N.0...*..t
+00000850: 485c 34b5 95d8 1082 07a4 6913 f09c b56e  H\4.......i....n
+00000860: 1b2d 894b e2ae f0f7 38ed 6e3c f014 fbc4  .-.K....8.n<....
+00000870: e7f8 d849 36a0 df87 1680 926f 6b5c c845  ...I6......ok\.E
+00000880: 4bd4 2da4 0c65 0b56 8519 76e0 f8a6 466f  K.-..e.V..v...Fo
+00000890: 1571 ea1b 193a 0faa 1a49 d6c8 9b34 bd93  .q...:...I...4..
+000008a0: 5669 278a 6cc4 d6be c8b0 27a3 1dac 7d12  Vi'.l.....'...}.
+000008b0: 7a6b 95ff 5982 c121 1773 7102 36ba 6969  zk..Y..!.sq.6.ii
+000008c0: 0464 9175 aa81 2dd0 7bc7 044e e559 a7d2  .d.u..-.{..N.Y..
+000008d0: 165c d0e8 120f 752e 1ee7 8be5 c418 2b3e  .\....u.......+>
+000008e0: 340c e12a 4ee2 303b c47d 4c5e ab5c a4d1  4..*N.0;.}L^.\..
+000008f0: 1318 2829 4a28 3e0e b002 63a2 123b f93a  ..()J(>...c..;.:
+00000900: 8a8a 4bd3 c8bc 8e4f f2cf e3fc 6c6f a702  ..K....O....lo..
+00000910: acd0 7cea 8ada 5c3c 88a4 825a f586 3638  ..|...\<...Z..68
+00000920: bcc0 71a6 db8b c527 45aa c83c 0e89 8fc3  ..q....'E..<....
+00000930: 1659 1983 d892 0bb5 8b4b da92 675c 7327  .Y.......K..g\s'
+00000940: 2a3a e595 0502 9f49 621b 1194 e591 b4fc  *:.....Ib.......
+00000950: 8f74 50a6 87bf 04c9 1d4f 634c 16e2 8adf  .tP......OcL....
+00000960: 946f b40b 8981 9a85 d2d9 3d1b f593 e729  .o........=....)
+00000970: 21ec c627 d921 11da 316c f9a9 c1c7 02be  !..'.!..1l......
+00000980: af11 e99c c49d 9d7f 4ff1 0b50 4b03 0414  ........O..PK...
+00000990: 0000 0008 0052 6372 580f 954d 3348 0100  .....RcrX..M3H..
+000009a0: 0049 0200 0018 0000 0078 6c2f 776f 726b  .I.......xl/work
+000009b0: 7368 6565 7473 2f73 6865 6574 322e 786d  sheets/sheet2.xm
+000009c0: 6c75 52db 4ec3 300c fd95 2a1f b074 485c  luR.N.0...*..tH\
+000009d0: 34b5 95d8 1082 07a4 6913 f09c b56e 1b2d  4.......i....n.-
+000009e0: 894b e2ae f0f7 38ed 6e3c f014 fbc4 e7f8  .K....8.n<......
+000009f0: d849 36a0 df87 1680 926f 6b5c c845 4bd4  .I6......ok\.EK.
+00000a00: 2da4 0c65 0b56 8519 76e0 f8a6 466f 1571  -..e.V..v...Fo.q
+00000a10: ea1b 193a 0faa 1a49 d6c8 9b34 bd93 5669  ...:...I...4..Vi
+00000a20: 278a 6cc4 d6be c8b0 27a3 1dac 7d12 7a6b  '.l.....'...}.zk
+00000a30: 95ff 5982 c121 1773 7102 36ba 6969 0464  ..Y..!.sq.6.ii.d
+00000a40: 9175 aa81 2dd0 7bc7 044e e559 a7d2 165c  .u..-.{..N.Y...\
+00000a50: d0e8 120f 752e 1ee7 8be5 c418 2b3e 340c  ....u.......+>4.
+00000a60: e12a 4ee2 303b c47d 4c5e ab5c a4d1 1318  .*N.0;.}L^.\....
+00000a70: 2829 4a28 3e0e b002 63a2 123b f93a 8a8a  ()J(>...c..;.:..
+00000a80: 4bd3 c8bc 8e4f f2cf e3fc 6c6f a702 acd0  K....O....lo....
+00000a90: 7cea 8ada 5c3c 88a4 825a f586 3638 bcc0  |...\<...Z..68..
+00000aa0: 71a6 db8b c527 45aa c83c 0e89 8fc3 1659  q....'E..<.....Y
+00000ab0: 1983 d892 0bb5 8b4b da92 675c 7327 2a3a  .......K..g\s'*:
+00000ac0: e595 0502 9f49 621b 1194 e591 b4fc 8f74  .....Ib........t
+00000ad0: 50a6 87bf 04c9 1d4f 634c 16e2 8adf 946f  P......OcL.....o
+00000ae0: b40b 8981 9a85 d2d9 3d1b f593 e729 21ec  ........=....)!.
+00000af0: c627 d921 11da 316c f9a9 c1c7 02be af11  .'.!..1l........
+00000b00: e99c c49d 9d7f 4ff1 0b50 4b03 0414 0000  ......O..PK.....
+00000b10: 0008 0052 6372 58b1 1155 4740 0200 0078  ...RcrX..UG@...x
+00000b20: 0500 0018 0000 0078 6c2f 776f 726b 7368  .......xl/worksh
+00000b30: 6565 7473 2f73 6865 6574 332e 786d 6cbd  eets/sheet3.xml.
+00000b40: 54db 6edb 300c fd15 c3cf 419d 04eb 0581  T.n.0.....A.....
+00000b50: 6320 97a6 29b0 005d 9376 8f03 6333 b116  c ..)..].v..c3..
+00000b60: 59f4 24ba 5eff 7e94 9da6 1724 79dc 8b2d  Y.$.^.~....$y..-
+00000b70: 1ef1 503c 12c9 b826 bb73 3922 077f 0b6d  ..P<...&.s9"...m
+00000b80: dc30 cc99 cb41 14b9 34c7 02dc 0595 6864  .0...A..4.....hd
+00000b90: 6743 b600 16d3 6e23 575a 84ac 2115 3aea  gC....n#WZ..!.:.
+00000ba0: 77bb 5751 01ca 8449 dc60 0f36 89a9 62ad  w.WQ...I.`.6..b.
+00000bb0: 0c3e d8c0 5545 01f6 758c 9aea 61d8 0bdf  .>..UE..u...a...
+00000bc0: 8047 b5cd b901 a224 2e61 8b4b e4a7 5208  .G.....$.a.K..R.
+00000bd0: 6246 8738 992a d038 4526 b0b8 1986 a3de  bF.8.*.8E&......
+00000be0: 60de 321a 8f67 85b5 fbb0 0ebc 9835 d1ce  `.2..g.......5..
+00000bf0: 1bf7 d930 ecfa 9c50 63ca 3e04 c8ef 0527  ...0...Pc.>....'
+00000c00: a8b5 8f24 99fc d907 0ddf 0ff5 cc8f ebb7  ...$............
+00000c10: f0b3 46bf a4b7 0687 13d2 3f55 c6f9 30bc  ..F.......?U..0.
+00000c20: 0983 0c37 5069 7ea4 7a8e 7b4d 97ef 294e  ...7Pi~.z.{M..)N
+00000c30: 8121 892d d581 f562 9338 f50b 7fa4 382a  .!.-...b.8....8*
+00000c40: e32f 69c9 5670 2527 71c2 e8f8 97a3 caa6  ./i.Vp%'q.......
+00000c50: 1847 2c89 7838 4af7 b4f1 599a 8841 8be6  .G,.x8J...Y..A..
+00000c60: 2873 7296 49eb dfd8 dccd 11e6 f42c 138c  (sr.I........,..
+00000c70: 2106 7fbb ee08 f7f6 1457 6547 bc67 a7bc  !........WeG.g..
+00000c80: 0d14 c732 bb3b e59f a14b ad2a 7d56 4768  ...2.;...K.*}VGh
+00000c90: f393 8260 fb45 4424 eff6 560c ed43 66f2  ...`.ED$..V..Cf.
+00000ca0: 7d06 adb2 5673 9052 6524 583f fcba 7528  }...Vs.Re$X?..u(
+00000cb0: aefe 60d4 eb7e bbb9 bcbe 9282 cba9 9e5a  ..`..~.........Z
+00000cc0: 2aa7 541b 5f9c 0d70 6fca 8a17 e89c f4c0  *.T._..po.......
+00000cd0: 01bc b596 ec47 10b4 f4cf 5883 d935 3dc3  .....G....X..5=.
+00000ce0: afa5 e05a 3996 937d 6f56 1a7a 49b8 5cdc  ...Z9..}oV.zI.\.
+00000cf0: 7696 8ba7 c759 e74e f1bc 5a3f 39b4 33c4  v....Y.N..Z?9.3.
+00000d00: 6c0d e9ae b31a 4d56 9db1 1448 be00 2ba6  l.....MV...H..+.
+00000d10: 05e3 3430 d915 42d1 59c9 737a 8ddf 296d  ..40..B.Y.sz..)m
+00000d20: 0484 7174 881b 479f c59d 123b e90f 26ff  ..qt..G....;..&.
+00000d30: 4fec 284d b164 9082 f7b9 b7ca 64b2 ec1a  O.(M.d......d...
+00000d40: eb47 0586 952f cd97 66fb bc9c 2f80 6b27  .G.../..f.../.k'
+00000d50: 925c d356 c923 6bdc c81b 772f aea5 af6d  .\.V.#k...w/...m
+00000d60: dbe2 adc1 5436 09ae 8999 8a66 99cb 6444  ....T6.....f..dD
+00000d70: eb1d 647f 43c4 07c3 8f98 c3b0 4dfe 0150  ..d.C.......M..P
+00000d80: 4b03 0414 0000 0008 0052 6372 5825 817d  K........RcrX%.}
+00000d90: dbbf 0200 0073 0800 0018 0000 0078 6c2f  .....s.......xl/
+00000da0: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
+00000db0: 342e 786d 6cbd 96db 72da 3010 865f c5e3  4.xml...r.0.._..
+00000dc0: 6b26 06a6 390c 633c 9384 a449 032d cd81  k&..9.c<...I.-..
+00000dd0: 5e32 c25e 8c06 59eb 48eb 3879 fbae 4c20  ^2.^..Y.H.8y..L 
+00000de0: 69c6 82bb 5e21 adf5 49fb af56 bbc4 359a  i...^!..I..V..5.
+00000df0: b55d 0150 f05a 286d 87e1 8aa8 1c44 914d  .].P.Z(m.....D.M
+00000e00: 5750 087b 8425 68fe b244 5308 e2a9 c923  WP.{.%h..DS....#
+00000e10: 5b1a 1059 0315 2aea 77bb 2751 21a4 0e93  [..Y..*.w.'Q!...
+00000e20: b8b1 4d4d 1263 454a 6a98 9ac0 5645 21cc  ..MM.cEJj...VE!.
+00000e30: db05 28ac 8761 2fdc 1aee 65be a2c6 1025  ..(..a/...e....%
+00000e40: 7129 7278 007a 2a19 e069 b4db 2793 0568  q)rx.z*..i..'..h
+00000e50: 2b51 0706 96c3 f0bc 3798 6d88 66c5 4c42  +Q......7.m.f.LB
+00000e60: 6d3f 8d03 2766 81b8 7693 db6c 1876 9d4f  m?..'f..v..l.v.O
+00000e70: a020 25b7 85e0 9f17 b804 a5dc 4eec c9f3  . %.........N...
+00000e80: fba6 e1c7 a18e fc3c de6e 7fdd e867 f716  .......<.n...g..
+00000e90: c2c2 25aa 3f32 a3d5 303c 0b83 0c96 a252  ..%.?2..0<.....R
+00000ea0: 748f f50d bc6b 3afe 7071 2448 24b1 c13a  t....k:.pq$H$..:
+00000eb0: 304e 6c12 a76e e08e e485 52bb 203d 9061  0Nl..n....R. =.a
+00000ec0: bbe4 9328 91ba ac68 2eb3 3822 f6c2 d9a2  ...(...h..8"....
+00000ed0: f49d b9d8 cf68 5140 0b75 b99f 4a05 418e  .....hQ@.u..J.A.
+00000ee0: e6ad 851c f948 befd 4c3a b0dd cfab c39c  .....H..L:......
+00000ef0: c7d7 6b1f c9d9 e40d cbf7 0390 e7ac 9b03  ..k.............
+00000f00: d89e c0dc fa50 612d a652 b85c 6bc1 7ef8  .....Pa-.R.\k.~.
+00000f10: b0e7 4a28 b994 606c 0b75 e7a3 e0b5 e4b4  ..J(..`l.u......
+00000f20: 866c be71 b805 1dfb 5002 cbc1 b4b6 6a0b  .l.q....P.....j.
+00000f30: ccc4 4759 2e07 9a64 3ab7 f002 4652 5b68  ..GY...d:...FR[h
+00000f40: 7efa b36d fed2 6b01 7ef9 809a 5fe9 7cad  ~..m..k.~..._.|.
+00000f50: b16e 0be5 74af 327e d460 40a7 6dea 7efb  .n..t.2~.`@.m.~.
+00000f60: 4853 690d 86b5 1149 9db7 ddc4 fdde 430b  HSi....I......C.
+00000f70: 2091 f15b 6f01 1fbc 4169 cbe7 47df 6a4f   ..[o...Ai..G.jO
+00000f80: 223f f9d6 6760 5323 4b4f 36ce bc6a c457  "?..g`S#KO6..j.W
+00000f90: f511 57af 6d49 dc94 3327 74c6 499b 35b9  ..W.mI..3't.I.5.
+00000fa0: 6e83 142b cd9b f5c3 af9f b625 76dc 1f8c  n..+.......%v...
+00000fb0: 7bdd 6f67 c7a7 275c 7657 588f 0c96 23be  {.og..'\vWX...#.
+00000fc0: 5c57 a21b c3ad 2b47 13b0 963b c1ce 7865  \W....+G...;..xe
+00000fd0: 0c9a cf46 a1b8 8b5c 28a1 d74d e7a0 b792  ...F...\(..M....
+00000fe0: ed4a 5ae2 935d 87aa 94e8 2561 2a2a 0b36  .JZ..]....%a**.6
+00000ff0: d048 0171 a722 db79 9cdc 4d3b db27 1d10  .H.q.".y..M;.'..
+00001000: 6290 035f b74c 3b29 6a32 dcbc 9aca e4c4  b.._.L;)j2......
+00001010: 745c dfe3 890a 0c2a b09d 8fc7 12c6 d1ee  t\.....*........
+00001020: 8c38 fa57 a84f f8a4 3f98 fc3f e137 dc7f  .8.W.O..?..?.7..
+00001030: 3a63 ac3b 3f91 cecb 52b1 8c85 3ae0 f717  :c.;?...R...:...
+00001040: 83dd 34e3 8930 b9e4 9b55 b0e4 8bed 1e9d  ..4..0...U......
+00001050: 724b 339b eeb6 9910 968d 270b 24c2 a219  rK3.......'.$...
+00001060: aef8 4f01 18b7 80bf 2f11 6937 71dd 75f7  ..O...../.i7q.u.
+00001070: 3f23 f90b 504b 0304 1400 0000 0800 5263  ?#..PK........Rc
+00001080: 7258 b356 a83b 9203 0000 8c0d 0000 1800  rX.V.;..........
+00001090: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
+000010a0: 7368 6565 7435 2e78 6d6c bd57 db6e db38  sheet5.xml.W.n.8
+000010b0: 10fd 1541 cf42 651b dbb4 3064 0376 aede  ...A.Be...0d.v..
+000010c0: 36dd 6cd2 3add 7d11 6872 6c73 4391 2a39  6.l.:.}.hrlsC.*9
+000010d0: b292 bfdf a11c 2769 40c6 401e fc24 5e74  ......'i@.@..$^t
+000010e0: 8687 c3e1 9961 d11a 7be7 d600 98dc 574a  .....a..{.....WJ
+000010f0: bb51 ba46 ac87 79ee f81a 2ae6 3e98 1a34  .Q.F..y...*.>..4
+00001100: cd2c 8dad 1852 d7ae 7257 5b60 a203 552a  .,...R..rW[`..U*
+00001110: 1ff4 7a47 79c5 a44e c745 3776 65c7 8569  ..zGy..N.E7ve..i
+00001120: 5049 0d57 3671 4d55 31fb 3005 65da 51da  PI.W6qMU1.0.e.Q.
+00001130: 4f77 03d7 72b5 c66e 201f 1735 5bc1 0de0  Ow..r..n ..5[...
+00001140: 8f9a 00d4 cd9f ec08 5981 76d2 e8c4 c272  ........Y.v....r
+00001150: 944e fac3 c9d9 16d2 fd32 97d0 ba17 edc4  .N.......2......
+00001160: ef66 61cc 9def ccc4 28ed 7952 a080 a3b7  .fa.....(.yR....
+00001170: c1e8 b381 6350 ca9b 222a bf1e ada6 cfab  ....cP.."*......
+00001180: 7ae4 cbf6 cefc 59e7 00e2 b760 0e8e 8dba  z.....Y....`....
+00001190: 9502 d7a3 f473 9a08 58b2 46e1 b569 2fe0  .....s..X.F..i/.
+000011a0: 7153 1f9f 299e 3064 e3c2 9a36 b17e b7e3  qS..).0d...6.~..
+000011b0: 82fb 865f 927e 94da 7be9 062d 8d4b 5a09  ..._.~..{..-.KZ.
+000011c0: c755 e3b0 ac99 73a5 6008 458e c4c5 cfe4  .U....s.`.E.....
+000011d0: fc11 39dd 8f04 bd91 d668 f21c 060c 1cc7  ..9......h......
+000011e0: 0c38 2e09 2197 9297 bf1a 70de 6301 f849  .8..!.....p.c..I
+000011f0: 148e 56ea 152d 8ef6 2180 3b8d e184 b4db  ..V..-..!.;.....
+00001200: e309 80ce 6220 a65d 0bb6 94ba 8b4b 5572  ....b .].....KUr
+00001210: a339 d4a1 ed9e c74c c07d 4deb 8228 2d38  .9.....L.}M..(-8
+00001220: 3abe 00f4 2206 4553 970a 36a0 02a0 590c  :...".ES..6...Y.
+00001230: 443e b50f a536 2274 aa7f c650 da20 b800  D>...6"t...P. ..
+00001240: e04b 0c20 75dd 6029 4500 f3f5 6d8c 6655  .K. u.`)E...m.fU
+00001250: 88da e5db 284e 61ba 32c1 23ff 1643 927e  ....(Na.2.#..C.~
+00001260: 08e9 8161 9e7f edc7 45b8 5ec5 90a4 4751  ...a....E.^...GQ
+00001270: b7fc bd07 1459 eb7a 0fec 0dc7 dc44 c3da  .....Y.z.....D..
+00001280: 39c3 258b dc86 eff1 d062 8aee 2dd8 50a4  9.%......b..-.P.
+00001290: fcd8 7b01 b684 03d0 79f4 0290 3c94 d2b9  ..{.....y...<...
+000012a0: 26e4 98db a842 5042 2181 e1a5 a3bb 6325  &....BPB!.....c%
+000012b0: 865c f333 1e6d e5a6 1f00 fc13 03b4 24f3  .\.3.m........$.
+000012c0: e59d 366d c895 ffbe b933 ca0a 6081 1425  ..6m.....3..`..%
+000012d0: 809c 44a5 db36 5a93 2639 4024 210c 1dc5  ..D..6Z.&9@$!...
+000012e0: 242a dedd b215 2023 d567 2164 54b5 8321  $*.... #.g!dT..!
+000012f0: 3d89 aa74 2498 2771 7906 c7ad ac23 2139  =..t$.'qy....#!9
+00001300: 892a 34b2 d72e c829 09ee 32eb 362b facd  .*4....)..2.6+..
+00001310: ce29 7445 17f1 2ee1 a6d1 64ec 287d 3db5  .)tE......d.(}=.
+00001320: cbd4 d3c1 70da effd f1f9 e3a7 23ca de6b  ....p.......#..k
+00001330: d39e 5853 9fd0 11fb 4cdf 0dcc bc28 5d82  ..XS....L....(].
+00001340: 7354 513c 0d9e 5a6b eccb 41a6 a81a 992a  sTQ<..Zk..A....*
+00001350: a6ef ba0a 041f 6a1a 57d2 21ad ec33 4aa3  ......j.W.!..3J.
+00001360: 587f 9c0a d864 5c66 fe6c b2da 1a91 16f9  X....d\f.l......
+00001370: d364 91ff ce30 c6f8 7430 3c3d 1c63 a939  .d...0..t0<=.c.9
+00001380: 9566 0e44 26e0 b1f5 1ed2 e783 e1f9 4149  .f.D&.........AI
+00001390: ab46 40b9 3246 6470 bfed 2cd8 bb98 cf06  .F@.2Fdp..,.....
+000013a0: c3d9 e198 bb66 f11f 4968 66ba cf7b f8ce  .....f..Ihf..{..
+000013b0: 07c3 f9e1 f872 d638 7009 d514 0952 74a0  .....r.8p....Rt.
+000013c0: cbbe 5f7e b9ca 7699 2a41 6392 1590 8849  .._~..v.*Ac....I
+000013d0: 9e51 4585 96aa fa2e e1fa db99 f907 0175  .QE............u
+000013e0: 5462 8d02 973d e780 f76c fc76 30bc 3ddc  Tb...=...l.v0.=.
+000013f0: c62f a82e cfbe 9a36 fb66 7052 d78a b6b1  ./.....6.fpR....
+00001400: 507b 78bf 1a70 db57 ca25 b32b 4952 a560  P{x..p.W.%.+IR.`
+00001410: 494a d5fb f089 4a7d bbad fab7 1daa 0d3b  IJ....J}.......;
+00001420: 260b 8368 aaae b9a6 d712 58ff 03cd 2f0d  &..h......X.../.
+00001430: 5574 bb8e 7f75 3c3d c0c6 ff03 504b 0304  Ut...u<=....PK..
+00001440: 1400 0000 0800 5263 7258 2581 7ddb bf02  ......RcrX%.}...
+00001450: 0000 7308 0000 1800 0000 786c 2f77 6f72  ..s.......xl/wor
+00001460: 6b73 6865 6574 732f 7368 6565 7436 2e78  ksheets/sheet6.x
+00001470: 6d6c bd96 db72 da30 1086 5fc5 e36b 2606  ml...r.0.._..k&.
+00001480: a639 0c63 3c93 84a4 4903 2dcd 815e 32c2  .9.c<...I.-..^2.
+00001490: 5e8c 0659 eb48 eb38 79fb ae4c 2069 c682  ^..Y.H.8y..L i..
+000014a0: bb5e 21ad f549 fbaf 56bb c435 9ab5 5d01  .^!..I..V..5..].
+000014b0: 50f0 5a28 6d87 e18a a81c 4491 4d57 5008  P.Z(m.....D.MWP.
+000014c0: 7b84 2568 feb2 4453 08e2 a9c9 235b 1a10  {.%h..DS....#[..
+000014d0: 5903 152a ea77 bb27 5121 a40e 93b8 b14d  Y..*.w.'Q!.....M
+000014e0: 4d12 6345 4a6a 989a c056 4521 ccdb 0528  M.cEJj...VE!...(
+000014f0: ac87 612f dc1a ee65 bea2 c610 2571 2972  ..a/...e....%q)r
+00001500: 7800 7a2a 19e0 69b4 db27 9305 682b 5107  x.z*..i..'..h+Q.
+00001510: 0696 c3f0 bc37 986d 8866 c54c 426d 3f8d  .....7.m.f.LBm?.
+00001520: 0327 6681 b876 93db 6c18 769d 4fa0 2025  .'f..v..l.v.O. %
+00001530: b785 e09f 17b8 04a5 dc4e ecc9 f3fb a6e1  .........N......
+00001540: c7a1 8efc 3cde 6e7f dde8 67f7 16c2 c225  ....<.n...g....%
+00001550: aa3f 32a3 d530 3c0b 830c 96a2 5274 8ff5  .?2..0<.....Rt..
+00001560: 0dbc 6b3a fe70 7124 4824 b1c1 3a30 4e6c  ..k:.pq$H$..:0Nl
+00001570: 12a7 6ee0 8ee4 8552 bb20 3d90 61bb e493  ..n....R. =.a...
+00001580: 2891 baac 682e b338 22f6 c2d9 a2f4 9db9  (...h..8".......
+00001590: d8cf 6851 400b 75b9 9f4a 0541 8ee6 ad85  ..hQ@.u..J.A....
+000015a0: 1cf9 48be fd4c 3ab0 ddcf abc3 9cc7 d76b  ..H..L:........k
+000015b0: 1fc9 d9e4 0dcb f703 90e7 ac9b 03d8 9ec0  ................
+000015c0: dcfa 5061 2da6 52b8 5c6b c17e f8b0 e74a  ..Pa-.R.\k.~...J
+000015d0: 28b9 9460 6c0b 75e7 a3e0 b5e4 b486 6cbe  (..`l.u.......l.
+000015e0: 71b8 051d fb50 02cb c1b4 b66a 0bcc c447  q....P.....j...G
+000015f0: 592e 079a 643a b7f0 0246 525b 687e fab3  Y...d:...FR[h~..
+00001600: 6dfe d26b 017e f980 9a5f e97c adb1 6e0b  m..k.~..._.|..n.
+00001610: e574 af32 7ed4 6040 a76d ea7e fb48 5369  .t.2~.`@.m.~.HSi
+00001620: 0d86 b511 499d b7dd c4fd de43 0b20 91f1  ....I......C. ..
+00001630: 5b6f 011f bc41 69cb e747 df6a 4f22 3ff9  [o...Ai..G.jO"?.
+00001640: d667 6053 234b 4f36 cebc 6ac4 57f5 1157  .g`S#KO6..j.W..W
+00001650: af6d 49dc 9433 2774 c649 9b35 b96e 8314  .mI..3't.I.5.n..
+00001660: 2bcd 9bf5 c3af 9fb6 2576 dc1f 8c7b dd6f  +.......%v...{.o
+00001670: 67c7 a727 5c76 5758 8f0c 9623 be5c 57a2  g..'\vWX...#.\W.
+00001680: 1bc3 ad2b 4713 b096 3bc1 ce78 650c 9acf  ...+G...;..xe...
+00001690: 46a1 b88b 5c28 a1d7 4de7 a0b7 92ed 4a5a  F...\(..M.....JZ
+000016a0: e293 5d87 aa94 e825 612a 2a0b 36d0 4801  ..]....%a**.6.H.
+000016b0: 71a7 22db 799c dc4d 3bdb 271d 1062 9003  q.".y..M;.'..b..
+000016c0: 5fb7 4c3b 296a 32dc bc9a cae4 c474 5cdf  _.L;)j2......t\.
+000016d0: e389 0a0c 2ab0 9d8f c712 c6d1 ee8c 38fa  ....*.........8.
+000016e0: 57a8 4ff8 a43f 98fc 3fe1 37dc 7f3a 63ac  W.O..?..?.7..:c.
+000016f0: 3b3f 91ce cb52 b18c 853a e0f7 1783 dd34  ;?...R...:.....4
+00001700: e389 30b9 e49b 55b0 e48b ed1e 9d72 4b33  ..0...U......rK3
+00001710: 9bee b699 1096 8d27 0b24 c2a2 19ae f84f  .......'.$.....O
+00001720: 0118 b780 bf2f 1169 3771 dd75 f73f 23f9  ...../.i7q.u.?#.
+00001730: 0b50 4b03 0414 0000 0008 0052 6372 5864  .PK........RcrXd
+00001740: 2f60 5f58 0100 00a8 0200 0018 0000 0078  /`_X...........x
+00001750: 6c2f 776f 726b 7368 6565 7473 2f73 6865  l/worksheets/she
+00001760: 6574 372e 786d 6c75 52db 4ec3 300c fd95  et7.xmluR.N.0...
+00001770: 2a1f b074 485c 34b5 95d8 2604 0f48 d326  *..tH\4...&..H.&
+00001780: e039 6bdd 365a 1297 c4a3 f0f7 38ed 2e20  .9k.6Z......8.. 
+00001790: 6d4f b19d 738e 7d9c 643d fa5d 6801 28f9  mO..s.}.d=.]h.(.
+000017a0: b6c6 855c b444 dd4c ca50 b660 5598 6007  ...\.D.L.P.`U.`.
+000017b0: 8e6f 6af4 5611 a7be 91a1 f3a0 aa81 648d  .oj.V.........d.
+000017c0: bc49 d33b 6995 76a2 c886 daca 1719 eec9  .I.;i.v.........
+000017d0: 6807 2b9f 84bd b5ca ffcc c160 9f8b a938  h.+........`...8
+000017e0: 16d6 ba69 6928 c822 eb54 031b a0b7 8e09  ...ii(.".T......
+000017f0: 9cca 934e a52d b8a0 d125 1eea 5c3c 4e67  ...N.-...%..\<Ng
+00001800: cb91 3120 de35 f4e1 4f9c 4433 5bc4 5d4c  ..1 .5..O.D3[.]L
+00001810: 5eaa 5ca4 7126 3050 5294 507c 7cc1 028c  ^.\.q&0PR.P||...
+00001820: 894a 3cc9 e741 549c 9b46 e6df f828 ff34  .J<..AT..F...(.4
+00001830: f8e7 f1b6 2ac0 02cd 87ae a8cd c583 482a  ....*.........H*
+00001840: a8d5 ded0 1afb 6738 78ba 3d8f b854 a48a  ......g8x.=..T..
+00001850: cc63 9ff8 68b6 c8ca 18c4 960c d42e 2e69  .c..h..........i
+00001860: 439e eb9a 3b51 a1ab 4c12 f78f 992c 0fe8  C...;Q..L....,..
+00001870: f935 b453 162e e017 d7f0 1584 d2eb 2e2e  .5.S............
+00001880: e302 6d79 8d46 aa09 fff1 920d 1db7 343a  ..my.F........4:
+00001890: 8c2f f8aa 7ca3 5d48 0cd4 ac93 4eee 790f  ./..|.]H....N.y.
+000018a0: 7e5c c998 1076 c38b 6f91 08ed 10b6 fc93  ~\...v..o.......
+000018b0: c047 00df d788 744a e293 9c3e 67f1 0b50  .G....tJ...>g..P
+000018c0: 4b03 0414 0000 0008 0052 6372 5855 85c6  K........RcrXU..
+000018d0: 84f8 0200 003f 0a00 0018 0000 0078 6c2f  .....?.......xl/
+000018e0: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
+000018f0: 382e 786d 6cbd 56db 72da 3010 fd15 c6cf  8.xml.V.r.0.....
+00001900: 4e0c 4c73 19c6 30c3 9db4 a1a5 81a4 8f1e  N.Ls..0.........
+00001910: 212f 5845 961c 691d 9abf efca 2424 cdd8  !/XE..i.....$$..
+00001920: 61ca 032f 20ad 7476 cf91 b4eb 0db7 da6c  a../ .tv.......l
+00001930: 6c02 80b5 3fa9 54b6 ed25 8859 2b08 2c4f  l...?.T..%.Y+.,O
+00001940: 2065 f65c 67a0 6865 a54d ca90 a666 1dd8   e.\g.he.M...f..
+00001950: cc00 8b0b 502a 8366 bd7e 19a4 4c28 af13  ....P*.f.~..L(..
+00001960: 16b6 99e9 843a 4729 14cc 4ccd e669 cacc  .....:G)..L..i..
+00001970: 730f a4de b6bd 86f7 6ab8 13eb 040b 43d0  s.......j.....C.
+00001980: 0933 b686 39e0 7d46 009a 067b 3fb1 4841  .3..9.}F...{?.HA
+00001990: 59a1 55cd c0aa ed75 1bad d90e 51ec 7810  Y.U....u....Q.x.
+000019a0: b0b5 efc6 3527 66a9 f5c6 4d6e e2b6 5777  ....5'f...Mn..Ww
+000019b0: 9c40 0247 e782 d1df 13f4 414a e789 983c  .@.G......AJ...<
+000019c0: be38 f5de 823a e4fb f1ab fb51 a19f e82d  .8...:.....Q...-
+000019d0: 9985 be96 bf44 8c49 dbbb f66a 31ac 582e  .....D.I...j1.X.
+000019e0: f14e 6f27 f0a2 e9e2 8de2 8021 eb84 466f  .No'.......!..Fo
+000019f0: 6bc6 89ed 84dc 0d5c 48da 2894 3ba4 391a  k......\H.(.;.9.
+00001a00: b20b 8a84 1d04 8b11 a8a7 3040 62e1 6c01  ..........0@b.l.
+00001a10: 7fc1 f4aa 308f 3998 e708 9f33 2841 f53f  ....0.9....3(A.?
+00001a20: 8dc4 ac05 b425 b041 158c ae9e 6b15 0b77  .....%.A....k..w
+00001a30: a065 c061 653c c332 1121 a499 6458 c674  .e.ae<.2.!..dX.t
+00001a40: 5485 e43a cdb4 0255 4a74 fca9 3e4e 9715  T..:...UJt..>N..
+00001a50: e9e5 6f28 6ebe 043e 390c b73a 37bc 0c7b  ..o(n..>9..:7..{
+00001a60: 7318 4ba7 150b 4e7a 23c5 d232 1f5f ffc7  s.K...Nz#..2._..
+00001a70: 8788 4b3c 7c3b ec41 a82c c772 f4ed 61b4  ..K<|;.A.,.r..a.
+00001a80: c995 0213 d143 41a1 d665 7730 ad72 521a  .....CA..ew0.rR.
+00001a90: f27b d5ee 8a23 fa51 b53f 06cb 8dc8 dc4b  .{...#.Q.?.....K
+00001aa0: 2c81 cd2a 95b1 8f22 024a cfd7 9cdf e56b  ,..*...".J.....k
+00001ab0: 4cbf 0f4c 0afa 77ef bcc6 75ae c8d9 a5f7  L..L..w...u.....
+00001ac0: 7169 5f43 9aad 6ea3 fee5 fae2 ea92 ea4a  qi_C..n........J
+00001ad0: a2b7 03a3 b381 de2a 5783 0ac3 8dbb 8429  .......*W......)
+00001ae0: 584b a56e 6f1c 1aa3 cd7b 2393 5426 7b92  XK.no....{#.T&{.
+00001af0: a94d 511a 5d52 b73d 292c 5264 5782 73c9  .MQ.]R.=),RdW.s.
+00001b00: 1a1d 2f86 279f 0bdf dd91 9f19 1d7b 61b0  ../.'........{a.
+00001b10: 5f0c 837f 1956 31ee 355b bdd3 3146 fa62  _....V1.5[..1F.b
+00001b20: a03d 86e7 b0d9 1a9e 8e27 3d41 29b4 a16c  .=.......'=A)..l
+00001b30: b3fe 8eb3 8f89 0188 129d f9b1 c9d7 d1ce  ................
+00001b40: 1a19 6620 8a85 054a 9162 e10c f5d9 1a14  ..f ...J.b......
+00001b50: 1ca3 71d4 6c8d 4ea7 f118 86e3 666b 7c3a  ..q.l.N.....fk|:
+00001b60: 865d ce21 43a6 382c dc13 ef81 e209 f50c  .].!C.8,........
+00001b70: 9b62 f633 670a 0532 57d1 9de1 1839 9366  .b.3g..2W....9.f
+00001b80: 6b72 3a39 f3e9 d09f 4fef ef46 fe58 e024  kr:9....O..F.X.$
+00001b90: 5fde 5b30 2380 78c9 f8c6 5f74 fb8b 9dc2  _.[0#.x..._t....
+00001ba0: 2929 f417 8629 4b5f 486d 16c0 52df 0974  ))...)K_Hm..R..t
+00001bb0: 25e9 56f3 42c0 e762 3f18 ecae b122 bf6b  %.V.B..b?....".k
+00001bc0: 4145 4cc2 8a6a 58fd fc8a da13 b3eb 5476  AEL..jX.......Tv
+00001bd0: 13d4 5941 7fa9 1175 5a0c 136a f0c0 b80d  ..YA...uZ..j....
+00001be0: b4be d21a f713 d729 ed7b c6ce 5f50 4b03  .......).{.._PK.
+00001bf0: 0414 0000 0008 0052 6372 5855 85c6 84f8  .......RcrXU....
+00001c00: 0200 003f 0a00 0018 0000 0078 6c2f 776f  ...?.......xl/wo
+00001c10: 726b 7368 6565 7473 2f73 6865 6574 392e  rksheets/sheet9.
+00001c20: 786d 6cbd 56db 72da 3010 fd15 c6cf 4e0c  xml.V.r.0.....N.
+00001c30: 4c73 19c6 30c3 9db4 a1a5 81a4 8f1e 212f  Ls..0.........!/
+00001c40: 5845 961c 691d 9abf efca 2424 cdd8 61ca  XE..i.....$$..a.
+00001c50: 032f 20ad 7476 cf91 b4eb 0db7 da6c 6c02  ./ .tv.......ll.
+00001c60: 80b5 3fa9 54b6 ed25 8859 2b08 2c4f 2065  ..?.T..%.Y+.,O e
+00001c70: f65c 67a0 6865 a54d ca90 a666 1dd8 cc00  .\g.he.M...f....
+00001c80: 8b0b 502a 8366 bd7e 19a4 4c28 af13 16b6  ..P*.f.~..L(....
+00001c90: 99e9 843a 4729 14cc 4ccd e669 cacc 730f  ...:G)..L..i..s.
+00001ca0: a4de b6bd 86f7 6ab8 13eb 040b 43d0 0933  ......j.....C..3
+00001cb0: b686 39e0 7d46 009a 067b 3fb1 4841 59a1  ..9.}F...{?.HAY.
+00001cc0: 55cd c0aa ed75 1bad d90e 51ec 7810 b0b5  U....u....Q.x...
+00001cd0: efc6 3527 66a9 f5c6 4d6e e2b6 5777 9c40  ..5'f...Mn..Ww.@
+00001ce0: 0247 e782 d1df 13f4 414a e789 983c be38  .G......AJ...<.8
+00001cf0: f5de 823a e4fb f1ab fb51 a19f e82d 9985  ...:.....Q...-..
+00001d00: be96 bf44 8c49 dbbb f66a 31ac 582e f14e  ...D.I...j1.X..N
+00001d10: 6f27 f0a2 e9e2 8de2 8021 eb84 466f 6bc6  o'.......!..Fok.
+00001d20: 89ed 84dc 0d5c 48da 2894 3ba4 391a b20b  .....\H.(.;.9...
+00001d30: 8a84 1d04 8b11 a8a7 3040 62e1 6c01 7fc1  ........0@b.l...
+00001d40: f4aa 308f 3998 e708 9f33 2841 f53f 8dc4  ..0.9....3(A.?..
+00001d50: ac05 b425 b041 158c ae9e 6b15 0b77 a065  ...%.A....k..w.e
+00001d60: c061 653c c332 1121 a499 6458 c674 5485  .ae<.2.!..dX.tT.
+00001d70: e43a cdb4 0255 4a74 fca9 3e4e 9715 e9e5  .:...UJt..>N....
+00001d80: 6f28 6ebe 043e 390c b73a 37bc 0c7b 7318  o(n..>9..:7..{s.
+00001d90: 4ba7 150b 4e7a 23c5 d232 1f5f ffc7 8788  K...Nz#..2._....
+00001da0: 4b3c 7c3b ec41 a82c c772 f4ed 61b4 c995  K<|;.A.,.r..a...
+00001db0: 0213 d143 41a1 d665 7730 ad72 521a f27b  ...CA..ew0.rR..{
+00001dc0: d5ee 8a23 fa51 b53f 06cb 8dc8 dc4b 2c81  ...#.Q.?.....K,.
+00001dd0: cd2a 95b1 8f22 024a cfd7 9cdf e56b 4cbf  .*...".J.....kL.
+00001de0: 0f4c 0afa 77ef bcc6 75ae c8d9 a5f7 7169  .L..w...u.....qi
+00001df0: 5f43 9aad 6ea3 fee5 fae2 ea92 ea4a a2b7  _C..n........J..
+00001e00: 03a3 b381 de2a 5783 0ac3 8dbb 8429 584b  .....*W......)XK
+00001e10: a56e 6f1c 1aa3 cd7b 2393 5426 7b92 a94d  .no....{#.T&{..M
+00001e20: 511a 5d52 b73d 292c 5264 5782 73c9 1a1d  Q.]R.=),RdW.s...
+00001e30: 2f86 279f 0bdf dd91 9f19 1d7b 61b0 5f0c  /.'........{a._.
+00001e40: 837f 1956 31ee 355b bdd3 3146 fa62 a03d  ...V1.5[..1F.b.=
+00001e50: 86e7 b0d9 1a9e 8e27 3d41 29b4 a16c b3fe  .......'=A)..l..
+00001e60: 8eb3 8f89 0188 129d f9b1 c9d7 d1ce 1a19  ................
+00001e70: 6620 8a85 054a 9162 e10c f5d9 1a14 1ca3  f ...J.b........
+00001e80: 71d4 6c8d 4ea7 f118 86e3 666b 7c3a 865d  q.l.N.....fk|:.]
+00001e90: ce21 43a6 382c dc13 ef81 e209 f50c 9b62  .!C.8,.........b
+00001ea0: f633 670a 0532 57d1 9de1 1839 9366 6b72  .3g..2W....9.fkr
+00001eb0: 3a39 f3e9 d09f 4fef ef46 fe58 e024 5fde  :9....O..F.X.$_.
+00001ec0: 5b30 2380 78c9 f8c6 5f74 fb8b 9dc2 2929  [0#.x..._t....))
+00001ed0: f417 8629 4b5f 486d 16c0 52df 0974 25e9  ...)K_Hm..R..t%.
+00001ee0: 56f3 42c0 e762 3f18 ecae b122 bf6b 4145  V.B..b?....".kAE
+00001ef0: 4cc2 8a6a 58fd fc8a da13 b3eb 5476 13d4  L..jX.......Tv..
+00001f00: 5941 7fa9 1175 5a0c 136a f0c0 b80d b4be  YA...uZ..j......
+00001f10: d21a f713 d729 ed7b c6ce 5f50 4b03 0414  .....).{.._PK...
+00001f20: 0000 0008 0052 6372 5855 85c6 84f8 0200  .....RcrXU......
+00001f30: 003f 0a00 0019 0000 0078 6c2f 776f 726b  .?.......xl/work
+00001f40: 7368 6565 7473 2f73 6865 6574 3130 2e78  sheets/sheet10.x
+00001f50: 6d6c bd56 db72 da30 10fd 15c6 cf4e 0c4c  ml.V.r.0.....N.L
+00001f60: 7319 c630 c39d b4a1 a581 a48f 1e21 2f58  s..0.........!/X
+00001f70: 4596 1c69 1d9a bfef ca24 24cd d861 ca03  E..i.....$$..a..
+00001f80: 2f20 ad74 76cf 91b4 eb0d b7da 6c6c 0280  / .tv.......ll..
+00001f90: b53f a954 b6ed 2588 592b 082c 4f20 65f6  .?.T..%.Y+.,O e.
+00001fa0: 5c67 a068 65a5 4dca 90a6 661d d8cc 008b  \g.he.M...f.....
+00001fb0: 0b50 2a83 66bd 7e19 a44c 28af 1316 b699  .P*.f.~..L(.....
+00001fc0: e984 3a47 2914 cc4c cde6 69ca cc73 0fa4  ..:G)..L..i..s..
+00001fd0: deb6 bd86 f76a b813 eb04 0b43 d009 33b6  .....j.....C..3.
+00001fe0: 8639 e07d 4600 9a06 7b3f b148 4159 a155  .9.}F...{?.HAY.U
+00001ff0: cdc0 aaed 751b add9 0e51 ec78 10b0 b5ef  ....u....Q.x....
+00002000: c635 2766 a9f5 c64d 6ee2 b657 779c 4002  .5'f...Mn..Ww.@.
+00002010: 47e7 82d1 df13 f441 4ae7 8998 3cbe 38f5  G......AJ...<.8.
+00002020: de82 3ae4 fbf1 abfb 51a1 9fe8 2d99 85be  ..:.....Q...-...
+00002030: 96bf 448c 49db bbf6 6a31 ac58 2ef1 4e6f  ..D.I...j1.X..No
+00002040: 27f0 a2e9 e28d e280 21eb 8446 6f6b c689  '.......!..Fok..
+00002050: ed84 dc0d 5c48 da28 943b a439 1ab2 0b8a  ....\H.(.;.9....
+00002060: 841d 048b 11a8 a730 4062 e16c 017f c1f4  .......0@b.l....
+00002070: aa30 8f39 98e7 089f 3328 41f5 3f8d c4ac  .0.9....3(A.?...
+00002080: 05b4 25b0 4115 8cae 9e6b 150b 77a0 65c0  ..%.A....k..w.e.
+00002090: 6165 3cc3 3211 21a4 9964 58c6 7454 85e4  ae<.2.!..dX.tT..
+000020a0: 3acd b402 554a 74fc a93e 4e97 15e9 e56f  :...UJt..>N....o
+000020b0: 286e be04 3e39 0cb7 3a37 bc0c 7b73 184b  (n..>9..:7..{s.K
+000020c0: a715 0b4e 7a23 c5d2 321f 5fff c787 884b  ...Nz#..2._....K
+000020d0: 3c7c 3bec 41a8 2cc7 72f4 ed61 b4c9 9502  <|;.A.,.r..a....
+000020e0: 13d1 4341 a1d6 6577 30ad 7252 1af2 7bd5  ..CA..ew0.rR..{.
+000020f0: ee8a 23fa 51b5 3f06 cb8d c8dc 4b2c 81cd  ..#.Q.?.....K,..
+00002100: 2a95 b18f 2202 4acf d79c dfe5 6b4c bf0f  *...".J.....kL..
+00002110: 4c0a fa77 efbc c675 aec8 d9a5 f771 695f  L..w...u.....qi_
+00002120: 439a ad6e a3fe e5fa e2ea 92ea 4aa2 b703  C..n........J...
+00002130: a3b3 81de 2a57 830a c38d bb84 2958 4ba5  ....*W......)XK.
+00002140: 6e6f 1c1a a3cd 7b23 9354 267b 92a9 4d51  no....{#.T&{..MQ
+00002150: 1a5d 52b7 3d29 2c52 6457 8273 c91a 1d2f  .]R.=),RdW.s.../
+00002160: 8627 9f0b dfdd 919f 191d 7b61 b05f 0c83  .'........{a._..
+00002170: 7f19 5631 ee35 5bbd d331 46fa 62a0 3d86  ..V1.5[..1F.b.=.
+00002180: e7b0 d91a 9e8e 273d 4129 b4a1 6cb3 fe8e  ......'=A)..l...
+00002190: b38f 8901 8812 9df9 b1c9 d7d1 ce1a 1966  ...............f
+000021a0: 208a 8505 4a91 62e1 0cf5 d91a 141c a371   ...J.b........q
+000021b0: d46c 8d4e a7f1 1886 e366 6b7c 3a86 5dce  .l.N.....fk|:.].
+000021c0: 2143 a638 2cdc 13ef 81e2 09f5 0c9b 62f6  !C.8,.........b.
+000021d0: 3367 0a05 3257 d19d e118 3993 666b 723a  3g..2W....9.fkr:
+000021e0: 39f3 e9d0 9f4f efef 46fe 58e0 245f de5b  9....O..F.X.$_.[
+000021f0: 3023 8078 c9f8 c65f 74fb 8b9d c229 29f4  0#.x..._t....)).
+00002200: 1786 294b 5f48 6d16 c052 df09 7425 e956  ..)K_Hm..R..t%.V
+00002210: f342 c0e7 623f 18ec aeb1 22bf 6b41 454c  .B..b?....".kAEL
+00002220: c28a 6a58 fdfc 8ada 13b3 eb54 7613 d459  ..jX.......Tv..Y
+00002230: 417f a911 755a 0c13 6af0 c0b8 0db4 bed2  A...uZ..j.......
+00002240: 1af7 13d7 29ed 7bc6 ce5f 504b 0304 1400  ....).{.._PK....
+00002250: 0000 0800 5263 7258 3013 165e 0d03 0000  ....RcrX0..^....
+00002260: b30a 0000 1900 0000 786c 2f77 6f72 6b73  ........xl/works
+00002270: 6865 6574 732f 7368 6565 7431 312e 786d  heets/sheet11.xm
+00002280: 6cbd 5651 53db 300c fe2b bd3c 67a4 f406  l.VQS.0..+.<g...
+00002290: e37a 69ef a005 5a46 3728 657b ccb9 8eda  .zi...ZF7(e{....
+000022a0: 7875 accc 56e8 f8f7 9353 288c 4bca 8d87  xu..V....S(.K...
+000022b0: beb4 b6ec 4ffa 3e5b 5614 afd1 ae5c 0640  ....O.>[V....\.@
+000022c0: ad3f b936 ae17 6444 4537 8a9c cc20 17ee  .?.6..dDE7... ..
+000022d0: 000b 30bc b240 9b0b e2a9 5d46 aeb0 20d2  ..0..@....]F.. .
+000022e0: 0a94 eba8 d36e 1f47 b950 26e8 c795 edc6  .....n.G.P&.....
+000022f0: f663 2c49 2b03 37b6 e5ca 3c17 f6f1 0c34  .c,I+.7...<....4
+00002300: ae7b c161 f06c 98aa 6546 9521 eac7 8558  .{.a.l..eF.!...X
+00002310: c21d d07d c100 9e46 5b3f a9ca c138 85a6  ...}...F[?...8..
+00002320: 6561 d10b 4e0f bbd3 0da2 daf1 43c1 dabd  ea..N.......C...
+00002330: 1ab7 bc98 39e2 ca4f c669 2f68 7b4e a041  ....9..O.i/h{N.A
+00002340: 9277 21f8 ef01 06a0 b5f7 c44c 7e3f 390d  .w!........L~?9.
+00002350: 5e82 7ae4 ebf1 b3fb 8b4a 3fd3 9b0b 0703  ^.z......J?.....
+00002360: d43f 554a 592f 3809 5a29 2c44 a969 8aeb  .?UJY/8.Z),D.i..
+00002370: 113c 693a 7aa1 3814 24fa b1c5 75cb 7ab1  .<i:z.8.$...u.z.
+00002380: fd58 fa81 0fc9 1b95 f187 7447 96ed 8a23  .X........tG...#
+00002390: 519f ac28 54f2 00d6 6b8e 2362 2a7e 2192  Q..(T...k.#b*~!.
+000023a0: 4fc0 b326 e05c 219b 563b a083 c698 e028  O..&.\!.V;.....(
+000023b0: 01f3 5083 1936 617e 9760 1f13 7a2c a006  ..P..6a~.`..z,..
+000023c0: 75be 3392 700e c8d5 c02e 9a60 9c6e 124d  u.3.p......`.n.M
+000023d0: aafc 25d6 012f 779f 2641 5e68 4175 4c47  ..%../w.&A^hAuLG
+000023e0: 4d48 8979 8106 4c2d d1f1 4e7d 9213 24c1  MH.y..L-..N}..$.
+000023f0: f92f a8b2 ad06 7ef5 3edc 6169 651d f6eb  ./....~.>.aie...
+00002400: fb58 3ead 5449 d69b 1891 d7f9 b8fe 1f1f  .X>.TI..........
+00002410: 2aad f130 79df 8332 4549 f5e8 6fef a36d  *..0y..2EI..o..m
+00002420: 690c d884 1385 9459 d6dd c1f7 2627 b521  i......Y....&'.!
+00002430: 6f9a 7637 1cd1 6dd3 fe14 9cb4 aaa0 fa27  o.v7..m........'
+00002440: 366d 5426 de8a 88b8 243c d799 4d8d 48f9  6mT&....$<..M.H.
+00002450: f787 d08a ff7d 9eb7 2496 869d 1d07 6f97  .....}..$.....o.
+00002460: 9eeb d6a0 d31d 1cb6 3f9f 1c7d 39e6 5a96  ........?..}9.Z.
+00002470: e17a 68b1 18e2 daf8 ba57 19c6 fe12 26e0  .zh......W....&.
+00002480: 1c97 d7ad f1dc 5ab4 af8d 4273 693e d3c2  ......Z...Bsi>..
+00002490: acaa 72ec 1f75 2fd0 ca11 47f6 65bf d4e2  ..r..u/...G.e...
+000024a0: b01f a4f0 104a 15fa 3b0a 0b8b 6910 47db  .....J..;...i.G.
+000024b0: c538 fa97 6113 e361 a73b dc1f 63e2 af14  .8..a..a.;..c...
+000024c0: b98f f0bc ec74 2ff7 c793 5350 2bb4 fcda  .....t/...SP+...
+000024d0: 5cb8 e11c 5266 0192 0c8b 30b5 e532 d958  \...Rf....0..2.X
+000024e0: 132b 2c24 a972 c04f a45a f844 f869 0906  .+,$.r.O.Z.D.i..
+000024f0: 3ea2 71d4 e98e f6a7 f123 0cc7 9dee 787f  >.q......#....x.
+00002500: 0c4f a584 8284 9130 f329 7e06 4666 dca7  .O.....0.)~.Ff..
+00002510: acaa d96d 290c 2912 bea2 7bc3 47e4 5c75  ...m).)...{.G.\u
+00002520: ba57 fb93 7337 390f ef26 f7d3 8bf0 52d1  .W..s79..&....R.
+00002530: a89c df3b b017 00e9 5cc8 5538 3b1d cc36  ...;....\.U8;..6
+00002540: 0a27 ac30 9c59 611c 7f21 d1ce 40e4 a117  .'.0.Ya..!..@...
+00002550: e84b d235 ca4a c06e b16f 0c6e d3cc b1df  .K.5.J.n.o.n....
+00002560: a5e2 22a6 61c1 35ac 7df0 855b 22bb e98e  ..".a.5.}..["...
+00002570: 3613 c2a2 a23f 4722 ccab 61c6 4d25 58bf  6....?G"..a.M%X.
+00002580: 81d7 1788 b49d f8ee 6cdb a7f6 ff02 504b  ........l.....PK
+00002590: 0304 1400 0000 0800 5263 7258 5585 c684  ........RcrXU...
+000025a0: f802 0000 3f0a 0000 1900 0000 786c 2f77  ....?.......xl/w
+000025b0: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
+000025c0: 322e 786d 6cbd 56db 72da 3010 fd15 c6cf  2.xml.V.r.0.....
+000025d0: 4e0c 4c73 19c6 30c3 9db4 a1a5 81a4 8f1e  N.Ls..0.........
+000025e0: 212f 5845 961c 691d 9abf efca 2424 cdd8  !/XE..i.....$$..
+000025f0: 61ca 032f 20ad 7476 cf91 b4eb 0db7 da6c  a../ .tv.......l
+00002600: 6c02 80b5 3fa9 54b6 ed25 8859 2b08 2c4f  l...?.T..%.Y+.,O
+00002610: 2065 f65c 67a0 6865 a54d ca90 a666 1dd8   e.\g.he.M...f..
+00002620: cc00 8b0b 502a 8366 bd7e 19a4 4c28 af13  ....P*.f.~..L(..
+00002630: 16b6 99e9 843a 4729 14cc 4ccd e669 cacc  .....:G)..L..i..
+00002640: 730f a4de b6bd 86f7 6ab8 13eb 040b 43d0  s.......j.....C.
+00002650: 0933 b686 39e0 7d46 009a 067b 3fb1 4841  .3..9.}F...{?.HA
+00002660: 59a1 55cd c0aa ed75 1bad d90e 51ec 7810  Y.U....u....Q.x.
+00002670: b0b5 efc6 3527 66a9 f5c6 4d6e e2b6 5777  ....5'f...Mn..Ww
+00002680: 9c40 0247 e782 d1df 13f4 414a e789 983c  .@.G......AJ...<
+00002690: be38 f5de 823a e4fb f1ab fb51 a19f e82d  .8...:.....Q...-
+000026a0: 9985 be96 bf44 8c49 dbbb f66a 31ac 582e  .....D.I...j1.X.
+000026b0: f14e 6f27 f0a2 e9e2 8de2 8021 eb84 466f  .No'.......!..Fo
+000026c0: 6bc6 89ed 84dc 0d5c 48da 2894 3ba4 391a  k......\H.(.;.9.
+000026d0: b20b 8a84 1d04 8b11 a8a7 3040 62e1 6c01  ..........0@b.l.
+000026e0: 7fc1 f4aa 308f 3998 e708 9f33 2841 f53f  ....0.9....3(A.?
+000026f0: 8dc4 ac05 b425 b041 158c ae9e 6b15 0b77  .....%.A....k..w
+00002700: a065 c061 653c c332 1121 a499 6458 c674  .e.ae<.2.!..dX.t
+00002710: 5485 e43a cdb4 0255 4a74 fca9 3e4e 9715  T..:...UJt..>N..
+00002720: e9e5 6f28 6ebe 043e 390c b73a 37bc 0c7b  ..o(n..>9..:7..{
+00002730: 7318 4ba7 150b 4e7a 23c5 d232 1f5f ffc7  s.K...Nz#..2._..
+00002740: 8788 4b3c 7c3b ec41 a82c c772 f4ed 61b4  ..K<|;.A.,.r..a.
+00002750: c995 0213 d143 41a1 d665 7730 ad72 521a  .....CA..ew0.rR.
+00002760: f27b d5ee 8a23 fa51 b53f 06cb 8dc8 dc4b  .{...#.Q.?.....K
+00002770: 2c81 cd2a 95b1 8f22 024a cfd7 9cdf e56b  ,..*...".J.....k
+00002780: 4cbf 0f4c 0afa 77ef bcc6 75ae c8d9 a5f7  L..L..w...u.....
+00002790: 7169 5f43 9aad 6ea3 fee5 fae2 ea92 ea4a  qi_C..n........J
+000027a0: a2b7 03a3 b381 de2a 5783 0ac3 8dbb 8429  .......*W......)
+000027b0: 584b a56e 6f1c 1aa3 cd7b 2393 5426 7b92  XK.no....{#.T&{.
+000027c0: a94d 511a 5d52 b73d 292c 5264 5782 73c9  .MQ.]R.=),RdW.s.
+000027d0: 1a1d 2f86 279f 0bdf dd91 9f19 1d7b 61b0  ../.'........{a.
+000027e0: 5f0c 837f 1956 31ee 355b bdd3 3146 fa62  _....V1.5[..1F.b
+000027f0: a03d 86e7 b0d9 1a9e 8e27 3d41 29b4 a16c  .=.......'=A)..l
+00002800: b3fe 8eb3 8f89 0188 129d f9b1 c9d7 d1ce  ................
+00002810: 1a19 6620 8a85 054a 9162 e10c f5d9 1a14  ..f ...J.b......
+00002820: 1ca3 71d4 6c8d 4ea7 f118 86e3 666b 7c3a  ..q.l.N.....fk|:
+00002830: 865d ce21 43a6 382c dc13 ef81 e209 f50c  .].!C.8,........
+00002840: 9b62 f633 670a 0532 57d1 9de1 1839 9366  .b.3g..2W....9.f
+00002850: 6b72 3a39 f3e9 d09f 4fef ef46 fe58 e024  kr:9....O..F.X.$
+00002860: 5fde 5b30 2380 78c9 f8c6 5f74 fb8b 9dc2  _.[0#.x..._t....
+00002870: 2929 f417 8629 4b5f 486d 16c0 52df 0974  ))...)K_Hm..R..t
+00002880: 25e9 56f3 42c0 e762 3f18 ecae b122 bf6b  %.V.B..b?....".k
+00002890: 4145 4cc2 8a6a 58fd fc8a da13 b3eb 5476  AEL..jX.......Tv
+000028a0: 13d4 5941 7fa9 1175 5a0c 136a f0c0 b80d  ..YA...uZ..j....
+000028b0: b4be d21a f713 d729 ed7b c6ce 5f50 4b03  .......).{.._PK.
+000028c0: 0414 0000 0008 0052 6372 5855 85c6 84f8  .......RcrXU....
+000028d0: 0200 003f 0a00 0019 0000 0078 6c2f 776f  ...?.......xl/wo
+000028e0: 726b 7368 6565 7473 2f73 6865 6574 3133  rksheets/sheet13
+000028f0: 2e78 6d6c bd56 db72 da30 10fd 15c6 cf4e  .xml.V.r.0.....N
+00002900: 0c4c 7319 c630 c39d b4a1 a581 a48f 1e21  .Ls..0.........!
+00002910: 2f58 4596 1c69 1d9a bfef ca24 24cd d861  /XE..i.....$$..a
+00002920: ca03 2f20 ad74 76cf 91b4 eb0d b7da 6c6c  ../ .tv.......ll
+00002930: 0280 b53f a954 b6ed 2588 592b 082c 4f20  ...?.T..%.Y+.,O 
+00002940: 65f6 5c67 a068 65a5 4dca 90a6 661d d8cc  e.\g.he.M...f...
+00002950: 008b 0b50 2a83 66bd 7e19 a44c 28af 1316  ...P*.f.~..L(...
+00002960: b699 e984 3a47 2914 cc4c cde6 69ca cc73  ....:G)..L..i..s
+00002970: 0fa4 deb6 bd86 f76a b813 eb04 0b43 d009  .......j.....C..
+00002980: 33b6 8639 e07d 4600 9a06 7b3f b148 4159  3..9.}F...{?.HAY
+00002990: a155 cdc0 aaed 751b add9 0e51 ec78 10b0  .U....u....Q.x..
+000029a0: b5ef c635 2766 a9f5 c64d 6ee2 b657 779c  ...5'f...Mn..Ww.
+000029b0: 4002 47e7 82d1 df13 f441 4ae7 8998 3cbe  @.G......AJ...<.
+000029c0: 38f5 de82 3ae4 fbf1 abfb 51a1 9fe8 2d99  8...:.....Q...-.
+000029d0: 85be 96bf 448c 49db bbf6 6a31 ac58 2ef1  ....D.I...j1.X..
+000029e0: 4e6f 27f0 a2e9 e28d e280 21eb 8446 6f6b  No'.......!..Fok
+000029f0: c689 ed84 dc0d 5c48 da28 943b a439 1ab2  ......\H.(.;.9..
+00002a00: 0b8a 841d 048b 11a8 a730 4062 e16c 017f  .........0@b.l..
+00002a10: c1f4 aa30 8f39 98e7 089f 3328 41f5 3f8d  ...0.9....3(A.?.
+00002a20: c4ac 05b4 25b0 4115 8cae 9e6b 150b 77a0  ....%.A....k..w.
+00002a30: 65c0 6165 3cc3 3211 21a4 9964 58c6 7454  e.ae<.2.!..dX.tT
+00002a40: 85e4 3acd b402 554a 74fc a93e 4e97 15e9  ..:...UJt..>N...
+00002a50: e56f 286e be04 3e39 0cb7 3a37 bc0c 7b73  .o(n..>9..:7..{s
+00002a60: 184b a715 0b4e 7a23 c5d2 321f 5fff c787  .K...Nz#..2._...
+00002a70: 884b 3c7c 3bec 41a8 2cc7 72f4 ed61 b4c9  .K<|;.A.,.r..a..
+00002a80: 9502 13d1 4341 a1d6 6577 30ad 7252 1af2  ....CA..ew0.rR..
+00002a90: 7bd5 ee8a 23fa 51b5 3f06 cb8d c8dc 4b2c  {...#.Q.?.....K,
+00002aa0: 81cd 2a95 b18f 2202 4acf d79c dfe5 6b4c  ..*...".J.....kL
+00002ab0: bf0f 4c0a fa77 efbc c675 aec8 d9a5 f771  ..L..w...u.....q
+00002ac0: 695f 439a ad6e a3fe e5fa e2ea 92ea 4aa2  i_C..n........J.
+00002ad0: b703 a3b3 81de 2a57 830a c38d bb84 2958  ......*W......)X
+00002ae0: 4ba5 6e6f 1c1a a3cd 7b23 9354 267b 92a9  K.no....{#.T&{..
+00002af0: 4d51 1a5d 52b7 3d29 2c52 6457 8273 c91a  MQ.]R.=),RdW.s..
+00002b00: 1d2f 8627 9f0b dfdd 919f 191d 7b61 b05f  ./.'........{a._
+00002b10: 0c83 7f19 5631 ee35 5bbd d331 46fa 62a0  ....V1.5[..1F.b.
+00002b20: 3d86 e7b0 d91a 9e8e 273d 4129 b4a1 6cb3  =.......'=A)..l.
+00002b30: fe8e b38f 8901 8812 9df9 b1c9 d7d1 ce1a  ................
+00002b40: 1966 208a 8505 4a91 62e1 0cf5 d91a 141c  .f ...J.b.......
+00002b50: a371 d46c 8d4e a7f1 1886 e366 6b7c 3a86  .q.l.N.....fk|:.
+00002b60: 5dce 2143 a638 2cdc 13ef 81e2 09f5 0c9b  ].!C.8,.........
+00002b70: 62f6 3367 0a05 3257 d19d e118 3993 666b  b.3g..2W....9.fk
+00002b80: 723a 39f3 e9d0 9f4f efef 46fe 58e0 245f  r:9....O..F.X.$_
+00002b90: de5b 3023 8078 c9f8 c65f 74fb 8b9d c229  .[0#.x..._t....)
+00002ba0: 29f4 1786 294b 5f48 6d16 c052 df09 7425  )...)K_Hm..R..t%
+00002bb0: e956 f342 c0e7 623f 18ec aeb1 22bf 6b41  .V.B..b?....".kA
+00002bc0: 454c c28a 6a58 fdfc 8ada 13b3 eb54 7613  EL..jX.......Tv.
+00002bd0: d459 417f a911 755a 0c13 6af0 c0b8 0db4  .YA...uZ..j.....
+00002be0: bed2 1af7 13d7 29ed 7bc6 ce5f 504b 0304  ......).{.._PK..
+00002bf0: 1400 0000 0800 5263 7258 2359 55fc e301  ......RcrX#YU...
+00002c00: 0000 0704 0000 1900 0000 786c 2f77 6f72  ..........xl/wor
+00002c10: 6b73 6865 6574 732f 7368 6565 7431 342e  ksheets/sheet14.
+00002c20: 786d 6c8d 536d 6fda 3010 fe2b 913f 5735  xml.Smo.0..+.?W5
+00002c30: 54eb 8b50 12a9 40d1 3a8d ad2a 1bd3 3e21  T..P..@.:..*..>!
+00002c40: 935c 8885 e3cb eccb b2fe fb9d 13a0 a081  .\..............
+00002c50: b44f be7b fcdc e37b 73dc a2db fa12 80a2  .O.{...{s.......
+00002c60: 3f95 b13e 1125 513d 92d2 6725 54ca 5f63  ?..>.%Q=..g%T._c
+00002c70: 0d96 6f0a 7495 2276 dd46 fada 81ca bba0  ..o.t."v.F......
+00002c80: cac8 9bc1 e04e 564a 5b91 c61d f6e2 d218  .....NVJ[.......
+00002c90: 1b32 dac2 8b8b 7c53 55ca bd8d c160 9b88  .2....|SU....`..
+00002ca0: a1d8 03af 7a53 5207 c834 aed5 0616 40df  ....zSR..4....@.
+00002cb0: 6b0e 6057 1e74 725d 81f5 1a6d e4a0 48c4  k.`W.tr]...m..H.
+00002cc0: e370 34eb 233a c652 43eb 8fec 2814 b346  .p4.#:.RC...(..F
+00002cd0: dc06 e739 4fc4 20e4 0406 320a 128a 8fdf  ...9O. ...2.....
+00002ce0: 3001 6382 1267 f26b 272a de1f 0d91 c7f6  0.c..g.k'*......
+00002cf0: 5e7e d6d5 cfe9 ad95 8709 9a1f 3aa7 3211  ^~..........:.2.
+00002d00: 0f22 caa1 508d a157 6c3f c2ae a6db f714  ."..P..Wl?......
+00002d10: a78a 541a 3b6c 2317 8a4d e32c 18e1 4926  ..T.;l#..M.,..I&
+00002d20: 6a1b 9ab4 20c7 b8e6 9728 25f0 b4ca 3966  j... ....(%...9f
+00002d30: 5568 032b 8399 2274 b124 ce29 3064 b653  Uh.+.."t.$.)0d.S
+00002d40: 18ff a742 3fb7 3302 934b 023a 3fc3 9e5e  ...B?.3..K.:?..^
+00002d50: 625b 55c1 19fe d325 7e0e 3e73 ba0e f338  b[U....%~.>s...8
+00002d60: 1336 bb58 95da f853 bee4 9eee 07d5 3739  .6.X...S......79
+00002d70: 14bd 5446 f3c9 ea3e cab0 b1d4 37fd f46a  ..TF...>....7..j
+00002d80: 3ff8 f1cd 683c 1c7c 78b8 bdbf e365 28b1  ?...h<.|x....e(.
+00002d90: 9d3a aca7 d8da b038 1df0 6ceb 86e6 e03d  .:.....8..l....=
+00002da0: efe7 017c 720e dd31 a80c eff6 d828 bbed  ...|r..1.....(..
+00002db0: f699 de6a c68d f6c4 2f87 fe37 460d 53f1  ...j..../..7F.S.
+00002dc0: 6db1 bcfa f938 ff7c f569 f1f5 8b88 e5e1  m....8.|.i......
+00002dd0: 2696 a7e9 fd03 f8fe 83cc 95db 68ae cb40  &...........h..@
+00002de0: c165 0dae ef79 cd5c bf71 bd43 5877 09ac  .e...y.\.q.CXw..
+00002df0: 9108 abce 2cf9 a382 0b04 be2f 10e9 e084  ....,....../....
+00002e00: 8d3f fcfd f42f 504b 0304 1400 0000 0800  .?.../PK........
+00002e10: 5263 7258 bc72 e0e6 ff01 0000 8104 0000  RcrX.r..........
+00002e20: 1900 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
+00002e30: 732f 7368 6565 7431 352e 786d 6c7d 54db  s/sheet15.xml}T.
+00002e40: 6edb 300c fd15 43cf 4195 14eb 0581 63a0  n.0...C.A.....c.
+00002e50: 49da a5c0 0214 2dda 3d16 8a4c c742 749b  I.....-.=..L.Bt.
+00002e60: 44cf ebdf 8fb2 9334 dd92 3c59 3ce2 2179  D......4..<Y<.!y
+00002e70: 44d2 79eb c226 d600 98fd 31da c609 ab11  D.y..&....1.....
+00002e80: fd98 f328 6b30 225e 380f 966e 2a17 8c40  ...(k0"^8..n*..@
+00002e90: 32c3 9a47 1f40 941d c968 7e39 1c5e 7323  2..G.@...h~9.^s#
+00002ea0: 9465 45de 614f a1c8 5d83 5a59 780a 596c  .eE.aO..].ZYx.Yl
+00002eb0: 8c11 e163 0ada b513 3662 3be0 59ad 6bec  ...c....6b;.Y.k.
+00002ec0: 005e e45e ace1 05f0 d513 814c be8f 532a  .^.^.......L..S*
+00002ed0: 0336 2a67 b300 d584 dd8d c68b 9ed1 79bc  .6*g..........y.
+00002ee0: 2968 e3c1 394b 6256 ce6d 92f1 584e d830  )h..9KbV.m..XN.0
+00002ef0: d504 1a24 a610 823e bf61 065a a748 54c9  ...$...>.a.Z.HT.
+00002f00: af6d 50f6 9934 310f cfbb f00f 9d7e 2a6f  .mP..41......~*o
+00002f10: 2522 cc9c fea9 4aac 27ec 9665 2554 a2d1  %"....J.'..e%T..
+00002f20: f8ec da05 6c35 5d7d 9638 1728 8a3c b836  ....l5]}.8.(.<.6
+00002f30: 0b49 6c91 cb74 4829 c951 d9f4 482f 1808  .Il..tH).Q..H/..
+00002f40: 5794 090b 8488 ef06 5094 c4cb 3952 29e9  W.......P...9R).
+00002f50: 82cb 2d71 7a96 e821 4467 8ff1 6667 7992  ..-qz..!Dg..fgy.
+00002f60: 34c5 23ac f959 566c 14c2 7bf4 2055 a5a4  4.#..YVl..{. U..
+00002f70: 484f 7c24 c6fd a918 aa3c e2fd 70ca db0a  HO|$.....<..p...
+00002f80: 0347 fcbf 9ff2 2f21 caa0 fc89 a216 2785  .G..../!......'.
+00002f90: 89f5 3f0f c1a9 77bb 81e8 9b99 5af3 26b4  ..?...w.....Z.&.
+00002fa0: 2a3b c931 93ae b1d8 37f7 ebd5 6ec0 a697  *;.1....7...n...
+00002fb0: e3e9 68f8 edf6 eae6 9a86 ae76 ed3c 383f  ..h........v.<8?
+00002fc0: 77ad 4d03 da01 8fd6 37b8 8418 690f f6e0  w.M.....7...i...
+00002fd0: 7d08 2e1c 8242 d30e 4db5 b09b 6e6f f0c3  }....B..M...no..
+00002fe0: 13ae 5544 ca9c f6b3 d162 54b0 3bad 0733  ..UD.....bT.;..3
+00002ff0: d245 2dd1 831f b40c af7e b004 590b 4b9e  .E-......~..Y.K.
+00003000: 4ab2 9cef 7d73 feb5 e0ff 80d8 afe6 5284  J...}s........R.
+00003010: b522 a51a 2a12 3abc b8a1 010f fdac f706  ."..*.:.........
+00003020: 3adf 95b4 7288 ce74 c79a 7e11 1092 03dd  :...r..t..~.....
+00003030: 57ce e1de 48bb b6ff eb14 7f01 504b 0304  W...H.......PK..
+00003040: 1400 0000 0800 5263 7258 bc72 e0e6 ff01  ......RcrX.r....
+00003050: 0000 8104 0000 1900 0000 786c 2f77 6f72  ..........xl/wor
+00003060: 6b73 6865 6574 732f 7368 6565 7431 362e  ksheets/sheet16.
+00003070: 786d 6c7d 54db 6edb 300c fd15 43cf 4195  xml}T.n.0...C.A.
+00003080: 14eb 0581 63a0 49da a5c0 0214 2dda 3d16  ....c.I.....-.=.
+00003090: 8a4c c742 749b 44cf ebdf 8fb2 9334 dd92  .L.Bt.D......4..
+000030a0: 3c59 3ce2 2179 44d2 79eb c226 d600 98fd  <Y<.!yD.y..&....
+000030b0: 31da c609 ab11 fd98 f328 6b30 225e 380f  1........(k0"^8.
+000030c0: 966e 2a17 8c40 32c3 9a47 1f40 941d c968  .n*..@2..G.@...h
+000030d0: 7e39 1c5e 7323 9465 45de 614f a1c8 5d83  ~9.^s#.eE.aO..].
+000030e0: 5a59 780a 596c 8c11 e163 0ada b513 3662  ZYx.Yl...c....6b
+000030f0: 3be0 59ad 6bec 005e e45e ace1 05f0 d513  ;.Y.k..^.^......
+00003100: 814c be8f 532a 0336 2a67 b300 d584 dd8d  .L..S*.6*g......
+00003110: c68b 9ed1 79bc 2968 e3c1 394b 6256 ce6d  ....y.)h..9KbV.m
+00003120: 92f1 584e d830 d504 1a24 a610 823e bf61  ..XN.0...$...>.a
+00003130: 065a a748 54c9 af6d 50f6 9934 310f cfbb  .Z.HT..mP..41...
+00003140: f00f 9d7e 2a6f 2522 cc9c fea9 4aac 27ec  ...~*o%"....J.'.
+00003150: 9665 2554 a2d1 f8ec da05 6c35 5d7d 9638  .e%T......l5]}.8
+00003160: 1728 8a3c b836 0b49 6c91 cb74 4829 c951  .(.<.6.Il..tH).Q
+00003170: d9f4 482f 1808 5794 090b 8488 ef06 5094  ..H/..W.......P.
+00003180: c4cb 3952 29e9 82cb 2d71 7a96 e821 4467  ..9R)...-qz..!Dg
+00003190: 8ff1 6667 7992 34c5 23ac f959 566c 14c2  ..fgy.4.#..YVl..
+000031a0: 7bf4 2055 a5a4 484f 7c24 c6fd a918 aa3c  {. U..HO|$.....<
+000031b0: e2fd 70ca db0a 0347 fcbf 9ff2 2f21 caa0  ..p....G..../!..
+000031c0: fc89 a216 2785 89f5 3f0f c1a9 77bb 81e8  ....'...?...w...
+000031d0: 9b99 5af3 26b4 2a3b c931 93ae b1d8 37f7  ..Z.&.*;.1....7.
+000031e0: ebd5 6ec0 a697 e3e9 68f8 edf6 eae6 9a86  ..n.....h.......
+000031f0: ae76 ed3c 383f 77ad 4d03 da01 8fd6 37b8  .v.<8?w.M.....7.
+00003200: 8418 690f f6e0 7d08 2e1c 8242 d30e 4db5  ..i...}....B..M.
+00003210: b09b 6e6f f0c3 13ae 5544 ca9c f6b3 d162  ..no....UD.....b
+00003220: 54b0 3bad 0733 d245 2dd1 831f b40c af7e  T.;..3.E-......~
+00003230: b004 590b 4b9e 4ab2 9cef 7d73 feb5 e0ff  ..Y.K.J...}s....
+00003240: 80d8 afe6 5284 b522 a51a 2a12 3abc b8a1  ....R.."..*.:...
+00003250: 010f fdac f706 3adf 95b4 7288 ce74 c79a  ......:...r..t..
+00003260: 7e11 1092 03dd 57ce e1de 48bb b6ff eb14  ~.....W...H.....
+00003270: 7f01 504b 0304 1400 0000 0800 5263 7258  ..PK........RcrX
+00003280: 953b a42f 1101 0000 c801 0000 1900 0000  .;./............
+00003290: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
+000032a0: 6565 7431 372e 786d 6c4d 51cb 6ec3 2010  eet17.xmlMQ.n. .
+000032b0: fc15 8b0f 084e a53e 14d9 96d2 5455 7ba8  .....N.>....TU{.
+000032c0: 14a5 6a7b c6f1 da46 0196 c2ba 6eff be80  ..j{...F....n...
+000032d0: 6327 2776 7677 8619 2846 7427 df03 50f6  c''vvw..(Ft'..P.
+000032e0: ab95 f125 eb89 ec86 737f ec41 0bbf 420b  ...%....s..A..B.
+000032f0: 264c 5a74 5a50 80ae e3de 3a10 4d22 69c5  &LZtZP....:.M"i.
+00003300: 6ff2 fc8e 6b21 0dab 8ad4 dbbb aac0 8194  o...k!..........
+00003310: 34b0 7799 1fb4 16ee ef11 148e 255b b3b9  4.w.........%[..
+00003320: 7190 5d4f a9c1 abc2 8a0e de81 3e6c 2004  q.]O........>l .
+00003330: c817 9d46 6a30 5ea2 c91c b425 dbae 37db  ...Fj0^....%..7.
+00003340: 8991 363e 258c feaa ce62 981a f114 c16b  ..6>%....b.....k
+00003350: 53b2 3c7a 0205 478a 1222 1c3f b003 a5a2  S.<z..G..".?....
+00003360: 5270 f27d 1665 974b 23f3 ba9e e59f 53fe  Rp.}.e.K#.....S.
+00003370: 60af 161e 76a8 be64 437d c91e 58d6 402b  `...v..dC}..X.@+
+00003380: 0645 071c 5fe0 9ce9 f662 f149 9098 13be  .E.._....b.I....
+00003390: 09d7 49e3 3305 6dd8 ca57 f761 cf4d 9409  ..I.3.m..W.a.M..
+000033a0: 10da f422 3512 a14e 651f 5e1a 5c5c 08f3  ..."5..Ne.^.\\..
+000033b0: 1691 1610 2d2f 9f57 fd03 504b 0304 1400  ....-/.W..PK....
+000033c0: 0000 0800 5263 7258 bc72 e0e6 ff01 0000  ....RcrX.r......
+000033d0: 8104 0000 1900 0000 786c 2f77 6f72 6b73  ........xl/works
+000033e0: 6865 6574 732f 7368 6565 7431 382e 786d  heets/sheet18.xm
+000033f0: 6c7d 54db 6edb 300c fd15 43cf 4195 14eb  l}T.n.0...C.A...
+00003400: 0581 63a0 49da a5c0 0214 2dda 3d16 8a4c  ..c.I.....-.=..L
+00003410: c742 749b 44cf ebdf 8fb2 9334 dd92 3c59  .Bt.D......4..<Y
+00003420: 3ce2 2179 44d2 79eb c226 d600 98fd 31da  <.!yD.y..&....1.
+00003430: c609 ab11 fd98 f328 6b30 225e 380f 966e  .......(k0"^8..n
+00003440: 2a17 8c40 32c3 9a47 1f40 941d c968 7e39  *..@2..G.@...h~9
+00003450: 1c5e 7323 9465 45de 614f a1c8 5d83 5a59  .^s#.eE.aO..].ZY
+00003460: 780a 596c 8c11 e163 0ada b513 3662 3be0  x.Yl...c....6b;.
+00003470: 59ad 6bec 005e e45e ace1 05f0 d513 814c  Y.k..^.^.......L
+00003480: be8f 532a 0336 2a67 b300 d584 dd8d c68b  ..S*.6*g........
+00003490: 9ed1 79bc 2968 e3c1 394b 6256 ce6d 92f1  ..y.)h..9KbV.m..
+000034a0: 584e d830 d504 1a24 a610 823e bf61 065a  XN.0...$...>.a.Z
+000034b0: a748 54c9 af6d 50f6 9934 310f cfbb f00f  .HT..mP..41.....
+000034c0: 9d7e 2a6f 2522 cc9c fea9 4aac 27ec 9665  .~*o%"....J.'..e
+000034d0: 2554 a2d1 f8ec da05 6c35 5d7d 9638 1728  %T......l5]}.8.(
+000034e0: 8a3c b836 0b49 6c91 cb74 4829 c951 d9f4  .<.6.Il..tH).Q..
+000034f0: 482f 1808 5794 090b 8488 ef06 5094 c4cb  H/..W.......P...
+00003500: 3952 29e9 82cb 2d71 7a96 e821 4467 8ff1  9R)...-qz..!Dg..
+00003510: 6667 7992 34c5 23ac f959 566c 14c2 7bf4  fgy.4.#..YVl..{.
+00003520: 2055 a5a4 484f 7c24 c6fd a918 aa3c e2fd   U..HO|$.....<..
+00003530: 70ca db0a 0347 fcbf 9ff2 2f21 caa0 fc89  p....G..../!....
+00003540: a216 2785 89f5 3f0f c1a9 77bb 81e8 9b99  ..'...?...w.....
+00003550: 5af3 26b4 2a3b c931 93ae b1d8 37f7 ebd5  Z.&.*;.1....7...
+00003560: 6ec0 a697 e3e9 68f8 edf6 eae6 9a86 ae76  n.....h........v
+00003570: ed3c 383f 77ad 4d03 da01 8fd6 37b8 8418  .<8?w.M.....7...
+00003580: 690f f6e0 7d08 2e1c 8242 d30e 4db5 b09b  i...}....B..M...
+00003590: 6e6f f0c3 13ae 5544 ca9c f6b3 d162 54b0  no....UD.....bT.
+000035a0: 3bad 0733 d245 2dd1 831f b40c af7e b004  ;..3.E-......~..
+000035b0: 590b 4b9e 4ab2 9cef 7d73 feb5 e0ff 80d8  Y.K.J...}s......
+000035c0: afe6 5284 b522 a51a 2a12 3abc b8a1 010f  ..R.."..*.:.....
+000035d0: fdac f706 3adf 95b4 7288 ce74 c79a 7e11  ....:...r..t..~.
+000035e0: 1092 03dd 57ce e1de 48bb b6ff eb14 7f01  ....W...H.......
+000035f0: 504b 0304 1400 0000 0800 5263 7258 bc72  PK........RcrX.r
+00003600: e0e6 ff01 0000 8104 0000 1900 0000 786c  ..............xl
+00003610: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
+00003620: 7431 392e 786d 6c7d 54db 6edb 300c fd15  t19.xml}T.n.0...
+00003630: 43cf 4195 14eb 0581 63a0 49da a5c0 0214  C.A.....c.I.....
+00003640: 2dda 3d16 8a4c c742 749b 44cf ebdf 8fb2  -.=..L.Bt.D.....
+00003650: 9334 dd92 3c59 3ce2 2179 44d2 79eb c226  .4..<Y<.!yD.y..&
+00003660: d600 98fd 31da c609 ab11 fd98 f328 6b30  ....1........(k0
+00003670: 225e 380f 966e 2a17 8c40 32c3 9a47 1f40  "^8..n*..@2..G.@
+00003680: 941d c968 7e39 1c5e 7323 9465 45de 614f  ...h~9.^s#.eE.aO
+00003690: a1c8 5d83 5a59 780a 596c 8c11 e163 0ada  ..].ZYx.Yl...c..
+000036a0: b513 3662 3be0 59ad 6bec 005e e45e ace1  ..6b;.Y.k..^.^..
+000036b0: 05f0 d513 814c be8f 532a 0336 2a67 b300  .....L..S*.6*g..
+000036c0: d584 dd8d c68b 9ed1 79bc 2968 e3c1 394b  ........y.)h..9K
+000036d0: 6256 ce6d 92f1 584e d830 d504 1a24 a610  bV.m..XN.0...$..
+000036e0: 823e bf61 065a a748 54c9 af6d 50f6 9934  .>.a.Z.HT..mP..4
+000036f0: 310f cfbb f00f 9d7e 2a6f 2522 cc9c fea9  1......~*o%"....
+00003700: 4aac 27ec 9665 2554 a2d1 f8ec da05 6c35  J.'..e%T......l5
+00003710: 5d7d 9638 1728 8a3c b836 0b49 6c91 cb74  ]}.8.(.<.6.Il..t
+00003720: 4829 c951 d9f4 482f 1808 5794 090b 8488  H).Q..H/..W.....
+00003730: ef06 5094 c4cb 3952 29e9 82cb 2d71 7a96  ..P...9R)...-qz.
+00003740: e821 4467 8ff1 6667 7992 34c5 23ac f959  .!Dg..fgy.4.#..Y
+00003750: 566c 14c2 7bf4 2055 a5a4 484f 7c24 c6fd  Vl..{. U..HO|$..
+00003760: a918 aa3c e2fd 70ca db0a 0347 fcbf 9ff2  ...<..p....G....
+00003770: 2f21 caa0 fc89 a216 2785 89f5 3f0f c1a9  /!......'...?...
+00003780: 77bb 81e8 9b99 5af3 26b4 2a3b c931 93ae  w.....Z.&.*;.1..
+00003790: b1d8 37f7 ebd5 6ec0 a697 e3e9 68f8 edf6  ..7...n.....h...
+000037a0: eae6 9a86 ae76 ed3c 383f 77ad 4d03 da01  .....v.<8?w.M...
+000037b0: 8fd6 37b8 8418 690f f6e0 7d08 2e1c 8242  ..7...i...}....B
+000037c0: d30e 4db5 b09b 6e6f f0c3 13ae 5544 ca9c  ..M...no....UD..
+000037d0: f6b3 d162 54b0 3bad 0733 d245 2dd1 831f  ...bT.;..3.E-...
+000037e0: b40c af7e b004 590b 4b9e 4ab2 9cef 7d73  ...~..Y.K.J...}s
+000037f0: feb5 e0ff 80d8 afe6 5284 b522 a51a 2a12  ........R.."..*.
+00003800: 3abc b8a1 010f fdac f706 3adf 95b4 7288  :.........:...r.
+00003810: ce74 c79a 7e11 1092 03dd 57ce e1de 48bb  .t..~.....W...H.
+00003820: b6ff eb14 7f01 504b 0304 1400 0000 0800  ......PK........
+00003830: 5263 7258 4f5c d595 6901 0000 e702 0000  RcrXO\..i.......
+00003840: 1900 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
+00003850: 732f 7368 6565 7432 302e 786d 6c75 52d9  s/sheet20.xmluR.
+00003860: 4ec3 400c fc95 683f 806d 9138 5425 91e8  N.@...h?.m.8T%..
+00003870: 81e0 01a9 6a05 3c56 dbc4 4956 dd23 785d  ....j.<V..IV.#x]
+00003880: 027f 8f37 3d85 daa7 d8de 99b1 3d71 da79  ...7=.......=q.y
+00003890: dc84 0680 921f 6b5c c844 43d4 8ea4 0c45  ......k\.DC....E
+000038a0: 0356 851b df82 e397 caa3 55c4 29d6 32b4  .V........U.).2.
+000038b0: 08aa ec49 d6c8 dbc1 e05e 5aa5 9dc8 d3be  ...I.....^Z.....
+000038c0: 36c7 3cf5 5b32 dac1 1c93 b0b5 56e1 ef18  6.<.[2......V...
+000038d0: 8cef 3231 1487 c242 d70d f505 99a7 adaa  ..21...B........
+000038e0: 6109 f4de 3281 5379 d429 b505 17b4 7709  a...2.Sy.)....w.
+000038f0: 4295 89a7 e168 b663 f488 0f0d 5d38 8b93  B....h.c....]8..
+00003900: b8cc dafb 4d4c 5ecb 4c0c e24c 60a0 a028  ....ML^.L..L`..(
+00003910: a1f8 f30d 1330 262a f124 5f7b 5171 6a1a  .....0&*.$_{Qqj.
+00003920: 99e7 f141 feb9 df9f c75b ab00 136f 3e75  ...A.....[...o>u
+00003930: 494d 261e 4552 42a5 b686 16be 7b81 fd4e  IM&.ERB.....{..N
+00003940: 77a7 11a7 8a54 9ea2 ef12 8ccb e669 1183  w....T.......i..
+00003950: d892 81da 4593 9684 5cd7 dc89 7282 402b  ....E...\...r.@+
+00003960: dcba 55ab 5059 20c0 904a e281 e2b3 2cf6  ..U.PY ..J....,.
+00003970: f4f1 35ba 2e2f a027 d7d0 8e3b 5cc0 4faf  ..5../.'...;\.O.
+00003980: e14b 0805 ea36 7a79 8136 bbba 93aa ff2d  .K...6zy.6.....-
+00003990: 21d9 8f83 c93b 83e2 01bc 29ac b50b 8981  !....;....).....
+000039a0: 8a75 0637 0f6c 23ee 1cdd 25e4 dbfe 60d6  .u.7.l#...%...`.
+000039b0: 9ec8 db3e 6cf8 1001 2380 df2b efe9 98c4  ...>l...#..+....
+000039c0: 3f7a bced fc0f 504b 0304 1400 0000 0800  ?z....PK........
+000039d0: 5263 7258 7d51 27cc ea01 0000 4504 0000  RcrX}Q'.....E...
+000039e0: 1900 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
+000039f0: 732f 7368 6565 7432 312e 786d 6c85 544d  s/sheet21.xml.TM
+00003a00: 6fdb 300c fd2b 86ce 4395 14eb 0702 c7c0  o.0..+..C.......
+00003a10: 92b4 5d0f 058a 166b 8f81 62d3 b110 59d2  ..]....k..b...Y.
+00003a20: 447a 5eff fd28 3949 132c d92e 36f9 c447  Dz^..(9I.,..6..G
+00003a30: 3d9a a4f3 de85 0d36 0094 fd6e 8dc5 a968  =......6...n...h
+00003a40: 88fc 444a 2c1b 6815 5e38 0f96 4f6a 175a  ..DJ,.h.^8..Oj.Z
+00003a50: 45ec 86b5 441f 4055 89d4 1a79 391a 5dcb  E...D.@U...y9.].
+00003a60: 5669 2b8a 3c61 cfa1 c85d 4746 5b78 0e19  Vi+.<a...]GF[x..
+00003a70: 766d abc2 c70c 8ceb a762 2c76 c08b 5e37  vm.......b,v..^7
+00003a80: 9400 59e4 5ead e115 e887 6702 bb72 9fa7  ..Y.^.....g..r..
+00003a90: d22d 58d4 ce66 01ea a9f8 369e 3c0c 8c14  .-X..f....6.<...
+00003aa0: f1a6 a1c7 033b 8bc5 ac9c db44 e7b1 9a8a  .....;.....D....
+00003ab0: 51d4 0406 4a8a 2914 bf7e c11c 8c89 9958  Q...J.)..~.....X
+00003ac0: c9cf 6d52 f179 6964 1eda bbf4 f7a9 7e96  ..mR.yid......~.
+00003ad0: b752 0873 67de 7545 cd54 dc8a ac82 5a75  .R.sg.uE.T....Zu
+00003ae0: 865e 5cff 1db6 355d 7d4a 5c28 5245 1e5c  .^\...5]}J\(RE.\
+00003af0: 9f85 586c 9197 d188 5772 a0b6 f123 bd52  ..Xl....Wr...#.R
+00003b00: 605c f34d 5410 202d b1d3 044b 5de5 9258  `\.MT. -...K]..X
+00003b10: 4a3c 90e5 9638 fb27 b164 6d27 48f3 ff92  J<...8.'.dm'H...
+00003b20: 9601 906b 38c1 5d9c e39e 9477 772e daaa  ...k8.]....ww...
+00003b30: f694 b2fb 73f1 1560 19b4 8f6d 3b41 7b38  ....s..`...m;A{8
+00003b40: 5b90 5ae3 71bc e44f bfeb e7d0 8b8a 9f6f  [.Z.q..O.......o
+00003b50: ca68 7e73 76cc 4ad7 591a 7a73 7cb4 9b8f  .h~sv.J.Y.zs|...
+00003b60: f9e5 643e 1e7d bdbd bab9 e699 695c bf08  ..d>.}......i\..
+00003b70: ce2f 5c6f e37c 25e0 d1fa 8e9e 0091 c778  ./\o.|%........x
+00003b80: 0fde 85e0 c221 a80c afc0 cc28 bb49 634f  .....!.....(.IcO
+00003b90: 1f9e 71a3 91f8 e6b8 5e9d 51e3 42a4 9e78  ..q.....^.Q.B..x
+00003ba0: 8508 d597 64d7 4a9b 9d8d 1bed 3d54 2297  ....d.J.....=T".
+00003bb0: 7b42 2e8f 55ff 05e0 b05e 4f2a ac35 976b  {B..U....^O*.5.k
+00003bc0: a0e6 6a47 1737 3ca4 6198 d7c1 21e7 93ae  ..jG.7<.a...!...
+00003bd0: 9523 726d 321b 5e73 0831 80cf 6be7 68ef  .#rm2.^s.1..k.h.
+00003be0: c47d d9ff 398a 3f50 4b03 0414 0000 0008  .}..9.?PK.......
+00003bf0: 0052 6372 58d4 5695 de87 0100 008f 0300  .RcrX.V.........
+00003c00: 0019 0000 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
+00003c10: 7473 2f73 6865 6574 3232 2e78 6d6c 7d93  ts/sheet22.xml}.
+00003c20: db4e c330 0c86 5fa5 ca03 900d 8983 a6b6  .N.0.._.........
+00003c30: 128c c3b8 409a 8680 cb29 6bdd 3622 87e2  ....@....)k.6"..
+00003c40: 7814 de1e a73b 8050 cb55 6dc7 9fe3 3f76  x....;.P.Um...?v
+00003c50: d3ce e35b 6800 28f9 b4c6 854c 3444 ed4c  ...[h.(....L4D.L
+00003c60: ca50 3460 5538 f12d 383e a93c 5a45 ec62  .P4`U8.-8>.<ZE.b
+00003c70: 2d43 8ba0 ca1e b246 9e4e 26e7 d22a ed44  -C.....F.N&..*.D
+00003c80: 9ef6 b125 e6a9 df92 d10e 9698 84ad b50a  ...%............
+00003c90: bfae c1f8 2e13 5371 08ac 74dd 501f 9079  ......Sq..t.P..y
+00003ca0: daaa 1a9e 809e 5b06 d895 c73a a5b6 e082  ......[....:....
+00003cb0: f62e 41a8 3271 359d 2d76 449f f1a2 a10b  ..A.2q5.-vD.....
+00003cc0: bfec 248a d978 ff16 9d87 3213 93d8 1318  ..$..x....2.....
+00003cd0: 2828 9650 fcf9 8039 1813 2b71 27ef fba2  ((.P...9..+q'...
+00003ce0: e2e7 d248 feb6 0fe5 ef7a fddc de46 0598  ...H.....z...F..
+00003cf0: 7bf3 aa4b 6a32 7129 9212 2ab5 35b4 f2dd  {..Kj2q)..*.5...
+00003d00: 02f6 9ace 7e5a bc51 a4f2 147d 9760 149b  ....~Z.Q...}.`..
+00003d10: a745 34e2 959c a85d 7ca4 2742 8e6b be89  .E4....]|.'B.k..
+00003d20: 7282 406b dc3a 07b8 76ca 422a 89bb 8967  r.@k.:..v.B*...g
+00003d30: b2d8 b3d7 ffb2 e048 9386 3000 ceff 050b  .......H..0.....
+00003d40: d6b5 4608 2c65 08be 1985 7942 8194 6d07  ..F.,e....yB..m.
+00003d50: a0db 3148 9703 d977 63d9 230f 713f 965f  ..1H...wc.#.q?._
+00003d60: 4228 50b7 71e6 03d8 6254 89aa ff28 973c  B(P.q...bT...(.<
+00003d70: b7c3 32ec 0619 17f5 5161 ad5d 480c 545c  ..2.....Qa.]H.T\
+00003d80: 6772 72c1 e3c6 dde4 770e f9b6 5fec 8d27  grr.....w..._..'
+00003d90: f2b6 371b fe61 0063 029f 57de d3d1 899b  ..7..a.c..W.....
+00003da0: 77fc 07f3 6f50 4b03 0414 0000 0008 0052  w...oPK........R
+00003db0: 6372 58c4 ce01 8a6c 0100 000f 0300 0019  crX....l........
+00003dc0: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
+00003dd0: 2f73 6865 6574 3233 2e78 6d6c 7553 db6e  /sheet23.xmluS.n
+00003de0: 8330 0cfd 1594 0f58 e8a4 5d54 01d2 daae  .0.....X..]T....
+00003df0: da1e 2655 adb6 3d56 2918 889a 0b4b dcb1  ..&U..=V)....K..
+00003e00: fdfd 1ce8 4d13 3c61 3be7 1cfb 3821 69ad  ....M.<a;...8!i.
+00003e10: dbfb 1a00 a31f ad8c 4f59 8dd8 4c39 f779  ........OY..L9.y
+00003e20: 0d5a f81b db80 a193 d23a 2d90 5257 71df  .Z.......:-.RWq.
+00003e30: 3810 4547 d28a dfc6 f13d d742 1a96 255d  8.EG.....=.B..%]
+00003e40: 6de5 b2c4 1e50 4903 2b17 f983 d6c2 fdce  m....PI.+.......
+00003e50: 40d9 3665 1376 2aac 6555 6357 e059 d288  @.6e.v*.eUcW.Y..
+00003e60: 0a36 80ef 0d11 28e5 679d 426a 305e 5a13  .6....(.g.Bj0^Z.
+00003e70: 3928 53f6 3499 2e7b 4687 f890 d0fa ab38  9(S.4..{F......8
+00003e80: 0a66 76d6 ee43 f25a a42c 0e33 8182 1c83  .fv..C.Z.,.3....
+00003e90: 84a0 cf37 cc41 a9a0 4493 7c1d 45d9 a569  ...7.A..D.|.E..i
+00003ea0: 605e c727 f965 e79f c6db 090f 73ab 3e65  `^.'.e......s.>e
+00003eb0: 8175 ca1e 5954 4029 0e0a d7b6 7d81 a3a7  .u..YT@)....}...
+00003ec0: bbcb 880b 8122 4b9c 6d23 17cc 6649 1e82  ....."K.m#..fI..
+00003ed0: d092 80d2 8425 6dd0 515d 5227 cc10 3c6e  .....%m.Q]R'..<n
+00003ee0: 736a b195 45c2 9126 0975 9e1f 79b3 315e  sj..E..&.u..y.1^
+00003ef0: b3f7 03f0 f918 7c50 7c31 8636 42c3 00fe  ......|P|1.6B...
+00003f00: 790c 5f80 cf9d 6cc2 ce07 68cb 51ef a2fa  y._...l...h.Q...
+00003f10: 6782 d3de 4e97 d12f 323c 9437 e12a 697c  g...N../2<.7.*i|
+00003f20: a4a0 249d f8e6 81d6 edfa cdf7 09da a67b  ..$............{
+00003f30: 583b 8b68 7517 d6f4 60c1 0500 9d97 d6e2  X;.hu...`.......
+00003f40: 3909 377f fe07 b23f 504b 0304 1400 0000  9.7....?PK......
+00003f50: 0800 5263 7258 1b56 7ebc 9c01 0000 0d04  ..RcrX.V~.......
+00003f60: 0000 1900 0000 786c 2f77 6f72 6b73 6865  ......xl/workshe
+00003f70: 6574 732f 7368 6565 7432 342e 786d 6c7d  ets/sheet24.xml}
+00003f80: 94db 6adc 3010 865f c5e8 01a2 4da1 0782  ..j.0.._....M...
+00003f90: 6d68 364d 9386 4248 687a 59b4 f6d8 162b  mh6M..BHhzY....+
+00003fa0: 69d4 d16c 9cbe 7d25 ef21 2948 bdf2 ccf8  i..l..}%.!)H....
+00003fb0: ff46 33e6 97eb 1969 1b26 00ae 5eac 71a1  .F3....i.&..^.q.
+00003fc0: 1113 b3bf 9032 7413 5815 ced0 838b 6f06  .....2t.X.....o.
+00003fd0: 24ab 38a6 34ca e009 54bf 40d6 c877 abd5  $.8.4...T.@..w..
+00003fe0: 0769 9576 a2ad 97da 3db5 35ee d868 07f7  .i.v....=.5..h..
+00003ff0: 5485 9db5 8afe 5c82 c1b9 11e7 e258 78d0  T.....\......Xx.
+00004000: e3c4 4b41 b6b5 5723 3c02 fff0 1188 a93c  ..KA..W#<......<
+00004010: f5e9 b505 1734 ba8a 6068 c4e7 f38b bb3d  .....4..`h.....=
+00004020: b128 9e34 cce1 4d5c a565 3688 db94 dcf6  .(.4..M\.e6.....
+00004030: 8d58 a599 c040 c7a9 858a 8f67 5883 31a9  .X...@.....gX.1.
+00004040: 539c e4f7 a1a9 783d 3491 6fe3 63fb eb65  S.....x=4.o.c..e
+00004050: ff38 de46 0558 a3f9 a97b 9e1a f149 543d  .8.F.X...{...IT=
+00004060: 0c6a 67f8 01e7 1b38 ecf4 fe75 c42b c5aa  .jg....8...u.+..
+00004070: ad09 e78a d2b2 6ddd a520 1d19 85da a58f  ......m.. ......
+00004080: f4c8 14eb 3a9e c4ad 5704 8e7f f96d 2d39  ....:...W....m-9
+00004090: 8e91 8ab2 3b40 9725 c802 8dd0 e7a1 7509  ....;@.%......u.
+000040a0: 52a4 4624 9741 aefe 83bc 64f4 5f4a fa9d  R.F$.A....d._J..
+000040b0: 0bd0 1170 86b9 2e31 1b86 8cfc 6b49 aead  ...p...1....kI..
+000040c0: 277c d66e cc40 3745 a8cf a86f 4b6a a76c  '|.n.@7E...oKj.l
+000040d0: 6ea4 6f25 7d0f a123 ed93 e332 d85d 0963  n.o%}..#...2.].c
+000040e0: 3586 7ff5 32ba e668 c5bd 8dd2 35f9 ae68  5...2..h....5..h
+000040f0: d42e 5406 86d8 6775 f631 9a8d f6be db27  ..T...gu.1.....'
+00004100: 8c7e b956 1b64 46bb 8453 bcae 4049 10df  .~.V.dF..S..@I..
+00004110: 0f88 7c4a 92ef 4f7f 80f6 2f50 4b03 0414  ..|J..O.../PK...
+00004120: 0000 0008 0052 6372 58d2 05f1 4652 0200  .....RcrX...FR..
+00004130: 0047 0a00 000d 0000 0078 6c2f 7374 796c  .G.......xl/styl
+00004140: 6573 2e78 6d6c dd56 db8a db30 10fd 15e3  es.xml.V...0....
+00004150: 0fa8 9398 9ab8 2479 a821 5068 cbc2 ee43  ......$y.!Ph...C
+00004160: 5fe5 584e 04ba b8b2 bc24 fdfa 6a24 e7b6  _.XN.....$..j$..
+00004170: 9be3 52fa 569b e099 393a 3367 a431 ceaa  ..R.V...9:3g.1..
+00004180: 7727 c99f 0f9c bbe4 a8a4 eed7 e9c1 b9ee  w'..............
+00004190: 5396 f5bb 0357 acff 603a ae3d d21a ab98  S....W..`:.=....
+000041a0: f3ae dd67 7d67 396b 7a22 2999 2d66 b322  ...g}g9kz").-f."
+000041b0: 534c e874 b3d2 83da 2ad7 273b 3368 b74e  SL.t....*.';3h.N
+000041c0: 6769 926d 56ad d1d7 d03c 8d01 bf96 299e  gi.mV....<....).
+000041d0: bc32 b94e 2b26 456d 455c cc94 90a7 185f  .2.N+&EmE\....._
+000041e0: 84c8 ce48 6313 e7d5 70a2 53a8 ff15 17cc  ...Hc...p.S.....
+000041f0: 4797 a48e b994 d0c6 8668 16cb 8447 ef13  G........h...G..
+00004200: 0b29 2f2a 1669 0c6c 561d 738e 5bbd f54e  .)/*.i.lV.s.[..N
+00004210: 2485 e87b 6cb4 5f4e 9d57 b1b7 ec34 5f7c  $..{l._N.W...4_|
+00004220: 4c6f 18e1 e1cb d4c6 36dc deb5 1b43 9b95  Lo......6....C..
+00004230: e4ad 2386 15fb 4330 9ce9 e851 1be7 8c22  ..#...C0...Q..."
+00004240: ab11 6c6f 348b 4ace b4d1 f0b9 775c ca67  ..lo4.J.....w\.g
+00004250: 3aaf 1fed 5d81 639b c48d ffd2 843d a78e  :...].c......=..
+00004260: cfa6 5735 9a31 cde8 5081 db74 31f9 bfe7  ..W5.1..P..t1...
+00004270: edc4 ab71 9f07 df90 0efe cfc1 38fe 6479  ...q........8.dy
+00004280: 2b8e c13f b66f 045c 6a07 2577 e52f d184  +..?.o.\j.%w./..
+00004290: 4665 9d7e a711 9437 39ea 4148 27f4 e81d  Fe.~...79.AH'...
+000042a0: 44d3 70fd be3b 9fdf b1da 0ff9 5d01 bfaa  D.p..;......]...
+000042b0: e12d 1ba4 7bb9 80eb f46a 7fe3 8d18 5479  .-..{....j....Ty
+000042c0: 59f5 448d 8dab aef6 573a ca79 719d 535f  Y.D.....W:.yq.S_
+000042d0: 4ce8 861f 7953 8dae ddd7 c14c bce1 cb8e  L...yS.....L....
+000042e0: 5760 bc85 b6e1 0210 6445 1040 04c2 5a50  W`......dE.@..ZP
+000042f0: 0664 451e acf5 3ff6 b5c4 7d45 102a 5c3e  .dE...?...}E.*\>
+00004300: 8696 98b5 c4ac c87b 0855 e186 b500 abf4  .......{.U......
+00004310: 1768 b92c f3bc 28e0 f656 d563 1915 dcc3  .h.,..(..V.c....
+00004320: a2a0 1f48 0815 1207 d6a2 6a7f bbf3 1303  ...H......j.....
+00004330: 3031 367f 980d 78ca 9363 035b 9e18 51d8  016...x..c.[..Q.
+00004340: f2c4 ce13 04f6 9038 6509 0600 d622 0e3c  .......8e....".<
+00004350: 1438 5124 02d4 a251 03ac 3ca7 7386 0ae1  .8Q$...Q..<.s...
+00004360: 6b3e 0195 2584 6848 c1f4 1605 daa8 826e  k>..%.hH.......n
+00004370: 705e f025 caf3 b204 1081 4046 9e43 885e  p^.%......@F.C.^
+00004380: d809 08ca 2021 10ca f3f8 217d f33d cbce  .... !....!}.=..
+00004390: dfb9 ecfa d771 f31b 504b 0304 1400 0000  .....q..PK......
+000043a0: 0800 5263 7258 b747 eb8a c000 0000 1602  ..RcrX.G........
+000043b0: 0000 0b00 0000 5f72 656c 732f 2e72 656c  ......_rels/.rel
+000043c0: 739d 924b 6e02 310c 40af 1265 5f4c a9c4  s..Kn.1.@..e_L..
+000043d0: 0231 acd8 b043 880b b889 e7a3 99c4 9163  .1...C.........c
+000043e0: c4f4 f68d d8c0 2068 114b ff9e 9e2d af0f  ...... h.K...-..
+000043f0: 34a0 761c 73db a56c c630 c45c d956 35ad  4.v.s..l.0.\.V5.
+00004400: 00b2 6b29 609e 71a2 582a 354b 402d a134  ..k)`.q.X*5K@-.4
+00004410: 90d0 f5d8 102c e6f3 25c8 2dc3 6ed6 b74c  .....,..%.-.n..L
+00004420: 73fc 49f4 0a91 ebba 73b4 6577 0a14 f501  s.I.....s.ew....
+00004430: f8ae c39a 234a 435a d971 8033 4bff cddc  ....#JCZ.q.3K...
+00004440: cf0a d49a 9daf acec fca7 35f0 a6cc f3f5  ..........5.....
+00004450: 2090 a247 4570 2cf4 91a4 4c8b 7694 af3e   ..GEp,...L.v..>
+00004460: 9edd bea4 f3a5 6362 b478 dfe8 fff3 d0a8  ......cb.x......
+00004470: 143d f9bf 9d30 a589 d2d7 4509 266f b0f9  .=...0....E.&o..
+00004480: 0550 4b03 0414 0000 0008 0052 6372 5821  .PK........RcrX!
+00004490: 0fd9 4c7b 0200 00e5 0800 000f 0000 0078  ..L{...........x
+000044a0: 6c2f 776f 726b 626f 6f6b 2e78 6d6c 8d96  l/workbook.xml..
+000044b0: 6d4f db30 1080 ff4a 951f b034 8196 1751  mO.0...J...4...Q
+000044c0: 24d6 3240 6cb4 2388 ef57 e7d2 9c70 ecc8  $.2@l.#..W...p..
+000044d0: 76e8 c6af 9f9d 5048 ebcc dba7 d467 ebe9  v.....PH.....g..
+000044e0: 5dfc 9c9d 8bad 542f 6b29 5f46 bf2a 2ef4  ].....T/k)_F.*..
+000044f0: b99a 45a5 31f5 791c 6b56 6205 fa8b ac51  ..E.1.y.kVb....Q
+00004500: d8b9 42aa 0a8c 1daa 4d2c 8b82 182e 246b  ..B.....M,....$k
+00004510: 2a14 264e c7e3 69ac 9083 2129 7449 b58e  *.&N..i...!)tI..
+00004520: 3ada ffb0 74ad 1072 5d22 9a8a 77a8 0a48  :...t..r]"..w..H
+00004530: 4497 17bb cc56 6a14 f747 d220 73ff e4a2  D....Vj..G. s...
+00004540: 2ef2 4cb8 d59f 0bdc 70f4 4a9a d6c4 c9fc  ..L.....p.J.....
+00004550: 9e45 ed6f 8ed1 a822 4115 bd61 3e8b c6d1  .E.o..."A..a>...
+00004560: 4897 727b 2b15 bd49 6180 674c 49ce 6751  H.r{+..Ia.gLI.gQ
+00004570: d24d 3ca3 32c4 bc70 e6d2 7c82 b56e 2306  .M<.2..p..|..n#.
+00004580: d68f aee6 5934 1d5b 6041 4a9b 7645 cb07  ....Y4.[`AJ.vE..
+00004590: 9be4 2bda c5dd a831 f21b 7183 6a01 066f  ..+....1..q.j..o
+000045a0: 946c 6a12 9b16 63cb 887b 75b4 af62 f71c  .lj...c..{u..b..
+000045b0: 09a8 7016 3da1 36d7 c2d8 7256 a06c c462  ..p.=.6...rV.l.b
+000045c0: 5c42 76c1 5dde 2567 2cb5 57aa 3a27 3ba1  \Bv.].%g,.W.:';.
+000045d0: eef2 8edf 67fd 6c80 5341 7b84 3440 483d  ....g.l.SA{.4@H=
+000045e0: 82cb e607 1ac8 c140 0f72 1480 1c0d 42ae  .......@.r....B.
+000045f0: b446 d323 1c07 08c7 1ee1 8a31 ac0d 0886  .F.#.......1....
+00004600: 43ac 4980 3519 cce6 3adf e062 bfa4 6900  C.I.5...:..b..i.
+00004610: 32f5 202b 854c 8a9c 9c9c 3dc8 4900 7232  2. +.L....=.I.r2
+00004620: 98c9 1c34 f600 a701 c0e9 3f5e cb01 ea2c  ...4......?^...,
+00004630: 803a 1b52 c549 07ad c83e 2c19 87c4 1b7b  .:.R.I...>,....{
+00004640: b8b9 ac6a 4e7f c92c 095a ec6b 7c2f e496  ...jN..,.Z.k|/..
+00004650: a3dd b21b 0575 f900 afb4 69cf 9f21 7448  .....u....i..!tH
+00004660: efc4 f77b 29f0 56d6 43a0 90e2 c9b0 e359  ...{).V.C......Y
+00004670: 4306 b31a 99ed 3906 076a 2421 e313 5ff9  C.....9..j$!.._.
+00004680: 0f60 9f11 323d f155 dff7 c3a3 8594 4f7c  .`..2=.U......O|
+00004690: e7bf a260 6505 ea65 1016 523f f1dd cf6c  ...`e..e..R?...l
+000046a0: 5a39 a85c ef9b e261 430d 91f8 1df1 b99f  Z9.\...aC.......
+000046b0: 1e29 d40f 89df 108e f1d8 0881 6a2e 4541  .)..........j.EA
+000046c0: 9b46 1dee 681a ea89 d4ef 899d 658f a81b  .F..h.......e...
+000046d0: de3f bfd2 503f a47e 3fbc a796 a1d6 0719  .?..P?.~?.......
+000046e0: 050f f7e1 d37d d998 bad9 cb26 647e 3a6c  .....}.....&d~:l
+000046f0: 7e57 d2ea 3edb 3b97 d390 f269 a77c bcbb  ~W..>.;....i.|..
+00004700: 0373 2c48 60fe 6099 da4d d81b 99d9 cf01  .s,H`.`..M......
+00004710: f7e8 1afb 78e2 76a9 6838 9fdb d852 7c97  ....x.v.h8...R|.
+00004720: 907f 5caa bb2f 82cb 3f50 4b03 0414 0000  ..\../..?PK.....
+00004730: 0008 0052 6372 5872 967e 9137 0100 0039  ...RcrXr.~.7...9
+00004740: 0f00 001a 0000 0078 6c2f 5f72 656c 732f  .......xl/_rels/
+00004750: 776f 726b 626f 6f6b 2e78 6d6c 2e72 656c  workbook.xml.rel
+00004760: 73cd d741 8e82 3014 c6f1 ab90 1ec0 f2aa  s..A..0.........
+00004770: a24e c495 1bb7 132f d0e0 1388 4049 dbc9  .N...../....@I..
+00004780: e8ed 87c8 023f 328b d998 792b d212 1eff  .....?2...y+....
+00004790: 45f3 0bec 3fb9 b1b1 765d a8ea 3e24 f7b6  E...?...v]..>$..
+000047a0: e942 aeaa 18fb 0fad 4351 716b c3c2 f5dc  .B......CQqk....
+000047b0: 0d77 aece b736 0e4b 5fea de16 375b b236  .w...6.K_...7[.6
+000047c0: 699a 69ff 3a43 1df6 af33 93f3 a3e7 bf4c  i.i.:C...3.....L
+000047d0: 74d7 6b5d f0d1 155f 2d77 f197 c1fa dbf9  t.k]..._-w......
+000047e0: 5ba8 98a3 4ace d697 1c73 a5ef cdb4 1df4  [...J....s......
+000047f0: f342 8b61 b24a 4e97 5cf9 d385 54a2 ffbb  .B.a.JN.\...T...
+00004800: c840 9111 50b4 84a2 a580 a215 14ad 0414  .@..P...........
+00004810: ada1 682d a028 83a2 4c40 d106 8a36 028a  ..h-.(..L@...6..
+00004820: b650 b415 50b4 83a2 9d80 224a 91c8 5442  .P..P....."J..TB
+00004830: d38c 6d09 6e13 c24d 12e4 26a4 9b24 d84d  ..m.n..M..&..$.M
+00004840: 8837 49d0 9b90 6f92 e037 21e0 2441 7042  .7I...o..7!.$ApB
+00004850: c249 82e1 8488 9304 c509 1927 098e 1b74  .I.........'...t
+00004860: dc48 70dc a0e3 4682 e366 f601 2ec1 7183  .Hp...F..f....q.
+00004870: 8e1b 098e 1b74 dcbc d5f1 101f 0d87 2968  .....t........)h
+00004880: 5c63 c05b d18e c3b3 3cbd ffb9 1c37 6747  \c.[....<....7gG
+00004890: 7864 5ac3 9ff2 e107 504b 0304 1400 0000  xdZ.....PK......
+000048a0: 0800 5263 7258 8b1a e4a4 7101 0000 3510  ..RcrX....q...5.
+000048b0: 0000 1300 0000 5b43 6f6e 7465 6e74 5f54  ......[Content_T
+000048c0: 7970 6573 5d2e 786d 6ccd 98cb 6ec2 3010  ypes].xml...n.0.
+000048d0: 457f 25ca 1611 63b7 a50f 019b b6db 9645  E.%...c........E
+000048e0: 7fc0 4d26 c4c2 2f79 0c85 bfaf 130a 522b  ..M&../y......R+
+000048f0: ca43 54ea 6c62 259e b9f7 c623 1d29 19bd  .CT.lb%....#.)..
+00004900: ad3d 60b6 32da e238 6f62 f40f 8c61 d980  .=`.2..8ob...a..
+00004910: 9158 380f 36ed d42e 1819 d36d 9831 2fcb  .X8.6......m.1/.
+00004920: b99c 0113 83c1 9095 ce46 b0b1 1f5b 8d7c  .........F...[.|
+00004930: 327a 825a 2e74 cc9e 57e9 312a 67c7 7900  2z.Z.t..W.1*g.y.
+00004940: 8d79 f6b8 296c bdc6 b9f4 5eab 52c6 b4cf  .y..)l....^.R...
+00004950: 96b6 fae1 d2ff 7228 5267 5783 8df2 d84b  ......r(RgW....K
+00004960: 0579 c6f6 5a74 5bbf 3a6c 1b5f 9710 82aa  .y..Zt[.:l._....
+00004970: 209b ca10 5fa4 4965 6ca5 19c6 b506 2c0e   ..._.Iel.....,.
+00004980: 6bec 49e9 ea5a 9550 b972 6152 4b81 3e80  k.I..Z.P.raRK.>.
+00004990: acb0 0188 4617 1bd1 de11 eb98 0e19 3657  ....F.........6W
+000049a0: 7e71 804e e6a0 632a 9d06 e731 4d2d c0f9  ~q.N..c*...1M-..
+000049b0: 7edb b1b4 dd7d 9f84 2044 75e4 2577 9649  ~....}.. Du.%w.I
+000049c0: fbe2 3784 76e2 1554 a79a a713 fe70 61de  ..7.v..T.....pa.
+000049d0: cd04 59b7 5c7e ccdf e7bc d33f 3788 a012  ..Y.\~.....?7...
+000049e0: e48a 4a90 6b2a 416e a804 1952 0972 4b25  ..J.k*An...R.rK%
+000049f0: c81d 9520 f754 82f0 0199 2464 d8ca c9c0  ... .T....$d....
+00004a00: 9593 a12b 2783 574e 86af 9c0c 6039 19c2  ...+'.WN....`9..
+00004a10: 7232 88e5 6418 2bc8 3056 9061 ac20 c358  r2..d.+.0V.a. .X
+00004a20: 4186 b1e2 5f19 fbee dcfc afbf 62db b530  A..._.......b..0
+00004a30: 52d9 5d00 d6fd 2d98 7c02 504b 0102 1403  R.]...-.|.PK....
+00004a40: 1400 0000 0800 5263 7258 465a c10c 8200  ......RcrXFZ....
+00004a50: 0000 b100 0000 1000 0000 0000 0000 0000  ................
+00004a60: 0000 8001 0000 0000 646f 6350 726f 7073  ........docProps
+00004a70: 2f61 7070 2e78 6d6c 504b 0102 1403 1400  /app.xmlPK......
+00004a80: 0000 0800 5263 7258 6a72 2c18 ed00 0000  ....RcrXjr,.....
+00004a90: cb01 0000 1100 0000 0000 0000 0000 0000  ................
+00004aa0: 8001 b000 0000 646f 6350 726f 7073 2f63  ......docProps/c
+00004ab0: 6f72 652e 786d 6c50 4b01 0214 0314 0000  ore.xmlPK.......
+00004ac0: 0008 0052 6372 5899 5c9c 2310 0600 009c  ...RcrX.\.#.....
+00004ad0: 2700 0013 0000 0000 0000 0000 0000 0080  '...............
+00004ae0: 01cc 0100 0078 6c2f 7468 656d 652f 7468  .....xl/theme/th
+00004af0: 656d 6531 2e78 6d6c 504b 0102 1403 1400  eme1.xmlPK......
+00004b00: 0000 0800 5263 7258 0f95 4d33 4801 0000  ....RcrX..M3H...
+00004b10: 4902 0000 1800 0000 0000 0000 0000 0000  I...............
+00004b20: 8081 0d08 0000 786c 2f77 6f72 6b73 6865  ......xl/workshe
+00004b30: 6574 732f 7368 6565 7431 2e78 6d6c 504b  ets/sheet1.xmlPK
+00004b40: 0102 1403 1400 0000 0800 5263 7258 0f95  ..........RcrX..
+00004b50: 4d33 4801 0000 4902 0000 1800 0000 0000  M3H...I.........
+00004b60: 0000 0000 0000 8081 8b09 0000 786c 2f77  ............xl/w
+00004b70: 6f72 6b73 6865 6574 732f 7368 6565 7432  orksheets/sheet2
+00004b80: 2e78 6d6c 504b 0102 1403 1400 0000 0800  .xmlPK..........
+00004b90: 5263 7258 b111 5547 4002 0000 7805 0000  RcrX..UG@...x...
+00004ba0: 1800 0000 0000 0000 0000 0000 8081 090b  ................
+00004bb0: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
+00004bc0: 7368 6565 7433 2e78 6d6c 504b 0102 1403  sheet3.xmlPK....
+00004bd0: 1400 0000 0800 5263 7258 2581 7ddb bf02  ......RcrX%.}...
+00004be0: 0000 7308 0000 1800 0000 0000 0000 0000  ..s.............
+00004bf0: 0000 8081 7f0d 0000 786c 2f77 6f72 6b73  ........xl/works
+00004c00: 6865 6574 732f 7368 6565 7434 2e78 6d6c  heets/sheet4.xml
+00004c10: 504b 0102 1403 1400 0000 0800 5263 7258  PK..........RcrX
+00004c20: b356 a83b 9203 0000 8c0d 0000 1800 0000  .V.;............
+00004c30: 0000 0000 0000 0000 8081 7410 0000 786c  ..........t...xl
+00004c40: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
+00004c50: 7435 2e78 6d6c 504b 0102 1403 1400 0000  t5.xmlPK........
+00004c60: 0800 5263 7258 2581 7ddb bf02 0000 7308  ..RcrX%.}.....s.
+00004c70: 0000 1800 0000 0000 0000 0000 0000 8081  ................
+00004c80: 3c14 0000 786c 2f77 6f72 6b73 6865 6574  <...xl/worksheet
+00004c90: 732f 7368 6565 7436 2e78 6d6c 504b 0102  s/sheet6.xmlPK..
+00004ca0: 1403 1400 0000 0800 5263 7258 642f 605f  ........RcrXd/`_
+00004cb0: 5801 0000 a802 0000 1800 0000 0000 0000  X...............
+00004cc0: 0000 0000 8081 3117 0000 786c 2f77 6f72  ......1...xl/wor
+00004cd0: 6b73 6865 6574 732f 7368 6565 7437 2e78  ksheets/sheet7.x
+00004ce0: 6d6c 504b 0102 1403 1400 0000 0800 5263  mlPK..........Rc
+00004cf0: 7258 5585 c684 f802 0000 3f0a 0000 1800  rXU.......?.....
+00004d00: 0000 0000 0000 0000 0000 8081 bf18 0000  ................
+00004d10: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
+00004d20: 6565 7438 2e78 6d6c 504b 0102 1403 1400  eet8.xmlPK......
+00004d30: 0000 0800 5263 7258 5585 c684 f802 0000  ....RcrXU.......
+00004d40: 3f0a 0000 1800 0000 0000 0000 0000 0000  ?...............
+00004d50: 8081 ed1b 0000 786c 2f77 6f72 6b73 6865  ......xl/workshe
+00004d60: 6574 732f 7368 6565 7439 2e78 6d6c 504b  ets/sheet9.xmlPK
+00004d70: 0102 1403 1400 0000 0800 5263 7258 5585  ..........RcrXU.
+00004d80: c684 f802 0000 3f0a 0000 1900 0000 0000  ......?.........
+00004d90: 0000 0000 0000 8081 1b1f 0000 786c 2f77  ............xl/w
+00004da0: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
+00004db0: 302e 786d 6c50 4b01 0214 0314 0000 0008  0.xmlPK.........
+00004dc0: 0052 6372 5830 1316 5e0d 0300 00b3 0a00  .RcrX0..^.......
+00004dd0: 0019 0000 0000 0000 0000 0000 0080 814a  ...............J
+00004de0: 2200 0078 6c2f 776f 726b 7368 6565 7473  "..xl/worksheets
+00004df0: 2f73 6865 6574 3131 2e78 6d6c 504b 0102  /sheet11.xmlPK..
+00004e00: 1403 1400 0000 0800 5263 7258 5585 c684  ........RcrXU...
+00004e10: f802 0000 3f0a 0000 1900 0000 0000 0000  ....?...........
+00004e20: 0000 0000 8081 8e25 0000 786c 2f77 6f72  .......%..xl/wor
+00004e30: 6b73 6865 6574 732f 7368 6565 7431 322e  ksheets/sheet12.
+00004e40: 786d 6c50 4b01 0214 0314 0000 0008 0052  xmlPK..........R
+00004e50: 6372 5855 85c6 84f8 0200 003f 0a00 0019  crXU.......?....
+00004e60: 0000 0000 0000 0000 0000 0080 81bd 2800  ..............(.
+00004e70: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
+00004e80: 6865 6574 3133 2e78 6d6c 504b 0102 1403  heet13.xmlPK....
+00004e90: 1400 0000 0800 5263 7258 2359 55fc e301  ......RcrX#YU...
+00004ea0: 0000 0704 0000 1900 0000 0000 0000 0000  ................
+00004eb0: 0000 8081 ec2b 0000 786c 2f77 6f72 6b73  .....+..xl/works
+00004ec0: 6865 6574 732f 7368 6565 7431 342e 786d  heets/sheet14.xm
+00004ed0: 6c50 4b01 0214 0314 0000 0008 0052 6372  lPK..........Rcr
+00004ee0: 58bc 72e0 e6ff 0100 0081 0400 0019 0000  X.r.............
+00004ef0: 0000 0000 0000 0000 0080 8106 2e00 0078  ...............x
+00004f00: 6c2f 776f 726b 7368 6565 7473 2f73 6865  l/worksheets/she
+00004f10: 6574 3135 2e78 6d6c 504b 0102 1403 1400  et15.xmlPK......
+00004f20: 0000 0800 5263 7258 bc72 e0e6 ff01 0000  ....RcrX.r......
+00004f30: 8104 0000 1900 0000 0000 0000 0000 0000  ................
+00004f40: 8081 3c30 0000 786c 2f77 6f72 6b73 6865  ..<0..xl/workshe
+00004f50: 6574 732f 7368 6565 7431 362e 786d 6c50  ets/sheet16.xmlP
+00004f60: 4b01 0214 0314 0000 0008 0052 6372 5895  K..........RcrX.
+00004f70: 3ba4 2f11 0100 00c8 0100 0019 0000 0000  ;./.............
+00004f80: 0000 0000 0000 0080 8172 3200 0078 6c2f  .........r2..xl/
+00004f90: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
+00004fa0: 3137 2e78 6d6c 504b 0102 1403 1400 0000  17.xmlPK........
+00004fb0: 0800 5263 7258 bc72 e0e6 ff01 0000 8104  ..RcrX.r........
+00004fc0: 0000 1900 0000 0000 0000 0000 0000 8081  ................
+00004fd0: ba33 0000 786c 2f77 6f72 6b73 6865 6574  .3..xl/worksheet
+00004fe0: 732f 7368 6565 7431 382e 786d 6c50 4b01  s/sheet18.xmlPK.
+00004ff0: 0214 0314 0000 0008 0052 6372 58bc 72e0  .........RcrX.r.
+00005000: e6ff 0100 0081 0400 0019 0000 0000 0000  ................
+00005010: 0000 0000 0080 81f0 3500 0078 6c2f 776f  ........5..xl/wo
+00005020: 726b 7368 6565 7473 2f73 6865 6574 3139  rksheets/sheet19
+00005030: 2e78 6d6c 504b 0102 1403 1400 0000 0800  .xmlPK..........
+00005040: 5263 7258 4f5c d595 6901 0000 e702 0000  RcrXO\..i.......
+00005050: 1900 0000 0000 0000 0000 0000 8081 2638  ..............&8
+00005060: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
+00005070: 7368 6565 7432 302e 786d 6c50 4b01 0214  sheet20.xmlPK...
+00005080: 0314 0000 0008 0052 6372 587d 5127 ccea  .......RcrX}Q'..
+00005090: 0100 0045 0400 0019 0000 0000 0000 0000  ...E............
+000050a0: 0000 0080 81c6 3900 0078 6c2f 776f 726b  ......9..xl/work
+000050b0: 7368 6565 7473 2f73 6865 6574 3231 2e78  sheets/sheet21.x
+000050c0: 6d6c 504b 0102 1403 1400 0000 0800 5263  mlPK..........Rc
+000050d0: 7258 d456 95de 8701 0000 8f03 0000 1900  rX.V............
+000050e0: 0000 0000 0000 0000 0000 8081 e73b 0000  .............;..
+000050f0: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
+00005100: 6565 7432 322e 786d 6c50 4b01 0214 0314  eet22.xmlPK.....
+00005110: 0000 0008 0052 6372 58c4 ce01 8a6c 0100  .....RcrX....l..
+00005120: 000f 0300 0019 0000 0000 0000 0000 0000  ................
+00005130: 0080 81a5 3d00 0078 6c2f 776f 726b 7368  ....=..xl/worksh
+00005140: 6565 7473 2f73 6865 6574 3233 2e78 6d6c  eets/sheet23.xml
+00005150: 504b 0102 1403 1400 0000 0800 5263 7258  PK..........RcrX
+00005160: 1b56 7ebc 9c01 0000 0d04 0000 1900 0000  .V~.............
+00005170: 0000 0000 0000 0000 8081 483f 0000 786c  ..........H?..xl
+00005180: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
+00005190: 7432 342e 786d 6c50 4b01 0214 0314 0000  t24.xmlPK.......
+000051a0: 0008 0052 6372 58d2 05f1 4652 0200 0047  ...RcrX...FR...G
+000051b0: 0a00 000d 0000 0000 0000 0000 0000 0080  ................
+000051c0: 011b 4100 0078 6c2f 7374 796c 6573 2e78  ..A..xl/styles.x
+000051d0: 6d6c 504b 0102 1403 1400 0000 0800 5263  mlPK..........Rc
+000051e0: 7258 b747 eb8a c000 0000 1602 0000 0b00  rX.G............
+000051f0: 0000 0000 0000 0000 0000 8001 9843 0000  .............C..
+00005200: 5f72 656c 732f 2e72 656c 7350 4b01 0214  _rels/.relsPK...
+00005210: 0314 0000 0008 0052 6372 5821 0fd9 4c7b  .......RcrX!..L{
+00005220: 0200 00e5 0800 000f 0000 0000 0000 0000  ................
+00005230: 0000 0080 0181 4400 0078 6c2f 776f 726b  ......D..xl/work
+00005240: 626f 6f6b 2e78 6d6c 504b 0102 1403 1400  book.xmlPK......
+00005250: 0000 0800 5263 7258 7296 7e91 3701 0000  ....RcrXr.~.7...
+00005260: 390f 0000 1a00 0000 0000 0000 0000 0000  9...............
+00005270: 8001 2947 0000 786c 2f5f 7265 6c73 2f77  ..)G..xl/_rels/w
+00005280: 6f72 6b62 6f6f 6b2e 786d 6c2e 7265 6c73  orkbook.xml.rels
+00005290: 504b 0102 1403 1400 0000 0800 5263 7258  PK..........RcrX
+000052a0: 8b1a e4a4 7101 0000 3510 0000 1300 0000  ....q...5.......
+000052b0: 0000 0000 0000 0000 8001 9848 0000 5b43  ...........H..[C
+000052c0: 6f6e 7465 6e74 5f54 7970 6573 5d2e 786d  ontent_Types].xm
+000052d0: 6c50 4b05 0600 0000 0020 0020 0097 0800  lPK...... . ....
+000052e0: 003a 4a00 0000 00                        .:J....
```

### Comparing `translator_testing_model-0.3.0/project/graphql/translator_testing_model.graphql` & `translator_testing_model-2.3.0/project/graphql/translator_testing_model.graphql`

 * *Files 10% similar despite different names*

```diff
@@ -16,19 +16,14 @@
     testIssue: TestIssueEnum
     semanticSeverity: SemanticSeverityEnum
     inV1: Boolean
     wellKnown: Boolean
     testReference: Uriorcurie
     runnerSettings: [String]!
     testMetadata: TestMetadata!
-    biolinkQualifiedPredicate: Uriorcurie
-    biolinkSubjectAspectQualifier: String
-    biolinkSubjectDirectionQualifier: String
-    biolinkObjectAspectQualifier: String
-    biolinkObjectDirectionQualifier: String
     id: Uriorcurie!
     tags: [String]
     mustPassDate: Date
     mustPassEnvironment: TestEnvEnum
     scientificQuestion: String
     stringEntry: String
     direction: DirectionEnum
@@ -213,19 +208,14 @@
     testIssue: TestIssueEnum
     semanticSeverity: SemanticSeverityEnum
     inV1: Boolean
     wellKnown: Boolean
     testReference: Uriorcurie
     runnerSettings: [String]!
     testMetadata: TestMetadata!
-    biolinkQualifiedPredicate: Uriorcurie
-    biolinkSubjectAspectQualifier: String
-    biolinkSubjectDirectionQualifier: String
-    biolinkObjectAspectQualifier: String
-    biolinkObjectDirectionQualifier: String
     id: Uriorcurie!
     tags: [String]
   }
 
 type TestCase
   {
     id: Uriorcurie!
@@ -275,19 +265,14 @@
     testIssue: TestIssueEnum
     semanticSeverity: SemanticSeverityEnum
     inV1: Boolean
     wellKnown: Boolean
     testReference: Uriorcurie
     runnerSettings: [String]!
     testMetadata: TestMetadata!
-    biolinkQualifiedPredicate: Uriorcurie
-    biolinkSubjectAspectQualifier: String
-    biolinkSubjectDirectionQualifier: String
-    biolinkObjectAspectQualifier: String
-    biolinkObjectDirectionQualifier: String
     id: Uriorcurie!
     tags: [String]
   }
 
 interface TestEntity
   {
     id: Uriorcurie!
```

### Comparing `translator_testing_model-0.3.0/project/jsonld/translator_testing_model.context.jsonld` & `translator_testing_model-2.3.0/project/jsonld/translator_testing_model.context.jsonld`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'comments'": "{'generation_date': '2024-03-18T12:26:22'}"}*

```diff
@@ -245,11 +245,11 @@
         "ttm": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/",
         "well_known": {
             "@type": "xsd:boolean"
         }
     },
     "comments": {
         "description": "Auto generated by LinkML jsonld context generator",
-        "generation_date": "2024-03-15T17:20:08",
+        "generation_date": "2024-03-18T12:26:22",
         "source": "translator_testing_model.yaml"
     }
 }
```

### Comparing `translator_testing_model-0.3.0/project/jsonld/translator_testing_model.jsonld` & `translator_testing_model-2.3.0/project/jsonld/translator_testing_model.jsonld`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9315151509595954%*

 * *Differences: {"'classes'": "{4: {'slots': {delete: [24, 23, 22, 21, 20]}}, 5: {'slots': {delete: [24, 23, 22, "*

 * *              "21, 20]}}, 6: {'slots': {delete: [24, 23, 22, 21, 20]}}}",*

 * * "'generation_date'": "'2024-03-18T12:26:22'",*

 * * "'slots'": "{33: {delete: ['owner', 'domain_of']}, 34: {delete: ['owner', 'domain_of']}, 35: "*

 * *            "{delete: ['owner', 'domain_of']}, 36: {delete: ['owner', 'domain_of']}, 37: {delete: "*

 * *            "['owner', 'domain_of']}}",*

 * * "'source_file_date'": "'2024-03-18T12:26:09'",*

 * * "'sourc […]*

```diff
@@ -97,19 +97,14 @@
                 "test_issue",
                 "semantic_severity",
                 "in_v1",
                 "well_known",
                 "test_reference",
                 "TestAsset_runner_settings",
                 "test_metadata",
-                "biolink_qualified_predicate",
-                "biolink_subject_aspect_qualifier",
-                "biolink_subject_direction_qualifier",
-                "biolink_object_aspect_qualifier",
-                "biolink_object_direction_qualifier",
                 "TestAsset_id",
                 "TestAsset_tags"
             ]
         },
         {
             "@type": "ClassDefinition",
             "class_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/AcceptanceTestAsset",
@@ -136,19 +131,14 @@
                 "test_issue",
                 "semantic_severity",
                 "in_v1",
                 "well_known",
                 "test_reference",
                 "TestAsset_runner_settings",
                 "test_metadata",
-                "biolink_qualified_predicate",
-                "biolink_subject_aspect_qualifier",
-                "biolink_subject_direction_qualifier",
-                "biolink_object_aspect_qualifier",
-                "biolink_object_direction_qualifier",
                 "TestAsset_id",
                 "TestAsset_tags",
                 "must_pass_date",
                 "must_pass_environment",
                 "scientific_question",
                 "string_entry",
                 "direction",
@@ -185,19 +175,14 @@
                 "test_issue",
                 "semantic_severity",
                 "in_v1",
                 "well_known",
                 "test_reference",
                 "TestAsset_runner_settings",
                 "test_metadata",
-                "biolink_qualified_predicate",
-                "biolink_subject_aspect_qualifier",
-                "biolink_subject_direction_qualifier",
-                "biolink_object_aspect_qualifier",
-                "biolink_object_direction_qualifier",
                 "TestAsset_id",
                 "TestAsset_tags"
             ]
         },
         {
             "@type": "ClassDefinition",
             "class_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/Precondition",
@@ -881,15 +866,15 @@
                 },
                 {
                     "text": "test_skipped"
                 }
             ]
         }
     ],
-    "generation_date": "2024-03-15T17:20:09",
+    "generation_date": "2024-03-18T12:26:22",
     "id": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
     "imports": [
         "linkml:types"
     ],
     "license": "MIT",
     "metamodel_version": "1.7.0",
     "name": "Translator-Testing-Model",
@@ -1377,72 +1362,52 @@
             "range": "uriorcurie",
             "slot_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/biolink_predicate"
         },
         {
             "@type": "SlotDefinition",
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/biolink_subject_aspect_qualifier",
             "description": "The aspect of the subject of the test asset predicate",
-            "domain_of": [
-                "TestAsset"
-            ],
             "from_schema": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
             "name": "biolink_subject_aspect_qualifier",
-            "owner": "TestAsset",
             "range": "string",
             "slot_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/biolink_subject_aspect_qualifier"
         },
         {
             "@type": "SlotDefinition",
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/biolink_subject_direction_qualifier",
             "description": "The direction of the subject of the test asset predicate",
-            "domain_of": [
-                "TestAsset"
-            ],
             "from_schema": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
             "name": "biolink_subject_direction_qualifier",
-            "owner": "TestAsset",
             "range": "string",
             "slot_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/biolink_subject_direction_qualifier"
         },
         {
             "@type": "SlotDefinition",
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/biolink_object_aspect_qualifier",
             "description": "The aspect of the object of the test asset predicate",
-            "domain_of": [
-                "TestAsset"
-            ],
             "from_schema": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
             "name": "biolink_object_aspect_qualifier",
-            "owner": "TestAsset",
             "range": "string",
             "slot_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/biolink_object_aspect_qualifier"
         },
         {
             "@type": "SlotDefinition",
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/biolink_object_direction_qualifier",
             "description": "The direction of the object of the test asset predicate",
-            "domain_of": [
-                "TestAsset"
-            ],
             "from_schema": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
             "name": "biolink_object_direction_qualifier",
-            "owner": "TestAsset",
             "range": "string",
             "slot_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/biolink_object_direction_qualifier"
         },
         {
             "@type": "SlotDefinition",
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/biolink_qualified_predicate",
             "description": "The qualified_predicate in Biolink model corresponding to the shorthand predicate name used in the test asset.",
-            "domain_of": [
-                "TestAsset"
-            ],
             "from_schema": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
             "name": "biolink_qualified_predicate",
-            "owner": "TestAsset",
             "range": "uriorcurie",
             "slot_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/biolink_qualified_predicate"
         },
         {
             "@type": "SlotDefinition",
             "aliases": [
                 "OutputID",
@@ -2330,16 +2295,16 @@
             "owner": "TestRunSession",
             "range": "TestEntity",
             "slot_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/test_entities",
             "usage_slot_name": "test_entities"
         }
     ],
     "source_file": "translator_testing_model.yaml",
-    "source_file_date": "2024-03-15T17:18:34",
-    "source_file_size": 27665,
+    "source_file_date": "2024-03-18T12:26:09",
+    "source_file_size": 27461,
     "title": "Translator Testing Data Model",
     "types": [
         {
             "@type": "TypeDefinition",
             "base": "URIorCURIE",
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/CategoryType",
             "description": "A primitive type in which the value denotes a class within the biolink model. The value must be a URI or a CURIE within the 'biolink' namespace.",
```

### Comparing `translator_testing_model-0.3.0/project/jsonschema/translator_testing_model.schema.json` & `translator_testing_model-2.3.0/project/jsonschema/translator_testing_model.schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999678921807986%*

 * *Differences: {"'$defs'": "{'AcceptanceTestAsset': {'properties': {delete: ['biolink_object_aspect_qualifier', "*

 * *            "'biolink_object_direction_qualifier', 'biolink_qualified_predicate', "*

 * *            "'biolink_subject_aspect_qualifier', 'biolink_subject_direction_qualifier']}}, "*

 * *            "'TestAsset': {'properties': {delete: ['biolink_object_aspect_qualifier', "*

 * *            "'biolink_object_direction_qualifier', 'biolink_qualified_predicate', "*

 * *            "'biolink_subject_aspect_qualifier', 'biolink_subjec […]*

```diff
@@ -8,34 +8,14 @@
                     "description": "An answer that is returned from the test case, note: this must be combined with the expected_result to form a complete answer.  It might make sense to couple these in their own object instead of strictly sticking to the flat schema introduced by the spreadsheet here: https://docs.google.com/spreadsheets/d/1yj7zIchFeVl1OHqL_kE_pqvzNLmGml_FLbHDs-8Yvig/edit#gid=0",
                     "type": "string"
                 },
                 "association": {
                     "description": "Specific Biolink Model association 'category' which applies to the test asset defined knowledge statement",
                     "type": "string"
                 },
-                "biolink_object_aspect_qualifier": {
-                    "description": "The aspect of the object of the test asset predicate",
-                    "type": "string"
-                },
-                "biolink_object_direction_qualifier": {
-                    "description": "The direction of the object of the test asset predicate",
-                    "type": "string"
-                },
-                "biolink_qualified_predicate": {
-                    "description": "The qualified_predicate in Biolink model corresponding to the shorthand predicate name used in the test asset.",
-                    "type": "string"
-                },
-                "biolink_subject_aspect_qualifier": {
-                    "description": "The aspect of the subject of the test asset predicate",
-                    "type": "string"
-                },
-                "biolink_subject_direction_qualifier": {
-                    "description": "The direction of the subject of the test asset predicate",
-                    "type": "string"
-                },
                 "description": {
                     "description": "A human-readable description for a Test Entity",
                     "type": "string"
                 },
                 "direction": {
                     "$ref": "#/$defs/DirectionEnum",
                     "description": "The direction of the expected query result triple"
@@ -884,34 +864,14 @@
             "additionalProperties": false,
             "description": "Represents a Test Asset, which is a single specific instance of TestCase-agnostic semantic parameters representing the specification of a Translator test target with inputs and (expected) outputs.",
             "properties": {
                 "association": {
                     "description": "Specific Biolink Model association 'category' which applies to the test asset defined knowledge statement",
                     "type": "string"
                 },
-                "biolink_object_aspect_qualifier": {
-                    "description": "The aspect of the object of the test asset predicate",
-                    "type": "string"
-                },
-                "biolink_object_direction_qualifier": {
-                    "description": "The direction of the object of the test asset predicate",
-                    "type": "string"
-                },
-                "biolink_qualified_predicate": {
-                    "description": "The qualified_predicate in Biolink model corresponding to the shorthand predicate name used in the test asset.",
-                    "type": "string"
-                },
-                "biolink_subject_aspect_qualifier": {
-                    "description": "The aspect of the subject of the test asset predicate",
-                    "type": "string"
-                },
-                "biolink_subject_direction_qualifier": {
-                    "description": "The direction of the subject of the test asset predicate",
-                    "type": "string"
-                },
                 "description": {
                     "description": "A human-readable description for a Test Entity",
                     "type": "string"
                 },
                 "expected_output": {
                     "type": "string"
                 },
@@ -1268,34 +1228,14 @@
             "additionalProperties": false,
             "description": "Represents a single Biolink Model compliant instance of a subject-predicate-object edge that can be used for testing.",
             "properties": {
                 "association": {
                     "description": "Specific Biolink Model association 'category' which applies to the test asset defined knowledge statement",
                     "type": "string"
                 },
-                "biolink_object_aspect_qualifier": {
-                    "description": "The aspect of the object of the test asset predicate",
-                    "type": "string"
-                },
-                "biolink_object_direction_qualifier": {
-                    "description": "The direction of the object of the test asset predicate",
-                    "type": "string"
-                },
-                "biolink_qualified_predicate": {
-                    "description": "The qualified_predicate in Biolink model corresponding to the shorthand predicate name used in the test asset.",
-                    "type": "string"
-                },
-                "biolink_subject_aspect_qualifier": {
-                    "description": "The aspect of the subject of the test asset predicate",
-                    "type": "string"
-                },
-                "biolink_subject_direction_qualifier": {
-                    "description": "The direction of the subject of the test asset predicate",
-                    "type": "string"
-                },
                 "description": {
                     "description": "A human-readable description for a Test Entity",
                     "type": "string"
                 },
                 "expected_output": {
                     "type": "string"
                 },
```

### Comparing `translator_testing_model-0.3.0/project/owl/translator_testing_model.owl.ttl` & `translator_testing_model-2.3.0/project/owl/translator_testing_model.owl.ttl`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 @prefix ttm: <https://w3id.org/TranslatorSRI/TranslatorTestingModel/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
 
 ttm:AcceptanceTestCase a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "AcceptanceTestCase" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:allValuesFrom ttm:AcceptanceTestAsset ;
+            owl:minCardinality 1 ;
             owl:onProperty ttm:test_assets ],
         [ a owl:Restriction ;
-            owl:minCardinality 1 ;
+            owl:allValuesFrom ttm:AcceptanceTestAsset ;
             owl:onProperty ttm:test_assets ],
         ttm:TestCase ;
     skos:definition "See AcceptanceTestAsset above for more details." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 ttm:AcceptanceTestSuite a owl:Class,
         linkml:ClassDefinition ;
@@ -34,30 +34,30 @@
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 ttm:ComplianceTestCase a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "ComplianceTestCase" ;
     rdfs:subClassOf [ a owl:Restriction ;
             owl:maxCardinality 1 ;
+            owl:onProperty ttm:trapi_version ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
             owl:onProperty ttm:biolink_version ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
             owl:onProperty ttm:trapi_version ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:trapi_version ],
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty ttm:biolink_version ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:biolink_version ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:trapi_version ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:biolink_version ],
         ttm:TestCase ;
     skos:definition "TRAPI and Biolink Model standards compliance test" ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 ttm:OneHopTestCase a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "OneHopTestCase" ;
@@ -93,176 +93,207 @@
     skos:definition "Represents a single Biolink Model compliant instance of a subject-predicate-object edge that can be used for testing." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 ttm:TestRunSession a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "TestRunSession" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:timestamp ],
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty ttm:test_runner_name ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Datetime ;
-            owl:onProperty ttm:timestamp ],
+            owl:allValuesFrom owl:Thing ;
+            owl:onProperty ttm:test_entities ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:allValuesFrom ttm:TestCaseResult ;
             owl:onProperty ttm:test_case_results ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:test_runner_name ],
-        [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty ttm:test_runner_name ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:test_entities ],
+            owl:onProperty ttm:test_case_results ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:timestamp ],
         [ a owl:Restriction ;
-            owl:allValuesFrom owl:Thing ;
+            owl:minCardinality 0 ;
             owl:onProperty ttm:test_entities ],
         [ a owl:Restriction ;
-            owl:allValuesFrom ttm:TestCaseResult ;
-            owl:onProperty ttm:test_case_results ],
+            owl:allValuesFrom linkml:Datetime ;
+            owl:onProperty ttm:timestamp ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:timestamp ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
             owl:onProperty ttm:test_runner_name ],
         ttm:TestEntity ;
     skos:definition "A single invocation of a TestRunner." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 ttm:TestRunnerConfiguration a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "TestRunnerConfiguration" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:test_run_parameters ],
-        [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty ttm:test_run_parameters ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:allValuesFrom linkml:String ;
             owl:onProperty ttm:tags ],
         [ a owl:Restriction ;
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty ttm:test_run_parameters ],
+        [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:test_run_parameters ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
+            owl:minCardinality 0 ;
             owl:onProperty ttm:tags ],
         ttm:TestEntity ;
     skos:definition "General configuration parameters and test data input  for a single invocation of a TestRunner." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
+ttm:biolink_object_aspect_qualifier a owl:ObjectProperty,
+        linkml:SlotDefinition ;
+    rdfs:label "biolink_object_aspect_qualifier" ;
+    skos:definition "The aspect of the object of the test asset predicate" ;
+    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
+
+ttm:biolink_object_direction_qualifier a owl:ObjectProperty,
+        linkml:SlotDefinition ;
+    rdfs:label "biolink_object_direction_qualifier" ;
+    skos:definition "The direction of the object of the test asset predicate" ;
+    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
+
 ttm:biolink_predicate a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "biolink_predicate" ;
     rdfs:range linkml:Uriorcurie ;
     skos:definition "the predicate in Biolink model corresponding to the shorthand predicate name used in the test asset." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
+ttm:biolink_qualified_predicate a owl:ObjectProperty,
+        linkml:SlotDefinition ;
+    rdfs:label "biolink_qualified_predicate" ;
+    rdfs:range linkml:Uriorcurie ;
+    skos:definition "The qualified_predicate in Biolink model corresponding to the shorthand predicate name used in the test asset." ;
+    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
+
+ttm:biolink_subject_aspect_qualifier a owl:ObjectProperty,
+        linkml:SlotDefinition ;
+    rdfs:label "biolink_subject_aspect_qualifier" ;
+    skos:definition "The aspect of the subject of the test asset predicate" ;
+    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
+
+ttm:biolink_subject_direction_qualifier a owl:ObjectProperty,
+        linkml:SlotDefinition ;
+    rdfs:label "biolink_subject_direction_qualifier" ;
+    skos:definition "The direction of the subject of the test asset predicate" ;
+    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
+
 ttm:results a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "results" ;
     rdfs:range ttm:TestOutput ;
     skos:definition "The results of a TestRunner run of one specific TestCase." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 ttm:AcceptanceTestAsset a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "AcceptanceTestAsset" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:scientific_question ],
-        [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:scientific_question ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
             owl:onProperty ttm:notes ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:top_level ],
-        [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:must_pass_environment ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
             owl:onProperty ttm:query_node ],
         [ a owl:Restriction ;
-            owl:allValuesFrom ttm:ExpectedResultsEnum ;
+            owl:maxCardinality 1 ;
             owl:onProperty ttm:expected_result ],
         [ a owl:Restriction ;
-            owl:allValuesFrom ttm:TestEnvEnum ;
-            owl:onProperty ttm:must_pass_environment ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:scientific_question ],
-        [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:string_entry ],
+            owl:onProperty ttm:top_level ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:notes ],
+            owl:allValuesFrom ttm:NodeEnum ;
+            owl:onProperty ttm:query_node ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:answer_informal_concept ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:must_pass_date ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:direction ],
+            owl:onProperty ttm:string_entry ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:must_pass_environment ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:answer_informal_concept ],
+            owl:onProperty ttm:query_node ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:answer_informal_concept ],
+            owl:onProperty ttm:scientific_question ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:query_node ],
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty ttm:scientific_question ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:allValuesFrom linkml:Date ;
             owl:onProperty ttm:must_pass_date ],
         [ a owl:Restriction ;
             owl:allValuesFrom ttm:DirectionEnum ;
             owl:onProperty ttm:direction ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:string_entry ],
+            owl:onProperty ttm:answer_informal_concept ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:string_entry ],
+            owl:onProperty ttm:must_pass_date ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:expected_result ],
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:direction ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom ttm:TestEnvEnum ;
+            owl:onProperty ttm:must_pass_environment ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:expected_result ],
+            owl:onProperty ttm:notes ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty ttm:notes ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:direction ],
+            owl:onProperty ttm:string_entry ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:notes ],
+            owl:onProperty ttm:top_level ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Date ;
+            owl:minCardinality 0 ;
             owl:onProperty ttm:must_pass_date ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:top_level ],
+            owl:onProperty ttm:must_pass_environment ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:answer_informal_concept ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:scientific_question ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:Integer ;
             owl:onProperty ttm:top_level ],
         [ a owl:Restriction ;
-            owl:allValuesFrom ttm:NodeEnum ;
-            owl:onProperty ttm:query_node ],
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:direction ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:must_pass_environment ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:expected_result ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom ttm:ExpectedResultsEnum ;
+            owl:onProperty ttm:expected_result ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty ttm:string_entry ],
         ttm:TestAsset ;
     skos:definition "Model derived from Jenn's test asset design and Shervin's runner JSON here as an example." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 ttm:KnowledgeGraphNavigationTestCase a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "KnowledgeGraphNavigationTestCase" ;
@@ -275,27 +306,27 @@
     rdfs:label "treats" ;
     rdfs:subClassOf ttm:QueryTypeEnum .
 
 ttm:TestOutput a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "TestOutput" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:test_case_id ],
-        [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:pks ],
         [ a owl:Restriction ;
             owl:allValuesFrom ttm:TestResultPKSet ;
             owl:onProperty ttm:pks ],
         [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:test_case_id ],
+        [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:test_case_id ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:allValuesFrom linkml:String ;
             owl:onProperty ttm:test_case_id ],
         ttm:TestEntity ;
     skos:definition "The output of a TestRunner run of one specific TestCase." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 ttm:ComponentEnum a owl:Class,
         linkml:EnumDefinition .
@@ -377,30 +408,30 @@
     skos:definition "Represents a precondition for a TestCase" ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 ttm:Qualifier a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "Qualifier" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
+            owl:maxCardinality 1 ;
             owl:onProperty ttm:parameter ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
+            owl:minCardinality 0 ;
             owl:onProperty ttm:value ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:allValuesFrom linkml:String ;
             owl:onProperty ttm:parameter ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty ttm:value ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:parameter ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:allValuesFrom linkml:String ;
             owl:onProperty ttm:value ],
         ttm:TestEntityParameter ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 <https://w3id.org/TranslatorSRI/TranslatorTestingModel/SemanticSeverityEnum#High> a owl:Class,
         ttm:SemanticSeverityEnum ;
     rdfs:label "High" ;
@@ -416,39 +447,39 @@
     rdfs:label "NotApplicable" ;
     rdfs:subClassOf ttm:SemanticSeverityEnum .
 
 ttm:TestCaseResult a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "TestCaseResult" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:minCardinality 0 ;
             owl:onProperty ttm:test_case ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:allValuesFrom linkml:Uriorcurie ;
             owl:onProperty ttm:test_suite_id ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:test_case_result ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:maxCardinality 1 ;
             owl:onProperty ttm:test_case ],
         [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:test_case_result ],
+        [ a owl:Restriction ;
             owl:allValuesFrom ttm:TestCase ;
             owl:onProperty ttm:test_case ],
         [ a owl:Restriction ;
-            owl:allValuesFrom ttm:TestCaseResultEnum ;
-            owl:onProperty ttm:test_case_result ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:minCardinality 0 ;
             owl:onProperty ttm:test_suite_id ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Uriorcurie ;
+            owl:maxCardinality 1 ;
             owl:onProperty ttm:test_suite_id ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:allValuesFrom ttm:TestCaseResultEnum ;
             owl:onProperty ttm:test_case_result ],
         ttm:TestEntity ;
     skos:definition "The outcome of a TestRunner run of one specific TestCase." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestCaseResultEnum#test_failed> a owl:Class,
         ttm:TestCaseResultEnum ;
@@ -465,31 +496,31 @@
     rdfs:label "test_skipped" ;
     rdfs:subClassOf ttm:TestCaseResultEnum .
 
 ttm:TestEntityParameter a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "TestEntityParameter" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:minCardinality 0 ;
             owl:onProperty ttm:value ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
             owl:onProperty ttm:parameter ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
+            owl:onProperty ttm:value ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
             owl:onProperty ttm:parameter ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:value ],
+            owl:onProperty ttm:parameter ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:value ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:parameter ] ;
+            owl:onProperty ttm:value ] ;
     skos:definition "A single 'tag = value' pair (where 'value' is a simple string)." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestEnvEnum#ci> a owl:Class,
         ttm:TestEnvEnum ;
     rdfs:label "ci" ;
     rdfs:subClassOf ttm:TestEnvEnum .
@@ -580,70 +611,70 @@
     rdfs:subClassOf [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:merged_pk ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
             owl:onProperty ttm:aragorn ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:parent_pk ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:minCardinality 0 ;
             owl:onProperty ttm:improving ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:bte ],
+            owl:onProperty ttm:parent_pk ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:improving ],
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:arax ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty ttm:aragorn ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:unsecret ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:maxCardinality 1 ;
             owl:onProperty ttm:improving ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:arax ],
+            owl:onProperty ttm:aragorn ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:merged_pk ],
+            owl:onProperty ttm:improving ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:unsecret ],
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty ttm:bte ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:arax ],
+            owl:onProperty ttm:bte ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty ttm:merged_pk ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:bte ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty ttm:merged_pk ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:arax ],
+            owl:onProperty ttm:unsecret ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:parent_pk ],
+            owl:onProperty ttm:unsecret ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:aragorn ],
+            owl:onProperty ttm:parent_pk ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:parent_pk ],
+            owl:onProperty ttm:unsecret ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:unsecret ],
+            owl:onProperty ttm:parent_pk ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty ttm:arax ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:bte ],
+            owl:onProperty ttm:arax ],
         ttm:TestEntity ;
     skos:definition "Primary keys for a given ARA result set from a SmokeTest result for a given TestCase." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestSourceEnum#BenchMark> a owl:Class,
         ttm:TestSourceEnum ;
     rdfs:label "BenchMark" ;
@@ -675,31 +706,31 @@
     rdfs:label "TranslatorTeam" ;
     rdfs:subClassOf ttm:TestSourceEnum .
 
 ttm:TestSuiteSpecification a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "TestSuiteSpecification" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:test_data_file_locator ],
+            owl:allValuesFrom ttm:FileFormatEnum ;
+            owl:onProperty ttm:test_data_file_format ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:test_data_file_format ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:test_data_file_locator ],
+            owl:onProperty ttm:test_data_file_format ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:Uriorcurie ;
             owl:onProperty ttm:test_data_file_locator ],
         [ a owl:Restriction ;
-            owl:allValuesFrom ttm:FileFormatEnum ;
-            owl:onProperty ttm:test_data_file_format ],
-        [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:test_data_file_format ],
+            owl:onProperty ttm:test_data_file_locator ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:test_data_file_locator ],
         ttm:TestEntity ;
     skos:definition "Parameters for a Test Case instances either dynamically generated from some external source of Test Assets." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TrapiTemplateEnum#ameliorates> a owl:Class,
         ttm:TrapiTemplateEnum ;
     rdfs:label "ameliorates" ;
@@ -808,317 +839,272 @@
     skos:definition "One or more parameters documenting target characteristics of a TestEntity." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 ttm:TestAsset a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "TestAsset" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:input_id ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom ttm:TestIssueEnum ;
-            owl:onProperty ttm:test_issue ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:well_known ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:test_issue ],
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty ttm:predicate_name ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:semantic_severity ],
+            owl:onProperty ttm:qualifiers ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:output_name ],
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:input_category ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Uriorcurie ;
-            owl:onProperty ttm:input_id ],
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty ttm:runner_settings ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:output_id ],
+            owl:onProperty ttm:test_metadata ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:association ],
+            owl:onProperty ttm:input_id ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:tags ],
+            owl:allValuesFrom ttm:predicate_type ;
+            owl:onProperty ttm:predicate_id ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:association ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:id ],
+            owl:onProperty ttm:predicate_id ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:biolink_subject_aspect_qualifier ],
+            owl:onProperty ttm:expected_output ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:output_name ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:predicate_name ],
+            owl:onProperty ttm:semantic_severity ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:test_issue ],
+            owl:onProperty ttm:id ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:biolink_object_direction_qualifier ],
+            owl:onProperty ttm:output_category ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:biolink_object_aspect_qualifier ],
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:predicate_name ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:biolink_subject_direction_qualifier ],
+            owl:allValuesFrom ttm:TestIssueEnum ;
+            owl:onProperty ttm:test_issue ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty ttm:test_reference ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:semantic_severity ],
+            owl:allValuesFrom ttm:concept_category ;
+            owl:onProperty ttm:output_category ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:input_category ],
+            owl:allValuesFrom linkml:Uriorcurie ;
+            owl:onProperty ttm:output_id ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:input_id ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom ttm:TestMetadata ;
-            owl:onProperty ttm:test_metadata ],
+            owl:onProperty ttm:in_v1 ],
         [ a owl:Restriction ;
-            owl:minCardinality 1 ;
-            owl:onProperty ttm:test_metadata ],
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty ttm:output_name ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:expected_output ],
+            owl:allValuesFrom linkml:Boolean ;
+            owl:onProperty ttm:well_known ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:biolink_object_aspect_qualifier ],
+            owl:onProperty ttm:output_category ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:output_category ],
+            owl:onProperty ttm:input_id ],
         [ a owl:Restriction ;
-            owl:allValuesFrom ttm:SemanticSeverityEnum ;
-            owl:onProperty ttm:semantic_severity ],
+            owl:allValuesFrom linkml:Uriorcurie ;
+            owl:onProperty ttm:id ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:biolink_qualified_predicate ],
+            owl:onProperty ttm:input_category ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:biolink_object_direction_qualifier ],
+            owl:onProperty ttm:association ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:input_name ],
+            owl:onProperty ttm:output_name ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:predicate_name ],
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:test_issue ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:output_name ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:Boolean ;
             owl:onProperty ttm:in_v1 ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:tags ],
         [ a owl:Restriction ;
+            owl:minCardinality 1 ;
+            owl:onProperty ttm:runner_settings ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:input_name ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom ttm:association_category ;
+            owl:onProperty ttm:association ],
+        [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:biolink_subject_aspect_qualifier ],
+            owl:onProperty ttm:well_known ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
             owl:onProperty ttm:input_name ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:predicate_id ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:predicate_id ],
+            owl:onProperty ttm:expected_output ],
         [ a owl:Restriction ;
-            owl:allValuesFrom ttm:Qualifier ;
-            owl:onProperty ttm:qualifiers ],
+            owl:allValuesFrom linkml:Uriorcurie ;
+            owl:onProperty ttm:input_id ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:test_reference ],
         [ a owl:Restriction ;
-            owl:minCardinality 1 ;
-            owl:onProperty ttm:id ],
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:output_id ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:output_id ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:test_metadata ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:biolink_subject_aspect_qualifier ],
-        [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:in_v1 ],
+            owl:onProperty ttm:input_name ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:qualifiers ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:in_v1 ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Boolean ;
-            owl:onProperty ttm:well_known ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Uriorcurie ;
-            owl:onProperty ttm:id ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Uriorcurie ;
-            owl:onProperty ttm:test_reference ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Uriorcurie ;
-            owl:onProperty ttm:biolink_qualified_predicate ],
+            owl:onProperty ttm:semantic_severity ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:output_name ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom ttm:predicate_type ;
-            owl:onProperty ttm:predicate_id ],
+            owl:onProperty ttm:expected_output ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:input_category ],
+            owl:allValuesFrom ttm:TestMetadata ;
+            owl:onProperty ttm:test_metadata ],
         [ a owl:Restriction ;
             owl:allValuesFrom ttm:concept_category ;
-            owl:onProperty ttm:output_category ],
+            owl:onProperty ttm:input_category ],
         [ a owl:Restriction ;
-            owl:allValuesFrom ttm:association_category ;
-            owl:onProperty ttm:association ],
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty ttm:tags ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:output_category ],
+            owl:allValuesFrom ttm:SemanticSeverityEnum ;
+            owl:onProperty ttm:semantic_severity ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:biolink_qualified_predicate ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:biolink_subject_direction_qualifier ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:well_known ],
+            owl:onProperty ttm:predicate_id ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:Uriorcurie ;
-            owl:onProperty ttm:output_id ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom ttm:concept_category ;
-            owl:onProperty ttm:input_category ],
+            owl:onProperty ttm:test_reference ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:biolink_object_direction_qualifier ],
+            owl:minCardinality 1 ;
+            owl:onProperty ttm:id ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:biolink_subject_direction_qualifier ],
+            owl:allValuesFrom ttm:Qualifier ;
+            owl:onProperty ttm:qualifiers ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:runner_settings ],
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:predicate_name ],
         [ a owl:Restriction ;
-            owl:minCardinality 1 ;
-            owl:onProperty ttm:runner_settings ],
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:in_v1 ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:input_name ],
+            owl:onProperty ttm:well_known ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:expected_output ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:expected_output ],
+            owl:onProperty ttm:test_issue ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:predicate_name ],
+            owl:minCardinality 1 ;
+            owl:onProperty ttm:test_metadata ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:biolink_object_aspect_qualifier ],
+            owl:onProperty ttm:association ],
         ttm:TestEntity ;
     skos:definition "Represents a Test Asset, which is a single specific instance of TestCase-agnostic semantic parameters representing the specification of a Translator test target with inputs and (expected) outputs." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 ttm:TestMetadata a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "TestMetadata" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:allValuesFrom ttm:TestObjectiveEnum ;
-            owl:onProperty ttm:test_objective ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:test_source ],
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty ttm:test_annotations ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty ttm:test_objective ],
         [ a owl:Restriction ;
+            owl:allValuesFrom ttm:TestObjectiveEnum ;
+            owl:onProperty ttm:test_objective ],
+        [ a owl:Restriction ;
             owl:allValuesFrom linkml:Uriorcurie ;
             owl:onProperty ttm:test_reference ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:test_annotations ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
             owl:onProperty ttm:test_reference ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:test_annotations ],
+            owl:onProperty ttm:test_source ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:allValuesFrom ttm:TestSourceEnum ;
             owl:onProperty ttm:test_source ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:test_annotations ],
+            owl:onProperty ttm:test_source ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:test_objective ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:maxCardinality 1 ;
             owl:onProperty ttm:test_reference ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
+            owl:maxCardinality 1 ;
             owl:onProperty ttm:test_annotations ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom ttm:TestSourceEnum ;
-            owl:onProperty ttm:test_source ],
         ttm:TestEntity ;
     skos:definition "Represents metadata related to (external SME, SMURF, Translator feedback,  large scale batch, etc.) like the provenance of test assets, cases and/or suites." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestSourceEnum#GitHubUserFeedback> a owl:Class,
         ttm:TestSourceEnum ;
     rdfs:label "GitHubUserFeedback" ;
     rdfs:subClassOf ttm:TestSourceEnum .
 
 ttm:TestSuite a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "TestSuite" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:allValuesFrom ttm:TestCase ;
-            owl:onProperty ttm:test_cases ],
-        [ a owl:Restriction ;
             owl:allValuesFrom ttm:TestSuiteSpecification ;
             owl:onProperty ttm:test_suite_specification ],
         [ a owl:Restriction ;
-            owl:allValuesFrom ttm:TestPersonaEnum ;
+            owl:allValuesFrom ttm:TestMetadata ;
+            owl:onProperty ttm:test_metadata ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
             owl:onProperty ttm:test_persona ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:test_suite_specification ],
+            owl:onProperty ttm:test_cases ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:test_persona ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom ttm:TestMetadata ;
-            owl:onProperty ttm:test_metadata ],
+            owl:onProperty ttm:test_suite_specification ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
             owl:onProperty ttm:test_metadata ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:maxCardinality 1 ;
             owl:onProperty ttm:test_persona ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:test_cases ],
-        [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty ttm:test_metadata ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:allValuesFrom ttm:TestCase ;
+            owl:onProperty ttm:test_cases ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
             owl:onProperty ttm:test_suite_specification ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom ttm:TestPersonaEnum ;
+            owl:onProperty ttm:test_persona ],
         ttm:TestEntity ;
     skos:definition "Specification of a set of Test Cases, one of either with a static list of 'test_cases' or a dynamic 'test_suite_specification' slot values. Note: at least one slot or the other, but generally not both(?) needs to be present." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 ttm:answer_informal_concept a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "answer_informal_concept" ;
@@ -1139,45 +1125,14 @@
 ttm:association a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "association" ;
     rdfs:range ttm:association_category ;
     skos:definition "Specific Biolink Model association 'category' which applies to the test asset defined knowledge statement" ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
-ttm:biolink_object_aspect_qualifier a owl:ObjectProperty,
-        linkml:SlotDefinition ;
-    rdfs:label "biolink_object_aspect_qualifier" ;
-    skos:definition "The aspect of the object of the test asset predicate" ;
-    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
-
-ttm:biolink_object_direction_qualifier a owl:ObjectProperty,
-        linkml:SlotDefinition ;
-    rdfs:label "biolink_object_direction_qualifier" ;
-    skos:definition "The direction of the object of the test asset predicate" ;
-    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
-
-ttm:biolink_qualified_predicate a owl:ObjectProperty,
-        linkml:SlotDefinition ;
-    rdfs:label "biolink_qualified_predicate" ;
-    rdfs:range linkml:Uriorcurie ;
-    skos:definition "The qualified_predicate in Biolink model corresponding to the shorthand predicate name used in the test asset." ;
-    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
-
-ttm:biolink_subject_aspect_qualifier a owl:ObjectProperty,
-        linkml:SlotDefinition ;
-    rdfs:label "biolink_subject_aspect_qualifier" ;
-    skos:definition "The aspect of the subject of the test asset predicate" ;
-    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
-
-ttm:biolink_subject_direction_qualifier a owl:ObjectProperty,
-        linkml:SlotDefinition ;
-    rdfs:label "biolink_subject_direction_qualifier" ;
-    skos:definition "The direction of the subject of the test asset predicate" ;
-    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
-
 ttm:biolink_version a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "biolink_version" ;
     skos:definition "Biolink Model release (SemVer string)" ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 ttm:bte a owl:ObjectProperty,
@@ -1613,113 +1568,113 @@
         <https://w3id.org/TranslatorSRI/TranslatorTestingModel/SemanticSeverityEnum#Low>,
         <https://w3id.org/TranslatorSRI/TranslatorTestingModel/SemanticSeverityEnum#NotApplicable> .
 
 ttm:TestCase a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "TestCase" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Uriorcurie ;
-            owl:onProperty ttm:test_case_input_id ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom ttm:TrapiTemplateEnum ;
+            owl:maxCardinality 1 ;
             owl:onProperty ttm:trapi_template ],
         [ a owl:Restriction ;
-            owl:minCardinality 1 ;
-            owl:onProperty ttm:test_case_runner_settings ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom ttm:TestEnvEnum ;
-            owl:onProperty ttm:test_env ],
+            owl:allValuesFrom ttm:QueryTypeEnum ;
+            owl:onProperty ttm:query_type ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:test_case_source ],
+            owl:onProperty ttm:test_env ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:trapi_template ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
             owl:onProperty ttm:test_case_input_id ],
         [ a owl:Restriction ;
-            owl:allValuesFrom ttm:ComponentEnum ;
-            owl:onProperty ttm:components ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:query_type ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom ttm:Precondition ;
-            owl:onProperty ttm:preconditions ],
+            owl:allValuesFrom ttm:TestObjectiveEnum ;
+            owl:onProperty ttm:test_case_objective ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty ttm:test_case_predicate_id ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:query_type ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
             owl:onProperty ttm:test_case_objective ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:test_case_predicate_name ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:test_env ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
             owl:onProperty ttm:test_case_source ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:test_case_predicate_id ],
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:query_type ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:test_case_predicate_name ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
             owl:onProperty ttm:trapi_template ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:test_case_objective ],
+            owl:onProperty ttm:components ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:test_case_predicate_id ],
         [ a owl:Restriction ;
-            owl:allValuesFrom owl:Thing ;
-            owl:onProperty ttm:test_assets ],
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty ttm:test_case_predicate_name ],
         [ a owl:Restriction ;
-            owl:allValuesFrom ttm:TestObjectiveEnum ;
-            owl:onProperty ttm:test_case_objective ],
+            owl:allValuesFrom ttm:TestSourceEnum ;
+            owl:onProperty ttm:test_case_source ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:test_env ],
+            owl:onProperty ttm:query_type ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:components ],
+            owl:onProperty ttm:test_case_source ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:test_case_predicate_name ],
+            owl:onProperty ttm:test_case_runner_settings ],
         [ a owl:Restriction ;
-            owl:allValuesFrom ttm:TestSourceEnum ;
-            owl:onProperty ttm:test_case_source ],
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:test_case_objective ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:test_case_input_id ],
+            owl:minCardinality 1 ;
+            owl:onProperty ttm:test_case_runner_settings ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom ttm:Precondition ;
+            owl:onProperty ttm:preconditions ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
             owl:onProperty ttm:test_assets ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:test_case_runner_settings ],
+            owl:allValuesFrom linkml:Uriorcurie ;
+            owl:onProperty ttm:test_case_input_id ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:tags ],
         [ a owl:Restriction ;
-            owl:allValuesFrom ttm:QueryTypeEnum ;
-            owl:onProperty ttm:query_type ],
+            owl:allValuesFrom owl:Thing ;
+            owl:onProperty ttm:test_assets ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom ttm:ComponentEnum ;
+            owl:onProperty ttm:components ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:test_case_predicate_name ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty ttm:test_case_predicate_id ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:preconditions ],
         [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:test_case_input_id ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom ttm:TestEnvEnum ;
+            owl:onProperty ttm:test_env ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:test_env ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:test_case_predicate_name ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom ttm:TrapiTemplateEnum ;
+            owl:onProperty ttm:trapi_template ],
+        [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
             owl:onProperty ttm:tags ],
         ttm:TestEntity ;
     skos:definition "Represents a single enumerated instance of Test Case, derived from a  given collection of one or more TestAsset instances (the value of the 'test_assets' slot) which define the 'inputs' and 'outputs' of the TestCase, used to probe a particular test condition." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 ttm:TestCaseResultEnum a owl:Class,
@@ -1760,44 +1715,44 @@
         <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestPersonaEnum#Mechanistic> .
 
 ttm:TestEntity a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "TestEntity" ;
     rdfs:subClassOf [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:tags ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
             owl:onProperty ttm:name ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
+            owl:maxCardinality 1 ;
             owl:onProperty ttm:description ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:tags ],
+            owl:onProperty ttm:name ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:allValuesFrom linkml:Uriorcurie ;
             owl:onProperty ttm:id ],
         [ a owl:Restriction ;
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty ttm:tags ],
+        [ a owl:Restriction ;
             owl:minCardinality 1 ;
             owl:onProperty ttm:id ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:name ],
-        [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:name ],
+            owl:onProperty ttm:description ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Uriorcurie ;
+            owl:maxCardinality 1 ;
             owl:onProperty ttm:id ],
         [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:name ],
+        [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:description ],
+            owl:onProperty ttm:tags ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:allValuesFrom linkml:String ;
             owl:onProperty ttm:description ] ;
     skos:definition "Abstract global 'identification' class shared as a parent with all major model classes within the data model for Translator testing." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 ttm:TestEnvEnum a owl:Class,
         linkml:EnumDefinition ;
     owl:unionOf ( <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestEnvEnum#dev> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestEnvEnum#ci> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestEnvEnum#test> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestEnvEnum#prod> ) ;
```

### Comparing `translator_testing_model-0.3.0/project/protobuf/translator_testing_model.proto` & `translator_testing_model-2.3.0/project/protobuf/translator_testing_model.proto`

 * *Files 12% similar despite different names*

```diff
@@ -17,19 +17,14 @@
   testIssueEnum testIssue = 0
   semanticSeverityEnum semanticSeverity = 0
   boolean inV1 = 0
   boolean wellKnown = 0
   uriorcurie testReference = 0
  repeated  string runnerSettings = 0
   testMetadata testMetadata = 0
-  uriorcurie biolinkQualifiedPredicate = 0
-  string biolinkSubjectAspectQualifier = 0
-  string biolinkSubjectDirectionQualifier = 0
-  string biolinkObjectAspectQualifier = 0
-  string biolinkObjectDirectionQualifier = 0
   uriorcurie id = 0
  repeated  string tags = 0
   date mustPassDate = 0
   testEnvEnum mustPassEnvironment = 0
   string scientificQuestion = 0
   string stringEntry = 0
   directionEnum direction = 0
@@ -208,19 +203,14 @@
   testIssueEnum testIssue = 0
   semanticSeverityEnum semanticSeverity = 0
   boolean inV1 = 0
   boolean wellKnown = 0
   uriorcurie testReference = 0
  repeated  string runnerSettings = 0
   testMetadata testMetadata = 0
-  uriorcurie biolinkQualifiedPredicate = 0
-  string biolinkSubjectAspectQualifier = 0
-  string biolinkSubjectDirectionQualifier = 0
-  string biolinkObjectAspectQualifier = 0
-  string biolinkObjectDirectionQualifier = 0
   uriorcurie id = 0
  repeated  string tags = 0
  }
 // Represents a single enumerated instance of Test Case, derived from a  given collection of one or more TestAsset instances (the value of the 'test_assets' slot) which define the 'inputs' and 'outputs' of the TestCase, used to probe a particular test condition.
 message TestCase
  {
   uriorcurie id = 0
@@ -270,19 +260,14 @@
   testIssueEnum testIssue = 0
   semanticSeverityEnum semanticSeverity = 0
   boolean inV1 = 0
   boolean wellKnown = 0
   uriorcurie testReference = 0
  repeated  string runnerSettings = 0
   testMetadata testMetadata = 0
-  uriorcurie biolinkQualifiedPredicate = 0
-  string biolinkSubjectAspectQualifier = 0
-  string biolinkSubjectDirectionQualifier = 0
-  string biolinkObjectAspectQualifier = 0
-  string biolinkObjectDirectionQualifier = 0
   uriorcurie id = 0
  repeated  string tags = 0
  }
 // A single 'tag = value' pair (where 'value' is a simple string).
 message TestEntityParameter
  {
   string parameter = 0
```

### Comparing `translator_testing_model-0.3.0/project/shacl/translator_testing_model.shacl.ttl` & `translator_testing_model-2.3.0/project/shacl/translator_testing_model.shacl.ttl`

 * *Files 2% similar despite different names*

```diff
@@ -4,1150 +4,1102 @@
 @prefix ttm: <https://w3id.org/TranslatorSRI/TranslatorTestingModel/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
 
 ttm:AcceptanceTestCase a sh:NodeShape ;
     sh:closed true ;
     sh:description "See AcceptanceTestAsset above for more details." ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:description "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)" ;
+    sh:property [ sh:class ttm:Precondition ;
+            sh:nodeKind sh:IRI ;
+            sh:order 3 ;
+            sh:path ttm:preconditions ],
+        [ sh:datatype xsd:string ;
+            sh:maxCount 1 ;
+            sh:order 8 ;
+            sh:path ttm:test_case_predicate_name ],
+        [ sh:maxCount 1 ;
+            sh:order 10 ;
+            sh:path ttm:test_case_input_id ],
+        [ sh:description "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)" ;
             sh:in ( "AcceptanceTest" "BenchmarkTest" "QuantitativeTest" ) ;
             sh:maxCount 1 ;
             sh:order 6 ;
             sh:path ttm:test_case_objective ],
         [ sh:description "A unique identifier for a Test Entity" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 12 ;
             sh:path schema1:identifier ],
-        [ sh:class ttm:Precondition ;
-            sh:nodeKind sh:IRI ;
-            sh:order 3 ;
-            sh:path ttm:preconditions ],
+        [ sh:description "Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string." ;
+            sh:in ( "SME" "SMURF" "GitHubUserFeedback" "TACT" "BenchMark" "TranslatorTeam" "TestDataLocation" ) ;
+            sh:maxCount 1 ;
+            sh:order 7 ;
+            sh:path ttm:test_case_source ],
         [ sh:datatype xsd:string ;
-            sh:description "A human-readable description for a Test Entity" ;
+            sh:description "A human-readable name for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 14 ;
-            sh:path schema1:description ],
+            sh:order 13 ;
+            sh:path schema1:name ],
         [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
-            sh:order 8 ;
-            sh:path ttm:test_case_predicate_name ],
-        [ sh:description "Deployment environment within which the associated TestSuite is run." ;
-            sh:in ( "dev" "ci" "test" "prod" ) ;
+            sh:order 9 ;
+            sh:path ttm:test_case_predicate_id ],
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path ttm:test_env ],
-        [ sh:description "The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX." ;
-            sh:in [ rdf:rest () ] ;
-            sh:order 5 ;
-            sh:path ttm:components ],
+            sh:order 14 ;
+            sh:path schema1:description ],
         [ sh:class ttm:AcceptanceTestAsset ;
             sh:description "One or more 'tags' slot values (inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in 'test_assets' slot (\"Block List\") collection." ;
             sh:minCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 2 ;
             sh:path ttm:test_assets ],
-        [ sh:maxCount 1 ;
-            sh:order 10 ;
-            sh:path ttm:test_case_input_id ],
-        [ sh:datatype xsd:string ;
-            sh:description "A human-readable name for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:order 13 ;
-            sh:path schema1:name ],
         [ sh:datatype xsd:string ;
             sh:description "Settings for the test harness for TestCase" ;
             sh:minCount 1 ;
             sh:order 11 ;
             sh:path ttm:test_case_runner_settings ],
-        [ sh:datatype xsd:string ;
-            sh:maxCount 1 ;
-            sh:order 9 ;
-            sh:path ttm:test_case_predicate_id ],
-        [ sh:datatype xsd:string ;
-            sh:description "One or more 'tags' slot values (slot inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in a \"Block List\" collection." ;
-            sh:order 15 ;
-            sh:path schema1:additionalType ],
-        [ sh:description "Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string." ;
-            sh:in ( "SME" "SMURF" "GitHubUserFeedback" "TACT" "BenchMark" "TranslatorTeam" "TestDataLocation" ) ;
+        [ sh:description "The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX." ;
+            sh:in [ rdf:rest () ] ;
+            sh:order 5 ;
+            sh:path ttm:components ],
+        [ sh:description "Type of TestCase query." ;
+            sh:in ( "treats" ) ;
             sh:maxCount 1 ;
-            sh:order 7 ;
-            sh:path ttm:test_case_source ],
+            sh:order 1 ;
+            sh:path ttm:query_type ],
         [ sh:description "A template for a query, which can be used to generate a query for a test case.  note: the current enumerated values for this slot come from the Benchmarks repo config/benchmarks.json \"templates\" collection and refer to the \"name\" field of each template.  Templates themselves are currently stored in the config/[source_name]/templates directory." ;
             sh:in ( "ameliorates" "treats" "three_hop" "drug_treats_rare_disease" "drug-to-gene" ) ;
             sh:maxCount 1 ;
             sh:order 4 ;
             sh:path ttm:trapi_template ],
-        [ sh:description "Type of TestCase query." ;
-            sh:in ( "treats" ) ;
+        [ sh:datatype xsd:string ;
+            sh:description "One or more 'tags' slot values (slot inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in a \"Block List\" collection." ;
+            sh:order 15 ;
+            sh:path schema1:additionalType ],
+        [ sh:description "Deployment environment within which the associated TestSuite is run." ;
+            sh:in ( "dev" "ci" "test" "prod" ) ;
             sh:maxCount 1 ;
-            sh:order 1 ;
-            sh:path ttm:query_type ] ;
+            sh:order 0 ;
+            sh:path ttm:test_env ] ;
     sh:targetClass ttm:AcceptanceTestCase .
 
 ttm:AcceptanceTestSuite a sh:NodeShape ;
     sh:closed true ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:string ;
-            sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
-            sh:order 7 ;
-            sh:path schema1:additionalType ],
+    sh:property [ sh:class ttm:TestMetadata ;
+            sh:description "Test metadata describes the external provenance, cross-references and objectives for a given test." ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 0 ;
+            sh:path ttm:test_metadata ],
+        [ sh:class ttm:TestSuiteSpecification ;
+            sh:description "Declarative specification of a Test Suite of Test Cases whose generation is deferred, (i.e. within a Test Runner) or whose creation is achieved by stream processing of an external data source." ;
+            sh:maxCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 3 ;
+            sh:path ttm:test_suite_specification ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable name for a Test Entity" ;
             sh:maxCount 1 ;
             sh:order 5 ;
             sh:path schema1:name ],
-        [ sh:description "A Test persona describes the user or operational context of a given test." ;
-            sh:in ( "All" "Clinical" "LookUp" "Mechanistic" ) ;
+        [ sh:description "A unique identifier for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 1 ;
-            sh:path ttm:test_persona ],
+            sh:minCount 1 ;
+            sh:order 4 ;
+            sh:path schema1:identifier ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
             sh:order 6 ;
             sh:path schema1:description ],
-        [ sh:class ttm:TestSuiteSpecification ;
-            sh:description "Declarative specification of a Test Suite of Test Cases whose generation is deferred, (i.e. within a Test Runner) or whose creation is achieved by stream processing of an external data source." ;
-            sh:maxCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 3 ;
-            sh:path ttm:test_suite_specification ],
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
+            sh:order 7 ;
+            sh:path schema1:additionalType ],
         [ sh:class ttm:TestCase ;
             sh:description "List of explicitly enumerated Test Cases." ;
             sh:nodeKind sh:IRI ;
             sh:order 2 ;
             sh:path ttm:test_cases ],
-        [ sh:class ttm:TestMetadata ;
-            sh:description "Test metadata describes the external provenance, cross-references and objectives for a given test." ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 0 ;
-            sh:path ttm:test_metadata ],
-        [ sh:description "A unique identifier for a Test Entity" ;
+        [ sh:description "A Test persona describes the user or operational context of a given test." ;
+            sh:in ( "All" "Clinical" "LookUp" "Mechanistic" ) ;
             sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 4 ;
-            sh:path schema1:identifier ] ;
+            sh:order 1 ;
+            sh:path ttm:test_persona ] ;
     sh:targetClass ttm:AcceptanceTestSuite .
 
 ttm:BenchmarkTestSuite a sh:NodeShape ;
     sh:closed true ;
     sh:description "JsonObj(is_a='TestSuite')" ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:targetClass ttm:BenchmarkTestSuite .
 
 ttm:ComplianceTestCase a sh:NodeShape ;
     sh:closed true ;
     sh:description "TRAPI and Biolink Model standards compliance test" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:string ;
-            sh:description "TRAPI version (SemVer string)" ;
-            sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path ttm:trapi_version ],
-        [ sh:description "Deployment environment within which the associated TestSuite is run." ;
-            sh:in ( "dev" "ci" "test" "prod" ) ;
-            sh:maxCount 1 ;
-            sh:order 2 ;
-            sh:path ttm:test_env ],
-        [ sh:datatype xsd:string ;
-            sh:description "One or more 'tags' slot values (slot inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in a \"Block List\" collection." ;
-            sh:order 17 ;
-            sh:path schema1:additionalType ],
-        [ sh:description "Type of TestCase query." ;
-            sh:in ( "treats" ) ;
-            sh:maxCount 1 ;
-            sh:order 3 ;
-            sh:path ttm:query_type ],
-        [ sh:datatype xsd:string ;
-            sh:description "A human-readable name for a Test Entity" ;
+    sh:property [ sh:description "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)" ;
+            sh:in ( "AcceptanceTest" "BenchmarkTest" "QuantitativeTest" ) ;
             sh:maxCount 1 ;
-            sh:order 15 ;
-            sh:path schema1:name ],
+            sh:order 8 ;
+            sh:path ttm:test_case_objective ],
+        [ sh:maxCount 1 ;
+            sh:order 12 ;
+            sh:path ttm:test_case_input_id ],
         [ sh:description "A template for a query, which can be used to generate a query for a test case.  note: the current enumerated values for this slot come from the Benchmarks repo config/benchmarks.json \"templates\" collection and refer to the \"name\" field of each template.  Templates themselves are currently stored in the config/[source_name]/templates directory." ;
             sh:in ( "ameliorates" "treats" "three_hop" "drug_treats_rare_disease" "drug-to-gene" ) ;
             sh:maxCount 1 ;
             sh:order 6 ;
             sh:path ttm:trapi_template ],
-        [ sh:description "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)" ;
-            sh:in ( "AcceptanceTest" "BenchmarkTest" "QuantitativeTest" ) ;
-            sh:maxCount 1 ;
-            sh:order 8 ;
-            sh:path ttm:test_case_objective ],
-        [ sh:class ttm:Precondition ;
-            sh:nodeKind sh:IRI ;
-            sh:order 5 ;
-            sh:path ttm:preconditions ],
-        [ sh:description "The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX." ;
-            sh:in [ rdf:rest () ] ;
-            sh:order 7 ;
-            sh:path ttm:components ],
         [ sh:description "Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string." ;
             sh:in ( "SME" "SMURF" "GitHubUserFeedback" "TACT" "BenchMark" "TranslatorTeam" "TestDataLocation" ) ;
             sh:maxCount 1 ;
             sh:order 9 ;
             sh:path ttm:test_case_source ],
-        [ sh:maxCount 1 ;
-            sh:order 12 ;
-            sh:path ttm:test_case_input_id ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
             sh:order 16 ;
             sh:path schema1:description ],
         [ sh:class ttm:TestAsset ;
             sh:description "One or more 'tags' slot values (inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in 'test_assets' slot (\"Block List\") collection." ;
             sh:minCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 4 ;
             sh:path ttm:test_assets ],
+        [ sh:description "The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX." ;
+            sh:in [ rdf:rest () ] ;
+            sh:order 7 ;
+            sh:path ttm:components ],
+        [ sh:datatype xsd:string ;
+            sh:description "Settings for the test harness for TestCase" ;
+            sh:minCount 1 ;
+            sh:order 13 ;
+            sh:path ttm:test_case_runner_settings ],
+        [ sh:description "Type of TestCase query." ;
+            sh:in ( "treats" ) ;
+            sh:maxCount 1 ;
+            sh:order 3 ;
+            sh:path ttm:query_type ],
+        [ sh:datatype xsd:string ;
+            sh:description "One or more 'tags' slot values (slot inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in a \"Block List\" collection." ;
+            sh:order 17 ;
+            sh:path schema1:additionalType ],
+        [ sh:datatype xsd:string ;
+            sh:description "Biolink Model release (SemVer string)" ;
+            sh:maxCount 1 ;
+            sh:order 1 ;
+            sh:path ttm:biolink_version ],
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable name for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:order 15 ;
+            sh:path schema1:name ],
         [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
             sh:order 11 ;
             sh:path ttm:test_case_predicate_id ],
         [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
             sh:order 10 ;
             sh:path ttm:test_case_predicate_name ],
         [ sh:description "A unique identifier for a Test Entity" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 14 ;
             sh:path schema1:identifier ],
-        [ sh:datatype xsd:string ;
-            sh:description "Biolink Model release (SemVer string)" ;
+        [ sh:class ttm:Precondition ;
+            sh:nodeKind sh:IRI ;
+            sh:order 5 ;
+            sh:path ttm:preconditions ],
+        [ sh:description "Deployment environment within which the associated TestSuite is run." ;
+            sh:in ( "dev" "ci" "test" "prod" ) ;
             sh:maxCount 1 ;
-            sh:order 1 ;
-            sh:path ttm:biolink_version ],
+            sh:order 2 ;
+            sh:path ttm:test_env ],
         [ sh:datatype xsd:string ;
-            sh:description "Settings for the test harness for TestCase" ;
-            sh:minCount 1 ;
-            sh:order 13 ;
-            sh:path ttm:test_case_runner_settings ] ;
+            sh:description "TRAPI version (SemVer string)" ;
+            sh:maxCount 1 ;
+            sh:order 0 ;
+            sh:path ttm:trapi_version ] ;
     sh:targetClass ttm:ComplianceTestCase .
 
 ttm:KnowledgeGraphNavigationTestCase a sh:NodeShape ;
     sh:closed true ;
     sh:description "Knowledge Graph navigation integration test" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:class ttm:Precondition ;
+    sh:property [ sh:class ttm:TestAsset ;
+            sh:description "One or more 'tags' slot values (inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in 'test_assets' slot (\"Block List\") collection." ;
+            sh:minCount 1 ;
             sh:nodeKind sh:IRI ;
-            sh:order 3 ;
-            sh:path ttm:preconditions ],
-        [ sh:maxCount 1 ;
-            sh:order 10 ;
-            sh:path ttm:test_case_input_id ],
+            sh:order 2 ;
+            sh:path ttm:test_assets ],
+        [ sh:description "Type of TestCase query." ;
+            sh:in ( "treats" ) ;
+            sh:maxCount 1 ;
+            sh:order 1 ;
+            sh:path ttm:query_type ],
+        [ sh:description "Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string." ;
+            sh:in ( "SME" "SMURF" "GitHubUserFeedback" "TACT" "BenchMark" "TranslatorTeam" "TestDataLocation" ) ;
+            sh:maxCount 1 ;
+            sh:order 7 ;
+            sh:path ttm:test_case_source ],
         [ sh:description "The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX." ;
             sh:in [ rdf:rest () ] ;
             sh:order 5 ;
             sh:path ttm:components ],
-        [ sh:description "A template for a query, which can be used to generate a query for a test case.  note: the current enumerated values for this slot come from the Benchmarks repo config/benchmarks.json \"templates\" collection and refer to the \"name\" field of each template.  Templates themselves are currently stored in the config/[source_name]/templates directory." ;
-            sh:in ( "ameliorates" "treats" "three_hop" "drug_treats_rare_disease" "drug-to-gene" ) ;
-            sh:maxCount 1 ;
-            sh:order 4 ;
-            sh:path ttm:trapi_template ],
-        [ sh:datatype xsd:string ;
-            sh:maxCount 1 ;
-            sh:order 8 ;
-            sh:path ttm:test_case_predicate_name ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable name for a Test Entity" ;
             sh:maxCount 1 ;
             sh:order 13 ;
             sh:path schema1:name ],
+        [ sh:maxCount 1 ;
+            sh:order 10 ;
+            sh:path ttm:test_case_input_id ],
+        [ sh:description "Deployment environment within which the associated TestSuite is run." ;
+            sh:in ( "dev" "ci" "test" "prod" ) ;
+            sh:maxCount 1 ;
+            sh:order 0 ;
+            sh:path ttm:test_env ],
+        [ sh:datatype xsd:string ;
+            sh:maxCount 1 ;
+            sh:order 8 ;
+            sh:path ttm:test_case_predicate_name ],
         [ sh:description "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)" ;
             sh:in ( "AcceptanceTest" "BenchmarkTest" "QuantitativeTest" ) ;
             sh:maxCount 1 ;
             sh:order 6 ;
             sh:path ttm:test_case_objective ],
         [ sh:datatype xsd:string ;
+            sh:description "Settings for the test harness for TestCase" ;
+            sh:minCount 1 ;
+            sh:order 11 ;
+            sh:path ttm:test_case_runner_settings ],
+        [ sh:description "A template for a query, which can be used to generate a query for a test case.  note: the current enumerated values for this slot come from the Benchmarks repo config/benchmarks.json \"templates\" collection and refer to the \"name\" field of each template.  Templates themselves are currently stored in the config/[source_name]/templates directory." ;
+            sh:in ( "ameliorates" "treats" "three_hop" "drug_treats_rare_disease" "drug-to-gene" ) ;
             sh:maxCount 1 ;
-            sh:order 9 ;
-            sh:path ttm:test_case_predicate_id ],
-        [ sh:description "Type of TestCase query." ;
-            sh:in ( "treats" ) ;
-            sh:maxCount 1 ;
-            sh:order 1 ;
-            sh:path ttm:query_type ],
+            sh:order 4 ;
+            sh:path ttm:trapi_template ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
             sh:order 14 ;
             sh:path schema1:description ],
+        [ sh:class ttm:Precondition ;
+            sh:nodeKind sh:IRI ;
+            sh:order 3 ;
+            sh:path ttm:preconditions ],
+        [ sh:datatype xsd:string ;
+            sh:maxCount 1 ;
+            sh:order 9 ;
+            sh:path ttm:test_case_predicate_id ],
         [ sh:datatype xsd:string ;
             sh:description "One or more 'tags' slot values (slot inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in a \"Block List\" collection." ;
             sh:order 15 ;
             sh:path schema1:additionalType ],
-        [ sh:datatype xsd:string ;
-            sh:description "Settings for the test harness for TestCase" ;
-            sh:minCount 1 ;
-            sh:order 11 ;
-            sh:path ttm:test_case_runner_settings ],
         [ sh:description "A unique identifier for a Test Entity" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 12 ;
-            sh:path schema1:identifier ],
-        [ sh:description "Deployment environment within which the associated TestSuite is run." ;
-            sh:in ( "dev" "ci" "test" "prod" ) ;
-            sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path ttm:test_env ],
-        [ sh:description "Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string." ;
-            sh:in ( "SME" "SMURF" "GitHubUserFeedback" "TACT" "BenchMark" "TranslatorTeam" "TestDataLocation" ) ;
-            sh:maxCount 1 ;
-            sh:order 7 ;
-            sh:path ttm:test_case_source ],
-        [ sh:class ttm:TestAsset ;
-            sh:description "One or more 'tags' slot values (inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in 'test_assets' slot (\"Block List\") collection." ;
-            sh:minCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 2 ;
-            sh:path ttm:test_assets ] ;
+            sh:path schema1:identifier ] ;
     sh:targetClass ttm:KnowledgeGraphNavigationTestCase .
 
 ttm:OneHopTestCase a sh:NodeShape ;
     sh:closed true ;
     sh:description "'One Hop' Knowledge Graph navigation integration test" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:description "Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string." ;
-            sh:in ( "SME" "SMURF" "GitHubUserFeedback" "TACT" "BenchMark" "TranslatorTeam" "TestDataLocation" ) ;
-            sh:maxCount 1 ;
-            sh:order 7 ;
-            sh:path ttm:test_case_source ],
-        [ sh:description "Type of TestCase query." ;
-            sh:in ( "treats" ) ;
+    sh:property [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
-            sh:order 1 ;
-            sh:path ttm:query_type ],
+            sh:order 9 ;
+            sh:path ttm:test_case_predicate_id ],
         [ sh:description "A template for a query, which can be used to generate a query for a test case.  note: the current enumerated values for this slot come from the Benchmarks repo config/benchmarks.json \"templates\" collection and refer to the \"name\" field of each template.  Templates themselves are currently stored in the config/[source_name]/templates directory." ;
             sh:in ( "ameliorates" "treats" "three_hop" "drug_treats_rare_disease" "drug-to-gene" ) ;
             sh:maxCount 1 ;
             sh:order 4 ;
             sh:path ttm:trapi_template ],
-        [ sh:description "The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX." ;
-            sh:in [ rdf:rest () ] ;
-            sh:order 5 ;
-            sh:path ttm:components ],
-        [ sh:description "Deployment environment within which the associated TestSuite is run." ;
-            sh:in ( "dev" "ci" "test" "prod" ) ;
+        [ sh:description "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)" ;
+            sh:in ( "AcceptanceTest" "BenchmarkTest" "QuantitativeTest" ) ;
             sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path ttm:test_env ],
+            sh:order 6 ;
+            sh:path ttm:test_case_objective ],
         [ sh:datatype xsd:string ;
+            sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 9 ;
-            sh:path ttm:test_case_predicate_id ],
+            sh:order 14 ;
+            sh:path schema1:description ],
         [ sh:maxCount 1 ;
             sh:order 10 ;
             sh:path ttm:test_case_input_id ],
-        [ sh:description "A unique identifier for a Test Entity" ;
+        [ sh:description "The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX." ;
+            sh:in [ rdf:rest () ] ;
+            sh:order 5 ;
+            sh:path ttm:components ],
+        [ sh:description "Type of TestCase query." ;
+            sh:in ( "treats" ) ;
             sh:maxCount 1 ;
+            sh:order 1 ;
+            sh:path ttm:query_type ],
+        [ sh:class ttm:Precondition ;
+            sh:nodeKind sh:IRI ;
+            sh:order 3 ;
+            sh:path ttm:preconditions ],
+        [ sh:class ttm:TestAsset ;
+            sh:description "One or more 'tags' slot values (inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in 'test_assets' slot (\"Block List\") collection." ;
             sh:minCount 1 ;
-            sh:order 12 ;
-            sh:path schema1:identifier ],
-        [ sh:description "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)" ;
-            sh:in ( "AcceptanceTest" "BenchmarkTest" "QuantitativeTest" ) ;
-            sh:maxCount 1 ;
-            sh:order 6 ;
-            sh:path ttm:test_case_objective ],
+            sh:nodeKind sh:IRI ;
+            sh:order 2 ;
+            sh:path ttm:test_assets ],
         [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
             sh:order 8 ;
             sh:path ttm:test_case_predicate_name ],
         [ sh:datatype xsd:string ;
             sh:description "One or more 'tags' slot values (slot inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in a \"Block List\" collection." ;
             sh:order 15 ;
             sh:path schema1:additionalType ],
         [ sh:datatype xsd:string ;
-            sh:description "A human-readable description for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:order 14 ;
-            sh:path schema1:description ],
+            sh:description "Settings for the test harness for TestCase" ;
+            sh:minCount 1 ;
+            sh:order 11 ;
+            sh:path ttm:test_case_runner_settings ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable name for a Test Entity" ;
             sh:maxCount 1 ;
             sh:order 13 ;
             sh:path schema1:name ],
-        [ sh:class ttm:TestAsset ;
-            sh:description "One or more 'tags' slot values (inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in 'test_assets' slot (\"Block List\") collection." ;
-            sh:minCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 2 ;
-            sh:path ttm:test_assets ],
-        [ sh:class ttm:Precondition ;
-            sh:nodeKind sh:IRI ;
-            sh:order 3 ;
-            sh:path ttm:preconditions ],
-        [ sh:datatype xsd:string ;
-            sh:description "Settings for the test harness for TestCase" ;
+        [ sh:description "Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string." ;
+            sh:in ( "SME" "SMURF" "GitHubUserFeedback" "TACT" "BenchMark" "TranslatorTeam" "TestDataLocation" ) ;
+            sh:maxCount 1 ;
+            sh:order 7 ;
+            sh:path ttm:test_case_source ],
+        [ sh:description "Deployment environment within which the associated TestSuite is run." ;
+            sh:in ( "dev" "ci" "test" "prod" ) ;
+            sh:maxCount 1 ;
+            sh:order 0 ;
+            sh:path ttm:test_env ],
+        [ sh:description "A unique identifier for a Test Entity" ;
+            sh:maxCount 1 ;
             sh:minCount 1 ;
-            sh:order 11 ;
-            sh:path ttm:test_case_runner_settings ] ;
+            sh:order 12 ;
+            sh:path schema1:identifier ] ;
     sh:targetClass ttm:OneHopTestCase .
 
 ttm:OneHopTestSuite a sh:NodeShape ;
     sh:closed true ;
     sh:description "Test case for testing the integrity of \"One Hop\" knowledge graph retrievals sensa legacy SRI_Testing harness." ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:string ;
-            sh:description "A human-readable description for a Test Entity" ;
+    sh:property [ sh:description "A unique identifier for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 6 ;
-            sh:path schema1:description ],
-        [ sh:datatype xsd:string ;
-            sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
-            sh:order 7 ;
-            sh:path schema1:additionalType ],
+            sh:minCount 1 ;
+            sh:order 4 ;
+            sh:path schema1:identifier ],
+        [ sh:class ttm:TestMetadata ;
+            sh:description "Test metadata describes the external provenance, cross-references and objectives for a given test." ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 0 ;
+            sh:path ttm:test_metadata ],
         [ sh:description "A Test persona describes the user or operational context of a given test." ;
             sh:in ( "All" "Clinical" "LookUp" "Mechanistic" ) ;
             sh:maxCount 1 ;
             sh:order 1 ;
             sh:path ttm:test_persona ],
-        [ sh:description "A unique identifier for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 4 ;
-            sh:path schema1:identifier ],
-        [ sh:datatype xsd:string ;
-            sh:description "A human-readable name for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:order 5 ;
-            sh:path schema1:name ],
         [ sh:class ttm:TestSuiteSpecification ;
             sh:description "Declarative specification of a Test Suite of Test Cases whose generation is deferred, (i.e. within a Test Runner) or whose creation is achieved by stream processing of an external data source." ;
             sh:maxCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 3 ;
             sh:path ttm:test_suite_specification ],
-        [ sh:class ttm:TestMetadata ;
-            sh:description "Test metadata describes the external provenance, cross-references and objectives for a given test." ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 0 ;
-            sh:path ttm:test_metadata ],
         [ sh:class ttm:TestCase ;
             sh:description "List of explicitly enumerated Test Cases." ;
             sh:nodeKind sh:IRI ;
             sh:order 2 ;
-            sh:path ttm:test_cases ] ;
+            sh:path ttm:test_cases ],
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
+            sh:order 7 ;
+            sh:path schema1:additionalType ],
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable description for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:order 6 ;
+            sh:path schema1:description ],
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable name for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:order 5 ;
+            sh:path schema1:name ] ;
     sh:targetClass ttm:OneHopTestSuite .
 
 ttm:QuantitativeTestCase a sh:NodeShape ;
     sh:closed true ;
     sh:description "Assumed additional model from Shervin's runner JSON here as an example.  This schema is not yet complete." ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:maxCount 1 ;
-            sh:order 10 ;
-            sh:path ttm:test_case_input_id ],
+    sh:property [ sh:description "Type of TestCase query." ;
+            sh:in ( "treats" ) ;
+            sh:maxCount 1 ;
+            sh:order 1 ;
+            sh:path ttm:query_type ],
+        [ sh:datatype xsd:string ;
+            sh:maxCount 1 ;
+            sh:order 8 ;
+            sh:path ttm:test_case_predicate_name ],
         [ sh:datatype xsd:string ;
             sh:description "One or more 'tags' slot values (slot inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in a \"Block List\" collection." ;
             sh:order 15 ;
             sh:path schema1:additionalType ],
-        [ sh:description "Deployment environment within which the associated TestSuite is run." ;
-            sh:in ( "dev" "ci" "test" "prod" ) ;
-            sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path ttm:test_env ],
-        [ sh:description "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)" ;
-            sh:in ( "AcceptanceTest" "BenchmarkTest" "QuantitativeTest" ) ;
-            sh:maxCount 1 ;
-            sh:order 6 ;
-            sh:path ttm:test_case_objective ],
-        [ sh:class ttm:Precondition ;
-            sh:nodeKind sh:IRI ;
-            sh:order 3 ;
-            sh:path ttm:preconditions ],
         [ sh:datatype xsd:string ;
-            sh:description "Settings for the test harness for TestCase" ;
-            sh:minCount 1 ;
-            sh:order 11 ;
-            sh:path ttm:test_case_runner_settings ],
-        [ sh:class ttm:TestAsset ;
-            sh:description "One or more 'tags' slot values (inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in 'test_assets' slot (\"Block List\") collection." ;
-            sh:minCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 2 ;
-            sh:path ttm:test_assets ],
+            sh:description "A human-readable description for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:order 14 ;
+            sh:path schema1:description ],
         [ sh:description "A template for a query, which can be used to generate a query for a test case.  note: the current enumerated values for this slot come from the Benchmarks repo config/benchmarks.json \"templates\" collection and refer to the \"name\" field of each template.  Templates themselves are currently stored in the config/[source_name]/templates directory." ;
             sh:in ( "ameliorates" "treats" "three_hop" "drug_treats_rare_disease" "drug-to-gene" ) ;
             sh:maxCount 1 ;
             sh:order 4 ;
             sh:path ttm:trapi_template ],
         [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
-            sh:order 8 ;
-            sh:path ttm:test_case_predicate_name ],
-        [ sh:datatype xsd:string ;
-            sh:description "A human-readable name for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:order 13 ;
-            sh:path schema1:name ],
+            sh:order 9 ;
+            sh:path ttm:test_case_predicate_id ],
+        [ sh:maxCount 1 ;
+            sh:order 10 ;
+            sh:path ttm:test_case_input_id ],
         [ sh:datatype xsd:string ;
-            sh:description "A human-readable description for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:order 14 ;
-            sh:path schema1:description ],
-        [ sh:description "Type of TestCase query." ;
-            sh:in ( "treats" ) ;
-            sh:maxCount 1 ;
-            sh:order 1 ;
-            sh:path ttm:query_type ],
+            sh:description "Settings for the test harness for TestCase" ;
+            sh:minCount 1 ;
+            sh:order 11 ;
+            sh:path ttm:test_case_runner_settings ],
         [ sh:description "A unique identifier for a Test Entity" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 12 ;
             sh:path schema1:identifier ],
-        [ sh:description "The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX." ;
-            sh:in [ rdf:rest () ] ;
-            sh:order 5 ;
-            sh:path ttm:components ],
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable name for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:order 13 ;
+            sh:path schema1:name ],
         [ sh:description "Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string." ;
             sh:in ( "SME" "SMURF" "GitHubUserFeedback" "TACT" "BenchMark" "TranslatorTeam" "TestDataLocation" ) ;
             sh:maxCount 1 ;
             sh:order 7 ;
             sh:path ttm:test_case_source ],
-        [ sh:datatype xsd:string ;
+        [ sh:description "The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX." ;
+            sh:in [ rdf:rest () ] ;
+            sh:order 5 ;
+            sh:path ttm:components ],
+        [ sh:description "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)" ;
+            sh:in ( "AcceptanceTest" "BenchmarkTest" "QuantitativeTest" ) ;
             sh:maxCount 1 ;
-            sh:order 9 ;
-            sh:path ttm:test_case_predicate_id ] ;
+            sh:order 6 ;
+            sh:path ttm:test_case_objective ],
+        [ sh:description "Deployment environment within which the associated TestSuite is run." ;
+            sh:in ( "dev" "ci" "test" "prod" ) ;
+            sh:maxCount 1 ;
+            sh:order 0 ;
+            sh:path ttm:test_env ],
+        [ sh:class ttm:TestAsset ;
+            sh:description "One or more 'tags' slot values (inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in 'test_assets' slot (\"Block List\") collection." ;
+            sh:minCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 2 ;
+            sh:path ttm:test_assets ],
+        [ sh:class ttm:Precondition ;
+            sh:nodeKind sh:IRI ;
+            sh:order 3 ;
+            sh:path ttm:preconditions ] ;
     sh:targetClass ttm:QuantitativeTestCase .
 
 ttm:StandardsComplianceTestSuite a sh:NodeShape ;
     sh:closed true ;
     sh:description "Test suite for testing Translator components against releases of standards like TRAPI and the Biolink Model." ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:string ;
-            sh:description "A human-readable description for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:order 6 ;
-            sh:path schema1:description ],
-        [ sh:description "A unique identifier for a Test Entity" ;
+    sh:property [ sh:description "A Test persona describes the user or operational context of a given test." ;
+            sh:in ( "All" "Clinical" "LookUp" "Mechanistic" ) ;
             sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 4 ;
-            sh:path schema1:identifier ],
-        [ sh:datatype xsd:string ;
-            sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
-            sh:order 7 ;
-            sh:path schema1:additionalType ],
+            sh:order 1 ;
+            sh:path ttm:test_persona ],
         [ sh:class ttm:TestMetadata ;
             sh:description "Test metadata describes the external provenance, cross-references and objectives for a given test." ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 0 ;
             sh:path ttm:test_metadata ],
-        [ sh:class ttm:TestSuiteSpecification ;
-            sh:description "Declarative specification of a Test Suite of Test Cases whose generation is deferred, (i.e. within a Test Runner) or whose creation is achieved by stream processing of an external data source." ;
+        [ sh:description "A unique identifier for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 3 ;
-            sh:path ttm:test_suite_specification ],
+            sh:minCount 1 ;
+            sh:order 4 ;
+            sh:path schema1:identifier ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable name for a Test Entity" ;
             sh:maxCount 1 ;
             sh:order 5 ;
             sh:path schema1:name ],
+        [ sh:class ttm:TestSuiteSpecification ;
+            sh:description "Declarative specification of a Test Suite of Test Cases whose generation is deferred, (i.e. within a Test Runner) or whose creation is achieved by stream processing of an external data source." ;
+            sh:maxCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 3 ;
+            sh:path ttm:test_suite_specification ],
         [ sh:class ttm:TestCase ;
             sh:description "List of explicitly enumerated Test Cases." ;
             sh:nodeKind sh:IRI ;
             sh:order 2 ;
             sh:path ttm:test_cases ],
-        [ sh:description "A Test persona describes the user or operational context of a given test." ;
-            sh:in ( "All" "Clinical" "LookUp" "Mechanistic" ) ;
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 1 ;
-            sh:path ttm:test_persona ] ;
+            sh:order 6 ;
+            sh:path schema1:description ],
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
+            sh:order 7 ;
+            sh:path schema1:additionalType ] ;
     sh:targetClass ttm:StandardsComplianceTestSuite .
 
 ttm:TestEdgeData a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents a single Biolink Model compliant instance of a subject-predicate-object edge that can be used for testing." ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:in ( "High" "Low" "NotApplicable" ) ;
-            sh:maxCount 1 ;
-            sh:order 12 ;
-            sh:path ttm:semantic_severity ],
-        [ sh:description "Specific Biolink Model association 'category' which applies to the test asset defined knowledge statement" ;
-            sh:maxCount 1 ;
-            sh:order 8 ;
-            sh:path ttm:association ],
-        [ sh:datatype xsd:boolean ;
-            sh:maxCount 1 ;
-            sh:order 14 ;
-            sh:path ttm:well_known ],
-        [ sh:datatype xsd:string ;
-            sh:description "The direction of the subject of the test asset predicate" ;
+    sh:property [ sh:datatype xsd:string ;
+            sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
             sh:order 20 ;
-            sh:path ttm:biolink_subject_direction_qualifier ],
-        [ sh:datatype xsd:string ;
+            sh:path schema1:description ],
+        [ sh:maxCount 1 ;
+            sh:order 3 ;
+            sh:path ttm:predicate_id ],
+        [ sh:maxCount 1 ;
+            sh:order 7 ;
+            sh:path ttm:output_category ],
+        [ sh:in ( "High" "Low" "NotApplicable" ) ;
             sh:maxCount 1 ;
-            sh:order 4 ;
-            sh:path ttm:predicate_name ],
-        [ sh:datatype xsd:string ;
+            sh:order 12 ;
+            sh:path ttm:semantic_severity ],
+        [ sh:description "A unique identifier for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 10 ;
-            sh:path ttm:expected_output ],
+            sh:minCount 1 ;
+            sh:order 18 ;
+            sh:path schema1:identifier ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable name for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 24 ;
+            sh:order 19 ;
             sh:path schema1:name ],
-        [ sh:datatype xsd:string ;
-            sh:description "A human-readable description for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:order 25 ;
-            sh:path schema1:description ],
-        [ sh:description "The qualified_predicate in Biolink model corresponding to the shorthand predicate name used in the test asset." ;
+        [ sh:description "Specific Biolink Model association 'category' which applies to the test asset defined knowledge statement" ;
             sh:maxCount 1 ;
-            sh:order 18 ;
-            sh:path ttm:biolink_qualified_predicate ],
+            sh:order 8 ;
+            sh:path ttm:association ],
         [ sh:datatype xsd:string ;
-            sh:description "One or more 'tags' slot values (inherited from TestEntity) should generally be defined to specify TestAsset membership in a \"Block List\" collection" ;
-            sh:order 26 ;
-            sh:path schema1:additionalType ],
+            sh:maxCount 1 ;
+            sh:order 6 ;
+            sh:path ttm:output_name ],
         [ sh:description "Document URL where original test source particulars are registered (e.g. Github repo)" ;
             sh:maxCount 1 ;
             sh:order 15 ;
             sh:path ttm:test_reference ],
-        [ sh:datatype xsd:string ;
-            sh:description "The aspect of the subject of the test asset predicate" ;
+        [ sh:datatype xsd:boolean ;
             sh:maxCount 1 ;
-            sh:order 19 ;
-            sh:path ttm:biolink_subject_aspect_qualifier ],
+            sh:order 13 ;
+            sh:path ttm:in_v1 ],
+        [ sh:datatype xsd:string ;
+            sh:description "One or more 'tags' slot values (inherited from TestEntity) should generally be defined to specify TestAsset membership in a \"Block List\" collection" ;
+            sh:order 21 ;
+            sh:path schema1:additionalType ],
         [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
             sh:order 1 ;
             sh:path ttm:input_name ],
-        [ sh:maxCount 1 ;
-            sh:order 3 ;
-            sh:path ttm:predicate_id ],
-        [ sh:maxCount 1 ;
-            sh:order 2 ;
-            sh:path ttm:input_category ],
-        [ sh:datatype xsd:string ;
-            sh:description "Settings for the test harness, e.g. \"inferred\"" ;
-            sh:minCount 1 ;
-            sh:order 16 ;
-            sh:path ttm:runner_settings ],
         [ sh:class ttm:Qualifier ;
             sh:description "Optional qualifiers which constrain to the test asset defined knowledge statement. Note that this field records such qualifier slots and values as tag=value pairs, where the tag is the Biolink Model qualifier slot named and the value is an acceptable (Biolink Model enum?) value of the said qualifier slot." ;
             sh:nodeKind sh:BlankNode ;
             sh:order 9 ;
             sh:path ttm:qualifiers ],
         [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
-            sh:order 6 ;
-            sh:path ttm:output_name ],
-        [ sh:datatype xsd:string ;
-            sh:description "The direction of the object of the test asset predicate" ;
-            sh:maxCount 1 ;
-            sh:order 22 ;
-            sh:path ttm:biolink_object_direction_qualifier ],
-        [ sh:datatype xsd:boolean ;
+            sh:order 10 ;
+            sh:path ttm:expected_output ],
+        [ sh:in ( "causes not treats" "TMKP" "category too generic" "contraindications" "chemical roles" "test_issue" ) ;
             sh:maxCount 1 ;
-            sh:order 13 ;
-            sh:path ttm:in_v1 ],
+            sh:order 11 ;
+            sh:path ttm:test_issue ],
         [ sh:maxCount 1 ;
             sh:order 5 ;
             sh:path ttm:output_id ],
-        [ sh:maxCount 1 ;
-            sh:order 7 ;
-            sh:path ttm:output_category ],
+        [ sh:datatype xsd:string ;
+            sh:maxCount 1 ;
+            sh:order 4 ;
+            sh:path ttm:predicate_name ],
+        [ sh:datatype xsd:string ;
+            sh:description "Settings for the test harness, e.g. \"inferred\"" ;
+            sh:minCount 1 ;
+            sh:order 16 ;
+            sh:path ttm:runner_settings ],
         [ sh:maxCount 1 ;
             sh:order 0 ;
             sh:path ttm:input_id ],
-        [ sh:datatype xsd:string ;
-            sh:description "The aspect of the object of the test asset predicate" ;
-            sh:maxCount 1 ;
-            sh:order 21 ;
-            sh:path ttm:biolink_object_aspect_qualifier ],
-        [ sh:in ( "causes not treats" "TMKP" "category too generic" "contraindications" "chemical roles" "test_issue" ) ;
+        [ sh:datatype xsd:boolean ;
             sh:maxCount 1 ;
-            sh:order 11 ;
-            sh:path ttm:test_issue ],
+            sh:order 14 ;
+            sh:path ttm:well_known ],
         [ sh:class ttm:TestMetadata ;
             sh:description "Test metadata describes the external provenance, cross-references and objectives for a given test." ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 17 ;
             sh:path ttm:test_metadata ],
-        [ sh:description "A unique identifier for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 23 ;
-            sh:path schema1:identifier ] ;
+        [ sh:maxCount 1 ;
+            sh:order 2 ;
+            sh:path ttm:input_category ] ;
     sh:targetClass ttm:TestEdgeData .
 
 ttm:TestOutput a sh:NodeShape ;
     sh:closed true ;
     sh:description "The output of a TestRunner run of one specific TestCase." ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:datatype xsd:string ;
-            sh:description "A human-readable description for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:order 4 ;
-            sh:path schema1:description ],
-        [ sh:datatype xsd:string ;
-            sh:description "A human-readable name for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:order 3 ;
-            sh:path schema1:name ],
-        [ sh:class ttm:TestResultPKSet ;
-            sh:description "Primary keys for a given ARA result set from a SmokeTest result for a given TestCase." ;
-            sh:nodeKind sh:IRI ;
-            sh:order 1 ;
-            sh:path ttm:pks ],
-        [ sh:datatype xsd:string ;
             sh:description "CURIE id of a TestCase registered in the system." ;
             sh:maxCount 1 ;
             sh:order 0 ;
             sh:path ttm:test_case_id ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
             sh:order 5 ;
             sh:path schema1:additionalType ],
         [ sh:description "A unique identifier for a Test Entity" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 2 ;
-            sh:path schema1:identifier ] ;
+            sh:path schema1:identifier ],
+        [ sh:class ttm:TestResultPKSet ;
+            sh:description "Primary keys for a given ARA result set from a SmokeTest result for a given TestCase." ;
+            sh:nodeKind sh:IRI ;
+            sh:order 1 ;
+            sh:path ttm:pks ],
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable description for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:order 4 ;
+            sh:path schema1:description ],
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable name for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:order 3 ;
+            sh:path schema1:name ] ;
     sh:targetClass ttm:TestOutput .
 
 ttm:TestRunSession a sh:NodeShape ;
     sh:closed true ;
     sh:description "A single invocation of a TestRunner." ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:description "A unique identifier for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 4 ;
-            sh:path schema1:identifier ],
-        [ sh:datatype xsd:string ;
-            sh:description "A human-readable name for a Test Entity" ;
+    sh:property [ sh:class ttm:TestCaseResult ;
+            sh:description "One or more instances of TestCaseResult." ;
+            sh:nodeKind sh:IRI ;
+            sh:order 2 ;
+            sh:path ttm:test_case_results ],
+        [ sh:datatype xsd:dateTime ;
+            sh:description "Date time when a given entity was created." ;
             sh:maxCount 1 ;
-            sh:order 5 ;
-            sh:path schema1:name ],
+            sh:order 3 ;
+            sh:path ttm:timestamp ],
         [ sh:datatype xsd:string ;
             sh:description "Global system name of a TestRunner." ;
             sh:maxCount 1 ;
             sh:order 0 ;
             sh:path ttm:test_runner_name ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
             sh:order 6 ;
             sh:path schema1:description ],
-        [ sh:datatype xsd:string ;
-            sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
-            sh:order 7 ;
-            sh:path schema1:additionalType ],
-        [ sh:datatype xsd:dateTime ;
-            sh:description "Date time when a given entity was created." ;
+        [ sh:description "A unique identifier for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 3 ;
-            sh:path ttm:timestamp ],
+            sh:minCount 1 ;
+            sh:order 4 ;
+            sh:path schema1:identifier ],
         [ sh:class ttm:TestEntity ;
             sh:description "Different TestRunners may expect specific kinds of TestEntity as input. These 'test_entities' one or more instances of TestAsset, TestCase or TestSuite." ;
             sh:nodeKind sh:IRI ;
             sh:order 1 ;
             sh:path ttm:test_entities ],
-        [ sh:class ttm:TestCaseResult ;
-            sh:description "One or more instances of TestCaseResult." ;
-            sh:nodeKind sh:IRI ;
-            sh:order 2 ;
-            sh:path ttm:test_case_results ] ;
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
+            sh:order 7 ;
+            sh:path schema1:additionalType ],
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable name for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:order 5 ;
+            sh:path schema1:name ] ;
     sh:targetClass ttm:TestRunSession .
 
 ttm:TestRunnerConfiguration a sh:NodeShape ;
     sh:closed true ;
     sh:description "General configuration parameters and test data input  for a single invocation of a TestRunner." ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:description "A unique identifier for a Test Entity" ;
+    sh:property [ sh:datatype xsd:string ;
+            sh:description "One or more 'tags' slot values (slot inherited from TestEntity)  should generally identify the TestRunner(s) using this configuration." ;
+            sh:order 4 ;
+            sh:path schema1:additionalType ],
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable name for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:order 2 ;
+            sh:path schema1:name ],
+        [ sh:description "A unique identifier for a Test Entity" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 1 ;
             sh:path schema1:identifier ],
         [ sh:class ttm:TestEntityParameter ;
             sh:description "Parameters for TestRunnerConfiguration that inform the TestHarness and TestRunners about the general characteristics of a test run." ;
             sh:nodeKind sh:BlankNode ;
             sh:order 0 ;
             sh:path ttm:test_run_parameters ],
         [ sh:datatype xsd:string ;
-            sh:description "A human-readable name for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:order 2 ;
-            sh:path schema1:name ],
-        [ sh:datatype xsd:string ;
             sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
             sh:order 3 ;
-            sh:path schema1:description ],
-        [ sh:datatype xsd:string ;
-            sh:description "One or more 'tags' slot values (slot inherited from TestEntity)  should generally identify the TestRunner(s) using this configuration." ;
-            sh:order 4 ;
-            sh:path schema1:additionalType ] ;
+            sh:path schema1:description ] ;
     sh:targetClass ttm:TestRunnerConfiguration .
 
 ttm:TestSuite a sh:NodeShape ;
     sh:closed true ;
     sh:description "Specification of a set of Test Cases, one of either with a static list of 'test_cases' or a dynamic 'test_suite_specification' slot values. Note: at least one slot or the other, but generally not both(?) needs to be present." ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:description "A Test persona describes the user or operational context of a given test." ;
-            sh:in ( "All" "Clinical" "LookUp" "Mechanistic" ) ;
+    sh:property [ sh:datatype xsd:string ;
+            sh:description "A human-readable name for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 1 ;
-            sh:path ttm:test_persona ],
-        [ sh:class ttm:TestSuiteSpecification ;
-            sh:description "Declarative specification of a Test Suite of Test Cases whose generation is deferred, (i.e. within a Test Runner) or whose creation is achieved by stream processing of an external data source." ;
+            sh:order 5 ;
+            sh:path schema1:name ],
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
+            sh:order 7 ;
+            sh:path schema1:additionalType ],
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 3 ;
-            sh:path ttm:test_suite_specification ],
+            sh:order 6 ;
+            sh:path schema1:description ],
         [ sh:description "A unique identifier for a Test Entity" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 4 ;
             sh:path schema1:identifier ],
+        [ sh:description "A Test persona describes the user or operational context of a given test." ;
+            sh:in ( "All" "Clinical" "LookUp" "Mechanistic" ) ;
+            sh:maxCount 1 ;
+            sh:order 1 ;
+            sh:path ttm:test_persona ],
         [ sh:class ttm:TestCase ;
             sh:description "List of explicitly enumerated Test Cases." ;
             sh:nodeKind sh:IRI ;
             sh:order 2 ;
             sh:path ttm:test_cases ],
         [ sh:class ttm:TestMetadata ;
             sh:description "Test metadata describes the external provenance, cross-references and objectives for a given test." ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 0 ;
             sh:path ttm:test_metadata ],
-        [ sh:datatype xsd:string ;
-            sh:description "A human-readable description for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:order 6 ;
-            sh:path schema1:description ],
-        [ sh:datatype xsd:string ;
-            sh:description "A human-readable name for a Test Entity" ;
+        [ sh:class ttm:TestSuiteSpecification ;
+            sh:description "Declarative specification of a Test Suite of Test Cases whose generation is deferred, (i.e. within a Test Runner) or whose creation is achieved by stream processing of an external data source." ;
             sh:maxCount 1 ;
-            sh:order 5 ;
-            sh:path schema1:name ],
-        [ sh:datatype xsd:string ;
-            sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
-            sh:order 7 ;
-            sh:path schema1:additionalType ] ;
+            sh:nodeKind sh:IRI ;
+            sh:order 3 ;
+            sh:path ttm:test_suite_specification ] ;
     sh:targetClass ttm:TestSuite .
 
 ttm:AcceptanceTestAsset a sh:NodeShape ;
     sh:closed true ;
     sh:description "Model derived from Jenn's test asset design and Shervin's runner JSON here as an example." ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:class ttm:Qualifier ;
             sh:description "Optional qualifiers which constrain to the test asset defined knowledge statement. Note that this field records such qualifier slots and values as tag=value pairs, where the tag is the Biolink Model qualifier slot named and the value is an acceptable (Biolink Model enum?) value of the said qualifier slot." ;
             sh:nodeKind sh:BlankNode ;
             sh:order 19 ;
             sh:path ttm:qualifiers ],
-        [ sh:in ( "High" "Low" "NotApplicable" ) ;
-            sh:maxCount 1 ;
-            sh:order 22 ;
-            sh:path ttm:semantic_severity ],
-        [ sh:datatype xsd:boolean ;
-            sh:maxCount 1 ;
-            sh:order 23 ;
-            sh:path ttm:in_v1 ],
-        [ sh:datatype xsd:boolean ;
-            sh:maxCount 1 ;
-            sh:order 24 ;
-            sh:path ttm:well_known ],
-        [ sh:datatype xsd:string ;
-            sh:description "The direction of the object of the test asset predicate" ;
+        [ sh:description "The deployment environment within which this test must pass." ;
+            sh:in ( "dev" "ci" "test" "prod" ) ;
             sh:maxCount 1 ;
-            sh:order 32 ;
-            sh:path ttm:biolink_object_direction_qualifier ],
+            sh:order 1 ;
+            sh:path ttm:must_pass_environment ],
         [ sh:description "The direction of the expected query result triple" ;
             sh:in ( "increased" "decreased" ) ;
             sh:maxCount 1 ;
             sh:order 4 ;
             sh:path ttm:direction ],
+        [ sh:in ( "causes not treats" "TMKP" "category too generic" "contraindications" "chemical roles" "test_issue" ) ;
+            sh:maxCount 1 ;
+            sh:order 21 ;
+            sh:path ttm:test_issue ],
         [ sh:datatype xsd:string ;
-            sh:description "The object of the core triple to be tested" ;
             sh:maxCount 1 ;
-            sh:order 3 ;
-            sh:path ttm:string_entry ],
+            sh:order 11 ;
+            sh:path ttm:input_name ],
+        [ sh:datatype xsd:string ;
+            sh:description "Settings for the test harness, e.g. \"inferred\"" ;
+            sh:minCount 1 ;
+            sh:order 26 ;
+            sh:path ttm:runner_settings ],
         [ sh:description "A unique identifier for a Test Entity" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
-            sh:order 33 ;
+            sh:order 28 ;
             sh:path schema1:identifier ],
-        [ sh:datatype xsd:string ;
-            sh:maxCount 1 ;
-            sh:order 20 ;
-            sh:path ttm:expected_output ],
-        [ sh:datatype xsd:string ;
-            sh:description "The notes of the query" ;
-            sh:maxCount 1 ;
-            sh:order 9 ;
-            sh:path ttm:notes ],
-        [ sh:datatype xsd:string ;
-            sh:maxCount 1 ;
-            sh:order 14 ;
-            sh:path ttm:predicate_name ],
-        [ sh:datatype xsd:string ;
-            sh:maxCount 1 ;
-            sh:order 16 ;
-            sh:path ttm:output_name ],
         [ sh:maxCount 1 ;
             sh:order 17 ;
             sh:path ttm:output_category ],
         [ sh:maxCount 1 ;
-            sh:order 13 ;
-            sh:path ttm:predicate_id ],
+            sh:order 10 ;
+            sh:path ttm:input_id ],
+        [ sh:class ttm:TestMetadata ;
+            sh:description "Test metadata describes the external provenance, cross-references and objectives for a given test." ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 27 ;
+            sh:path ttm:test_metadata ],
+        [ sh:datatype xsd:boolean ;
+            sh:maxCount 1 ;
+            sh:order 23 ;
+            sh:path ttm:in_v1 ],
+        [ sh:maxCount 1 ;
+            sh:order 12 ;
+            sh:path ttm:input_category ],
+        [ sh:datatype xsd:integer ;
+            sh:description "The answer must return in these many results" ;
+            sh:maxCount 1 ;
+            sh:order 7 ;
+            sh:path ttm:top_level ],
         [ sh:maxCount 1 ;
             sh:order 15 ;
             sh:path ttm:output_id ],
         [ sh:datatype xsd:string ;
+            sh:maxCount 1 ;
+            sh:order 14 ;
+            sh:path ttm:predicate_name ],
+        [ sh:in ( "High" "Low" "NotApplicable" ) ;
+            sh:maxCount 1 ;
+            sh:order 22 ;
+            sh:path ttm:semantic_severity ],
+        [ sh:datatype xsd:string ;
             sh:description "One or more 'tags' slot values (inherited from TestEntity) should generally be defined to specify TestAsset membership in a \"Block List\" collection" ;
-            sh:order 36 ;
+            sh:order 31 ;
             sh:path schema1:additionalType ],
-        [ sh:description "The deployment environment within which this test must pass." ;
-            sh:in ( "dev" "ci" "test" "prod" ) ;
-            sh:maxCount 1 ;
-            sh:order 1 ;
-            sh:path ttm:must_pass_environment ],
-        [ sh:description "Document URL where original test source particulars are registered (e.g. Github repo)" ;
+        [ sh:description "The expected result of the query" ;
+            sh:in ( "include_good" "exclude_bad" ) ;
             sh:maxCount 1 ;
-            sh:order 25 ;
-            sh:path ttm:test_reference ],
-        [ sh:datatype xsd:date ;
-            sh:description "The date by which this test must pass" ;
+            sh:order 6 ;
+            sh:path ttm:expected_result ],
+        [ sh:datatype xsd:string ;
+            sh:description "An answer that is returned from the test case, note: this must be combined with the expected_result to form a complete answer.  It might make sense to couple these in their own object instead of strictly sticking to the flat schema introduced by the spreadsheet here: https://docs.google.com/spreadsheets/d/1yj7zIchFeVl1OHqL_kE_pqvzNLmGml_FLbHDs-8Yvig/edit#gid=0" ;
             sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path ttm:must_pass_date ],
+            sh:order 5 ;
+            sh:path ttm:answer_informal_concept ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 35 ;
+            sh:order 30 ;
             sh:path schema1:description ],
         [ sh:datatype xsd:string ;
-            sh:description "A human-readable name for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 34 ;
-            sh:path schema1:name ],
-        [ sh:class ttm:TestMetadata ;
-            sh:description "Test metadata describes the external provenance, cross-references and objectives for a given test." ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 27 ;
-            sh:path ttm:test_metadata ],
+            sh:order 20 ;
+            sh:path ttm:expected_output ],
         [ sh:description "The node of the (templated) TRAPI query to replace" ;
             sh:in ( "subject" "object" ) ;
             sh:maxCount 1 ;
             sh:order 8 ;
             sh:path ttm:query_node ],
         [ sh:datatype xsd:string ;
+            sh:description "The object of the core triple to be tested" ;
+            sh:maxCount 1 ;
+            sh:order 3 ;
+            sh:path ttm:string_entry ],
+        [ sh:datatype xsd:string ;
             sh:description "The full human-readable scientific question a SME would ask, which is encoded into the test asset." ;
             sh:maxCount 1 ;
             sh:order 2 ;
             sh:path ttm:scientific_question ],
-        [ sh:datatype xsd:string ;
-            sh:description "The aspect of the subject of the test asset predicate" ;
+        [ sh:description "Document URL where original test source particulars are registered (e.g. Github repo)" ;
             sh:maxCount 1 ;
-            sh:order 29 ;
-            sh:path ttm:biolink_subject_aspect_qualifier ],
-        [ sh:in ( "causes not treats" "TMKP" "category too generic" "contraindications" "chemical roles" "test_issue" ) ;
+            sh:order 25 ;
+            sh:path ttm:test_reference ],
+        [ sh:datatype xsd:date ;
+            sh:description "The date by which this test must pass" ;
             sh:maxCount 1 ;
-            sh:order 21 ;
-            sh:path ttm:test_issue ],
-        [ sh:maxCount 1 ;
-            sh:order 10 ;
-            sh:path ttm:input_id ],
+            sh:order 0 ;
+            sh:path ttm:must_pass_date ],
         [ sh:datatype xsd:string ;
+            sh:description "The notes of the query" ;
             sh:maxCount 1 ;
-            sh:order 11 ;
-            sh:path ttm:input_name ],
-        [ sh:description "The expected result of the query" ;
-            sh:in ( "include_good" "exclude_bad" ) ;
-            sh:maxCount 1 ;
-            sh:order 6 ;
-            sh:path ttm:expected_result ],
-        [ sh:datatype xsd:string ;
-            sh:description "Settings for the test harness, e.g. \"inferred\"" ;
-            sh:minCount 1 ;
-            sh:order 26 ;
-            sh:path ttm:runner_settings ],
-        [ sh:datatype xsd:integer ;
-            sh:description "The answer must return in these many results" ;
+            sh:order 9 ;
+            sh:path ttm:notes ],
+        [ sh:datatype xsd:boolean ;
             sh:maxCount 1 ;
-            sh:order 7 ;
-            sh:path ttm:top_level ],
+            sh:order 24 ;
+            sh:path ttm:well_known ],
         [ sh:datatype xsd:string ;
-            sh:description "The direction of the subject of the test asset predicate" ;
+            sh:description "A human-readable name for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 30 ;
-            sh:path ttm:biolink_subject_direction_qualifier ],
-        [ sh:maxCount 1 ;
-            sh:order 12 ;
-            sh:path ttm:input_category ],
+            sh:order 29 ;
+            sh:path schema1:name ],
         [ sh:datatype xsd:string ;
-            sh:description "The aspect of the object of the test asset predicate" ;
-            sh:maxCount 1 ;
-            sh:order 31 ;
-            sh:path ttm:biolink_object_aspect_qualifier ],
-        [ sh:description "The qualified_predicate in Biolink model corresponding to the shorthand predicate name used in the test asset." ;
             sh:maxCount 1 ;
-            sh:order 28 ;
-            sh:path ttm:biolink_qualified_predicate ],
+            sh:order 16 ;
+            sh:path ttm:output_name ],
         [ sh:description "Specific Biolink Model association 'category' which applies to the test asset defined knowledge statement" ;
             sh:maxCount 1 ;
             sh:order 18 ;
             sh:path ttm:association ],
-        [ sh:datatype xsd:string ;
-            sh:description "An answer that is returned from the test case, note: this must be combined with the expected_result to form a complete answer.  It might make sense to couple these in their own object instead of strictly sticking to the flat schema introduced by the spreadsheet here: https://docs.google.com/spreadsheets/d/1yj7zIchFeVl1OHqL_kE_pqvzNLmGml_FLbHDs-8Yvig/edit#gid=0" ;
-            sh:maxCount 1 ;
-            sh:order 5 ;
-            sh:path ttm:answer_informal_concept ] ;
+        [ sh:maxCount 1 ;
+            sh:order 13 ;
+            sh:path ttm:predicate_id ] ;
     sh:targetClass ttm:AcceptanceTestAsset .
 
 ttm:TestCaseResult a sh:NodeShape ;
     sh:closed true ;
     sh:description "The outcome of a TestRunner run of one specific TestCase." ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:class ttm:TestCase ;
-            sh:description "Slot referencing a single TestCase." ;
+    sh:property [ sh:datatype xsd:string ;
+            sh:description "A human-readable name for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 1 ;
-            sh:path ttm:test_case ],
-        [ sh:datatype xsd:string ;
-            sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
-            sh:order 6 ;
-            sh:path schema1:additionalType ],
+            sh:order 4 ;
+            sh:path schema1:name ],
+        [ sh:description "Encoded result of a single test run of a given test case" ;
+            sh:in ( "test_passed" "test_failed" "test_skipped" ) ;
+            sh:maxCount 1 ;
+            sh:order 2 ;
+            sh:path ttm:test_case_result ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
             sh:order 5 ;
             sh:path schema1:description ],
         [ sh:description "CURIE id of a TestSuite registered in the system." ;
             sh:maxCount 1 ;
             sh:order 0 ;
             sh:path ttm:test_suite_id ],
-        [ sh:description "Encoded result of a single test run of a given test case" ;
-            sh:in ( "test_passed" "test_failed" "test_skipped" ) ;
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
+            sh:order 6 ;
+            sh:path schema1:additionalType ],
+        [ sh:class ttm:TestCase ;
+            sh:description "Slot referencing a single TestCase." ;
             sh:maxCount 1 ;
-            sh:order 2 ;
-            sh:path ttm:test_case_result ],
+            sh:nodeKind sh:IRI ;
+            sh:order 1 ;
+            sh:path ttm:test_case ],
         [ sh:description "A unique identifier for a Test Entity" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 3 ;
-            sh:path schema1:identifier ],
-        [ sh:datatype xsd:string ;
-            sh:description "A human-readable name for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:order 4 ;
-            sh:path schema1:name ] ;
+            sh:path schema1:identifier ] ;
     sh:targetClass ttm:TestCaseResult .
 
 ttm:TestEntity a sh:NodeShape ;
     sh:closed false ;
     sh:description "Abstract global 'identification' class shared as a parent with all major model classes within the data model for Translator testing." ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:string ;
-            sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
-            sh:order 3 ;
-            sh:path schema1:additionalType ],
+    sh:property [ sh:description "A unique identifier for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:order 0 ;
+            sh:path schema1:identifier ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable name for a Test Entity" ;
             sh:maxCount 1 ;
             sh:order 1 ;
             sh:path schema1:name ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
             sh:order 2 ;
             sh:path schema1:description ],
-        [ sh:description "A unique identifier for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path schema1:identifier ] ;
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
+            sh:order 3 ;
+            sh:path schema1:additionalType ] ;
     sh:targetClass ttm:TestEntity .
 
 ttm:TestResultPKSet a sh:NodeShape ;
     sh:closed true ;
     sh:description "Primary keys for a given ARA result set from a SmokeTest result for a given TestCase." ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:string ;
-            sh:description "A human-readable description for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:order 9 ;
-            sh:path schema1:description ],
-        [ sh:description "A unique identifier for a Test Entity" ;
+    sh:property [ sh:description "A unique identifier for a Test Entity" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 7 ;
             sh:path schema1:identifier ],
         [ sh:datatype xsd:string ;
+            sh:maxCount 1 ;
+            sh:order 0 ;
+            sh:path ttm:parent_pk ],
+        [ sh:datatype xsd:string ;
             sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
             sh:order 10 ;
             sh:path schema1:additionalType ],
         [ sh:datatype xsd:string ;
+            sh:description "A human-readable name for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 4 ;
-            sh:path ttm:unsecret ],
+            sh:order 8 ;
+            sh:path schema1:name ],
+        [ sh:datatype xsd:string ;
+            sh:maxCount 1 ;
+            sh:order 2 ;
+            sh:path ttm:aragorn ],
         [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
             sh:order 6 ;
             sh:path ttm:improving ],
         [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
-            sh:order 5 ;
-            sh:path ttm:bte ],
+            sh:order 3 ;
+            sh:path ttm:arax ],
         [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
             sh:order 1 ;
             sh:path ttm:merged_pk ],
         [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
-            sh:order 2 ;
-            sh:path ttm:aragorn ],
-        [ sh:datatype xsd:string ;
-            sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path ttm:parent_pk ],
+            sh:order 5 ;
+            sh:path ttm:bte ],
         [ sh:datatype xsd:string ;
+            sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 3 ;
-            sh:path ttm:arax ],
+            sh:order 9 ;
+            sh:path schema1:description ],
         [ sh:datatype xsd:string ;
-            sh:description "A human-readable name for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 8 ;
-            sh:path schema1:name ] ;
+            sh:order 4 ;
+            sh:path ttm:unsecret ] ;
     sh:targetClass ttm:TestResultPKSet .
 
 ttm:TestEntityParameter a sh:NodeShape ;
     sh:closed true ;
     sh:description "A single 'tag = value' pair (where 'value' is a simple string)." ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:datatype xsd:string ;
-            sh:description "Name of a TestParameter." ;
-            sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path ttm:parameter ],
-        [ sh:datatype xsd:string ;
             sh:description "(String) value of a TestParameter." ;
             sh:maxCount 1 ;
             sh:order 1 ;
-            sh:path ttm:value ] ;
+            sh:path ttm:value ],
+        [ sh:datatype xsd:string ;
+            sh:description "Name of a TestParameter." ;
+            sh:maxCount 1 ;
+            sh:order 0 ;
+            sh:path ttm:parameter ] ;
     sh:targetClass ttm:TestEntityParameter .
 
 ttm:Qualifier a sh:NodeShape ;
     sh:closed true ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:datatype xsd:string ;
             sh:description "The 'value' of should be a suitable value generally drawn from an applicable Biolink Model (\"Enum\") value set of the specified Qualifier." ;
@@ -1161,307 +1113,283 @@
             sh:path ttm:parameter ] ;
     sh:targetClass ttm:Qualifier .
 
 ttm:TestSuiteSpecification a sh:NodeShape ;
     sh:closed true ;
     sh:description "Parameters for a Test Case instances either dynamically generated from some external source of Test Assets." ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:description "File format of test entity data (e.g. TSV, YAML or JSON)" ;
-            sh:in ( "TSV" "YAML" "JSON" ) ;
+    sh:property [ sh:description "A unique identifier for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 1 ;
-            sh:path ttm:test_data_file_format ],
+            sh:minCount 1 ;
+            sh:order 2 ;
+            sh:path schema1:identifier ],
         [ sh:datatype xsd:string ;
-            sh:description "A human-readable description for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:order 4 ;
-            sh:path schema1:description ],
-        [ sh:description "An web accessible file resource link to test entity data (e.g. a web accessible text file of Test Asset entries)" ;
+            sh:description "A human-readable name for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path ttm:test_data_file_locator ],
+            sh:order 3 ;
+            sh:path schema1:name ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
             sh:order 5 ;
             sh:path schema1:additionalType ],
         [ sh:datatype xsd:string ;
-            sh:description "A human-readable name for a Test Entity" ;
+            sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 3 ;
-            sh:path schema1:name ],
-        [ sh:description "A unique identifier for a Test Entity" ;
+            sh:order 4 ;
+            sh:path schema1:description ],
+        [ sh:description "File format of test entity data (e.g. TSV, YAML or JSON)" ;
+            sh:in ( "TSV" "YAML" "JSON" ) ;
             sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 2 ;
-            sh:path schema1:identifier ] ;
+            sh:order 1 ;
+            sh:path ttm:test_data_file_format ],
+        [ sh:description "An web accessible file resource link to test entity data (e.g. a web accessible text file of Test Asset entries)" ;
+            sh:maxCount 1 ;
+            sh:order 0 ;
+            sh:path ttm:test_data_file_locator ] ;
     sh:targetClass ttm:TestSuiteSpecification .
 
 ttm:TestAsset a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents a Test Asset, which is a single specific instance of TestCase-agnostic semantic parameters representing the specification of a Translator test target with inputs and (expected) outputs." ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:string ;
-            sh:description "One or more 'tags' slot values (inherited from TestEntity) should generally be defined to specify TestAsset membership in a \"Block List\" collection" ;
-            sh:order 26 ;
-            sh:path schema1:additionalType ],
+    sh:property [ sh:description "Document URL where original test source particulars are registered (e.g. Github repo)" ;
+            sh:maxCount 1 ;
+            sh:order 15 ;
+            sh:path ttm:test_reference ],
         [ sh:maxCount 1 ;
-            sh:order 7 ;
-            sh:path ttm:output_category ],
+            sh:order 2 ;
+            sh:path ttm:input_category ],
         [ sh:datatype xsd:string ;
-            sh:description "The direction of the subject of the test asset predicate" ;
+            sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
             sh:order 20 ;
-            sh:path ttm:biolink_subject_direction_qualifier ],
-        [ sh:datatype xsd:string ;
-            sh:description "The direction of the object of the test asset predicate" ;
-            sh:maxCount 1 ;
-            sh:order 22 ;
-            sh:path ttm:biolink_object_direction_qualifier ],
-        [ sh:class ttm:TestMetadata ;
-            sh:description "Test metadata describes the external provenance, cross-references and objectives for a given test." ;
+            sh:path schema1:description ],
+        [ sh:in ( "High" "Low" "NotApplicable" ) ;
             sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 17 ;
-            sh:path ttm:test_metadata ],
-        [ sh:maxCount 1 ;
-            sh:order 2 ;
-            sh:path ttm:input_category ],
-        [ sh:maxCount 1 ;
-            sh:order 5 ;
-            sh:path ttm:output_id ],
+            sh:order 12 ;
+            sh:path ttm:semantic_severity ],
         [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
-            sh:order 6 ;
-            sh:path ttm:output_name ],
+            sh:order 4 ;
+            sh:path ttm:predicate_name ],
         [ sh:description "A unique identifier for a Test Entity" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
-            sh:order 23 ;
+            sh:order 18 ;
             sh:path schema1:identifier ],
         [ sh:datatype xsd:string ;
-            sh:maxCount 1 ;
-            sh:order 10 ;
-            sh:path ttm:expected_output ],
-        [ sh:class ttm:Qualifier ;
-            sh:description "Optional qualifiers which constrain to the test asset defined knowledge statement. Note that this field records such qualifier slots and values as tag=value pairs, where the tag is the Biolink Model qualifier slot named and the value is an acceptable (Biolink Model enum?) value of the said qualifier slot." ;
-            sh:nodeKind sh:BlankNode ;
-            sh:order 9 ;
-            sh:path ttm:qualifiers ],
-        [ sh:maxCount 1 ;
-            sh:order 3 ;
-            sh:path ttm:predicate_id ],
-        [ sh:datatype xsd:string ;
-            sh:description "The aspect of the subject of the test asset predicate" ;
+            sh:description "A human-readable name for a Test Entity" ;
             sh:maxCount 1 ;
             sh:order 19 ;
-            sh:path ttm:biolink_subject_aspect_qualifier ],
+            sh:path schema1:name ],
         [ sh:datatype xsd:string ;
-            sh:description "A human-readable name for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 24 ;
-            sh:path schema1:name ],
+            sh:order 1 ;
+            sh:path ttm:input_name ],
         [ sh:datatype xsd:string ;
-            sh:description "The aspect of the object of the test asset predicate" ;
             sh:maxCount 1 ;
-            sh:order 21 ;
-            sh:path ttm:biolink_object_aspect_qualifier ],
+            sh:order 6 ;
+            sh:path ttm:output_name ],
         [ sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path ttm:input_id ],
-        [ sh:description "Document URL where original test source particulars are registered (e.g. Github repo)" ;
+            sh:order 7 ;
+            sh:path ttm:output_category ],
+        [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
-            sh:order 15 ;
-            sh:path ttm:test_reference ],
+            sh:order 10 ;
+            sh:path ttm:expected_output ],
         [ sh:datatype xsd:boolean ;
             sh:maxCount 1 ;
             sh:order 13 ;
             sh:path ttm:in_v1 ],
+        [ sh:datatype xsd:boolean ;
+            sh:maxCount 1 ;
+            sh:order 14 ;
+            sh:path ttm:well_known ],
         [ sh:datatype xsd:string ;
             sh:description "Settings for the test harness, e.g. \"inferred\"" ;
             sh:minCount 1 ;
             sh:order 16 ;
             sh:path ttm:runner_settings ],
-        [ sh:datatype xsd:string ;
-            sh:maxCount 1 ;
-            sh:order 4 ;
-            sh:path ttm:predicate_name ],
-        [ sh:in ( "causes not treats" "TMKP" "category too generic" "contraindications" "chemical roles" "test_issue" ) ;
-            sh:maxCount 1 ;
-            sh:order 11 ;
-            sh:path ttm:test_issue ],
         [ sh:description "Specific Biolink Model association 'category' which applies to the test asset defined knowledge statement" ;
             sh:maxCount 1 ;
             sh:order 8 ;
             sh:path ttm:association ],
-        [ sh:description "The qualified_predicate in Biolink model corresponding to the shorthand predicate name used in the test asset." ;
-            sh:maxCount 1 ;
-            sh:order 18 ;
-            sh:path ttm:biolink_qualified_predicate ],
-        [ sh:datatype xsd:string ;
-            sh:maxCount 1 ;
-            sh:order 1 ;
-            sh:path ttm:input_name ],
-        [ sh:datatype xsd:boolean ;
-            sh:maxCount 1 ;
-            sh:order 14 ;
-            sh:path ttm:well_known ],
-        [ sh:in ( "High" "Low" "NotApplicable" ) ;
+        [ sh:maxCount 1 ;
+            sh:order 0 ;
+            sh:path ttm:input_id ],
+        [ sh:class ttm:Qualifier ;
+            sh:description "Optional qualifiers which constrain to the test asset defined knowledge statement. Note that this field records such qualifier slots and values as tag=value pairs, where the tag is the Biolink Model qualifier slot named and the value is an acceptable (Biolink Model enum?) value of the said qualifier slot." ;
+            sh:nodeKind sh:BlankNode ;
+            sh:order 9 ;
+            sh:path ttm:qualifiers ],
+        [ sh:class ttm:TestMetadata ;
+            sh:description "Test metadata describes the external provenance, cross-references and objectives for a given test." ;
             sh:maxCount 1 ;
-            sh:order 12 ;
-            sh:path ttm:semantic_severity ],
+            sh:minCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 17 ;
+            sh:path ttm:test_metadata ],
+        [ sh:maxCount 1 ;
+            sh:order 3 ;
+            sh:path ttm:predicate_id ],
+        [ sh:maxCount 1 ;
+            sh:order 5 ;
+            sh:path ttm:output_id ],
         [ sh:datatype xsd:string ;
-            sh:description "A human-readable description for a Test Entity" ;
+            sh:description "One or more 'tags' slot values (inherited from TestEntity) should generally be defined to specify TestAsset membership in a \"Block List\" collection" ;
+            sh:order 21 ;
+            sh:path schema1:additionalType ],
+        [ sh:in ( "causes not treats" "TMKP" "category too generic" "contraindications" "chemical roles" "test_issue" ) ;
             sh:maxCount 1 ;
-            sh:order 25 ;
-            sh:path schema1:description ] ;
+            sh:order 11 ;
+            sh:path ttm:test_issue ] ;
     sh:targetClass ttm:TestAsset .
 
 ttm:TestCase a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents a single enumerated instance of Test Case, derived from a  given collection of one or more TestAsset instances (the value of the 'test_assets' slot) which define the 'inputs' and 'outputs' of the TestCase, used to probe a particular test condition." ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:string ;
+    sh:property [ sh:description "The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX." ;
+            sh:in [ rdf:rest () ] ;
+            sh:order 5 ;
+            sh:path ttm:components ],
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable name for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:order 13 ;
+            sh:path schema1:name ],
+        [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
             sh:order 8 ;
             sh:path ttm:test_case_predicate_name ],
         [ sh:datatype xsd:string ;
-            sh:description "One or more 'tags' slot values (slot inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in a \"Block List\" collection." ;
-            sh:order 15 ;
-            sh:path schema1:additionalType ],
+            sh:description "A human-readable description for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:order 14 ;
+            sh:path schema1:description ],
         [ sh:description "A unique identifier for a Test Entity" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 12 ;
             sh:path schema1:identifier ],
-        [ sh:class ttm:TestAsset ;
-            sh:description "One or more 'tags' slot values (inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in 'test_assets' slot (\"Block List\") collection." ;
+        [ sh:datatype xsd:string ;
+            sh:description "Settings for the test harness for TestCase" ;
             sh:minCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 2 ;
-            sh:path ttm:test_assets ],
-        [ sh:description "The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX." ;
-            sh:in [ rdf:rest () ] ;
-            sh:order 5 ;
-            sh:path ttm:components ],
-        [ sh:description "Deployment environment within which the associated TestSuite is run." ;
-            sh:in ( "dev" "ci" "test" "prod" ) ;
-            sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path ttm:test_env ],
-        [ sh:description "Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string." ;
-            sh:in ( "SME" "SMURF" "GitHubUserFeedback" "TACT" "BenchMark" "TranslatorTeam" "TestDataLocation" ) ;
-            sh:maxCount 1 ;
-            sh:order 7 ;
-            sh:path ttm:test_case_source ],
+            sh:order 11 ;
+            sh:path ttm:test_case_runner_settings ],
+        [ sh:datatype xsd:string ;
+            sh:description "One or more 'tags' slot values (slot inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in a \"Block List\" collection." ;
+            sh:order 15 ;
+            sh:path schema1:additionalType ],
         [ sh:class ttm:Precondition ;
             sh:nodeKind sh:IRI ;
             sh:order 3 ;
             sh:path ttm:preconditions ],
+        [ sh:description "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)" ;
+            sh:in ( "AcceptanceTest" "BenchmarkTest" "QuantitativeTest" ) ;
+            sh:maxCount 1 ;
+            sh:order 6 ;
+            sh:path ttm:test_case_objective ],
         [ sh:maxCount 1 ;
             sh:order 10 ;
             sh:path ttm:test_case_input_id ],
-        [ sh:description "Type of TestCase query." ;
-            sh:in ( "treats" ) ;
+        [ sh:description "Deployment environment within which the associated TestSuite is run." ;
+            sh:in ( "dev" "ci" "test" "prod" ) ;
             sh:maxCount 1 ;
-            sh:order 1 ;
-            sh:path ttm:query_type ],
+            sh:order 0 ;
+            sh:path ttm:test_env ],
         [ sh:description "A template for a query, which can be used to generate a query for a test case.  note: the current enumerated values for this slot come from the Benchmarks repo config/benchmarks.json \"templates\" collection and refer to the \"name\" field of each template.  Templates themselves are currently stored in the config/[source_name]/templates directory." ;
             sh:in ( "ameliorates" "treats" "three_hop" "drug_treats_rare_disease" "drug-to-gene" ) ;
             sh:maxCount 1 ;
             sh:order 4 ;
             sh:path ttm:trapi_template ],
         [ sh:datatype xsd:string ;
-            sh:description "Settings for the test harness for TestCase" ;
-            sh:minCount 1 ;
-            sh:order 11 ;
-            sh:path ttm:test_case_runner_settings ],
-        [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
             sh:order 9 ;
             sh:path ttm:test_case_predicate_id ],
-        [ sh:datatype xsd:string ;
-            sh:description "A human-readable name for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:order 13 ;
-            sh:path schema1:name ],
-        [ sh:description "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)" ;
-            sh:in ( "AcceptanceTest" "BenchmarkTest" "QuantitativeTest" ) ;
+        [ sh:description "Type of TestCase query." ;
+            sh:in ( "treats" ) ;
             sh:maxCount 1 ;
-            sh:order 6 ;
-            sh:path ttm:test_case_objective ],
-        [ sh:datatype xsd:string ;
-            sh:description "A human-readable description for a Test Entity" ;
+            sh:order 1 ;
+            sh:path ttm:query_type ],
+        [ sh:class ttm:TestAsset ;
+            sh:description "One or more 'tags' slot values (inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in 'test_assets' slot (\"Block List\") collection." ;
+            sh:minCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 2 ;
+            sh:path ttm:test_assets ],
+        [ sh:description "Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string." ;
+            sh:in ( "SME" "SMURF" "GitHubUserFeedback" "TACT" "BenchMark" "TranslatorTeam" "TestDataLocation" ) ;
             sh:maxCount 1 ;
-            sh:order 14 ;
-            sh:path schema1:description ] ;
+            sh:order 7 ;
+            sh:path ttm:test_case_source ] ;
     sh:targetClass ttm:TestCase .
 
 ttm:Precondition a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents a precondition for a TestCase" ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:datatype xsd:string ;
-            sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
-            sh:order 3 ;
-            sh:path schema1:additionalType ],
+            sh:description "A human-readable description for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:order 2 ;
+            sh:path schema1:description ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable name for a Test Entity" ;
             sh:maxCount 1 ;
             sh:order 1 ;
             sh:path schema1:name ],
-        [ sh:datatype xsd:string ;
-            sh:description "A human-readable description for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:order 2 ;
-            sh:path schema1:description ],
         [ sh:description "A unique identifier for a Test Entity" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 0 ;
-            sh:path schema1:identifier ] ;
+            sh:path schema1:identifier ],
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
+            sh:order 3 ;
+            sh:path schema1:additionalType ] ;
     sh:targetClass ttm:Precondition .
 
 ttm:TestMetadata a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents metadata related to (external SME, SMURF, Translator feedback,  large scale batch, etc.) like the provenance of test assets, cases and/or suites." ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:string ;
-            sh:description "A human-readable name for a Test Entity" ;
+    sh:property [ sh:description "A unique identifier for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 5 ;
-            sh:path schema1:name ],
+            sh:minCount 1 ;
+            sh:order 4 ;
+            sh:path schema1:identifier ],
         [ sh:description "Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string." ;
             sh:in ( "SME" "SMURF" "GitHubUserFeedback" "TACT" "BenchMark" "TranslatorTeam" "TestDataLocation" ) ;
             sh:maxCount 1 ;
             sh:order 0 ;
             sh:path ttm:test_source ],
+        [ sh:description "Document URL where original test source particulars are registered (e.g. Github repo)" ;
+            sh:maxCount 1 ;
+            sh:order 1 ;
+            sh:path ttm:test_reference ],
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
+            sh:order 7 ;
+            sh:path schema1:additionalType ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
             sh:order 6 ;
             sh:path schema1:description ],
-        [ sh:description "A unique identifier for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 4 ;
-            sh:path schema1:identifier ],
         [ sh:class ttm:TestEntityParameter ;
             sh:description "Metadata annotation." ;
             sh:nodeKind sh:BlankNode ;
             sh:order 3 ;
             sh:path ttm:test_annotations ],
-        [ sh:datatype xsd:string ;
-            sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
-            sh:order 7 ;
-            sh:path schema1:additionalType ],
         [ sh:description "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)" ;
             sh:in ( "AcceptanceTest" "BenchmarkTest" "QuantitativeTest" ) ;
             sh:maxCount 1 ;
             sh:order 2 ;
             sh:path ttm:test_objective ],
-        [ sh:description "Document URL where original test source particulars are registered (e.g. Github repo)" ;
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable name for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 1 ;
-            sh:path ttm:test_reference ] ;
+            sh:order 5 ;
+            sh:path schema1:name ] ;
     sh:targetClass ttm:TestMetadata .
```

### Comparing `translator_testing_model-0.3.0/project/shex/translator_testing_model.shex` & `translator_testing_model-2.3.0/project/shex/translator_testing_model.shex`

 * *Files 2% similar despite different names*

```diff
@@ -180,19 +180,14 @@
              <test_issue> @<TestIssueEnum> ? ;
              <semantic_severity> @<SemanticSeverityEnum> ? ;
              <in_v1> @linkml:Boolean ? ;
              <well_known> @linkml:Boolean ? ;
              <test_reference> @linkml:Uriorcurie ? ;
              <runner_settings> @linkml:String + ;
              <test_metadata> @<TestMetadata> ;
-             <biolink_qualified_predicate> @linkml:Uriorcurie ? ;
-             <biolink_subject_aspect_qualifier> @linkml:String ? ;
-             <biolink_subject_direction_qualifier> @linkml:String ? ;
-             <biolink_object_aspect_qualifier> @linkml:String ? ;
-             <biolink_object_direction_qualifier> @linkml:String ? ;
              schema1:additionalType @linkml:String *
           ) ;
           rdf:type [ <TestAsset> ]
        )
     } OR @<AcceptanceTestAsset> OR @<TestEdgeData>
 )
```

### Comparing `translator_testing_model-0.3.0/project/sqlschema/translator_testing_model.sql` & `translator_testing_model-2.3.0/project/sqlschema/translator_testing_model.sql`

 * *Files 4% similar despite different names*

```diff
@@ -183,19 +183,14 @@
 	expected_output TEXT, 
 	test_issue VARCHAR(20), 
 	semantic_severity VARCHAR(13), 
 	in_v1 BOOLEAN, 
 	well_known BOOLEAN, 
 	test_reference TEXT, 
 	test_metadata TEXT NOT NULL, 
-	biolink_qualified_predicate TEXT, 
-	biolink_subject_aspect_qualifier TEXT, 
-	biolink_subject_direction_qualifier TEXT, 
-	biolink_object_aspect_qualifier TEXT, 
-	biolink_object_direction_qualifier TEXT, 
 	id TEXT NOT NULL, 
 	must_pass_date DATE, 
 	must_pass_environment VARCHAR(4), 
 	scientific_question TEXT, 
 	string_entry TEXT, 
 	direction VARCHAR(9), 
 	answer_informal_concept TEXT, 
@@ -264,19 +259,14 @@
 	expected_output TEXT, 
 	test_issue VARCHAR(20), 
 	semantic_severity VARCHAR(13), 
 	in_v1 BOOLEAN, 
 	well_known BOOLEAN, 
 	test_reference TEXT, 
 	test_metadata TEXT NOT NULL, 
-	biolink_qualified_predicate TEXT, 
-	biolink_subject_aspect_qualifier TEXT, 
-	biolink_subject_direction_qualifier TEXT, 
-	biolink_object_aspect_qualifier TEXT, 
-	biolink_object_direction_qualifier TEXT, 
 	id TEXT NOT NULL, 
 	PRIMARY KEY (id), 
 	FOREIGN KEY(test_metadata) REFERENCES "TestMetadata" (id)
 );
 
 CREATE TABLE "TestCaseResult" (
 	id TEXT NOT NULL, 
@@ -307,19 +297,14 @@
 	expected_output TEXT, 
 	test_issue VARCHAR(20), 
 	semantic_severity VARCHAR(13), 
 	in_v1 BOOLEAN, 
 	well_known BOOLEAN, 
 	test_reference TEXT, 
 	test_metadata TEXT NOT NULL, 
-	biolink_qualified_predicate TEXT, 
-	biolink_subject_aspect_qualifier TEXT, 
-	biolink_subject_direction_qualifier TEXT, 
-	biolink_object_aspect_qualifier TEXT, 
-	biolink_object_direction_qualifier TEXT, 
 	id TEXT NOT NULL, 
 	PRIMARY KEY (id), 
 	FOREIGN KEY(test_metadata) REFERENCES "TestMetadata" (id)
 );
 
 CREATE TABLE "TestResultPKSet" (
 	id TEXT NOT NULL,
```

### Comparing `translator_testing_model-0.3.0/pyproject.toml` & `translator_testing_model-2.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "translator_testing_model"
-version = "0.3.0"
+version = "2.3.0"
 description = "This is the project description."
 authors = ["Sierra Moxon <sierra.taylor@gmail.com>", "Richard Bruskiewich <richard.bruskiewich@delphinai.com>"]
 license = "MIT"
 readme = "README.md"
 include = [
     "README.md",
     "src/data/examples",
```

### Comparing `translator_testing_model-0.3.0/src/data/examples/Bad-AcceptanceTestAsset-001.yaml` & `translator_testing_model-2.3.0/src/data/examples/Bad-AcceptanceTestAsset-001.yaml`

 * *Files identical despite different names*

### Comparing `translator_testing_model-0.3.0/src/data/examples/Bad-TestCase-001.yaml` & `translator_testing_model-2.3.0/src/data/examples/Bad-TestCase-001.yaml`

 * *Files identical despite different names*

### Comparing `translator_testing_model-0.3.0/src/data/examples/Bad-TestEntity-001.yaml` & `translator_testing_model-2.3.0/src/data/examples/Bad-TestEntity-001.yaml`

 * *Files identical despite different names*

### Comparing `translator_testing_model-0.3.0/src/data/examples/Bad-TestEntity-002.yaml-uriorcurie_should_fail_but_does_not` & `translator_testing_model-2.3.0/src/data/examples/Bad-TestEntity-002.yaml-uriorcurie_should_fail_but_does_not`

 * *Files identical despite different names*

### Comparing `translator_testing_model-0.3.0/src/data/examples/Bad-TestMetadata-001.yaml` & `translator_testing_model-2.3.0/src/data/examples/Bad-TestMetadata-001.yaml`

 * *Files identical despite different names*

### Comparing `translator_testing_model-0.3.0/src/data/examples/Bad-TestSuite-001.yaml` & `translator_testing_model-2.3.0/src/data/examples/Bad-TestSuite-001.yaml`

 * *Files identical despite different names*

### Comparing `translator_testing_model-0.3.0/src/data/examples/Good-AcceptanceTestAsset-001.yaml` & `translator_testing_model-2.3.0/src/data/examples/Good-AcceptanceTestAsset-001.yaml`

 * *Files identical despite different names*

### Comparing `translator_testing_model-0.3.0/src/data/examples/Good-AcceptanceTestCase-001.yaml` & `translator_testing_model-2.3.0/src/data/examples/Good-AcceptanceTestCase-001.yaml`

 * *Files identical despite different names*

### Comparing `translator_testing_model-0.3.0/src/data/examples/Good-TestAsset-001.yaml` & `translator_testing_model-2.3.0/src/data/examples/Good-TestAsset-001.yaml`

 * *Files identical despite different names*

### Comparing `translator_testing_model-0.3.0/src/data/examples/Good-TestCase-001.json` & `translator_testing_model-2.3.0/src/data/examples/Good-TestCase-001.json`

 * *Files identical despite different names*

### Comparing `translator_testing_model-0.3.0/src/data/examples/Good-TestCase-001.yaml` & `translator_testing_model-2.3.0/src/data/examples/Good-TestCase-001.yaml`

 * *Files identical despite different names*

### Comparing `translator_testing_model-0.3.0/src/data/examples/Good-TestCaseSpecification-001.yaml` & `translator_testing_model-2.3.0/src/data/examples/Good-TestCaseSpecification-001.yaml`

 * *Files identical despite different names*

### Comparing `translator_testing_model-0.3.0/src/data/examples/Good-TestEntity-Complete.yaml` & `translator_testing_model-2.3.0/src/data/examples/Good-TestEntity-Complete.yaml`

 * *Files identical despite different names*

### Comparing `translator_testing_model-0.3.0/src/data/examples/Good-TestSuite-001.yaml` & `translator_testing_model-2.3.0/src/data/examples/Good-TestSuite-001.yaml`

 * *Files identical despite different names*

### Comparing `translator_testing_model-0.3.0/src/data/examples/SampleTestAssetList.json` & `translator_testing_model-2.3.0/src/data/examples/SampleTestAssetList.json`

 * *Files identical despite different names*

### Comparing `translator_testing_model-0.3.0/src/translator_testing_model/adaptor/test_case_generator.py` & `translator_testing_model-2.3.0/src/translator_testing_model/adaptor/test_case_generator.py`

 * *Files identical despite different names*

### Comparing `translator_testing_model-0.3.0/src/translator_testing_model/adaptor/testrunner.py` & `translator_testing_model-2.3.0/src/translator_testing_model/adaptor/testrunner.py`

 * *Files identical despite different names*

### Comparing `translator_testing_model-0.3.0/src/translator_testing_model/datamodel/pydanticmodel.py` & `translator_testing_model-2.3.0/src/translator_testing_model/datamodel/pydanticmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,19 +276,14 @@
     test_issue: Optional[TestIssueEnum] = Field(None)
     semantic_severity: Optional[SemanticSeverityEnum] = Field(None)
     in_v1: Optional[bool] = Field(None)
     well_known: Optional[bool] = Field(None)
     test_reference: Optional[str] = Field(None, description="""Document URL where original test source particulars are registered (e.g. Github repo)""")
     runner_settings: List[str] = Field(default_factory=list, description="""Settings for the test harness, e.g. \"inferred\"""")
     test_metadata: TestMetadata = Field(..., description="""Test metadata describes the external provenance, cross-references and objectives for a given test.""")
-    biolink_qualified_predicate: Optional[str] = Field(None, description="""The qualified_predicate in Biolink model corresponding to the shorthand predicate name used in the test asset.""")
-    biolink_subject_aspect_qualifier: Optional[str] = Field(None, description="""The aspect of the subject of the test asset predicate""")
-    biolink_subject_direction_qualifier: Optional[str] = Field(None, description="""The direction of the subject of the test asset predicate""")
-    biolink_object_aspect_qualifier: Optional[str] = Field(None, description="""The aspect of the object of the test asset predicate""")
-    biolink_object_direction_qualifier: Optional[str] = Field(None, description="""The direction of the object of the test asset predicate""")
     id: str = Field(..., description="""A unique identifier for a Test Entity""")
     name: Optional[str] = Field(None, description="""A human-readable name for a Test Entity""")
     description: Optional[str] = Field(None, description="""A human-readable description for a Test Entity""")
     tags: Optional[List[str]] = Field(default_factory=list, description="""One or more 'tags' slot values (inherited from TestEntity) should generally be defined to specify TestAsset membership in a \"Block List\" collection""")
     
 
 class AcceptanceTestAsset(TestAsset):
@@ -319,19 +314,14 @@
     test_issue: Optional[TestIssueEnum] = Field(None)
     semantic_severity: Optional[SemanticSeverityEnum] = Field(None)
     in_v1: Optional[bool] = Field(None)
     well_known: Optional[bool] = Field(None)
     test_reference: Optional[str] = Field(None, description="""Document URL where original test source particulars are registered (e.g. Github repo)""")
     runner_settings: List[str] = Field(default_factory=list, description="""Settings for the test harness, e.g. \"inferred\"""")
     test_metadata: TestMetadata = Field(..., description="""Test metadata describes the external provenance, cross-references and objectives for a given test.""")
-    biolink_qualified_predicate: Optional[str] = Field(None, description="""The qualified_predicate in Biolink model corresponding to the shorthand predicate name used in the test asset.""")
-    biolink_subject_aspect_qualifier: Optional[str] = Field(None, description="""The aspect of the subject of the test asset predicate""")
-    biolink_subject_direction_qualifier: Optional[str] = Field(None, description="""The direction of the subject of the test asset predicate""")
-    biolink_object_aspect_qualifier: Optional[str] = Field(None, description="""The aspect of the object of the test asset predicate""")
-    biolink_object_direction_qualifier: Optional[str] = Field(None, description="""The direction of the object of the test asset predicate""")
     id: str = Field(..., description="""A unique identifier for a Test Entity""")
     name: Optional[str] = Field(None, description="""A human-readable name for a Test Entity""")
     description: Optional[str] = Field(None, description="""A human-readable description for a Test Entity""")
     tags: Optional[List[str]] = Field(default_factory=list, description="""One or more 'tags' slot values (inherited from TestEntity) should generally be defined to specify TestAsset membership in a \"Block List\" collection""")
     
 
 class TestEdgeData(TestAsset):
@@ -352,19 +342,14 @@
     test_issue: Optional[TestIssueEnum] = Field(None)
     semantic_severity: Optional[SemanticSeverityEnum] = Field(None)
     in_v1: Optional[bool] = Field(None)
     well_known: Optional[bool] = Field(None)
     test_reference: Optional[str] = Field(None, description="""Document URL where original test source particulars are registered (e.g. Github repo)""")
     runner_settings: List[str] = Field(default_factory=list, description="""Settings for the test harness, e.g. \"inferred\"""")
     test_metadata: TestMetadata = Field(..., description="""Test metadata describes the external provenance, cross-references and objectives for a given test.""")
-    biolink_qualified_predicate: Optional[str] = Field(None, description="""The qualified_predicate in Biolink model corresponding to the shorthand predicate name used in the test asset.""")
-    biolink_subject_aspect_qualifier: Optional[str] = Field(None, description="""The aspect of the subject of the test asset predicate""")
-    biolink_subject_direction_qualifier: Optional[str] = Field(None, description="""The direction of the subject of the test asset predicate""")
-    biolink_object_aspect_qualifier: Optional[str] = Field(None, description="""The aspect of the object of the test asset predicate""")
-    biolink_object_direction_qualifier: Optional[str] = Field(None, description="""The direction of the object of the test asset predicate""")
     id: str = Field(..., description="""A unique identifier for a Test Entity""")
     name: Optional[str] = Field(None, description="""A human-readable name for a Test Entity""")
     description: Optional[str] = Field(None, description="""A human-readable description for a Test Entity""")
     tags: Optional[List[str]] = Field(default_factory=list, description="""One or more 'tags' slot values (inherited from TestEntity) should generally be defined to specify TestAsset membership in a \"Block List\" collection""")
     
 
 class Precondition(TestEntity):
```

### Comparing `translator_testing_model-0.3.0/src/translator_testing_model/datamodel/pydanticmodel_v2.py` & `translator_testing_model-2.3.0/src/translator_testing_model/datamodel/pydanticmodel_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,19 +272,14 @@
     test_issue: Optional[TestIssueEnum] = Field(None)
     semantic_severity: Optional[SemanticSeverityEnum] = Field(None)
     in_v1: Optional[bool] = Field(None)
     well_known: Optional[bool] = Field(None)
     test_reference: Optional[str] = Field(None, description="""Document URL where original test source particulars are registered (e.g. Github repo)""")
     runner_settings: List[str] = Field(default_factory=list, description="""Settings for the test harness, e.g. \"inferred\"""")
     test_metadata: TestMetadata = Field(..., description="""Test metadata describes the external provenance, cross-references and objectives for a given test.""")
-    biolink_qualified_predicate: Optional[str] = Field(None, description="""The qualified_predicate in Biolink model corresponding to the shorthand predicate name used in the test asset.""")
-    biolink_subject_aspect_qualifier: Optional[str] = Field(None, description="""The aspect of the subject of the test asset predicate""")
-    biolink_subject_direction_qualifier: Optional[str] = Field(None, description="""The direction of the subject of the test asset predicate""")
-    biolink_object_aspect_qualifier: Optional[str] = Field(None, description="""The aspect of the object of the test asset predicate""")
-    biolink_object_direction_qualifier: Optional[str] = Field(None, description="""The direction of the object of the test asset predicate""")
     id: str = Field(..., description="""A unique identifier for a Test Entity""")
     name: Optional[str] = Field(None, description="""A human-readable name for a Test Entity""")
     description: Optional[str] = Field(None, description="""A human-readable description for a Test Entity""")
     tags: Optional[List[str]] = Field(default_factory=list, description="""One or more 'tags' slot values (inherited from TestEntity) should generally be defined to specify TestAsset membership in a \"Block List\" collection""")
     
 
 class AcceptanceTestAsset(TestAsset):
@@ -315,19 +310,14 @@
     test_issue: Optional[TestIssueEnum] = Field(None)
     semantic_severity: Optional[SemanticSeverityEnum] = Field(None)
     in_v1: Optional[bool] = Field(None)
     well_known: Optional[bool] = Field(None)
     test_reference: Optional[str] = Field(None, description="""Document URL where original test source particulars are registered (e.g. Github repo)""")
     runner_settings: List[str] = Field(default_factory=list, description="""Settings for the test harness, e.g. \"inferred\"""")
     test_metadata: TestMetadata = Field(..., description="""Test metadata describes the external provenance, cross-references and objectives for a given test.""")
-    biolink_qualified_predicate: Optional[str] = Field(None, description="""The qualified_predicate in Biolink model corresponding to the shorthand predicate name used in the test asset.""")
-    biolink_subject_aspect_qualifier: Optional[str] = Field(None, description="""The aspect of the subject of the test asset predicate""")
-    biolink_subject_direction_qualifier: Optional[str] = Field(None, description="""The direction of the subject of the test asset predicate""")
-    biolink_object_aspect_qualifier: Optional[str] = Field(None, description="""The aspect of the object of the test asset predicate""")
-    biolink_object_direction_qualifier: Optional[str] = Field(None, description="""The direction of the object of the test asset predicate""")
     id: str = Field(..., description="""A unique identifier for a Test Entity""")
     name: Optional[str] = Field(None, description="""A human-readable name for a Test Entity""")
     description: Optional[str] = Field(None, description="""A human-readable description for a Test Entity""")
     tags: Optional[List[str]] = Field(default_factory=list, description="""One or more 'tags' slot values (inherited from TestEntity) should generally be defined to specify TestAsset membership in a \"Block List\" collection""")
     
 
 class TestEdgeData(TestAsset):
@@ -348,19 +338,14 @@
     test_issue: Optional[TestIssueEnum] = Field(None)
     semantic_severity: Optional[SemanticSeverityEnum] = Field(None)
     in_v1: Optional[bool] = Field(None)
     well_known: Optional[bool] = Field(None)
     test_reference: Optional[str] = Field(None, description="""Document URL where original test source particulars are registered (e.g. Github repo)""")
     runner_settings: List[str] = Field(default_factory=list, description="""Settings for the test harness, e.g. \"inferred\"""")
     test_metadata: TestMetadata = Field(..., description="""Test metadata describes the external provenance, cross-references and objectives for a given test.""")
-    biolink_qualified_predicate: Optional[str] = Field(None, description="""The qualified_predicate in Biolink model corresponding to the shorthand predicate name used in the test asset.""")
-    biolink_subject_aspect_qualifier: Optional[str] = Field(None, description="""The aspect of the subject of the test asset predicate""")
-    biolink_subject_direction_qualifier: Optional[str] = Field(None, description="""The direction of the subject of the test asset predicate""")
-    biolink_object_aspect_qualifier: Optional[str] = Field(None, description="""The aspect of the object of the test asset predicate""")
-    biolink_object_direction_qualifier: Optional[str] = Field(None, description="""The direction of the object of the test asset predicate""")
     id: str = Field(..., description="""A unique identifier for a Test Entity""")
     name: Optional[str] = Field(None, description="""A human-readable name for a Test Entity""")
     description: Optional[str] = Field(None, description="""A human-readable description for a Test Entity""")
     tags: Optional[List[str]] = Field(default_factory=list, description="""One or more 'tags' slot values (inherited from TestEntity) should generally be defined to specify TestAsset membership in a \"Block List\" collection""")
     
 
 class Precondition(TestEntity):
```

### Comparing `translator_testing_model-0.3.0/src/translator_testing_model/datamodel/translator_testing_model.py` & `translator_testing_model-2.3.0/src/translator_testing_model/datamodel/translator_testing_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Auto generated from translator_testing_model.yaml by pythongen.py version: 0.0.1
-# Generation date: 2024-03-15T17:20:13
+# Generation date: 2024-03-18T12:26:26
 # Schema: Translator-Testing-Model
 #
 # id: https://w3id.org/TranslatorSRI/TranslatorTestingModel
 # description: Data model to formalize the structure of test assets, cases, suites and related metadata
 #   applied to run the diverse polymorphic testing objectives for the Biomedical Data Translator system.
 # license: MIT
 
@@ -316,19 +316,14 @@
     qualifiers: Optional[Union[Union[dict, Qualifier], List[Union[dict, Qualifier]]]] = empty_list()
     expected_output: Optional[str] = None
     test_issue: Optional[Union[str, "TestIssueEnum"]] = None
     semantic_severity: Optional[Union[str, "SemanticSeverityEnum"]] = None
     in_v1: Optional[Union[bool, Bool]] = None
     well_known: Optional[Union[bool, Bool]] = None
     test_reference: Optional[Union[str, URIorCURIE]] = None
-    biolink_qualified_predicate: Optional[Union[str, URIorCURIE]] = None
-    biolink_subject_aspect_qualifier: Optional[str] = None
-    biolink_subject_direction_qualifier: Optional[str] = None
-    biolink_object_aspect_qualifier: Optional[str] = None
-    biolink_object_direction_qualifier: Optional[str] = None
     tags: Optional[Union[str, List[str]]] = empty_list()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, TestAssetId):
             self.id = TestAssetId(self.id)
@@ -389,29 +384,14 @@
 
         if self.well_known is not None and not isinstance(self.well_known, Bool):
             self.well_known = Bool(self.well_known)
 
         if self.test_reference is not None and not isinstance(self.test_reference, URIorCURIE):
             self.test_reference = URIorCURIE(self.test_reference)
 
-        if self.biolink_qualified_predicate is not None and not isinstance(self.biolink_qualified_predicate, URIorCURIE):
-            self.biolink_qualified_predicate = URIorCURIE(self.biolink_qualified_predicate)
-
-        if self.biolink_subject_aspect_qualifier is not None and not isinstance(self.biolink_subject_aspect_qualifier, str):
-            self.biolink_subject_aspect_qualifier = str(self.biolink_subject_aspect_qualifier)
-
-        if self.biolink_subject_direction_qualifier is not None and not isinstance(self.biolink_subject_direction_qualifier, str):
-            self.biolink_subject_direction_qualifier = str(self.biolink_subject_direction_qualifier)
-
-        if self.biolink_object_aspect_qualifier is not None and not isinstance(self.biolink_object_aspect_qualifier, str):
-            self.biolink_object_aspect_qualifier = str(self.biolink_object_aspect_qualifier)
-
-        if self.biolink_object_direction_qualifier is not None and not isinstance(self.biolink_object_direction_qualifier, str):
-            self.biolink_object_direction_qualifier = str(self.biolink_object_direction_qualifier)
-
         if not isinstance(self.tags, list):
             self.tags = [self.tags] if self.tags is not None else []
         self.tags = [v if isinstance(v, str) else str(v) for v in self.tags]
 
         super().__post_init__(**kwargs)
```

### Comparing `translator_testing_model-0.3.0/src/translator_testing_model/schema/translator_testing_model.yaml` & `translator_testing_model-2.3.0/src/translator_testing_model/schema/translator_testing_model.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -125,19 +125,14 @@
       - test_issue
       - semantic_severity
       - in_v1
       - well_known
       - test_reference
       - runner_settings
       - test_metadata
-      - biolink_qualified_predicate
-      - biolink_subject_aspect_qualifier
-      - biolink_subject_direction_qualifier
-      - biolink_object_aspect_qualifier
-      - biolink_object_direction_qualifier
     slot_usage:
       id:
         aliases: ["AssetIdentifier"]
         range: uriorcurie
       tags:
         description: >-
           One or more 'tags' slot values (inherited from TestEntity) should generally
```

### Comparing `translator_testing_model-0.3.0/src/translator_testing_model/scripts/GitHub_issue_parser.py` & `translator_testing_model-2.3.0/src/translator_testing_model/scripts/GitHub_issue_parser.py`

 * *Files identical despite different names*

### Comparing `translator_testing_model-0.3.0/src/translator_testing_model/scripts/generate_suite_for_demo.py` & `translator_testing_model-2.3.0/src/translator_testing_model/scripts/generate_suite_for_demo.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from src.translator_testing_model.datamodel.pydanticmodel import TestAsset, TestCase, TestSuite, TestMetadata
+from src.translator_testing_model.datamodel.pydanticmodel import TestAsset, TestCase, TestSuite, TestMetadata, Qualifier
 import csv
 import json
 import requests
 import yaml
 import bmt
 toolkit = bmt.Toolkit()
 
@@ -50,27 +50,32 @@
             continue
 
         converted_predicate = None
         biolink_qualified_predicate = ""
         biolink_object_aspect_qualifier = ""
         biolink_object_direction_qualifier = ""
         specified_predicate = row.get("Relationship").lower().strip()
+        if specified_predicate == "decreases abundance or activity of":
+            specified_predicate = "decreases activity or abundance of"
+            print("specified predicate", specified_predicate)
         if toolkit.get_element(specified_predicate) is not None:
             converted_predicate = toolkit.get_element(specified_predicate).name
             converted_predicate = converted_predicate.replace(" ", "_")
+            print("converted predicate", specified_predicate)
         else:
             pred_mapping = toolkit.pmap
             for collct in pred_mapping.values():
                 for map_item in collct:
                     if map_item.get("mapped predicate") == specified_predicate:
+                        print("mapped it", map_item.get("mapped predicate"))
                         converted_predicate = map_item.get("predicate")
                         converted_predicate = converted_predicate.replace(" ", "_")
                         biolink_object_aspect_qualifier = map_item.get("object aspect qualifier")
                         biolink_object_direction_qualifier = map_item.get("object direction qualifier")
-                        biolink_qualified_predicate = map_item.get("qualified predicate")
+                        biolink_qualified_predicate = "biolink:"+map_item.get("qualified predicate")
 
         if row.get("Expected Result / Suggested Comparator") == "4_NeverShow":
             expected_output = "NeverShow"
         elif row.get("Expected Result / Suggested Comparator") == "3_BadButForgivable":
             expected_output = "BadButForgivable"
         elif row.get("Expected Result / Suggested Comparator") == "2_Acceptable":
             expected_output = "Acceptable"
@@ -101,45 +106,55 @@
             output_category = 'biolink:ChemicalEntity'
         if row.get("OutputID").startswith("MONDO:"):
             output_category = 'biolink:Disease'
         if row.get("OutputID").startswith("UBERON:"):
             output_category = 'biolink:AnatomicalEntity'
         if row.get("OutputID").startswith("HP:"):
             output_category = 'biolink:PhenotypicFeature'
+        if row.get("OutputID").startswith("DRUGBANK:"):
+            output_category = 'biolink:ChemicalEntity'
 
+        print(converted_predicate, row, expected_output)
         ta = TestAsset(id=row.get("id").replace(":", "_"),
-                       name=expected_output + ': ' + row.get("OutputName").replace(" ", "_") + "_" + row.get("Relationship").lower() + "_" + row.get("InputName").strip().replace(" ", "_"),
-                       description=expected_output + ': ' + row.get("OutputName").replace(" ", "_") + "_" + row.get("Relationship").lower() + "_" + row.get("InputName").strip().replace(" ", "_"),
+                       name=expected_output + ': ' + row.get("OutputName").strip() +" "+ row.get("Relationship").strip().lower() +" "+ row.get("InputName").strip(),
+                       description=expected_output + ': ' + row.get("OutputName").strip() +" "+ row.get("Relationship").strip().lower() +" "+ row.get("InputName").strip(),
                        input_id=row.get("InputID").strip(),
-                       predicate_name=row.get("Relationship").lower().strip(),
-                       predicate_id=converted_predicate,
+                       predicate_name=converted_predicate,
+                       predicate_id="biolink:"+converted_predicate,
                        output_id=row.get("OutputID").strip(),
+                       output_name=row.get("OutputName").strip(),
                        output_category=output_category,
                        expected_output=expected_output.strip(),
                        test_metadata=TestMetadata(id=1),
                        input_category=input_category,
                        )
-        ta.input_name = row.get("InputID")
+        ta.input_name = row.get("InputName").strip()
         if row.get("Translator GitHubIssue") != "" and row.get("Translator GitHubIssue") is not None:
             tmd = TestMetadata(id=1,
                                test_source="SMURF",
                                test_reference=row.get("Translator GitHubIssue").strip(),
                                test_objective="AcceptanceTest")
             ta.test_metadata = tmd
         else:
             tmd = TestMetadata(id=1,
                                test_source="SMURF",
                                test_objective="AcceptanceTest")
             ta.test_metadata = tmd
         ta.runner_settings = [row.get("Settings").lower()]
 
         if biolink_qualified_predicate != "":
-            ta.biolink_qualified_predicate = biolink_qualified_predicate
-            ta.biolink_object_aspect_qualifier = biolink_object_aspect_qualifier
-            ta.biolink_object_direction_qualifier = biolink_object_direction_qualifier
+            qp = Qualifier(parameter="biolink_qualified_predicate",
+                           value=biolink_qualified_predicate)
+            oaq = Qualifier(parameter="biolink_object_aspect_qualifier",
+                            value=biolink_object_aspect_qualifier.replace(" ", "_"))
+            odq = Qualifier(parameter="biolink_object_direction_qualifier",
+                            value=biolink_object_direction_qualifier)
+            qualifiers = [qp, oaq, odq]
+
+            ta.qualifiers=qualifiers
         if row.get("Well Known") == "yes":
             ta.well_known = True
         else:
             ta.well_known = False
         assets.append(ta)
 
     return assets
```

### Comparing `translator_testing_model-0.3.0/src/translator_testing_model/scripts/test_suite_generator.py` & `translator_testing_model-2.3.0/src/translator_testing_model/scripts/test_suite_generator.py`

 * *Files identical despite different names*

### Comparing `translator_testing_model-0.3.0/PKG-INFO` & `translator_testing_model-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: translator_testing_model
-Version: 0.3.0
+Version: 2.3.0
 Summary: This is the project description.
 License: MIT
 Author: Sierra Moxon
 Author-email: sierra.taylor@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

