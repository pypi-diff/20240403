# Comparing `tmp/mdof-0.0.8.tar.gz` & `tmp/mdof-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdof-0.0.8.tar", last modified: Mon Jan 15 15:56:39 2024, max compression
+gzip compressed data, was "mdof-0.0.9.tar", last modified: Mon Jan 22 05:16:13 2024, max compression
```

## Comparing `mdof-0.0.8.tar` & `mdof-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0 xstal     (1000) xstal     (1000)        0 2024-01-16 06:10:17.173786 mdof-0.0.8/
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)     1327 2023-10-31 00:35:00.000000 mdof-0.0.8/LICENSE.txt
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)     3343 2024-01-16 06:10:17.167455 mdof-0.0.8/PKG-INFO
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)     1752 2024-01-16 05:38:26.000000 mdof-0.0.8/README.md
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)     1622 2024-01-16 06:09:39.000000 mdof-0.0.8/pyproject.toml
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)       38 2024-01-16 06:10:17.173786 mdof-0.0.8/setup.cfg
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)       98 2023-10-31 00:35:02.000000 mdof-0.0.8/setup.py
-drwxrwxrwx   0 xstal     (1000) xstal     (1000)        0 2024-01-16 06:10:16.663327 mdof-0.0.8/src/
-drwxrwxrwx   0 xstal     (1000) xstal     (1000)        0 2024-01-16 06:10:16.936015 mdof-0.0.8/src/mdof/
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)     3651 2023-10-31 00:35:02.000000 mdof-0.0.8/src/mdof/__init__.py
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)     9072 2024-01-07 00:20:58.000000 mdof-0.0.8/src/mdof/__main__.py
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)     2602 2023-10-31 00:35:02.000000 mdof-0.0.8/src/mdof/macro.py
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)     3923 2023-10-31 00:35:02.000000 mdof-0.0.8/src/mdof/markov.py
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)     5052 2023-12-28 18:04:06.000000 mdof-0.0.8/src/mdof/modal.py
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)      919 2023-10-31 00:35:02.000000 mdof-0.0.8/src/mdof/numerics.py
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)    14033 2023-10-31 00:35:02.000000 mdof-0.0.8/src/mdof/realize.py
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)     1814 2023-10-31 00:35:02.000000 mdof-0.0.8/src/mdof/system.py
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)     5655 2023-12-30 02:54:13.000000 mdof-0.0.8/src/mdof/transform.py
-drwxrwxrwx   0 xstal     (1000) xstal     (1000)        0 2024-01-16 06:10:17.141098 mdof-0.0.8/src/mdof/utilities/
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)      148 2023-10-31 00:35:02.000000 mdof-0.0.8/src/mdof/utilities/__init__.py
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)     1192 2023-10-31 00:35:02.000000 mdof-0.0.8/src/mdof/utilities/config.py
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)     7456 2023-10-31 00:35:02.000000 mdof-0.0.8/src/mdof/utilities/printing.py
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)     1202 2023-10-31 00:35:02.000000 mdof-0.0.8/src/mdof/utilities/testing.py
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)     5374 2023-10-31 00:35:02.000000 mdof-0.0.8/src/mdof/validation.py
-drwxrwxrwx   0 xstal     (1000) xstal     (1000)        0 2024-01-16 06:10:17.157146 mdof-0.0.8/src/mdof.egg-info/
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)     3343 2024-01-16 06:10:16.000000 mdof-0.0.8/src/mdof.egg-info/PKG-INFO
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)      562 2024-01-16 06:10:16.000000 mdof-0.0.8/src/mdof.egg-info/SOURCES.txt
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)        1 2024-01-16 06:10:16.000000 mdof-0.0.8/src/mdof.egg-info/dependency_links.txt
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)       44 2024-01-16 06:10:16.000000 mdof-0.0.8/src/mdof.egg-info/entry_points.txt
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)       71 2024-01-16 06:10:16.000000 mdof-0.0.8/src/mdof.egg-info/requires.txt
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)        5 2024-01-16 06:10:16.000000 mdof-0.0.8/src/mdof.egg-info/top_level.txt
+drwxrwxrwx   0 xstal     (1000) xstal     (1000)        0 2024-01-22 05:16:13.092119 mdof-0.0.9/
+-rwxrwxrwx   0 xstal     (1000) xstal     (1000)     1327 2023-10-31 00:35:00.000000 mdof-0.0.9/LICENSE.txt
+-rwxrwxrwx   0 xstal     (1000) xstal     (1000)     4047 2024-01-22 05:16:13.075321 mdof-0.0.9/PKG-INFO
+-rwxrwxrwx   0 xstal     (1000) xstal     (1000)     2483 2024-01-16 07:04:02.000000 mdof-0.0.9/README.md
+-rwxrwxrwx   0 xstal     (1000) xstal     (1000)     1621 2024-01-22 05:16:05.000000 mdof-0.0.9/pyproject.toml
+-rwxrwxrwx   0 xstal     (1000) xstal     (1000)       38 2024-01-22 05:16:13.092119 mdof-0.0.9/setup.cfg
+-rwxrwxrwx   0 xstal     (1000) xstal     (1000)       98 2023-10-31 00:35:02.000000 mdof-0.0.9/setup.py
+drwxrwxrwx   0 xstal     (1000) xstal     (1000)        0 2024-01-22 05:16:12.611878 mdof-0.0.9/src/
+drwxrwxrwx   0 xstal     (1000) xstal     (1000)        0 2024-01-22 05:16:12.858290 mdof-0.0.9/src/mdof/
+-rwxrwxrwx   0 xstal     (1000) xstal     (1000)     3651 2023-10-31 00:35:02.000000 mdof-0.0.9/src/mdof/__init__.py
+-rwxrwxrwx   0 xstal     (1000) xstal     (1000)     9072 2024-01-07 00:20:58.000000 mdof-0.0.9/src/mdof/__main__.py
+-rwxrwxrwx   0 xstal     (1000) xstal     (1000)     2602 2023-10-31 00:35:02.000000 mdof-0.0.9/src/mdof/macro.py
+-rwxrwxrwx   0 xstal     (1000) xstal     (1000)     3923 2023-10-31 00:35:02.000000 mdof-0.0.9/src/mdof/markov.py
+-rwxrwxrwx   0 xstal     (1000) xstal     (1000)     5052 2023-12-28 18:04:06.000000 mdof-0.0.9/src/mdof/modal.py
+-rwxrwxrwx   0 xstal     (1000) xstal     (1000)      919 2023-10-31 00:35:02.000000 mdof-0.0.9/src/mdof/numerics.py
+-rwxrwxrwx   0 xstal     (1000) xstal     (1000)    14033 2023-10-31 00:35:02.000000 mdof-0.0.9/src/mdof/realize.py
+-rwxrwxrwx   0 xstal     (1000) xstal     (1000)     1814 2023-10-31 00:35:02.000000 mdof-0.0.9/src/mdof/system.py
+-rwxrwxrwx   0 xstal     (1000) xstal     (1000)     5655 2023-12-30 02:54:13.000000 mdof-0.0.9/src/mdof/transform.py
+drwxrwxrwx   0 xstal     (1000) xstal     (1000)        0 2024-01-22 05:16:13.044652 mdof-0.0.9/src/mdof/utilities/
+-rwxrwxrwx   0 xstal     (1000) xstal     (1000)      148 2023-10-31 00:35:02.000000 mdof-0.0.9/src/mdof/utilities/__init__.py
+-rwxrwxrwx   0 xstal     (1000) xstal     (1000)     1192 2023-10-31 00:35:02.000000 mdof-0.0.9/src/mdof/utilities/config.py
+-rwxrwxrwx   0 xstal     (1000) xstal     (1000)     9977 2024-01-22 02:43:12.000000 mdof-0.0.9/src/mdof/utilities/printing.py
+-rwxrwxrwx   0 xstal     (1000) xstal     (1000)     1202 2023-10-31 00:35:02.000000 mdof-0.0.9/src/mdof/utilities/testing.py
+-rwxrwxrwx   0 xstal     (1000) xstal     (1000)     5374 2023-10-31 00:35:02.000000 mdof-0.0.9/src/mdof/validation.py
+drwxrwxrwx   0 xstal     (1000) xstal     (1000)        0 2024-01-22 05:16:13.075321 mdof-0.0.9/src/mdof.egg-info/
+-rwxrwxrwx   0 xstal     (1000) xstal     (1000)     4047 2024-01-22 05:16:12.000000 mdof-0.0.9/src/mdof.egg-info/PKG-INFO
+-rwxrwxrwx   0 xstal     (1000) xstal     (1000)      562 2024-01-22 05:16:12.000000 mdof-0.0.9/src/mdof.egg-info/SOURCES.txt
+-rwxrwxrwx   0 xstal     (1000) xstal     (1000)        1 2024-01-22 05:16:12.000000 mdof-0.0.9/src/mdof.egg-info/dependency_links.txt
+-rwxrwxrwx   0 xstal     (1000) xstal     (1000)       44 2024-01-22 05:16:12.000000 mdof-0.0.9/src/mdof.egg-info/entry_points.txt
+-rwxrwxrwx   0 xstal     (1000) xstal     (1000)       71 2024-01-22 05:16:12.000000 mdof-0.0.9/src/mdof.egg-info/requires.txt
+-rwxrwxrwx   0 xstal     (1000) xstal     (1000)        5 2024-01-22 05:16:12.000000 mdof-0.0.9/src/mdof.egg-info/top_level.txt
```

### Comparing `mdof-0.0.8/LICENSE.txt` & `mdof-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mdof-0.0.8/PKG-INFO` & `mdof-0.0.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6d64 6f66  : 2.1.Name: mdof
-00000020: 0a56 6572 7369 6f6e 3a20 302e 302e 380a  .Version: 0.0.8.
+00000020: 0a56 6572 7369 6f6e 3a20 302e 302e 390a  .Version: 0.0.9.
 00000030: 5375 6d6d 6172 793a 2046 6173 7420 616e  Summary: Fast an
 00000040: 6420 6672 6965 6e64 6c79 2073 7973 7465  d friendly syste
 00000050: 6d20 6964 656e 7469 6669 6361 7469 6f6e  m identification
 00000060: 2066 6f72 2073 7472 7563 7475 7265 732e   for structures.
 00000070: 0a41 7574 686f 722d 656d 6169 6c3a 2043  .Author-email: C
 00000080: 6872 7973 7461 6c20 4368 6572 6e20 3c35  hrystal Chern <5
 00000090: 3238 3933 3436 372b 6368 7279 7374 616c  2893467+chrystal
@@ -112,98 +112,142 @@
 000006f0: 6722 2077 6964 7468 3d22 3235 3070 7822  g" width="250px"
 00000700: 2061 6c74 3d22 6d64 6f66 206c 6f67 6f22   alt="mdof logo"
 00000710: 3e0a 0a46 6173 7420 616e 6420 6672 6965  >..Fast and frie
 00000720: 6e64 6c79 2073 7973 7465 6d20 6964 656e  ndly system iden
 00000730: 7469 6669 6361 7469 6f6e 2066 6f72 2073  tification for s
 00000740: 7472 7563 7475 7265 732e 202a 5b4c 6561  tructures. *[Lea
 00000750: 726e 204d 6f72 655d 2868 7474 7073 3a2f  rn More](https:/
-00000760: 2f62 7261 6365 322e 6769 7468 7562 2e69  /brace2.github.i
-00000770: 6f2f 6d64 6f66 2f29 2a0a 0a3c 6469 7620  o/mdof/)*..<div 
-00000780: 7374 796c 653d 2261 6c69 676e 3a63 656e  style="align:cen
-00000790: 7465 7222 3e0a 0a5b 215b 4c61 7465 7374  ter">..[![Latest
-000007a0: 2050 7950 4920 7665 7273 696f 6e5d 2868   PyPI version](h
-000007b0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-000007c0: 6473 2e69 6f2f 7079 7069 2f76 2f6d 646f  ds.io/pypi/v/mdo
-000007d0: 663f 6c6f 676f 3d70 7970 6926 7374 796c  f?logo=pypi&styl
-000007e0: 653d 666f 722d 7468 652d 6261 6467 6529  e=for-the-badge)
-000007f0: 5d28 6874 7470 733a 2f2f 7079 7069 2e70  ](https://pypi.p
-00000800: 7974 686f 6e2e 6f72 672f 7079 7069 2f6d  ython.org/pypi/m
-00000810: 646f 6629 0a5b 215b 446f 776e 6c6f 6164  dof).[![Download
-00000820: 7320 7065 7220 4d6f 6e74 685d 2868 7474  s per Month](htt
-00000830: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000840: 2e69 6f2f 7079 7069 2f64 6d2f 6d64 6f66  .io/pypi/dm/mdof
-00000850: 3f73 7479 6c65 3d66 6f72 2d74 6865 2d62  ?style=for-the-b
-00000860: 6164 6765 295d 2828 6874 7470 733a 2f2f  adge)]((https://
-00000870: 7079 7069 2e70 7974 686f 6e2e 6f72 672f  pypi.python.org/
-00000880: 7079 7069 2f6d 646f 6629 290a 0a3c 2f64  pypi/mdof))..</d
-00000890: 6976 3e0a 0a3c 6872 3e0a 3c62 723e 0a0a  iv>..<hr>.<br>..
-000008a0: 2a2a 436f 6e76 656e 7469 6f6e 616c 2064  **Conventional d
-000008b0: 796e 616d 6963 2065 6967 656e 616e 616c  ynamic eigenanal
-000008c0: 7973 6973 2a2a 2069 7320 7765 6c6c 2d6b  ysis** is well-k
-000008d0: 6e6f 776e 2074 6f20 7374 7275 6374 7572  nown to structur
-000008e0: 616c 2065 6e67 696e 6565 7273 202d 2d20  al engineers -- 
-000008f0: 6672 6f6d 2073 7973 7465 6d20 7072 6f70  from system prop
-00000900: 6572 7469 6573 2061 6e64 2061 2067 6976  erties and a giv
-00000910: 656e 2065 7863 6974 6174 696f 6e2c 2074  en excitation, t
-00000920: 6865 2067 6f61 6c20 6973 2074 6f20 6465  he goal is to de
-00000930: 7465 726d 696e 6520 7468 6520 7379 7374  termine the syst
-00000940: 656d 2773 2064 796e 616d 6963 2072 6573  em's dynamic res
-00000950: 706f 6e73 652e 0a0a 6060 6070 7974 686f  ponse...```pytho
-00000960: 6e0a 6f75 7470 7574 5f6d 6f74 696f 6e20  n.output_motion 
-00000970: 3d20 6569 6765 6e28 4d2c 432c 4b2c 2069  = eigen(M,C,K, i
-00000980: 6e70 7574 5f6d 6f74 696f 6e29 0a60 6060  nput_motion).```
-00000990: 0a0a 2a2a 5468 6520 606d 646f 6660 2073  ..**The `mdof` s
-000009a0: 7973 7465 6d20 6964 2070 6163 6b61 6765  ystem id package
-000009b0: 2a2a 2061 6c6c 6f77 7320 7374 7275 6374  ** allows struct
-000009c0: 7572 616c 2065 6e67 696e 6565 7273 2074  ural engineers t
-000009d0: 6f20 736f 6c76 6520 2a2a 696e 7665 7273  o solve **invers
-000009e0: 6520 6569 6765 6e61 6e61 6c79 7369 732a  e eigenanalysis*
-000009f0: 2a20 616e 6420 7265 6c61 7465 6420 7072  * and related pr
-00000a00: 6f62 6c65 6d73 202d 2d20 6672 6f6d 2073  oblems -- from s
-00000a10: 7472 7563 7475 7261 6c20 7669 6272 6174  tructural vibrat
-00000a20: 696f 6e73 2c20 7468 6520 676f 616c 2069  ions, the goal i
-00000a30: 7320 746f 2069 6465 6e74 6966 7920 7468  s to identify th
-00000a40: 6520 7379 7374 656d 2070 726f 7065 7274  e system propert
-00000a50: 6965 732e 0a0a 496e 7665 7273 6520 6569  ies...Inverse ei
-00000a60: 6765 6e61 6e61 6c79 7369 733a 0a60 6060  genanalysis:.```
-00000a70: 7079 7468 6f6e 0a65 6967 7665 6373 2c20  python.eigvecs, 
-00000a80: 6569 6776 616c 7320 3d20 6569 6769 6428  eigvals = eigid(
-00000a90: 696e 7075 745f 6d6f 7469 6f6e 2c20 6f75  input_motion, ou
-00000aa0: 7470 7574 5f6d 6f74 696f 6e29 0a60 6060  tput_motion).```
-00000ab0: 0a0a 5374 6174 6520 7370 6163 6520 7379  ..State space sy
-00000ac0: 7374 656d 2069 6465 6e74 6966 6963 6174  stem identificat
-00000ad0: 696f 6e3a 0a60 6060 7079 7468 6f6e 0a41  ion:.```python.A
-00000ae0: 2c42 2c43 2c44 203d 2073 7973 6964 2869  ,B,C,D = sysid(i
-00000af0: 6e70 7574 5f6d 6f74 696f 6e2c 206f 7574  nput_motion, out
-00000b00: 7075 745f 6d6f 7469 6f6e 290a 6060 600a  put_motion).```.
-00000b10: 0a0a 2323 2047 6574 7469 6e67 2053 7461  ..## Getting Sta
-00000b20: 7274 6564 0a0a 436c 6963 6b20 5b2a 2a4a  rted..Click [**J
-00000b30: 7570 7974 6572 4c61 6220 6f6e 2044 6174  upyterLab on Dat
-00000b40: 6148 7562 2a2a 5d28 6874 7470 733a 2f2f  aHub**](https://
-00000b50: 6461 7461 6875 622e 6265 726b 656c 6579  datahub.berkeley
-00000b60: 2e65 6475 2f68 7562 2f75 7365 722d 7265  .edu/hub/user-re
-00000b70: 6469 7265 6374 2f67 6974 2d70 756c 6c3f  direct/git-pull?
-00000b80: 7265 706f 3d68 7474 7073 2533 4125 3246  repo=https%3A%2F
-00000b90: 2532 4667 6974 6875 622e 636f 6d25 3246  %2Fgithub.com%2F
-00000ba0: 4252 4143 4532 2532 466d 646f 6626 7572  BRACE2%2Fmdof&ur
-00000bb0: 6c70 6174 683d 6c61 6225 3246 7472 6565  lpath=lab%2Ftree
-00000bc0: 2532 466d 646f 6625 3246 6e6f 7465 626f  %2Fmdof%2Fnotebo
-00000bd0: 6f6b 7325 3246 5245 4144 4d45 2e69 7079  oks%2FREADME.ipy
-00000be0: 6e62 2662 7261 6e63 683d 6d61 7374 6572  nb&branch=master
-00000bf0: 2920 2855 4320 4265 726b 656c 6579 2075  ) (UC Berkeley u
-00000c00: 7365 7273 2920 6f72 2020 5b21 5b42 696e  sers) or  [![Bin
-00000c10: 6465 725d 2868 7474 7073 3a2f 2f6d 7962  der](https://myb
-00000c20: 696e 6465 722e 6f72 672f 6261 6467 655f  inder.org/badge_
-00000c30: 6c6f 676f 2e73 7667 295d 2868 7474 7073  logo.svg)](https
-00000c40: 3a2f 2f6d 7962 696e 6465 722e 6f72 672f  ://mybinder.org/
-00000c50: 7632 2f67 682f 4252 4143 4532 2f6d 646f  v2/gh/BRACE2/mdo
-00000c60: 662f 4845 4144 3f6c 6162 7061 7468 3d6e  f/HEAD?labpath=n
-00000c70: 6f74 6562 6f6f 6b73 2532 4652 4541 444d  otebooks%2FREADM
-00000c80: 452e 6970 796e 6229 2028 6e6f 6e2d 5543  E.ipynb) (non-UC
-00000c90: 2042 6572 6b65 6c65 7920 7573 6572 7329   Berkeley users)
-00000ca0: 2074 6f20 6163 6365 7373 2061 6e64 2065   to access and e
-00000cb0: 7870 6572 696d 656e 7420 7769 7468 2065  xperiment with e
-00000cc0: 7861 6d70 6c65 204a 7570 7974 6572 206e  xample Jupyter n
-00000cd0: 6f74 6562 6f6f 6b73 2e0a 0a2d 2d2d 2d2d  otebooks...-----
-00000ce0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000760: 2f63 6872 7973 7461 6c63 6865 726e 2e67  /chrystalchern.g
+00000770: 6974 6875 622e 696f 2f6d 646f 662f 292a  ithub.io/mdof/)*
+00000780: 0a0a 3c64 6976 2073 7479 6c65 3d22 616c  ..<div style="al
+00000790: 6967 6e3a 6365 6e74 6572 223e 0a0a 5b21  ign:center">..[!
+000007a0: 5b4c 6174 6573 7420 5079 5049 2076 6572  [Latest PyPI ver
+000007b0: 7369 6f6e 5d28 6874 7470 733a 2f2f 696d  sion](https://im
+000007c0: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+000007d0: 692f 762f 6d64 6f66 3f6c 6f67 6f3d 7079  i/v/mdof?logo=py
+000007e0: 7069 2673 7479 6c65 3d66 6f72 2d74 6865  pi&style=for-the
+000007f0: 2d62 6164 6765 295d 2868 7474 7073 3a2f  -badge)](https:/
+00000800: 2f70 7970 692e 7079 7468 6f6e 2e6f 7267  /pypi.python.org
+00000810: 2f70 7970 692f 6d64 6f66 290a 5b21 5b44  /pypi/mdof).[![D
+00000820: 6f77 6e6c 6f61 6473 2070 6572 204d 6f6e  ownloads per Mon
+00000830: 7468 5d28 6874 7470 733a 2f2f 696d 672e  th](https://img.
+00000840: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+00000850: 646d 2f6d 646f 663f 7374 796c 653d 666f  dm/mdof?style=fo
+00000860: 722d 7468 652d 6261 6467 6529 5d28 2868  r-the-badge)]((h
+00000870: 7474 7073 3a2f 2f70 7970 692e 7079 7468  ttps://pypi.pyth
+00000880: 6f6e 2e6f 7267 2f70 7970 692f 6d64 6f66  on.org/pypi/mdof
+00000890: 2929 0a0a 3c2f 6469 763e 0a0a 3c68 723e  ))..</div>..<hr>
+000008a0: 0a3c 6272 3e0a 0a2a 2a43 6f6e 7665 6e74  .<br>..**Convent
+000008b0: 696f 6e61 6c20 6479 6e61 6d69 6320 6569  ional dynamic ei
+000008c0: 6765 6e61 6e61 6c79 7369 732a 2a20 6973  genanalysis** is
+000008d0: 2077 656c 6c2d 6b6e 6f77 6e20 746f 2073   well-known to s
+000008e0: 7472 7563 7475 7261 6c20 656e 6769 6e65  tructural engine
+000008f0: 6572 7320 2d2d 2066 726f 6d20 7379 7374  ers -- from syst
+00000900: 656d 2070 726f 7065 7274 6965 7320 616e  em properties an
+00000910: 6420 6120 6769 7665 6e20 6578 6369 7461  d a given excita
+00000920: 7469 6f6e 2c20 7468 6520 676f 616c 2069  tion, the goal i
+00000930: 7320 746f 2064 6574 6572 6d69 6e65 2074  s to determine t
+00000940: 6865 2073 7973 7465 6d27 7320 6479 6e61  he system's dyna
+00000950: 6d69 6320 7265 7370 6f6e 7365 2e0a 0a60  mic response...`
+00000960: 6060 7079 7468 6f6e 0a6f 7574 7075 745f  ``python.output_
+00000970: 6d6f 7469 6f6e 203d 2065 6967 656e 284d  motion = eigen(M
+00000980: 2c43 2c4b 2c20 696e 7075 745f 6d6f 7469  ,C,K, input_moti
+00000990: 6f6e 290a 6060 600a 0a2a 2a54 6865 2060  on).```..**The `
+000009a0: 6d64 6f66 6020 7379 7374 656d 2069 6420  mdof` system id 
+000009b0: 7061 636b 6167 652a 2a20 616c 6c6f 7773  package** allows
+000009c0: 2073 7472 7563 7475 7261 6c20 656e 6769   structural engi
+000009d0: 6e65 6572 7320 746f 2073 6f6c 7665 202a  neers to solve *
+000009e0: 2a69 6e76 6572 7365 2065 6967 656e 616e  *inverse eigenan
+000009f0: 616c 7973 6973 2a2a 2061 6e64 2072 656c  alysis** and rel
+00000a00: 6174 6564 2070 726f 626c 656d 7320 2d2d  ated problems --
+00000a10: 2066 726f 6d20 7374 7275 6374 7572 616c   from structural
+00000a20: 2076 6962 7261 7469 6f6e 732c 2074 6865   vibrations, the
+00000a30: 2067 6f61 6c20 6973 2074 6f20 6964 656e   goal is to iden
+00000a40: 7469 6679 2074 6865 2073 7973 7465 6d20  tify the system 
+00000a50: 7072 6f70 6572 7469 6573 2e0a 0a49 6e76  properties...Inv
+00000a60: 6572 7365 2065 6967 656e 616e 616c 7973  erse eigenanalys
+00000a70: 6973 3a0a 6060 6070 7974 686f 6e0a 6569  is:.```python.ei
+00000a80: 6776 6563 732c 2065 6967 7661 6c73 203d  gvecs, eigvals =
+00000a90: 2065 6967 6964 2869 6e70 7574 5f6d 6f74   eigid(input_mot
+00000aa0: 696f 6e2c 206f 7574 7075 745f 6d6f 7469  ion, output_moti
+00000ab0: 6f6e 290a 6060 600a 0a53 7461 7465 2073  on).```..State s
+00000ac0: 7061 6365 2073 7973 7465 6d20 6964 656e  pace system iden
+00000ad0: 7469 6669 6361 7469 6f6e 3a0a 6060 6070  tification:.```p
+00000ae0: 7974 686f 6e0a 412c 422c 432c 4420 3d20  ython.A,B,C,D = 
+00000af0: 7379 7369 6428 696e 7075 745f 6d6f 7469  sysid(input_moti
+00000b00: 6f6e 2c20 6f75 7470 7574 5f6d 6f74 696f  on, output_motio
+00000b10: 6e29 0a60 6060 0a0a 0a23 2320 4765 7474  n).```...## Gett
+00000b20: 696e 6720 5374 6172 7465 640a 0a43 6c69  ing Started..Cli
+00000b30: 636b 205b 2a2a 4a75 7079 7465 724c 6162  ck [**JupyterLab
+00000b40: 206f 6e20 4461 7461 4875 622a 2a5d 2868   on DataHub**](h
+00000b50: 7474 7073 3a2f 2f64 6174 6168 7562 2e62  ttps://datahub.b
+00000b60: 6572 6b65 6c65 792e 6564 752f 6875 622f  erkeley.edu/hub/
+00000b70: 7573 6572 2d72 6564 6972 6563 742f 6769  user-redirect/gi
+00000b80: 742d 7075 6c6c 3f72 6570 6f3d 6874 7470  t-pull?repo=http
+00000b90: 7325 3341 2532 4625 3246 6769 7468 7562  s%3A%2F%2Fgithub
+00000ba0: 2e63 6f6d 2532 4642 5241 4345 3225 3246  .com%2FBRACE2%2F
+00000bb0: 6d64 6f66 2675 726c 7061 7468 3d6c 6162  mdof&urlpath=lab
+00000bc0: 2532 4674 7265 6525 3246 6d64 6f66 2532  %2Ftree%2Fmdof%2
+00000bd0: 466e 6f74 6562 6f6f 6b73 2532 4652 4541  Fnotebooks%2FREA
+00000be0: 444d 452e 6970 796e 6226 6272 616e 6368  DME.ipynb&branch
+00000bf0: 3d6d 6173 7465 7229 2028 5543 2042 6572  =master) (UC Ber
+00000c00: 6b65 6c65 7920 7573 6572 7329 206f 7220  keley users) or 
+00000c10: 205b 215b 4269 6e64 6572 5d28 6874 7470   [![Binder](http
+00000c20: 733a 2f2f 6d79 6269 6e64 6572 2e6f 7267  s://mybinder.org
+00000c30: 2f62 6164 6765 5f6c 6f67 6f2e 7376 6729  /badge_logo.svg)
+00000c40: 5d28 6874 7470 733a 2f2f 6d79 6269 6e64  ](https://mybind
+00000c50: 6572 2e6f 7267 2f76 322f 6768 2f42 5241  er.org/v2/gh/BRA
+00000c60: 4345 322f 6d64 6f66 2f48 4541 443f 6c61  CE2/mdof/HEAD?la
+00000c70: 6270 6174 683d 6e6f 7465 626f 6f6b 7325  bpath=notebooks%
+00000c80: 3246 5245 4144 4d45 2e69 7079 6e62 2920  2FREADME.ipynb) 
+00000c90: 286e 6f6e 2d55 4320 4265 726b 656c 6579  (non-UC Berkeley
+00000ca0: 2075 7365 7273 2920 746f 2061 6363 6573   users) to acces
+00000cb0: 7320 616e 6420 6578 7065 7269 6d65 6e74  s and experiment
+00000cc0: 2077 6974 6820 6578 616d 706c 6520 4a75   with example Ju
+00000cd0: 7079 7465 7220 6e6f 7465 626f 6f6b 732e  pyter notebooks.
+00000ce0: 0a0a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ..--------------
 00000cf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000d00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 0a    ------------...
+00000d00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000d10: 2d2d 2d0a 0a23 2320 5375 7070 6f72 740a  ---..## Support.
+00000d20: 0a3c 7461 626c 6520 616c 6967 6e3d 2263  .<table align="c
+00000d30: 656e 7465 7222 3e0a 3c74 723e 0a0a 2020  enter">.<tr>..  
+00000d40: 3c74 643e 0a20 2020 203c 6120 6872 6566  <td>.    <a href
+00000d50: 3d22 6874 7470 733a 2f2f 7065 6572 2e62  ="https://peer.b
+00000d60: 6572 6b65 6c65 792e 6564 7522 3e0a 2020  erkeley.edu">.  
+00000d70: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00000d80: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00000d90: 6572 636f 6e74 656e 742e 636f 6d2f 636c  ercontent.com/cl
+00000da0: 6175 6469 6f70 6572 657a 2f73 646f 662f  audioperez/sdof/
+00000db0: 6d61 7374 6572 2f64 6f63 732f 6173 7365  master/docs/asse
+00000dc0: 7473 2f70 6565 722d 626c 6163 6b2d 3330  ts/peer-black-30
+00000dd0: 302e 706e 6722 0a20 2020 2020 2020 2020  0.png".         
+00000de0: 616c 743d 2250 4545 5220 4c6f 676f 2220  alt="PEER Logo" 
+00000df0: 7769 6474 683d 2231 3230 222f 3e0a 2020  width="120"/>.  
+00000e00: 2020 3c2f 613e 0a20 203c 2f74 643e 0a0a    </a>.  </td>..
+00000e10: 2020 3c74 643e 0a20 2020 203c 6120 6872    <td>.    <a hr
+00000e20: 6566 3d22 6874 7470 733a 2f2f 646f 742e  ef="https://dot.
+00000e30: 6361 2e67 6f76 2f22 3e0a 2020 2020 3c69  ca.gov/">.    <i
+00000e40: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000e50: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
+00000e60: 6e74 656e 742e 636f 6d2f 636c 6175 6469  ntent.com/claudi
+00000e70: 6f70 6572 657a 2f73 646f 662f 6d61 7374  operez/sdof/mast
+00000e80: 6572 2f64 6f63 732f 6173 7365 7473 2f43  er/docs/assets/C
+00000e90: 616c 7472 616e 732e 7376 672e 706e 6722  altrans.svg.png"
+00000ea0: 0a20 2020 2020 2020 2020 616c 743d 2243  .         alt="C
+00000eb0: 616c 7472 616e 7320 4c6f 676f 2220 7769  altrans Logo" wi
+00000ec0: 6474 683d 2231 3230 222f 3e0a 2020 2020  dth="120"/>.    
+00000ed0: 3c2f 613e 0a20 203c 2f74 643e 0a0a 2020  </a>.  </td>..  
+00000ee0: 3c74 643e 0a20 2020 203c 6120 6872 6566  <td>.    <a href
+00000ef0: 3d22 6874 7470 733a 2f2f 7065 6572 2e62  ="https://peer.b
+00000f00: 6572 6b65 6c65 792e 6564 7522 3e0a 2020  erkeley.edu">.  
+00000f10: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00000f20: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00000f30: 6572 636f 6e74 656e 742e 636f 6d2f 636c  ercontent.com/cl
+00000f40: 6175 6469 6f70 6572 657a 2f73 646f 662f  audioperez/sdof/
+00000f50: 6d61 7374 6572 2f64 6f63 732f 6173 7365  master/docs/asse
+00000f60: 7473 2f62 7261 6365 325f 6c6f 676f 2d6e  ts/brace2_logo-n
+00000f70: 6577 335f 756e 6772 6f75 7065 642e 7376  ew3_ungrouped.sv
+00000f80: 6722 0a20 2020 2020 2020 2020 616c 743d  g".         alt=
+00000f90: 2242 5241 4345 3220 4c6f 676f 2220 7769  "BRACE2 Logo" wi
+00000fa0: 6474 683d 2231 3230 222f 3e0a 2020 2020  dth="120"/>.    
+00000fb0: 3c2f 613e 0a20 203c 2f74 643e 0a20 0a20  </a>.  </td>. . 
+00000fc0: 3c2f 7472 3e0a 3c2f 7461 626c 653e 0a    </tr>.</table>.
```

### Comparing `mdof-0.0.8/pyproject.toml` & `mdof-0.0.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mdof"
-version = "0.0.8" 
+version = "0.0.9"
 authors = [
   {name="Chrystal Chern", email="52893467+chrystalchern@users.noreply.github.com"}
 ]
 
 description="Fast and friendly system identification for structures."
 
 readme = "README.md"
```

### Comparing `mdof-0.0.8/src/mdof/__init__.py` & `mdof-0.0.9/src/mdof/__init__.py`

 * *Files identical despite different names*

### Comparing `mdof-0.0.8/src/mdof/__main__.py` & `mdof-0.0.9/src/mdof/__main__.py`

 * *Files identical despite different names*

### Comparing `mdof-0.0.8/src/mdof/macro.py` & `mdof-0.0.9/src/mdof/macro.py`

 * *Files identical despite different names*

### Comparing `mdof-0.0.8/src/mdof/markov.py` & `mdof-0.0.9/src/mdof/markov.py`

 * *Files identical despite different names*

### Comparing `mdof-0.0.8/src/mdof/modal.py` & `mdof-0.0.9/src/mdof/modal.py`

 * *Files identical despite different names*

### Comparing `mdof-0.0.8/src/mdof/numerics.py` & `mdof-0.0.9/src/mdof/numerics.py`

 * *Files identical despite different names*

### Comparing `mdof-0.0.8/src/mdof/realize.py` & `mdof-0.0.9/src/mdof/realize.py`

 * *Files identical despite different names*

### Comparing `mdof-0.0.8/src/mdof/system.py` & `mdof-0.0.9/src/mdof/system.py`

 * *Files identical despite different names*

### Comparing `mdof-0.0.8/src/mdof/transform.py` & `mdof-0.0.9/src/mdof/transform.py`

 * *Files identical despite different names*

### Comparing `mdof-0.0.8/src/mdof/utilities/config.py` & `mdof-0.0.9/src/mdof/utilities/config.py`

 * *Files identical despite different names*

### Comparing `mdof-0.0.8/src/mdof/utilities/testing.py` & `mdof-0.0.9/src/mdof/utilities/testing.py`

 * *Files identical despite different names*

### Comparing `mdof-0.0.8/src/mdof/validation.py` & `mdof-0.0.9/src/mdof/validation.py`

 * *Files identical despite different names*

### Comparing `mdof-0.0.8/src/mdof.egg-info/PKG-INFO` & `mdof-0.0.9/src/mdof.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6d64 6f66  : 2.1.Name: mdof
-00000020: 0a56 6572 7369 6f6e 3a20 302e 302e 380a  .Version: 0.0.8.
+00000020: 0a56 6572 7369 6f6e 3a20 302e 302e 390a  .Version: 0.0.9.
 00000030: 5375 6d6d 6172 793a 2046 6173 7420 616e  Summary: Fast an
 00000040: 6420 6672 6965 6e64 6c79 2073 7973 7465  d friendly syste
 00000050: 6d20 6964 656e 7469 6669 6361 7469 6f6e  m identification
 00000060: 2066 6f72 2073 7472 7563 7475 7265 732e   for structures.
 00000070: 0a41 7574 686f 722d 656d 6169 6c3a 2043  .Author-email: C
 00000080: 6872 7973 7461 6c20 4368 6572 6e20 3c35  hrystal Chern <5
 00000090: 3238 3933 3436 372b 6368 7279 7374 616c  2893467+chrystal
@@ -112,98 +112,142 @@
 000006f0: 6722 2077 6964 7468 3d22 3235 3070 7822  g" width="250px"
 00000700: 2061 6c74 3d22 6d64 6f66 206c 6f67 6f22   alt="mdof logo"
 00000710: 3e0a 0a46 6173 7420 616e 6420 6672 6965  >..Fast and frie
 00000720: 6e64 6c79 2073 7973 7465 6d20 6964 656e  ndly system iden
 00000730: 7469 6669 6361 7469 6f6e 2066 6f72 2073  tification for s
 00000740: 7472 7563 7475 7265 732e 202a 5b4c 6561  tructures. *[Lea
 00000750: 726e 204d 6f72 655d 2868 7474 7073 3a2f  rn More](https:/
-00000760: 2f62 7261 6365 322e 6769 7468 7562 2e69  /brace2.github.i
-00000770: 6f2f 6d64 6f66 2f29 2a0a 0a3c 6469 7620  o/mdof/)*..<div 
-00000780: 7374 796c 653d 2261 6c69 676e 3a63 656e  style="align:cen
-00000790: 7465 7222 3e0a 0a5b 215b 4c61 7465 7374  ter">..[![Latest
-000007a0: 2050 7950 4920 7665 7273 696f 6e5d 2868   PyPI version](h
-000007b0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-000007c0: 6473 2e69 6f2f 7079 7069 2f76 2f6d 646f  ds.io/pypi/v/mdo
-000007d0: 663f 6c6f 676f 3d70 7970 6926 7374 796c  f?logo=pypi&styl
-000007e0: 653d 666f 722d 7468 652d 6261 6467 6529  e=for-the-badge)
-000007f0: 5d28 6874 7470 733a 2f2f 7079 7069 2e70  ](https://pypi.p
-00000800: 7974 686f 6e2e 6f72 672f 7079 7069 2f6d  ython.org/pypi/m
-00000810: 646f 6629 0a5b 215b 446f 776e 6c6f 6164  dof).[![Download
-00000820: 7320 7065 7220 4d6f 6e74 685d 2868 7474  s per Month](htt
-00000830: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000840: 2e69 6f2f 7079 7069 2f64 6d2f 6d64 6f66  .io/pypi/dm/mdof
-00000850: 3f73 7479 6c65 3d66 6f72 2d74 6865 2d62  ?style=for-the-b
-00000860: 6164 6765 295d 2828 6874 7470 733a 2f2f  adge)]((https://
-00000870: 7079 7069 2e70 7974 686f 6e2e 6f72 672f  pypi.python.org/
-00000880: 7079 7069 2f6d 646f 6629 290a 0a3c 2f64  pypi/mdof))..</d
-00000890: 6976 3e0a 0a3c 6872 3e0a 3c62 723e 0a0a  iv>..<hr>.<br>..
-000008a0: 2a2a 436f 6e76 656e 7469 6f6e 616c 2064  **Conventional d
-000008b0: 796e 616d 6963 2065 6967 656e 616e 616c  ynamic eigenanal
-000008c0: 7973 6973 2a2a 2069 7320 7765 6c6c 2d6b  ysis** is well-k
-000008d0: 6e6f 776e 2074 6f20 7374 7275 6374 7572  nown to structur
-000008e0: 616c 2065 6e67 696e 6565 7273 202d 2d20  al engineers -- 
-000008f0: 6672 6f6d 2073 7973 7465 6d20 7072 6f70  from system prop
-00000900: 6572 7469 6573 2061 6e64 2061 2067 6976  erties and a giv
-00000910: 656e 2065 7863 6974 6174 696f 6e2c 2074  en excitation, t
-00000920: 6865 2067 6f61 6c20 6973 2074 6f20 6465  he goal is to de
-00000930: 7465 726d 696e 6520 7468 6520 7379 7374  termine the syst
-00000940: 656d 2773 2064 796e 616d 6963 2072 6573  em's dynamic res
-00000950: 706f 6e73 652e 0a0a 6060 6070 7974 686f  ponse...```pytho
-00000960: 6e0a 6f75 7470 7574 5f6d 6f74 696f 6e20  n.output_motion 
-00000970: 3d20 6569 6765 6e28 4d2c 432c 4b2c 2069  = eigen(M,C,K, i
-00000980: 6e70 7574 5f6d 6f74 696f 6e29 0a60 6060  nput_motion).```
-00000990: 0a0a 2a2a 5468 6520 606d 646f 6660 2073  ..**The `mdof` s
-000009a0: 7973 7465 6d20 6964 2070 6163 6b61 6765  ystem id package
-000009b0: 2a2a 2061 6c6c 6f77 7320 7374 7275 6374  ** allows struct
-000009c0: 7572 616c 2065 6e67 696e 6565 7273 2074  ural engineers t
-000009d0: 6f20 736f 6c76 6520 2a2a 696e 7665 7273  o solve **invers
-000009e0: 6520 6569 6765 6e61 6e61 6c79 7369 732a  e eigenanalysis*
-000009f0: 2a20 616e 6420 7265 6c61 7465 6420 7072  * and related pr
-00000a00: 6f62 6c65 6d73 202d 2d20 6672 6f6d 2073  oblems -- from s
-00000a10: 7472 7563 7475 7261 6c20 7669 6272 6174  tructural vibrat
-00000a20: 696f 6e73 2c20 7468 6520 676f 616c 2069  ions, the goal i
-00000a30: 7320 746f 2069 6465 6e74 6966 7920 7468  s to identify th
-00000a40: 6520 7379 7374 656d 2070 726f 7065 7274  e system propert
-00000a50: 6965 732e 0a0a 496e 7665 7273 6520 6569  ies...Inverse ei
-00000a60: 6765 6e61 6e61 6c79 7369 733a 0a60 6060  genanalysis:.```
-00000a70: 7079 7468 6f6e 0a65 6967 7665 6373 2c20  python.eigvecs, 
-00000a80: 6569 6776 616c 7320 3d20 6569 6769 6428  eigvals = eigid(
-00000a90: 696e 7075 745f 6d6f 7469 6f6e 2c20 6f75  input_motion, ou
-00000aa0: 7470 7574 5f6d 6f74 696f 6e29 0a60 6060  tput_motion).```
-00000ab0: 0a0a 5374 6174 6520 7370 6163 6520 7379  ..State space sy
-00000ac0: 7374 656d 2069 6465 6e74 6966 6963 6174  stem identificat
-00000ad0: 696f 6e3a 0a60 6060 7079 7468 6f6e 0a41  ion:.```python.A
-00000ae0: 2c42 2c43 2c44 203d 2073 7973 6964 2869  ,B,C,D = sysid(i
-00000af0: 6e70 7574 5f6d 6f74 696f 6e2c 206f 7574  nput_motion, out
-00000b00: 7075 745f 6d6f 7469 6f6e 290a 6060 600a  put_motion).```.
-00000b10: 0a0a 2323 2047 6574 7469 6e67 2053 7461  ..## Getting Sta
-00000b20: 7274 6564 0a0a 436c 6963 6b20 5b2a 2a4a  rted..Click [**J
-00000b30: 7570 7974 6572 4c61 6220 6f6e 2044 6174  upyterLab on Dat
-00000b40: 6148 7562 2a2a 5d28 6874 7470 733a 2f2f  aHub**](https://
-00000b50: 6461 7461 6875 622e 6265 726b 656c 6579  datahub.berkeley
-00000b60: 2e65 6475 2f68 7562 2f75 7365 722d 7265  .edu/hub/user-re
-00000b70: 6469 7265 6374 2f67 6974 2d70 756c 6c3f  direct/git-pull?
-00000b80: 7265 706f 3d68 7474 7073 2533 4125 3246  repo=https%3A%2F
-00000b90: 2532 4667 6974 6875 622e 636f 6d25 3246  %2Fgithub.com%2F
-00000ba0: 4252 4143 4532 2532 466d 646f 6626 7572  BRACE2%2Fmdof&ur
-00000bb0: 6c70 6174 683d 6c61 6225 3246 7472 6565  lpath=lab%2Ftree
-00000bc0: 2532 466d 646f 6625 3246 6e6f 7465 626f  %2Fmdof%2Fnotebo
-00000bd0: 6f6b 7325 3246 5245 4144 4d45 2e69 7079  oks%2FREADME.ipy
-00000be0: 6e62 2662 7261 6e63 683d 6d61 7374 6572  nb&branch=master
-00000bf0: 2920 2855 4320 4265 726b 656c 6579 2075  ) (UC Berkeley u
-00000c00: 7365 7273 2920 6f72 2020 5b21 5b42 696e  sers) or  [![Bin
-00000c10: 6465 725d 2868 7474 7073 3a2f 2f6d 7962  der](https://myb
-00000c20: 696e 6465 722e 6f72 672f 6261 6467 655f  inder.org/badge_
-00000c30: 6c6f 676f 2e73 7667 295d 2868 7474 7073  logo.svg)](https
-00000c40: 3a2f 2f6d 7962 696e 6465 722e 6f72 672f  ://mybinder.org/
-00000c50: 7632 2f67 682f 4252 4143 4532 2f6d 646f  v2/gh/BRACE2/mdo
-00000c60: 662f 4845 4144 3f6c 6162 7061 7468 3d6e  f/HEAD?labpath=n
-00000c70: 6f74 6562 6f6f 6b73 2532 4652 4541 444d  otebooks%2FREADM
-00000c80: 452e 6970 796e 6229 2028 6e6f 6e2d 5543  E.ipynb) (non-UC
-00000c90: 2042 6572 6b65 6c65 7920 7573 6572 7329   Berkeley users)
-00000ca0: 2074 6f20 6163 6365 7373 2061 6e64 2065   to access and e
-00000cb0: 7870 6572 696d 656e 7420 7769 7468 2065  xperiment with e
-00000cc0: 7861 6d70 6c65 204a 7570 7974 6572 206e  xample Jupyter n
-00000cd0: 6f74 6562 6f6f 6b73 2e0a 0a2d 2d2d 2d2d  otebooks...-----
-00000ce0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000760: 2f63 6872 7973 7461 6c63 6865 726e 2e67  /chrystalchern.g
+00000770: 6974 6875 622e 696f 2f6d 646f 662f 292a  ithub.io/mdof/)*
+00000780: 0a0a 3c64 6976 2073 7479 6c65 3d22 616c  ..<div style="al
+00000790: 6967 6e3a 6365 6e74 6572 223e 0a0a 5b21  ign:center">..[!
+000007a0: 5b4c 6174 6573 7420 5079 5049 2076 6572  [Latest PyPI ver
+000007b0: 7369 6f6e 5d28 6874 7470 733a 2f2f 696d  sion](https://im
+000007c0: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+000007d0: 692f 762f 6d64 6f66 3f6c 6f67 6f3d 7079  i/v/mdof?logo=py
+000007e0: 7069 2673 7479 6c65 3d66 6f72 2d74 6865  pi&style=for-the
+000007f0: 2d62 6164 6765 295d 2868 7474 7073 3a2f  -badge)](https:/
+00000800: 2f70 7970 692e 7079 7468 6f6e 2e6f 7267  /pypi.python.org
+00000810: 2f70 7970 692f 6d64 6f66 290a 5b21 5b44  /pypi/mdof).[![D
+00000820: 6f77 6e6c 6f61 6473 2070 6572 204d 6f6e  ownloads per Mon
+00000830: 7468 5d28 6874 7470 733a 2f2f 696d 672e  th](https://img.
+00000840: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+00000850: 646d 2f6d 646f 663f 7374 796c 653d 666f  dm/mdof?style=fo
+00000860: 722d 7468 652d 6261 6467 6529 5d28 2868  r-the-badge)]((h
+00000870: 7474 7073 3a2f 2f70 7970 692e 7079 7468  ttps://pypi.pyth
+00000880: 6f6e 2e6f 7267 2f70 7970 692f 6d64 6f66  on.org/pypi/mdof
+00000890: 2929 0a0a 3c2f 6469 763e 0a0a 3c68 723e  ))..</div>..<hr>
+000008a0: 0a3c 6272 3e0a 0a2a 2a43 6f6e 7665 6e74  .<br>..**Convent
+000008b0: 696f 6e61 6c20 6479 6e61 6d69 6320 6569  ional dynamic ei
+000008c0: 6765 6e61 6e61 6c79 7369 732a 2a20 6973  genanalysis** is
+000008d0: 2077 656c 6c2d 6b6e 6f77 6e20 746f 2073   well-known to s
+000008e0: 7472 7563 7475 7261 6c20 656e 6769 6e65  tructural engine
+000008f0: 6572 7320 2d2d 2066 726f 6d20 7379 7374  ers -- from syst
+00000900: 656d 2070 726f 7065 7274 6965 7320 616e  em properties an
+00000910: 6420 6120 6769 7665 6e20 6578 6369 7461  d a given excita
+00000920: 7469 6f6e 2c20 7468 6520 676f 616c 2069  tion, the goal i
+00000930: 7320 746f 2064 6574 6572 6d69 6e65 2074  s to determine t
+00000940: 6865 2073 7973 7465 6d27 7320 6479 6e61  he system's dyna
+00000950: 6d69 6320 7265 7370 6f6e 7365 2e0a 0a60  mic response...`
+00000960: 6060 7079 7468 6f6e 0a6f 7574 7075 745f  ``python.output_
+00000970: 6d6f 7469 6f6e 203d 2065 6967 656e 284d  motion = eigen(M
+00000980: 2c43 2c4b 2c20 696e 7075 745f 6d6f 7469  ,C,K, input_moti
+00000990: 6f6e 290a 6060 600a 0a2a 2a54 6865 2060  on).```..**The `
+000009a0: 6d64 6f66 6020 7379 7374 656d 2069 6420  mdof` system id 
+000009b0: 7061 636b 6167 652a 2a20 616c 6c6f 7773  package** allows
+000009c0: 2073 7472 7563 7475 7261 6c20 656e 6769   structural engi
+000009d0: 6e65 6572 7320 746f 2073 6f6c 7665 202a  neers to solve *
+000009e0: 2a69 6e76 6572 7365 2065 6967 656e 616e  *inverse eigenan
+000009f0: 616c 7973 6973 2a2a 2061 6e64 2072 656c  alysis** and rel
+00000a00: 6174 6564 2070 726f 626c 656d 7320 2d2d  ated problems --
+00000a10: 2066 726f 6d20 7374 7275 6374 7572 616c   from structural
+00000a20: 2076 6962 7261 7469 6f6e 732c 2074 6865   vibrations, the
+00000a30: 2067 6f61 6c20 6973 2074 6f20 6964 656e   goal is to iden
+00000a40: 7469 6679 2074 6865 2073 7973 7465 6d20  tify the system 
+00000a50: 7072 6f70 6572 7469 6573 2e0a 0a49 6e76  properties...Inv
+00000a60: 6572 7365 2065 6967 656e 616e 616c 7973  erse eigenanalys
+00000a70: 6973 3a0a 6060 6070 7974 686f 6e0a 6569  is:.```python.ei
+00000a80: 6776 6563 732c 2065 6967 7661 6c73 203d  gvecs, eigvals =
+00000a90: 2065 6967 6964 2869 6e70 7574 5f6d 6f74   eigid(input_mot
+00000aa0: 696f 6e2c 206f 7574 7075 745f 6d6f 7469  ion, output_moti
+00000ab0: 6f6e 290a 6060 600a 0a53 7461 7465 2073  on).```..State s
+00000ac0: 7061 6365 2073 7973 7465 6d20 6964 656e  pace system iden
+00000ad0: 7469 6669 6361 7469 6f6e 3a0a 6060 6070  tification:.```p
+00000ae0: 7974 686f 6e0a 412c 422c 432c 4420 3d20  ython.A,B,C,D = 
+00000af0: 7379 7369 6428 696e 7075 745f 6d6f 7469  sysid(input_moti
+00000b00: 6f6e 2c20 6f75 7470 7574 5f6d 6f74 696f  on, output_motio
+00000b10: 6e29 0a60 6060 0a0a 0a23 2320 4765 7474  n).```...## Gett
+00000b20: 696e 6720 5374 6172 7465 640a 0a43 6c69  ing Started..Cli
+00000b30: 636b 205b 2a2a 4a75 7079 7465 724c 6162  ck [**JupyterLab
+00000b40: 206f 6e20 4461 7461 4875 622a 2a5d 2868   on DataHub**](h
+00000b50: 7474 7073 3a2f 2f64 6174 6168 7562 2e62  ttps://datahub.b
+00000b60: 6572 6b65 6c65 792e 6564 752f 6875 622f  erkeley.edu/hub/
+00000b70: 7573 6572 2d72 6564 6972 6563 742f 6769  user-redirect/gi
+00000b80: 742d 7075 6c6c 3f72 6570 6f3d 6874 7470  t-pull?repo=http
+00000b90: 7325 3341 2532 4625 3246 6769 7468 7562  s%3A%2F%2Fgithub
+00000ba0: 2e63 6f6d 2532 4642 5241 4345 3225 3246  .com%2FBRACE2%2F
+00000bb0: 6d64 6f66 2675 726c 7061 7468 3d6c 6162  mdof&urlpath=lab
+00000bc0: 2532 4674 7265 6525 3246 6d64 6f66 2532  %2Ftree%2Fmdof%2
+00000bd0: 466e 6f74 6562 6f6f 6b73 2532 4652 4541  Fnotebooks%2FREA
+00000be0: 444d 452e 6970 796e 6226 6272 616e 6368  DME.ipynb&branch
+00000bf0: 3d6d 6173 7465 7229 2028 5543 2042 6572  =master) (UC Ber
+00000c00: 6b65 6c65 7920 7573 6572 7329 206f 7220  keley users) or 
+00000c10: 205b 215b 4269 6e64 6572 5d28 6874 7470   [![Binder](http
+00000c20: 733a 2f2f 6d79 6269 6e64 6572 2e6f 7267  s://mybinder.org
+00000c30: 2f62 6164 6765 5f6c 6f67 6f2e 7376 6729  /badge_logo.svg)
+00000c40: 5d28 6874 7470 733a 2f2f 6d79 6269 6e64  ](https://mybind
+00000c50: 6572 2e6f 7267 2f76 322f 6768 2f42 5241  er.org/v2/gh/BRA
+00000c60: 4345 322f 6d64 6f66 2f48 4541 443f 6c61  CE2/mdof/HEAD?la
+00000c70: 6270 6174 683d 6e6f 7465 626f 6f6b 7325  bpath=notebooks%
+00000c80: 3246 5245 4144 4d45 2e69 7079 6e62 2920  2FREADME.ipynb) 
+00000c90: 286e 6f6e 2d55 4320 4265 726b 656c 6579  (non-UC Berkeley
+00000ca0: 2075 7365 7273 2920 746f 2061 6363 6573   users) to acces
+00000cb0: 7320 616e 6420 6578 7065 7269 6d65 6e74  s and experiment
+00000cc0: 2077 6974 6820 6578 616d 706c 6520 4a75   with example Ju
+00000cd0: 7079 7465 7220 6e6f 7465 626f 6f6b 732e  pyter notebooks.
+00000ce0: 0a0a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ..--------------
 00000cf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000d00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 0a    ------------...
+00000d00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000d10: 2d2d 2d0a 0a23 2320 5375 7070 6f72 740a  ---..## Support.
+00000d20: 0a3c 7461 626c 6520 616c 6967 6e3d 2263  .<table align="c
+00000d30: 656e 7465 7222 3e0a 3c74 723e 0a0a 2020  enter">.<tr>..  
+00000d40: 3c74 643e 0a20 2020 203c 6120 6872 6566  <td>.    <a href
+00000d50: 3d22 6874 7470 733a 2f2f 7065 6572 2e62  ="https://peer.b
+00000d60: 6572 6b65 6c65 792e 6564 7522 3e0a 2020  erkeley.edu">.  
+00000d70: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00000d80: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00000d90: 6572 636f 6e74 656e 742e 636f 6d2f 636c  ercontent.com/cl
+00000da0: 6175 6469 6f70 6572 657a 2f73 646f 662f  audioperez/sdof/
+00000db0: 6d61 7374 6572 2f64 6f63 732f 6173 7365  master/docs/asse
+00000dc0: 7473 2f70 6565 722d 626c 6163 6b2d 3330  ts/peer-black-30
+00000dd0: 302e 706e 6722 0a20 2020 2020 2020 2020  0.png".         
+00000de0: 616c 743d 2250 4545 5220 4c6f 676f 2220  alt="PEER Logo" 
+00000df0: 7769 6474 683d 2231 3230 222f 3e0a 2020  width="120"/>.  
+00000e00: 2020 3c2f 613e 0a20 203c 2f74 643e 0a0a    </a>.  </td>..
+00000e10: 2020 3c74 643e 0a20 2020 203c 6120 6872    <td>.    <a hr
+00000e20: 6566 3d22 6874 7470 733a 2f2f 646f 742e  ef="https://dot.
+00000e30: 6361 2e67 6f76 2f22 3e0a 2020 2020 3c69  ca.gov/">.    <i
+00000e40: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000e50: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
+00000e60: 6e74 656e 742e 636f 6d2f 636c 6175 6469  ntent.com/claudi
+00000e70: 6f70 6572 657a 2f73 646f 662f 6d61 7374  operez/sdof/mast
+00000e80: 6572 2f64 6f63 732f 6173 7365 7473 2f43  er/docs/assets/C
+00000e90: 616c 7472 616e 732e 7376 672e 706e 6722  altrans.svg.png"
+00000ea0: 0a20 2020 2020 2020 2020 616c 743d 2243  .         alt="C
+00000eb0: 616c 7472 616e 7320 4c6f 676f 2220 7769  altrans Logo" wi
+00000ec0: 6474 683d 2231 3230 222f 3e0a 2020 2020  dth="120"/>.    
+00000ed0: 3c2f 613e 0a20 203c 2f74 643e 0a0a 2020  </a>.  </td>..  
+00000ee0: 3c74 643e 0a20 2020 203c 6120 6872 6566  <td>.    <a href
+00000ef0: 3d22 6874 7470 733a 2f2f 7065 6572 2e62  ="https://peer.b
+00000f00: 6572 6b65 6c65 792e 6564 7522 3e0a 2020  erkeley.edu">.  
+00000f10: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00000f20: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00000f30: 6572 636f 6e74 656e 742e 636f 6d2f 636c  ercontent.com/cl
+00000f40: 6175 6469 6f70 6572 657a 2f73 646f 662f  audioperez/sdof/
+00000f50: 6d61 7374 6572 2f64 6f63 732f 6173 7365  master/docs/asse
+00000f60: 7473 2f62 7261 6365 325f 6c6f 676f 2d6e  ts/brace2_logo-n
+00000f70: 6577 335f 756e 6772 6f75 7065 642e 7376  ew3_ungrouped.sv
+00000f80: 6722 0a20 2020 2020 2020 2020 616c 743d  g".         alt=
+00000f90: 2242 5241 4345 3220 4c6f 676f 2220 7769  "BRACE2 Logo" wi
+00000fa0: 6474 683d 2231 3230 222f 3e0a 2020 2020  dth="120"/>.    
+00000fb0: 3c2f 613e 0a20 203c 2f74 643e 0a20 0a20  </a>.  </td>. . 
+00000fc0: 3c2f 7472 3e0a 3c2f 7461 626c 653e 0a    </tr>.</table>.
```

### Comparing `mdof-0.0.8/src/mdof.egg-info/SOURCES.txt` & `mdof-0.0.9/src/mdof.egg-info/SOURCES.txt`

 * *Files identical despite different names*

