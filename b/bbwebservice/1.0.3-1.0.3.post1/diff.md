# Comparing `tmp/bbwebservice-1.0.3.tar.gz` & `tmp/bbwebservice-1.0.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbwebservice-1.0.3.tar", last modified: Sat Mar 30 23:51:18 2024, max compression
+gzip compressed data, was "bbwebservice-1.0.3.post1.tar", last modified: Wed Apr  3 16:28:51 2024, max compression
```

## Comparing `bbwebservice-1.0.3.tar` & `bbwebservice-1.0.3.post1.tar`

### file list

```diff
@@ -1,21 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 23:51:18.531366 bbwebservice-1.0.3/
--rw-rw-rw-   0        0        0     1092 2022-11-21 21:52:54.000000 bbwebservice-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     5184 2024-03-30 23:51:18.396065 bbwebservice-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4799 2024-03-30 23:50:09.000000 bbwebservice-1.0.3/README.md
--rw-rw-rw-   0        0        0      108 2022-11-21 16:45:12.000000 bbwebservice-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      523 2024-03-30 23:51:18.541369 bbwebservice-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-30 23:51:14.363462 bbwebservice-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-03-30 23:51:16.090869 bbwebservice-1.0.3/src/bbwebservice/
--rw-rw-rw-   0        0        0     1892 2024-03-21 01:05:32.000000 bbwebservice-1.0.3/src/bbwebservice/__init__.py
--rw-rw-rw-   0        0        0      796 2024-03-29 16:07:29.000000 bbwebservice-1.0.3/src/bbwebservice/app_utils.py
--rw-rw-rw-   0        0        0     1949 2022-11-22 10:00:46.000000 bbwebservice-1.0.3/src/bbwebservice/config_loader.py
--rw-rw-rw-   0        0        0     4970 2024-03-29 19:35:56.000000 bbwebservice-1.0.3/src/bbwebservice/core.py
--rw-rw-rw-   0        0        0    30227 2024-03-29 19:57:59.000000 bbwebservice-1.0.3/src/bbwebservice/http_parser.py
--rw-rw-rw-   0        0        0     1009 2023-09-09 12:34:49.000000 bbwebservice-1.0.3/src/bbwebservice/special_media_type.py
--rw-rw-rw-   0        0        0     3328 2024-03-30 23:49:49.000000 bbwebservice-1.0.3/src/bbwebservice/url_utils.py
--rw-rw-rw-   0        0        0     9736 2024-03-29 19:45:30.000000 bbwebservice-1.0.3/src/bbwebservice/webserver.py
-drwxrwxrwx   0        0        0        0 2024-03-30 23:51:18.380060 bbwebservice-1.0.3/src/bbwebservice.egg-info/
--rw-rw-rw-   0        0        0     5184 2024-03-30 23:51:14.000000 bbwebservice-1.0.3/src/bbwebservice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      451 2024-03-30 23:51:14.000000 bbwebservice-1.0.3/src/bbwebservice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 23:51:14.000000 bbwebservice-1.0.3/src/bbwebservice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-03-30 23:51:14.000000 bbwebservice-1.0.3/src/bbwebservice.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 16:28:51.121047 bbwebservice-1.0.3.post1/
+-rw-rw-rw-   0        0        0     1092 2022-11-21 21:52:54.000000 bbwebservice-1.0.3.post1/LICENSE
+-rw-rw-rw-   0        0        0     5190 2024-04-03 16:28:50.983978 bbwebservice-1.0.3.post1/PKG-INFO
+-rw-rw-rw-   0        0        0     4799 2024-03-30 23:50:09.000000 bbwebservice-1.0.3.post1/README.md
+-rw-rw-rw-   0        0        0      108 2022-11-21 16:45:12.000000 bbwebservice-1.0.3.post1/pyproject.toml
+-rw-rw-rw-   0        0        0      525 2024-04-03 16:28:51.131049 bbwebservice-1.0.3.post1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 16:28:50.179751 bbwebservice-1.0.3.post1/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 16:28:50.968930 bbwebservice-1.0.3.post1/src/bbwebservice.egg-info/
+-rw-rw-rw-   0        0        0     5190 2024-04-03 16:28:49.000000 bbwebservice-1.0.3.post1/src/bbwebservice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-04-03 16:28:50.000000 bbwebservice-1.0.3.post1/src/bbwebservice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 16:28:50.000000 bbwebservice-1.0.3.post1/src/bbwebservice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 16:28:50.000000 bbwebservice-1.0.3.post1/src/bbwebservice.egg-info/top_level.txt
```

### Comparing `bbwebservice-1.0.3/LICENSE` & `bbwebservice-1.0.3.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `bbwebservice-1.0.3/PKG-INFO` & `bbwebservice-1.0.3.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbwebservice
-Version: 1.0.3
+Version: 1.0.3.post1
 Summary: A bare bone webserver
 Author: Lukas
 Author-email: lukasogwalker@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `bbwebservice-1.0.3/README.md` & `bbwebservice-1.0.3.post1/README.md`

 * *Files identical despite different names*

### Comparing `bbwebservice-1.0.3/setup.cfg` & `bbwebservice-1.0.3.post1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 6277 6562 7365 7276 6963 650d   = bbwebservice.
 00000020: 0a76 6572 7369 6f6e 203d 2031 2e30 2e33  .version = 1.0.3
-00000030: 0d0a 6175 7468 6f72 203d 204c 756b 6173  ..author = Lukas
-00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
-00000050: 206c 756b 6173 6f67 7761 6c6b 6572 4067   lukasogwalker@g
-00000060: 6d61 696c 2e63 6f6d 0d0a 6465 7363 7269  mail.com..descri
-00000070: 7074 696f 6e20 3d20 4120 6261 7265 2062  ption = A bare b
-00000080: 6f6e 6520 7765 6273 6572 7665 720d 0a6c  one webserver..l
-00000090: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
-000000a0: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
-000000b0: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
-000000c0: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
-000000d0: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
-000000e0: 0d0a 636c 6173 7369 6669 6572 7320 3d20  ..classifiers = 
-000000f0: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-00000100: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000110: 6e20 3a3a 2033 0d0a 094c 6963 656e 7365  n :: 3...License
-00000120: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-00000130: 203a 3a20 4d49 5420 4c69 6365 6e73 650d   :: MIT License.
-00000140: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
-00000150: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
-00000160: 6465 6e74 0d0a 0d0a 5b6f 7074 696f 6e73  dent....[options
-00000170: 5d0d 0a70 6163 6b61 6765 5f64 6972 203d  ]..package_dir =
-00000180: 200d 0a09 3d20 7372 630d 0a70 6163 6b61   ...= src..packa
-00000190: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
-000001a0: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
-000001b0: 3d33 2e31 300d 0a0d 0a5b 6f70 7469 6f6e  =3.10....[option
-000001c0: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
-000001d0: 0d0a 7768 6572 6520 3d20 7372 630d 0a0d  ..where = src...
-000001e0: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
-000001f0: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
-00000200: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
+00000030: 2d31 0d0a 6175 7468 6f72 203d 204c 756b  -1..author = Luk
+00000040: 6173 0d0a 6175 7468 6f72 5f65 6d61 696c  as..author_email
+00000050: 203d 206c 756b 6173 6f67 7761 6c6b 6572   = lukasogwalker
+00000060: 4067 6d61 696c 2e63 6f6d 0d0a 6465 7363  @gmail.com..desc
+00000070: 7269 7074 696f 6e20 3d20 4120 6261 7265  ription = A bare
+00000080: 2062 6f6e 6520 7765 6273 6572 7665 720d   bone webserver.
+00000090: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
+000000a0: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
+000000b0: 2e6d 640d 0a6c 6f6e 675f 6465 7363 7269  .md..long_descri
+000000c0: 7074 696f 6e5f 636f 6e74 656e 745f 7479  ption_content_ty
+000000d0: 7065 203d 2074 6578 742f 6d61 726b 646f  pe = text/markdo
+000000e0: 776e 0d0a 636c 6173 7369 6669 6572 7320  wn..classifiers 
+000000f0: 3d20 0d0a 0950 726f 6772 616d 6d69 6e67  = ...Programming
+00000100: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000110: 686f 6e20 3a3a 2033 0d0a 094c 6963 656e  hon :: 3...Licen
+00000120: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
+00000130: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
+00000140: 650d 0a09 4f70 6572 6174 696e 6720 5379  e...Operating Sy
+00000150: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
+00000160: 656e 6465 6e74 0d0a 0d0a 5b6f 7074 696f  endent....[optio
+00000170: 6e73 5d0d 0a70 6163 6b61 6765 5f64 6972  ns]..package_dir
+00000180: 203d 200d 0a09 3d20 7372 630d 0a70 6163   = ...= src..pac
+00000190: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a70  kages = find:..p
+000001a0: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
+000001b0: 203e 3d33 2e31 300d 0a0d 0a5b 6f70 7469   >=3.10....[opti
+000001c0: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
+000001d0: 645d 0d0a 7768 6572 6520 3d20 7372 630d  d]..where = src.
+000001e0: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
+000001f0: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
+00000200: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

### Comparing `bbwebservice-1.0.3/src/bbwebservice.egg-info/PKG-INFO` & `bbwebservice-1.0.3.post1/src/bbwebservice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbwebservice
-Version: 1.0.3
+Version: 1.0.3.post1
 Summary: A bare bone webserver
 Author: Lukas
 Author-email: lukasogwalker@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

