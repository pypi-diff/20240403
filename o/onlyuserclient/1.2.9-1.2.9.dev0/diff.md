# Comparing `tmp/onlyuserclient-1.2.9-py3-none-any.whl.zip` & `tmp/onlyuserclient-1.2.9.dev0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 35066 bytes, number of entries: 33
--rw-rw-rw-  2.0 fat       83 b- defN 23-Oct-12 14:29 onlyuserclient/__init__.py
+Zip file size: 35074 bytes, number of entries: 33
+-rw-rw-rw-  2.0 fat       88 b- defN 23-Oct-12 14:09 onlyuserclient/__init__.py
 -rw-rw-rw-  2.0 fat      108 b- defN 21-Dec-19 13:10 onlyuserclient/apps.py
 -rw-rw-rw-  2.0 fat     3115 b- defN 22-Mar-13 02:04 onlyuserclient/exceptions.py
 -rw-rw-rw-  2.0 fat       30 b- defN 22-Mar-13 02:04 onlyuserclient/models.py
 -rw-rw-rw-  2.0 fat     1879 b- defN 23-Oct-12 14:01 onlyuserclient/settings.py
 -rw-rw-rw-  2.0 fat     9535 b- defN 21-Dec-19 13:10 onlyuserclient/viewsets.py
 -rw-rw-rw-  2.0 fat       74 b- defN 22-Mar-13 02:04 onlyuserclient/api/__init__.py
 -rw-rw-rw-  2.0 fat     1146 b- defN 22-Mar-13 02:04 onlyuserclient/api/base.py
@@ -23,13 +23,13 @@
 -rw-rw-rw-  2.0 fat     1879 b- defN 22-Mar-13 02:04 onlyuserclient/middleware/billing.py
 -rw-rw-rw-  2.0 fat     1057 b- defN 21-Dec-19 13:10 onlyuserclient/middleware/onlyuser.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Dec-19 13:10 onlyuserclient/rpc/__init__.py
 -rw-rw-rw-  2.0 fat       21 b- defN 20-Jun-19 04:09 onlyuserclient/serializers/__init__.py
 -rw-rw-rw-  2.0 fat     5855 b- defN 23-Oct-12 14:05 onlyuserclient/serializers/fields.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Mar-13 02:04 onlyuserclient/utils/__init__.py
 -rw-rw-rw-  2.0 fat     1754 b- defN 23-Oct-12 13:36 onlyuserclient/utils/functions.py
--rw-rw-rw-  2.0 fat     1112 b- defN 23-Oct-12 14:31 onlyuserclient-1.2.9.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    21431 b- defN 23-Oct-12 14:31 onlyuserclient-1.2.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Oct-12 14:31 onlyuserclient-1.2.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-Oct-12 14:31 onlyuserclient-1.2.9.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     2930 b- defN 23-Oct-12 14:31 onlyuserclient-1.2.9.dist-info/RECORD
-33 files, 124222 bytes uncompressed, 30272 bytes compressed:  75.6%
+-rw-rw-rw-  2.0 fat     1112 b- defN 23-Oct-12 14:15 onlyuserclient-1.2.9.dev0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    21329 b- defN 23-Oct-12 14:15 onlyuserclient-1.2.9.dev0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Oct-12 14:15 onlyuserclient-1.2.9.dev0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-Oct-12 14:15 onlyuserclient-1.2.9.dev0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     2955 b- defN 23-Oct-12 14:15 onlyuserclient-1.2.9.dev0.dist-info/RECORD
+33 files, 124150 bytes uncompressed, 30230 bytes compressed:  75.7%
```

## zipnote {}

```diff
@@ -78,23 +78,23 @@
 
 Filename: onlyuserclient/utils/__init__.py
 Comment: 
 
 Filename: onlyuserclient/utils/functions.py
 Comment: 
 
-Filename: onlyuserclient-1.2.9.dist-info/LICENSE
+Filename: onlyuserclient-1.2.9.dev0.dist-info/LICENSE
 Comment: 
 
-Filename: onlyuserclient-1.2.9.dist-info/METADATA
+Filename: onlyuserclient-1.2.9.dev0.dist-info/METADATA
 Comment: 
 
-Filename: onlyuserclient-1.2.9.dist-info/WHEEL
+Filename: onlyuserclient-1.2.9.dev0.dist-info/WHEEL
 Comment: 
 
-Filename: onlyuserclient-1.2.9.dist-info/top_level.txt
+Filename: onlyuserclient-1.2.9.dev0.dist-info/top_level.txt
 Comment: 
 
-Filename: onlyuserclient-1.2.9.dist-info/RECORD
+Filename: onlyuserclient-1.2.9.dev0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## onlyuserclient/__init__.py

```diff
@@ -1,6 +1,6 @@
 '''onlyuser 客户端开发包
 '''
 
-__version__='1.2.9'
+__version__='1.2.9.dev0'
 
 VERSION = __version__
```

## Comparing `onlyuserclient-1.2.9.dist-info/LICENSE` & `onlyuserclient-1.2.9.dev0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `onlyuserclient-1.2.9.dist-info/METADATA` & `onlyuserclient-1.2.9.dev0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onlyuserclient
-Version: 1.2.9
+Version: 1.2.9.dev0
 Summary: onlyuser client
 Home-page: https://github.com/tangdyy/onlyuserclient
 Author: Tang dayong
 Author-email: tangdyy@126.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,20 +23,14 @@
 + 角色权限控制，包括数据记录和字段权限控制。
 + 计费相关功能
 
 ## 依赖包
 + django >= 2.0.0
 + djangorestframework >= 3.10.0
 
-## 发布包
-```shell
-python setup.py bdist_wheel
-twine upload -u tangdyy -p Tdy741013 ./dist/*
-```
-
 ## 安装
 + 源码包安装    
 ```shell
 python setup.py install
 ```
 + pip安装  
 ```shell
```

## Comparing `onlyuserclient-1.2.9.dist-info/RECORD` & `onlyuserclient-1.2.9.dev0.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-onlyuserclient/__init__.py,sha256=uZk5yVK2Y1JJF3I2o0SynivMdEsr3Z-8MwKXgkeedmk,83
+onlyuserclient/__init__.py,sha256=WqgaqnOf6N4n13JqcXm0nF0LDQ9E5BMYm_3HCCmgeOc,88
 onlyuserclient/apps.py,sha256=LmXP_dvFSPZ6_LGQMMacfGplw6rts7CO6fGLEI0RxiA,108
 onlyuserclient/exceptions.py,sha256=pG6oIss8Eer801IP6d25xdq-5MUXwN3b5yTsvZTusm4,3115
 onlyuserclient/models.py,sha256=rSUWra3oKaxjQiuj-lQOX4WH2zd5gPwKnJooNwUecZM,30
 onlyuserclient/settings.py,sha256=MGsgBjuEh1J-klbWKOPQfHNAWqveEKhclEpeol7A3VY,1879
 onlyuserclient/viewsets.py,sha256=eK_y8rGK-KubELFPBhwBo1z7_qms8AOIXN8smTzKJOI,9535
 onlyuserclient/api/__init__.py,sha256=tfE4pSeWHXNM88I9pmo9hnztsucTK1bvKyaNp9w_hbE,74
 onlyuserclient/api/base.py,sha256=uDmUTirbMQdz6e1qlawYW9m_vPm6rY-SxBg_YVfpEeg,1146
@@ -22,12 +22,12 @@
 onlyuserclient/middleware/billing.py,sha256=goW2n2IYoqMx19B_hppm-92KhTgDv7j5Dc3Hfv_ASq8,1879
 onlyuserclient/middleware/onlyuser.py,sha256=7XKUQtDwqwmt20gKmTiSthK3KSWnUhbQeOLzi_4ylfs,1057
 onlyuserclient/rpc/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 onlyuserclient/serializers/__init__.py,sha256=EJ8xYx6F3RiAbmCvDEJs1YlalGf6xjn4F20xPVPMQrQ,21
 onlyuserclient/serializers/fields.py,sha256=CteBUOQf91t7CGBOji59x_xShIMuhuX6BHbuJ9bvuO0,5855
 onlyuserclient/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 onlyuserclient/utils/functions.py,sha256=zw9f-CAal1wr5eAWyhGV4-9d4iCAVgSWnTldumIwDZQ,1754
-onlyuserclient-1.2.9.dist-info/LICENSE,sha256=AVviKFjo38UGDPwN18Ry8JgdplTkrwdWN_MUQG026ps,1112
-onlyuserclient-1.2.9.dist-info/METADATA,sha256=HlsqrBsKoI1ZlXjs6ZrF-aXBiWDz2YcvJQiWrjPEGCw,21431
-onlyuserclient-1.2.9.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-onlyuserclient-1.2.9.dist-info/top_level.txt,sha256=szZ8VluvTniv_FeDJe0AIi4MbuRX4COCYRZ4MvnOOzU,15
-onlyuserclient-1.2.9.dist-info/RECORD,,
+onlyuserclient-1.2.9.dev0.dist-info/LICENSE,sha256=AVviKFjo38UGDPwN18Ry8JgdplTkrwdWN_MUQG026ps,1112
+onlyuserclient-1.2.9.dev0.dist-info/METADATA,sha256=ou0U5Cn4V5cuJsZJBqEjkTb_3x1ZBQp9_sY-xPYB9Bg,21329
+onlyuserclient-1.2.9.dev0.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+onlyuserclient-1.2.9.dev0.dist-info/top_level.txt,sha256=szZ8VluvTniv_FeDJe0AIi4MbuRX4COCYRZ4MvnOOzU,15
+onlyuserclient-1.2.9.dev0.dist-info/RECORD,,
```

