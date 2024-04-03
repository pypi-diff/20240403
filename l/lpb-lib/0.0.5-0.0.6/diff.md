# Comparing `tmp/lpb_lib-0.0.5.tar.gz` & `tmp/lpb_lib-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lpb_lib-0.0.5.tar", last modified: Wed Apr  3 13:22:34 2024, max compression
+gzip compressed data, was "lpb_lib-0.0.6.tar", last modified: Wed Apr  3 13:33:03 2024, max compression
```

## Comparing `lpb_lib-0.0.5.tar` & `lpb_lib-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 13:22:34.182755 lpb_lib-0.0.5/
--rw-rw-rw-   0        0        0        0 2024-04-03 09:50:17.000000 lpb_lib-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      573 2024-04-03 13:22:34.180756 lpb_lib-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       83 2024-04-03 09:45:26.000000 lpb_lib-0.0.5/README.md
--rw-rw-rw-   0        0        0     1207 2024-04-03 13:20:54.000000 lpb_lib-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0      623 2024-04-03 13:22:34.187754 lpb_lib-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-03 13:22:34.115095 lpb_lib-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-03 13:22:34.163826 lpb_lib-0.0.5/src/lpb_lib/
--rw-rw-rw-   0        0        0       24 2024-04-03 13:12:40.000000 lpb_lib-0.0.5/src/lpb_lib/__init__.py
--rw-rw-rw-   0        0        0     1530 2024-04-03 13:21:41.000000 lpb_lib-0.0.5/src/lpb_lib/big_query.py
--rw-rw-rw-   0        0        0      367 2024-04-03 13:13:33.000000 lpb_lib-0.0.5/src/lpb_lib/compute_log.py
-drwxrwxrwx   0        0        0        0 2024-04-03 13:22:34.178754 lpb_lib-0.0.5/src/lpb_lib.egg-info/
--rw-rw-rw-   0        0        0      573 2024-04-03 13:22:32.000000 lpb_lib-0.0.5/src/lpb_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-04-03 13:22:33.000000 lpb_lib-0.0.5/src/lpb_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 13:22:32.000000 lpb_lib-0.0.5/src/lpb_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-03 13:22:32.000000 lpb_lib-0.0.5/src/lpb_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 13:33:03.497618 lpb_lib-0.0.6/
+-rw-rw-rw-   0        0        0        0 2024-04-03 09:50:17.000000 lpb_lib-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      668 2024-04-03 13:33:03.496660 lpb_lib-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2024-04-03 13:27:03.000000 lpb_lib-0.0.6/README.md
+-rw-rw-rw-   0        0        0     1207 2024-04-03 13:20:54.000000 lpb_lib-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0      626 2024-04-03 13:33:03.503986 lpb_lib-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 13:33:03.406110 lpb_lib-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 13:33:03.449791 lpb_lib-0.0.6/src/lpb_lib/
+-rw-rw-rw-   0        0        0        0 2024-04-03 13:32:04.000000 lpb_lib-0.0.6/src/lpb_lib/__init__.py
+-rw-rw-rw-   0        0        0     1530 2024-04-03 13:21:41.000000 lpb_lib-0.0.6/src/lpb_lib/big_query.py
+-rw-rw-rw-   0        0        0      367 2024-04-03 13:13:33.000000 lpb_lib-0.0.6/src/lpb_lib/compute_log.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:33:03.487831 lpb_lib-0.0.6/src/lpb_lib.egg-info/
+-rw-rw-rw-   0        0        0      668 2024-04-03 13:33:02.000000 lpb_lib-0.0.6/src/lpb_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-04-03 13:33:02.000000 lpb_lib-0.0.6/src/lpb_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 13:33:02.000000 lpb_lib-0.0.6/src/lpb_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-03 13:33:02.000000 lpb_lib-0.0.6/src/lpb_lib.egg-info/top_level.txt
```

### Comparing `lpb_lib-0.0.5/pyproject.toml` & `lpb_lib-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lpb_lib-0.0.5/setup.cfg` & `lpb_lib-0.0.6/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 7062 5f6c 6962 0d0a 7665 7273   = lpb_lib..vers
-00000020: 696f 6e20 3d20 302e 302e 350d 0a61 7574  ion = 0.0.5..aut
-00000030: 686f 7220 3d20 6661 6a69 7461 7333 300d  hor = fajitas30.
-00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
-00000050: 6d61 7869 6d65 2e72 656e 6163 406c 6570  maxime.renac@lep
-00000060: 6574 6974 6261 6c6c 6f6e 2e63 6f6d 0d0a  etitballon.com..
-00000070: 6465 7363 7269 7074 696f 6e20 3d20 5468  description = Th
-00000080: 6973 2070 6163 6b61 6765 2063 6f6e 7461  is package conta
-00000090: 696e 7320 746f 6f6c 7320 7468 6174 2077  ins tools that w
-000000a0: 696c 6c20 6865 6c70 206d 6520 746f 2064  ill help me to d
-000000b0: 6576 656c 6f70 206d 7920 7072 6f6a 6563  evelop my projec
-000000c0: 7473 0d0a 6c6f 6e67 5f64 6573 6372 6970  ts..long_descrip
-000000d0: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
-000000e0: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
-000000f0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
-00000100: 5f74 7970 6520 3d20 7465 7874 2f6d 6172  _type = text/mar
-00000110: 6b64 6f77 6e0d 0a75 726c 203d 2068 7474  kdown..url = htt
-00000120: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000130: 4661 6a69 7461 7330 3830 3930 2f6c 7062  Fajitas08090/lpb
-00000140: 5f6c 6962 0d0a 636c 6173 7369 6669 6572  _lib..classifier
-00000150: 7320 3d20 0d0a 0950 726f 6772 616d 6d69  s = ...Programmi
-00000160: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000170: 7974 686f 6e20 3a3a 2033 0d0a 094c 6963  ython :: 3...Lic
-00000180: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
-00000190: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
-000001a0: 6e73 650d 0a09 4f70 6572 6174 696e 6720  nse...Operating 
-000001b0: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
-000001c0: 6570 656e 6465 6e74 0d0a 0d0a 5b6f 7074  ependent....[opt
-000001d0: 696f 6e73 5d0d 0a70 6163 6b61 6765 5f64  ions]..package_d
-000001e0: 6972 203d 200d 0a09 3d20 7372 630d 0a70  ir = ...= src..p
-000001f0: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
-00000200: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
-00000210: 203d 203e 3d33 2e31 320d 0a0d 0a5b 6f70   = >=3.12....[op
-00000220: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
-00000230: 696e 645d 0d0a 7768 6572 6520 3d20 7372  ind]..where = sr
-00000240: 630d 0a0d 0a5b 6567 675f 696e 666f 5d0d  c....[egg_info].
-00000250: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
-00000260: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
+00000020: 696f 6e20 3d20 302e 302e 360d 0a61 7574  ion = 0.0.6..aut
+00000030: 686f 7220 3d20 4d61 7869 6d65 2052 656e  hor = Maxime Ren
+00000040: 6163 0d0a 6175 7468 6f72 5f65 6d61 696c  ac..author_email
+00000050: 203d 206d 6178 696d 652e 7265 6e61 6340   = maxime.renac@
+00000060: 6c65 7065 7469 7462 616c 6c6f 6e2e 636f  lepetitballon.co
+00000070: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
+00000080: 2054 6869 7320 7061 636b 6167 6520 636f   This package co
+00000090: 6e74 6169 6e73 2074 6f6f 6c73 2074 6861  ntains tools tha
+000000a0: 7420 7769 6c6c 2068 656c 7020 6d65 2074  t will help me t
+000000b0: 6f20 6465 7665 6c6f 7020 6d79 2070 726f  o develop my pro
+000000c0: 6a65 6374 730d 0a6c 6f6e 675f 6465 7363  jects..long_desc
+000000d0: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
+000000e0: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
+000000f0: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
+00000100: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
+00000110: 6d61 726b 646f 776e 0d0a 7572 6c20 3d20  markdown..url = 
+00000120: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000130: 6f6d 2f46 616a 6974 6173 3038 3039 302f  om/Fajitas08090/
+00000140: 6c70 625f 6c69 620d 0a63 6c61 7373 6966  lpb_lib..classif
+00000150: 6965 7273 203d 200d 0a09 5072 6f67 7261  iers = ...Progra
+00000160: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000170: 3a20 5079 7468 6f6e 203a 3a20 330d 0a09  : Python :: 3...
+00000180: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
+00000190: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
+000001a0: 6963 656e 7365 0d0a 094f 7065 7261 7469  icense...Operati
+000001b0: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
+000001c0: 496e 6465 7065 6e64 656e 740d 0a0d 0a5b  Independent....[
+000001d0: 6f70 7469 6f6e 735d 0d0a 7061 636b 6167  options]..packag
+000001e0: 655f 6469 7220 3d20 0d0a 093d 2073 7263  e_dir = ...= src
+000001f0: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
+00000200: 643a 0d0a 7079 7468 6f6e 5f72 6571 7569  d:..python_requi
+00000210: 7265 7320 3d20 3e3d 332e 3132 0d0a 0d0a  res = >=3.12....
+00000220: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
+00000230: 732e 6669 6e64 5d0d 0a77 6865 7265 203d  s.find]..where =
+00000240: 2073 7263 0d0a 0d0a 5b65 6767 5f69 6e66   src....[egg_inf
+00000250: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
+00000260: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
+00000270: 0d0a                                     ..
```

### Comparing `lpb_lib-0.0.5/src/lpb_lib/big_query.py` & `lpb_lib-0.0.6/src/lpb_lib/big_query.py`

 * *Files identical despite different names*

