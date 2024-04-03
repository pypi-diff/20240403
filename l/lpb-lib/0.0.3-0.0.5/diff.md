# Comparing `tmp/lpb_lib-0.0.3.tar.gz` & `tmp/lpb_lib-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lpb_lib-0.0.3.tar", last modified: Wed Apr  3 13:02:16 2024, max compression
+gzip compressed data, was "lpb_lib-0.0.5.tar", last modified: Wed Apr  3 13:22:34 2024, max compression
```

## Comparing `lpb_lib-0.0.3.tar` & `lpb_lib-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 13:02:16.398530 lpb_lib-0.0.3/
--rw-rw-rw-   0        0        0        0 2024-04-03 09:50:17.000000 lpb_lib-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      564 2024-04-03 13:02:16.397530 lpb_lib-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       83 2024-04-03 09:45:26.000000 lpb_lib-0.0.3/README.md
--rw-rw-rw-   0        0        0      156 2024-04-03 13:02:05.000000 lpb_lib-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      614 2024-04-03 13:02:16.412563 lpb_lib-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-03 13:02:16.331054 lpb_lib-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-03 13:02:16.359532 lpb_lib-0.0.3/src/lpb_lib/
--rw-rw-rw-   0        0        0        0 2024-04-03 09:52:21.000000 lpb_lib-0.0.3/src/lpb_lib/__init__.py
--rw-rw-rw-   0        0        0       22 2024-04-03 09:57:22.000000 lpb_lib-0.0.3/src/lpb_lib/big_query.py
-drwxrwxrwx   0        0        0        0 2024-04-03 13:02:16.393529 lpb_lib-0.0.3/src/lpb_lib.egg-info/
--rw-rw-rw-   0        0        0      564 2024-04-03 13:02:16.000000 lpb_lib-0.0.3/src/lpb_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2024-04-03 13:02:16.000000 lpb_lib-0.0.3/src/lpb_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 13:02:16.000000 lpb_lib-0.0.3/src/lpb_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-03 13:02:16.000000 lpb_lib-0.0.3/src/lpb_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 13:22:34.182755 lpb_lib-0.0.5/
+-rw-rw-rw-   0        0        0        0 2024-04-03 09:50:17.000000 lpb_lib-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      573 2024-04-03 13:22:34.180756 lpb_lib-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       83 2024-04-03 09:45:26.000000 lpb_lib-0.0.5/README.md
+-rw-rw-rw-   0        0        0     1207 2024-04-03 13:20:54.000000 lpb_lib-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      623 2024-04-03 13:22:34.187754 lpb_lib-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 13:22:34.115095 lpb_lib-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 13:22:34.163826 lpb_lib-0.0.5/src/lpb_lib/
+-rw-rw-rw-   0        0        0       24 2024-04-03 13:12:40.000000 lpb_lib-0.0.5/src/lpb_lib/__init__.py
+-rw-rw-rw-   0        0        0     1530 2024-04-03 13:21:41.000000 lpb_lib-0.0.5/src/lpb_lib/big_query.py
+-rw-rw-rw-   0        0        0      367 2024-04-03 13:13:33.000000 lpb_lib-0.0.5/src/lpb_lib/compute_log.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:22:34.178754 lpb_lib-0.0.5/src/lpb_lib.egg-info/
+-rw-rw-rw-   0        0        0      573 2024-04-03 13:22:32.000000 lpb_lib-0.0.5/src/lpb_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-04-03 13:22:33.000000 lpb_lib-0.0.5/src/lpb_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 13:22:32.000000 lpb_lib-0.0.5/src/lpb_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-03 13:22:32.000000 lpb_lib-0.0.5/src/lpb_lib.egg-info/top_level.txt
```

### Comparing `lpb_lib-0.0.3/PKG-INFO` & `lpb_lib-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: lpb_lib
-Version: 0.0.3
+Version: 0.0.5
 Summary: This package contains tools that will help me to develop my projects
 Home-page: https://github.com/Fajitas08090/lpb_lib
 Author: fajitas30
-Author-email: maxime.renac@gmail.com
+Author-email: maxime.renac@lepetitballon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lpb_lib
 This repo allows me to deploy the tools I need for my projects at LPB.
```

### Comparing `lpb_lib-0.0.3/setup.cfg` & `lpb_lib-0.0.5/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 7062 5f6c 6962 0d0a 7665 7273   = lpb_lib..vers
-00000020: 696f 6e20 3d20 302e 302e 330d 0a61 7574  ion = 0.0.3..aut
+00000020: 696f 6e20 3d20 302e 302e 350d 0a61 7574  ion = 0.0.5..aut
 00000030: 686f 7220 3d20 6661 6a69 7461 7333 300d  hor = fajitas30.
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
-00000050: 6d61 7869 6d65 2e72 656e 6163 4067 6d61  maxime.renac@gma
-00000060: 696c 2e63 6f6d 0d0a 6465 7363 7269 7074  il.com..descript
-00000070: 696f 6e20 3d20 5468 6973 2070 6163 6b61  ion = This packa
-00000080: 6765 2063 6f6e 7461 696e 7320 746f 6f6c  ge contains tool
-00000090: 7320 7468 6174 2077 696c 6c20 6865 6c70  s that will help
-000000a0: 206d 6520 746f 2064 6576 656c 6f70 206d   me to develop m
-000000b0: 7920 7072 6f6a 6563 7473 0d0a 6c6f 6e67  y projects..long
-000000c0: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
-000000d0: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
-000000e0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-000000f0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
-00000100: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
-00000110: 726c 203d 2068 7474 7073 3a2f 2f67 6974  rl = https://git
-00000120: 6875 622e 636f 6d2f 4661 6a69 7461 7330  hub.com/Fajitas0
-00000130: 3830 3930 2f6c 7062 5f6c 6962 0d0a 636c  8090/lpb_lib..cl
-00000140: 6173 7369 6669 6572 7320 3d20 0d0a 0950  assifiers = ...P
-00000150: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000160: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000170: 2033 0d0a 094c 6963 656e 7365 203a 3a20   3...License :: 
-00000180: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
-00000190: 4d49 5420 4c69 6365 6e73 650d 0a09 4f70  MIT License...Op
-000001a0: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
-000001b0: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
-000001c0: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a70  ....[options]..p
-000001d0: 6163 6b61 6765 5f64 6972 203d 200d 0a09  ackage_dir = ...
-000001e0: 3d20 7372 630d 0a70 6163 6b61 6765 7320  = src..packages 
-000001f0: 3d20 6669 6e64 3a0d 0a70 7974 686f 6e5f  = find:..python_
-00000200: 7265 7175 6972 6573 203d 203e 3d33 2e36  requires = >=3.6
-00000210: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
-00000220: 6b61 6765 732e 6669 6e64 5d0d 0a77 6865  kages.find]..whe
-00000230: 7265 203d 2073 7263 0d0a 0d0a 5b65 6767  re = src....[egg
-00000240: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-00000250: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-00000260: 2030 0d0a 0d0a                            0....
+00000050: 6d61 7869 6d65 2e72 656e 6163 406c 6570  maxime.renac@lep
+00000060: 6574 6974 6261 6c6c 6f6e 2e63 6f6d 0d0a  etitballon.com..
+00000070: 6465 7363 7269 7074 696f 6e20 3d20 5468  description = Th
+00000080: 6973 2070 6163 6b61 6765 2063 6f6e 7461  is package conta
+00000090: 696e 7320 746f 6f6c 7320 7468 6174 2077  ins tools that w
+000000a0: 696c 6c20 6865 6c70 206d 6520 746f 2064  ill help me to d
+000000b0: 6576 656c 6f70 206d 7920 7072 6f6a 6563  evelop my projec
+000000c0: 7473 0d0a 6c6f 6e67 5f64 6573 6372 6970  ts..long_descrip
+000000d0: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
+000000e0: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
+000000f0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
+00000100: 5f74 7970 6520 3d20 7465 7874 2f6d 6172  _type = text/mar
+00000110: 6b64 6f77 6e0d 0a75 726c 203d 2068 7474  kdown..url = htt
+00000120: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000130: 4661 6a69 7461 7330 3830 3930 2f6c 7062  Fajitas08090/lpb
+00000140: 5f6c 6962 0d0a 636c 6173 7369 6669 6572  _lib..classifier
+00000150: 7320 3d20 0d0a 0950 726f 6772 616d 6d69  s = ...Programmi
+00000160: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000170: 7974 686f 6e20 3a3a 2033 0d0a 094c 6963  ython :: 3...Lic
+00000180: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
+00000190: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
+000001a0: 6e73 650d 0a09 4f70 6572 6174 696e 6720  nse...Operating 
+000001b0: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
+000001c0: 6570 656e 6465 6e74 0d0a 0d0a 5b6f 7074  ependent....[opt
+000001d0: 696f 6e73 5d0d 0a70 6163 6b61 6765 5f64  ions]..package_d
+000001e0: 6972 203d 200d 0a09 3d20 7372 630d 0a70  ir = ...= src..p
+000001f0: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
+00000200: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
+00000210: 203d 203e 3d33 2e31 320d 0a0d 0a5b 6f70   = >=3.12....[op
+00000220: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
+00000230: 696e 645d 0d0a 7768 6572 6520 3d20 7372  ind]..where = sr
+00000240: 630d 0a0d 0a5b 6567 675f 696e 666f 5d0d  c....[egg_info].
+00000250: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
+00000260: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
```

### Comparing `lpb_lib-0.0.3/src/lpb_lib.egg-info/PKG-INFO` & `lpb_lib-0.0.5/src/lpb_lib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: lpb_lib
-Version: 0.0.3
+Version: 0.0.5
 Summary: This package contains tools that will help me to develop my projects
 Home-page: https://github.com/Fajitas08090/lpb_lib
 Author: fajitas30
-Author-email: maxime.renac@gmail.com
+Author-email: maxime.renac@lepetitballon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lpb_lib
 This repo allows me to deploy the tools I need for my projects at LPB.
```

