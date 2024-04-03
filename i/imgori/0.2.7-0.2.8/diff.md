# Comparing `tmp/imgori-0.2.7-py3-none-any.whl.zip` & `tmp/imgori-0.2.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 11847 bytes, number of entries: 26
+Zip file size: 11846 bytes, number of entries: 26
 -rwxr-xr-x  2.0 unx      139 b- defN 80-Jan-01 00:00 imgori/__init__.py
 -rw-r--r--  2.0 unx       50 b- defN 80-Jan-01 00:00 imgori/cli.py
 -rw-r--r--  2.0 unx       25 b- defN 80-Jan-01 00:00 imgori/commands/__init__.py
 -rw-r--r--  2.0 unx     1344 b- defN 80-Jan-01 00:00 imgori/commands/train.py
 -rwxr-xr-x  2.0 unx       72 b- defN 80-Jan-01 00:00 imgori/datasets/__init__.py
 -rw-r--r--  2.0 unx     2156 b- defN 80-Jan-01 00:00 imgori/datasets/imgori.py
 -rwxr-xr-x  2.0 unx      650 b- defN 80-Jan-01 00:00 imgori/datasets/mnist.py
@@ -17,12 +17,12 @@
 -rw-r--r--  2.0 unx     4073 b- defN 80-Jan-01 00:00 imgori/trainers/imgori.py
 -rw-r--r--  2.0 unx     4087 b- defN 80-Jan-01 00:00 imgori/trainers/mnist.py
 -rw-r--r--  2.0 unx       70 b- defN 80-Jan-01 00:00 imgori/trainers/trainer.py
 -rw-r--r--  2.0 unx     2398 b- defN 80-Jan-01 00:00 imgori/typing.py
 -rwxr-xr-x  2.0 unx      233 b- defN 80-Jan-01 00:00 imgori/utils/__init__.py
 -rw-r--r--  2.0 unx     1212 b- defN 80-Jan-01 00:00 imgori/utils/s3.py
 -rw-r--r--  2.0 unx      744 b- defN 80-Jan-01 00:00 imgori/utils/utils.py
--rw-r--r--  2.0 unx      681 b- defN 80-Jan-01 00:00 imgori-0.2.7.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 imgori-0.2.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       41 b- defN 80-Jan-01 00:00 imgori-0.2.7.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     2013 b- defN 16-Jan-01 00:00 imgori-0.2.7.dist-info/RECORD
-26 files, 24239 bytes uncompressed, 8629 bytes compressed:  64.4%
+-rw-r--r--  2.0 unx      681 b- defN 80-Jan-01 00:00 imgori-0.2.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 imgori-0.2.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       41 b- defN 80-Jan-01 00:00 imgori-0.2.8.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     2013 b- defN 16-Jan-01 00:00 imgori-0.2.8.dist-info/RECORD
+26 files, 24239 bytes uncompressed, 8628 bytes compressed:  64.4%
```

## zipnote {}

```diff
@@ -60,20 +60,20 @@
 
 Filename: imgori/utils/s3.py
 Comment: 
 
 Filename: imgori/utils/utils.py
 Comment: 
 
-Filename: imgori-0.2.7.dist-info/METADATA
+Filename: imgori-0.2.8.dist-info/METADATA
 Comment: 
 
-Filename: imgori-0.2.7.dist-info/WHEEL
+Filename: imgori-0.2.8.dist-info/WHEEL
 Comment: 
 
-Filename: imgori-0.2.7.dist-info/entry_points.txt
+Filename: imgori-0.2.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: imgori-0.2.7.dist-info/RECORD
+Filename: imgori-0.2.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## imgori/imgori.py

```diff
@@ -6,15 +6,15 @@
 from .nn import mobilenet_v3
 from .typing import Orientation
 from .typing import PathLike
 from .typing import PILImage
 from .utils import load_state_dict_from_s3_url
 
 DEFAULT_MODEL = (
-    "https://github.com/narumiruna/imgori/releases/download/v0.2.1-mobilenet-v3/imgori_mobilenet_v3_small.pth"  # noqa
+    "https://github.com/narumiruna/imgori/releases/download/v0.2.7-mobilenet-v3/imgori_mobilenet_v3_small.pth"  # noqa
 )
 
 
 def load_model(model_path: PathLike, device: torch.device | str = "cpu") -> nn.Module:
     model_path = str(model_path)
 
     if model_path.startswith("https://"):
```

## Comparing `imgori-0.2.7.dist-info/METADATA` & `imgori-0.2.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgori
-Version: 0.2.7
+Version: 0.2.8
 Summary: 
 Author: narumi
 Author-email: toucans-cutouts0f@icloud.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

## Comparing `imgori-0.2.7.dist-info/RECORD` & `imgori-0.2.8.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 imgori/cli.py,sha256=9-LsBqnc0-ncex4EbIOHEAGPw5xBXZ57pHZW1R7a1Pk,50
 imgori/commands/__init__.py,sha256=tNKqfMuVB5L96buP08z08lQhgFmW-OSxvVuodpRbQfM,25
 imgori/commands/train.py,sha256=8-K4aToL4z4mwRQ4AUL7ENwkqQ06SEuMhEu2fkBMfAQ,1344
 imgori/datasets/__init__.py,sha256=4IEJ1jDWbYPWQhyS0-aU3r4m5hJ58pZn0DSiYqnZyhc,72
 imgori/datasets/imgori.py,sha256=OgfwW0sa1NgI7jibg7DPhO11BuMaxU7VOydlhjETANA,2156
 imgori/datasets/mnist.py,sha256=eAk2Ecyp51Xu84Y-RJi5VYiyBpTosX2IvsKpBiE3Fls,650
 imgori/datasets/utils.py,sha256=2fEk28jop1QgfwhiniYtEvbVdr3fE-DMDq9y0m8SVNM,267
-imgori/imgori.py,sha256=X4s-Vs2mJ-m4v6fQ3TSfvsB7FKlu4tdstwt927KTfu8,1673
+imgori/imgori.py,sha256=N0Oy-fv1P_H-4hs-z_heu3PvswJw75oKCJ48HbeASbk,1673
 imgori/nn/__init__.py,sha256=Kc8dsNIqvRWAD0N9tkvLsqRL29ePjCEYQHaeQzG2U9k,103
 imgori/nn/efficientnet.py,sha256=QvKjk1q-CpdIesgOKUNtSjsdmPsXSxllWd1_8o_RMXc,436
 imgori/nn/lenet.py,sha256=g5gz1u_RAFSLuDvnMqDg2ZejoQk9lNBIZqCh-LP0Ws0,968
 imgori/nn/mobilenet_v3.py,sha256=eFENzM9P2ZJHNQ3UurqLAoRZgJargYPB7th_HdcM0hs,448
 imgori/optim.py,sha256=E_eXbOhpeYRqr70ghXTYLB7GeyNBsiTv3ycw2fe1VWU,202
 imgori/trainers/__init__.py,sha256=LA1hhnTzmv_EpMtqivqmMrIR6JLXFFlWBRFcASwiaGY,66
 imgori/trainers/imgori.py,sha256=cCUgTc2HkLOVSvzvLxVQpTHF3ImoG77AmfKHlk5w4zU,4073
 imgori/trainers/mnist.py,sha256=2DAhfGS5BYr9Bf9JVK_8FxwXbycvGansGqtAXfmieYI,4087
 imgori/trainers/trainer.py,sha256=72H5BlWgjYNV1YOwiePjP-PlSANx-kzz3jhCItsZxJs,70
 imgori/typing.py,sha256=2dVGFx8tHvn69yBb587pnvOFTaGGq0-XTGakXq1NUyM,2398
 imgori/utils/__init__.py,sha256=Z6XbCnKBP5UGMxt60JvwNu69XDJkVSHHZSW1SManhCA,233
 imgori/utils/s3.py,sha256=JA6NeafTO4JtGsbuohNKfKSEK7m9Mf9QPxzAUZJAN2c,1212
 imgori/utils/utils.py,sha256=cnfH6VaOeBzZNVfsEIesXG6eTP1RgivFW5qjk_msOxg,744
-imgori-0.2.7.dist-info/METADATA,sha256=BwE2ePqj8jmma5qNamt9QTFKCwGMn-6bv7GTrN_vYHs,681
-imgori-0.2.7.dist-info/WHEEL,sha256=FMvqSimYX_P7y0a7UY-_Mc83r5zkBZsCYPm7Lr0Bsq4,88
-imgori-0.2.7.dist-info/entry_points.txt,sha256=RBRze5SLMBGEr6NDoc_nszbzHABf-V8Wl_-VYMRwwic,41
-imgori-0.2.7.dist-info/RECORD,,
+imgori-0.2.8.dist-info/METADATA,sha256=Nrzk1mhK5vq4x0nNDDOdhN_upoK3oW7AfAdVcmEueQM,681
+imgori-0.2.8.dist-info/WHEEL,sha256=FMvqSimYX_P7y0a7UY-_Mc83r5zkBZsCYPm7Lr0Bsq4,88
+imgori-0.2.8.dist-info/entry_points.txt,sha256=RBRze5SLMBGEr6NDoc_nszbzHABf-V8Wl_-VYMRwwic,41
+imgori-0.2.8.dist-info/RECORD,,
```

