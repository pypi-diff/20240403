# Comparing `tmp/modlee-0.0.1.post7-py3-none-any.whl.zip` & `tmp/modlee-0.0.1.post8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 59264 bytes, number of entries: 24
+Zip file size: 59218 bytes, number of entries: 24
 -rw-rw-r--  2.0 unx     5648 b- defN 24-Apr-02 13:51 modlee/__init__.py
 -rw-rw-r--  2.0 unx    10669 b- defN 24-Apr-02 13:51 modlee/client.py
--rw-rw-r--  2.0 unx      422 b- defN 24-Apr-02 17:54 modlee/config.py
+-rw-rw-r--  2.0 unx      369 b- defN 24-Apr-02 18:16 modlee/config.py
 -rw-rw-r--  2.0 unx    39155 b- defN 24-Mar-19 02:55 modlee/converter.py
 -rw-rw-r--  2.0 unx    20782 b- defN 24-Mar-28 18:38 modlee/data_metafeatures.py
 -rw-rw-r--  2.0 unx    11976 b- defN 24-Mar-19 02:55 modlee/exp_loss_logger.py
 -rw-rw-r--  2.0 unx      272 b- defN 24-Mar-19 02:55 modlee/loss_sweeper.py
 -rw-rw-r--  2.0 unx    15787 b- defN 24-Mar-28 18:38 modlee/model_text_converter.py
 -rw-rw-r--  2.0 unx     5050 b- defN 24-Mar-19 02:55 modlee/modlee_image_model.py
 -rw-rw-r--  2.0 unx     3638 b- defN 24-Mar-19 02:55 modlee/retriever.py
@@ -15,12 +15,12 @@
 -rw-rw-r--  2.0 unx    18673 b- defN 24-Apr-02 13:51 modlee/model/callbacks.py
 -rw-rw-r--  2.0 unx     3443 b- defN 24-Mar-19 02:55 modlee/model/image_model.py
 -rw-rw-r--  2.0 unx     6055 b- defN 24-Apr-02 13:51 modlee/model/model.py
 -rw-rw-r--  2.0 unx     1867 b- defN 24-Mar-19 02:55 modlee/model/recommended_model.py
 -rw-rw-r--  2.0 unx      793 b- defN 24-Apr-01 19:23 modlee/recommender/__init__.py
 -rw-rw-r--  2.0 unx     5563 b- defN 24-Apr-01 19:23 modlee/recommender/image_recommender.py
 -rw-rw-r--  2.0 unx    14640 b- defN 24-Apr-02 13:51 modlee/recommender/recommender.py
--rw-rw-r--  2.0 unx    20067 b- defN 24-Apr-02 18:04 modlee-0.0.1.post7.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-02 18:04 modlee-0.0.1.post7.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-02 18:04 modlee-0.0.1.post7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1944 b- defN 24-Apr-02 18:04 modlee-0.0.1.post7.dist-info/RECORD
-24 files, 196119 bytes uncompressed, 56154 bytes compressed:  71.4%
+-rw-rw-r--  2.0 unx    20047 b- defN 24-Apr-02 18:31 modlee-0.0.1.post8.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-02 18:31 modlee-0.0.1.post8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-02 18:31 modlee-0.0.1.post8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1944 b- defN 24-Apr-02 18:31 modlee-0.0.1.post8.dist-info/RECORD
+24 files, 196046 bytes uncompressed, 56108 bytes compressed:  71.4%
```

## zipnote {}

```diff
@@ -54,20 +54,20 @@
 
 Filename: modlee/recommender/image_recommender.py
 Comment: 
 
 Filename: modlee/recommender/recommender.py
 Comment: 
 
-Filename: modlee-0.0.1.post7.dist-info/METADATA
+Filename: modlee-0.0.1.post8.dist-info/METADATA
 Comment: 
 
-Filename: modlee-0.0.1.post7.dist-info/WHEEL
+Filename: modlee-0.0.1.post8.dist-info/WHEEL
 Comment: 
 
-Filename: modlee-0.0.1.post7.dist-info/top_level.txt
+Filename: modlee-0.0.1.post8.dist-info/top_level.txt
 Comment: 
 
-Filename: modlee-0.0.1.post7.dist-info/RECORD
+Filename: modlee-0.0.1.post8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## modlee/config.py

```diff
@@ -1,9 +1,9 @@
 """ 
-Configuration variables: relative folder paths, server origins and endpoints.
+Configuration variables.
 """
 import pathlib
 
 ROOT_DIR = pathlib.Path(__file__).parent.absolute()
 MODLEE_DIR = ROOT_DIR / "modlee"
 TMP_DIR = ROOT_DIR / "tmp"
 MLRUNS_DIR = ROOT_DIR / "mlruns"
```

## Comparing `modlee-0.0.1.post7.dist-info/METADATA` & `modlee-0.0.1.post8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modlee
-Version: 0.0.1.post7
+Version: 0.0.1.post8
 Summary: modlee package
 Author-email: modlee <michael@modlee.ai>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -213,15 +213,15 @@
 Requires-Dist: mlflow ==2.6.0
 Requires-Dist: numpy ==1.26.4
 Requires-Dist: pydantic ==1.10.12
 Requires-Dist: setuptools >=68.0.0
 Requires-Dist: torch >=2.0.1
 Requires-Dist: torchmetrics >=1.0.0
 Requires-Dist: torchvision >=0.15.2
-Requires-Dist: onnx ==1.14.1
+Requires-Dist: onnx >=1.14.1
 Requires-Dist: torchsummary ==1.5.1
 Requires-Dist: modlee-onnx2torch ==1.5.11
 Requires-Dist: modlee-onnx-graphsurgeon ==0.3.27
 Requires-Dist: pymfe ==0.4.2
 Requires-Dist: pytest ==8.1.1
 Requires-Dist: nbsphinx
 Requires-Dist: sphinx-rtd-theme
@@ -250,15 +250,15 @@
 ```shell
 git clone https://github.com/modlee-ai/modlee
 cd modlee
 pip install .
 ```
 
 We have developed the package in Python 3.10. 
-Please [raise an issue](https://github.com/modlee-ai/modlee/blob/main/issues)) if you experience environment errors.
+Please [raise an issue](https://github.com/modlee-ai/modlee/issues)) if you experience environment errors.
 
 ### Set API key
 Either save your API key to an environment variable: 
 ```shell
 export MODLEE_API_KEY="my-api-key"
 ```
 Or pass directly to the  `modlee.init` function (less recommended):
@@ -373,15 +373,15 @@
     )
 ```
 
 ## Support
 
 ### Contributing
 We welcome contributions of any kind: bug reports, feature requests, tutorials, etc.
-Before submitting a pull request, [please read the contribution guidelines](https://github.com/modlee-ai/modlee/blob/main/docs/CONTRIBUTING.md).
+Before submitting a pull request, [please read the contribution guidelines](https://github.com/modlee-ai/modlee/docs/CONTRIBUTING.md).
 
 ### Issues
 If you encounter errors, [please raise an issue in this repository](https://github.com/modlee-ai/modlee/issues).
 
 ### Community
 [Join our Discord server](https://discord.com/invite/m8YDbWDvrF) to discuss and contribute with other Modlee users.
```

## Comparing `modlee-0.0.1.post7.dist-info/RECORD` & `modlee-0.0.1.post8.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 modlee/__init__.py,sha256=rouh4c8RfeNMpd1IyZRI6L_VCtfoNmoZ0ddjn6X2GtU,5648
 modlee/client.py,sha256=L1kgrsrFHsTJt65f4fTMq7BaWDJWQA9cTMgPVwDZVaU,10669
-modlee/config.py,sha256=8dQTrCYKt2tDyccQZfU7d6KgYgasSNfCAKt2Fn3AR-U,422
+modlee/config.py,sha256=uWvuAkvxvAmUDR4J3flbkFWUbdgj8bRWFNwkuqsR98g,369
 modlee/converter.py,sha256=L58ITzciixs2J64MZayNoNoqKH1T9R5cl488HZzdlZY,39155
 modlee/data_metafeatures.py,sha256=r2rAOmnLvqdkftO3pyioK11cqFCD10r0dTIfeggWmIA,20782
 modlee/exp_loss_logger.py,sha256=gzb3qzPJPMjlUrhrobaBH19smKBfMlj39ARyG-fKqDg,11976
 modlee/loss_sweeper.py,sha256=zZVRdce9JhwwdEF2tttL1A0umd-m7KW9m8tP-c-rNvA,272
 modlee/model_text_converter.py,sha256=dliQWiYrogtRiYmbCKxhDxOoCRYa5A_m6ySzimDehV0,15787
 modlee/modlee_image_model.py,sha256=QSij2rk_7v31TnnJ3Ra0mtwz6TiT2LKKnk9-XvExD14,5050
 modlee/retriever.py,sha256=KBpLOT_fwioSbfPlJ2Gt8SfpSzwApmcWyxT_8XI06EY,3638
@@ -14,11 +14,11 @@
 modlee/model/callbacks.py,sha256=GeQu18SDwx3MUZBXT2VFfEubiIS1CR9tTmsUHRZC5J4,18673
 modlee/model/image_model.py,sha256=DcYaf2b3htIpP6VwgwzUT2P3Dl5M7jh4yUbhOSHFjao,3443
 modlee/model/model.py,sha256=gMo1xS3P1VRPgm7uyqn_KaedxC8N5bW0CrKlBn_JbI0,6055
 modlee/model/recommended_model.py,sha256=kL0Uu2DhoBeqX-D_TzXmrJiIX9Bpewb-isWYmEjYEfs,1867
 modlee/recommender/__init__.py,sha256=kE-auY7fRWCMU6SoLH1ASJeHdcIC0uZ1w2E1e9glWlo,793
 modlee/recommender/image_recommender.py,sha256=o07RJ-ZxJLAp1hj5qj_IXiQCBXDBD0fJX_Om76wQmTc,5563
 modlee/recommender/recommender.py,sha256=b6XSb78gOFNX425fX_VHDP3Si52tg_bOHoH0Ba_O9uU,14640
-modlee-0.0.1.post7.dist-info/METADATA,sha256=1Tah8nYuiLQFkGttqq_EgBtXdxZ4KrPXt6uMwxC_hO8,20067
-modlee-0.0.1.post7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-modlee-0.0.1.post7.dist-info/top_level.txt,sha256=qYTpeC-xJutbXh2WQDzH5JlYcLETEeYfBkyRnloU904,7
-modlee-0.0.1.post7.dist-info/RECORD,,
+modlee-0.0.1.post8.dist-info/METADATA,sha256=3pjpFe0tEAh5MyoQwb2rOsyh4S0bZIyQK3dyjFlpi_c,20047
+modlee-0.0.1.post8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+modlee-0.0.1.post8.dist-info/top_level.txt,sha256=qYTpeC-xJutbXh2WQDzH5JlYcLETEeYfBkyRnloU904,7
+modlee-0.0.1.post8.dist-info/RECORD,,
```

