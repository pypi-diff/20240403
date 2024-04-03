# Comparing `tmp/data-analysis-tfidf-tool-jms-0.0.1.tar.gz` & `tmp/data-analysis-tfidf-tool-jms-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-analysis-tfidf-tool-jms-0.0.1.tar", last modified: Fri Mar 15 12:14:13 2024, max compression
+gzip compressed data, was "data-analysis-tfidf-tool-jms-0.0.2.tar", last modified: Wed Apr  3 17:15:37 2024, max compression
```

## Comparing `data-analysis-tfidf-tool-jms-0.0.1.tar` & `data-analysis-tfidf-tool-jms-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,13 @@
-drwxr-xr-x   0 jms        (501) staff       (20)        0 2024-03-15 12:14:13.539715 data-analysis-tfidf-tool-jms-0.0.1/
--rw-r--r--   0 jms        (501) staff       (20)     1067 2024-03-15 11:23:38.000000 data-analysis-tfidf-tool-jms-0.0.1/LICENSE
--rw-r--r--   0 jms        (501) staff       (20)     1106 2024-03-15 12:14:13.539314 data-analysis-tfidf-tool-jms-0.0.1/PKG-INFO
--rw-r--r--   0 jms        (501) staff       (20)      142 2024-03-15 12:03:58.000000 data-analysis-tfidf-tool-jms-0.0.1/README.md
-drwxr-xr-x   0 jms        (501) staff       (20)        0 2024-03-15 12:14:13.528812 data-analysis-tfidf-tool-jms-0.0.1/data/
--rw-r--r--   0 jms        (501) staff       (20)        0 2024-03-15 12:03:22.000000 data-analysis-tfidf-tool-jms-0.0.1/data/__init__.py
-drwxr-xr-x   0 jms        (501) staff       (20)        0 2024-03-15 12:14:13.529499 data-analysis-tfidf-tool-jms-0.0.1/data/analysis/
--rw-r--r--   0 jms        (501) staff       (20)        0 2024-03-15 12:03:22.000000 data-analysis-tfidf-tool-jms-0.0.1/data/analysis/__init__.py
-drwxr-xr-x   0 jms        (501) staff       (20)        0 2024-03-15 12:14:13.530138 data-analysis-tfidf-tool-jms-0.0.1/data/analysis/tfidf/
--rw-r--r--   0 jms        (501) staff       (20)        0 2024-03-15 12:03:22.000000 data-analysis-tfidf-tool-jms-0.0.1/data/analysis/tfidf/__init__.py
-drwxr-xr-x   0 jms        (501) staff       (20)        0 2024-03-15 12:14:13.530625 data-analysis-tfidf-tool-jms-0.0.1/data/analysis/tfidf/tool/
--rw-r--r--   0 jms        (501) staff       (20)        0 2024-03-15 12:03:22.000000 data-analysis-tfidf-tool-jms-0.0.1/data/analysis/tfidf/tool/__init__.py
-drwxr-xr-x   0 jms        (501) staff       (20)        0 2024-03-15 12:14:13.531703 data-analysis-tfidf-tool-jms-0.0.1/data/analysis/tfidf/tool/jms/
--rw-r--r--   0 jms        (501) staff       (20)        0 2024-03-15 12:03:22.000000 data-analysis-tfidf-tool-jms-0.0.1/data/analysis/tfidf/tool/jms/__init__.py
--rw-r--r--   0 jms        (501) staff       (20)     2922 2024-03-15 12:13:22.000000 data-analysis-tfidf-tool-jms-0.0.1/data/analysis/tfidf/tool/jms/data_tfidf_tool.py
-drwxr-xr-x   0 jms        (501) staff       (20)        0 2024-03-15 12:14:13.537950 data-analysis-tfidf-tool-jms-0.0.1/data_analysis_tfidf_tool_jms.egg-info/
--rw-r--r--   0 jms        (501) staff       (20)     1106 2024-03-15 12:14:13.000000 data-analysis-tfidf-tool-jms-0.0.1/data_analysis_tfidf_tool_jms.egg-info/PKG-INFO
--rw-r--r--   0 jms        (501) staff       (20)      511 2024-03-15 12:14:13.000000 data-analysis-tfidf-tool-jms-0.0.1/data_analysis_tfidf_tool_jms.egg-info/SOURCES.txt
--rw-r--r--   0 jms        (501) staff       (20)        1 2024-03-15 12:14:13.000000 data-analysis-tfidf-tool-jms-0.0.1/data_analysis_tfidf_tool_jms.egg-info/dependency_links.txt
--rw-r--r--   0 jms        (501) staff       (20)      269 2024-03-15 12:14:13.000000 data-analysis-tfidf-tool-jms-0.0.1/data_analysis_tfidf_tool_jms.egg-info/requires.txt
--rw-r--r--   0 jms        (501) staff       (20)        5 2024-03-15 12:14:13.000000 data-analysis-tfidf-tool-jms-0.0.1/data_analysis_tfidf_tool_jms.egg-info/top_level.txt
--rw-r--r--   0 jms        (501) staff       (20)      300 2024-03-15 12:13:22.000000 data-analysis-tfidf-tool-jms-0.0.1/pyproject.toml
--rw-r--r--   0 jms        (501) staff       (20)      824 2024-03-15 12:14:13.541212 data-analysis-tfidf-tool-jms-0.0.1/setup.cfg
--rw-r--r--   0 jms        (501) staff       (20)      143 2024-03-15 12:03:58.000000 data-analysis-tfidf-tool-jms-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 17:15:37.744594 data-analysis-tfidf-tool-jms-0.0.2/
+-rw-rw-rw-   0        0        0     1088 2024-04-03 17:08:31.000000 data-analysis-tfidf-tool-jms-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1243 2024-04-03 17:15:37.742592 data-analysis-tfidf-tool-jms-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      146 2024-04-03 17:10:28.000000 data-analysis-tfidf-tool-jms-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 17:15:37.739594 data-analysis-tfidf-tool-jms-0.0.2/data_analysis_tfidf_tool_jms.egg-info/
+-rw-rw-rw-   0        0        0     1243 2024-04-03 17:15:37.000000 data-analysis-tfidf-tool-jms-0.0.2/data_analysis_tfidf_tool_jms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2024-04-03 17:15:37.000000 data-analysis-tfidf-tool-jms-0.0.2/data_analysis_tfidf_tool_jms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 17:15:37.000000 data-analysis-tfidf-tool-jms-0.0.2/data_analysis_tfidf_tool_jms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      344 2024-04-03 17:15:37.000000 data-analysis-tfidf-tool-jms-0.0.2/data_analysis_tfidf_tool_jms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 17:15:37.000000 data-analysis-tfidf-tool-jms-0.0.2/data_analysis_tfidf_tool_jms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      382 2024-04-03 17:10:09.000000 data-analysis-tfidf-tool-jms-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      936 2024-04-03 17:15:37.746592 data-analysis-tfidf-tool-jms-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      149 2024-04-03 17:08:31.000000 data-analysis-tfidf-tool-jms-0.0.2/setup.py
```

### Comparing `data-analysis-tfidf-tool-jms-0.0.1/PKG-INFO` & `data-analysis-tfidf-tool-jms-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-Metadata-Version: 2.1
-Name: data-analysis-tfidf-tool-jms
-Version: 0.0.1
-Summary: A data processor package
-Home-page: https://github.com/Jane-Dream/data-analysis-tfidf-tool-jms
-Author: Jane-Dream
-Author-email: janedream515@gmail.com
-Project-URL: Source, https://github.com/Jane-Dream/data-analysis-tfidf-tool-jms
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.24.0
-Requires-Dist: setuptools>=42
-Requires-Dist: numpy>=1.24.4
-Requires-Dist: data-analysis-tools-fdx>=0.0.1
-Requires-Dist: data-analysis-tools-jms-diy>=0.0.1
-Requires-Dist: data-analysis-tools-alpha>=0.0.1
-Requires-Dist: data-analysis-tools-bet>=0.0.1
-Requires-Dist: data-analysis-tools-cat>=0.0.1
-Requires-Dist: data-analysis-tools-dog>=0.0.1
-Requires-Dist: data-analysis-tools-eth>=0.0.1
-
-# data-analysis-tfidf-tool-jms
-
-使用fasttext工具，实现简单的噪音模型判断接口
-添加数据集分割接口dataset_spliter()。
+Metadata-Version: 2.1
+Name: data-analysis-tfidf-tool-jms
+Version: 0.0.2
+Summary: A data processor package
+Home-page: https://github.com/Jane-Dream/data-analysis-tfidf-tool-jms
+Author: Jane-Dream
+Author-email: janedream515@gmail.com
+Project-URL: Source, https://github.com/Jane-Dream/data-analysis-tfidf-tool-jms
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.24.0
+Requires-Dist: setuptools>=42
+Requires-Dist: numpy>=1.24.4
+Requires-Dist: data-analysis-tools-fdx>=0.0.1
+Requires-Dist: data-analysis-tools-jms-diy>=0.0.1
+Requires-Dist: data-analysis-tools-alpha>=0.0.1
+Requires-Dist: data-analysis-tools-bet>=0.0.1
+Requires-Dist: data-analysis-tools-cat>=0.0.1
+Requires-Dist: data-analysis-tools-dog>=0.0.1
+Requires-Dist: data-analysis-tools-eth>=0.0.1
+Requires-Dist: data-analysis-attribute-tool-jms>=0.0.2
+Requires-Dist: data-analysis-tools-jms-seg>=0.0.2
+
+# data-analysis-tfidf-tool-jms
+
+使用fasttext工具，实现简单的噪音模型判断接口，添加数据集分割接口dataset_spliter()。
```

### Comparing `data-analysis-tfidf-tool-jms-0.0.1/data_analysis_tfidf_tool_jms.egg-info/PKG-INFO` & `data-analysis-tfidf-tool-jms-0.0.2/data_analysis_tfidf_tool_jms.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-Metadata-Version: 2.1
-Name: data-analysis-tfidf-tool-jms
-Version: 0.0.1
-Summary: A data processor package
-Home-page: https://github.com/Jane-Dream/data-analysis-tfidf-tool-jms
-Author: Jane-Dream
-Author-email: janedream515@gmail.com
-Project-URL: Source, https://github.com/Jane-Dream/data-analysis-tfidf-tool-jms
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.24.0
-Requires-Dist: setuptools>=42
-Requires-Dist: numpy>=1.24.4
-Requires-Dist: data-analysis-tools-fdx>=0.0.1
-Requires-Dist: data-analysis-tools-jms-diy>=0.0.1
-Requires-Dist: data-analysis-tools-alpha>=0.0.1
-Requires-Dist: data-analysis-tools-bet>=0.0.1
-Requires-Dist: data-analysis-tools-cat>=0.0.1
-Requires-Dist: data-analysis-tools-dog>=0.0.1
-Requires-Dist: data-analysis-tools-eth>=0.0.1
-
-# data-analysis-tfidf-tool-jms
-
-使用fasttext工具，实现简单的噪音模型判断接口
-添加数据集分割接口dataset_spliter()。
+Metadata-Version: 2.1
+Name: data-analysis-tfidf-tool-jms
+Version: 0.0.2
+Summary: A data processor package
+Home-page: https://github.com/Jane-Dream/data-analysis-tfidf-tool-jms
+Author: Jane-Dream
+Author-email: janedream515@gmail.com
+Project-URL: Source, https://github.com/Jane-Dream/data-analysis-tfidf-tool-jms
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.24.0
+Requires-Dist: setuptools>=42
+Requires-Dist: numpy>=1.24.4
+Requires-Dist: data-analysis-tools-fdx>=0.0.1
+Requires-Dist: data-analysis-tools-jms-diy>=0.0.1
+Requires-Dist: data-analysis-tools-alpha>=0.0.1
+Requires-Dist: data-analysis-tools-bet>=0.0.1
+Requires-Dist: data-analysis-tools-cat>=0.0.1
+Requires-Dist: data-analysis-tools-dog>=0.0.1
+Requires-Dist: data-analysis-tools-eth>=0.0.1
+Requires-Dist: data-analysis-attribute-tool-jms>=0.0.2
+Requires-Dist: data-analysis-tools-jms-seg>=0.0.2
+
+# data-analysis-tfidf-tool-jms
+
+使用fasttext工具，实现简单的噪音模型判断接口，添加数据集分割接口dataset_spliter()。
```

### Comparing `data-analysis-tfidf-tool-jms-0.0.1/setup.cfg` & `data-analysis-tfidf-tool-jms-0.0.2/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,59 @@
-00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
-00000010: 3d20 6461 7461 2d61 6e61 6c79 7369 732d  = data-analysis-
-00000020: 7466 6964 662d 746f 6f6c 2d6a 6d73 0a76  tfidf-tool-jms.v
-00000030: 6572 7369 6f6e 203d 2030 2e30 2e31 0a61  ersion = 0.0.1.a
-00000040: 7574 686f 7220 3d20 4a61 6e65 2d44 7265  uthor = Jane-Dre
-00000050: 616d 0a61 7574 686f 725f 656d 6169 6c20  am.author_email 
-00000060: 3d20 6a61 6e65 6472 6561 6d35 3135 4067  = janedream515@g
-00000070: 6d61 696c 2e63 6f6d 0a64 6573 6372 6970  mail.com.descrip
-00000080: 7469 6f6e 203d 2041 2064 6174 6120 7072  tion = A data pr
-00000090: 6f63 6573 736f 7220 7061 636b 6167 650a  ocessor package.
-000000a0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-000000b0: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
-000000c0: 6d64 0a6c 6f6e 675f 6465 7363 7269 7074  md.long_descript
-000000d0: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
-000000e0: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
-000000f0: 0a75 726c 203d 2068 7474 7073 3a2f 2f67  .url = https://g
-00000100: 6974 6875 622e 636f 6d2f 4a61 6e65 2d44  ithub.com/Jane-D
-00000110: 7265 616d 2f64 6174 612d 616e 616c 7973  ream/data-analys
-00000120: 6973 2d74 6669 6466 2d74 6f6f 6c2d 6a6d  is-tfidf-tool-jm
-00000130: 730a 636c 6173 7369 6669 6572 7320 3d20  s.classifiers = 
-00000140: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000150: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000160: 203a 3a20 330a 094c 6963 656e 7365 203a   :: 3..License :
-00000170: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-00000180: 3a20 4d49 5420 4c69 6365 6e73 650a 094f  : MIT License..O
-00000190: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-000001a0: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
-000001b0: 740a 0a5b 6f70 7469 6f6e 735d 0a70 6163  t..[options].pac
-000001c0: 6b61 6765 7320 3d20 6669 6e64 3a0a 7079  kages = find:.py
-000001d0: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
-000001e0: 3e3d 332e 360a 696e 7374 616c 6c5f 7265  >=3.6.install_re
-000001f0: 7175 6972 6573 203d 200a 0972 6571 7565  quires = ..reque
-00000200: 7374 733e 3d32 2e32 342e 300a 0973 6574  sts>=2.24.0..set
-00000210: 7570 746f 6f6c 733e 3d34 320a 096e 756d  uptools>=42..num
-00000220: 7079 3e3d 312e 3234 2e34 0a09 6461 7461  py>=1.24.4..data
-00000230: 2d61 6e61 6c79 7369 732d 746f 6f6c 732d  -analysis-tools-
-00000240: 6664 783e 3d30 2e30 2e31 0a09 6461 7461  fdx>=0.0.1..data
-00000250: 2d61 6e61 6c79 7369 732d 746f 6f6c 732d  -analysis-tools-
-00000260: 6a6d 732d 6469 793e 3d30 2e30 2e31 0a09  jms-diy>=0.0.1..
-00000270: 6461 7461 2d61 6e61 6c79 7369 732d 746f  data-analysis-to
-00000280: 6f6c 732d 616c 7068 613e 3d30 2e30 2e31  ols-alpha>=0.0.1
-00000290: 0a09 6461 7461 2d61 6e61 6c79 7369 732d  ..data-analysis-
-000002a0: 746f 6f6c 732d 6265 743e 3d30 2e30 2e31  tools-bet>=0.0.1
-000002b0: 0a09 6461 7461 2d61 6e61 6c79 7369 732d  ..data-analysis-
-000002c0: 746f 6f6c 732d 6361 743e 3d30 2e30 2e31  tools-cat>=0.0.1
-000002d0: 0a09 6461 7461 2d61 6e61 6c79 7369 732d  ..data-analysis-
-000002e0: 746f 6f6c 732d 646f 673e 3d30 2e30 2e31  tools-dog>=0.0.1
-000002f0: 0a09 6461 7461 2d61 6e61 6c79 7369 732d  ..data-analysis-
-00000300: 746f 6f6c 732d 6574 683e 3d30 2e30 2e31  tools-eth>=0.0.1
-00000310: 0a0a 5b65 6767 5f69 6e66 6f5d 0a74 6167  ..[egg_info].tag
-00000320: 5f62 7569 6c64 203d 200a 7461 675f 6461  _build = .tag_da
-00000330: 7465 203d 2030 0a0a                      te = 0..
+00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
+00000010: 203d 2064 6174 612d 616e 616c 7973 6973   = data-analysis
+00000020: 2d74 6669 6466 2d74 6f6f 6c2d 6a6d 730d  -tfidf-tool-jms.
+00000030: 0a76 6572 7369 6f6e 203d 2030 2e30 2e32  .version = 0.0.2
+00000040: 0d0a 6175 7468 6f72 203d 204a 616e 652d  ..author = Jane-
+00000050: 4472 6561 6d0d 0a61 7574 686f 725f 656d  Dream..author_em
+00000060: 6169 6c20 3d20 6a61 6e65 6472 6561 6d35  ail = janedream5
+00000070: 3135 4067 6d61 696c 2e63 6f6d 0d0a 6465  15@gmail.com..de
+00000080: 7363 7269 7074 696f 6e20 3d20 4120 6461  scription = A da
+00000090: 7461 2070 726f 6365 7373 6f72 2070 6163  ta processor pac
+000000a0: 6b61 6765 0d0a 6c6f 6e67 5f64 6573 6372  kage..long_descr
+000000b0: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
+000000c0: 4541 444d 452e 6d64 0d0a 6c6f 6e67 5f64  EADME.md..long_d
+000000d0: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
+000000e0: 6e74 5f74 7970 6520 3d20 7465 7874 2f6d  nt_type = text/m
+000000f0: 6172 6b64 6f77 6e0d 0a75 726c 203d 2068  arkdown..url = h
+00000100: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000110: 6d2f 4a61 6e65 2d44 7265 616d 2f64 6174  m/Jane-Dream/dat
+00000120: 612d 616e 616c 7973 6973 2d74 6669 6466  a-analysis-tfidf
+00000130: 2d74 6f6f 6c2d 6a6d 730d 0a63 6c61 7373  -tool-jms..class
+00000140: 6966 6965 7273 203d 200d 0a09 5072 6f67  ifiers = ...Prog
+00000150: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000160: 203a 3a20 5079 7468 6f6e 203a 3a20 330d   :: Python :: 3.
+00000170: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
+00000180: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
+00000190: 204c 6963 656e 7365 0d0a 094f 7065 7261   License...Opera
+000001a0: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
+000001b0: 5320 496e 6465 7065 6e64 656e 740d 0a0d  S Independent...
+000001c0: 0a5b 6f70 7469 6f6e 735d 0d0a 7061 636b  .[options]..pack
+000001d0: 6167 6573 203d 2066 696e 643a 0d0a 7079  ages = find:..py
+000001e0: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
+000001f0: 3e3d 332e 360d 0a69 6e73 7461 6c6c 5f72  >=3.6..install_r
+00000200: 6571 7569 7265 7320 3d20 0d0a 0972 6571  equires = ...req
+00000210: 7565 7374 733e 3d32 2e32 342e 300d 0a09  uests>=2.24.0...
+00000220: 7365 7475 7074 6f6f 6c73 3e3d 3432 0d0a  setuptools>=42..
+00000230: 096e 756d 7079 3e3d 312e 3234 2e34 0d0a  .numpy>=1.24.4..
+00000240: 0964 6174 612d 616e 616c 7973 6973 2d74  .data-analysis-t
+00000250: 6f6f 6c73 2d66 6478 3e3d 302e 302e 310d  ools-fdx>=0.0.1.
+00000260: 0a09 6461 7461 2d61 6e61 6c79 7369 732d  ..data-analysis-
+00000270: 746f 6f6c 732d 6a6d 732d 6469 793e 3d30  tools-jms-diy>=0
+00000280: 2e30 2e31 0d0a 0964 6174 612d 616e 616c  .0.1...data-anal
+00000290: 7973 6973 2d74 6f6f 6c73 2d61 6c70 6861  ysis-tools-alpha
+000002a0: 3e3d 302e 302e 310d 0a09 6461 7461 2d61  >=0.0.1...data-a
+000002b0: 6e61 6c79 7369 732d 746f 6f6c 732d 6265  nalysis-tools-be
+000002c0: 743e 3d30 2e30 2e31 0d0a 0964 6174 612d  t>=0.0.1...data-
+000002d0: 616e 616c 7973 6973 2d74 6f6f 6c73 2d63  analysis-tools-c
+000002e0: 6174 3e3d 302e 302e 310d 0a09 6461 7461  at>=0.0.1...data
+000002f0: 2d61 6e61 6c79 7369 732d 746f 6f6c 732d  -analysis-tools-
+00000300: 646f 673e 3d30 2e30 2e31 0d0a 0964 6174  dog>=0.0.1...dat
+00000310: 612d 616e 616c 7973 6973 2d74 6f6f 6c73  a-analysis-tools
+00000320: 2d65 7468 3e3d 302e 302e 310d 0a09 6461  -eth>=0.0.1...da
+00000330: 7461 2d61 6e61 6c79 7369 732d 6174 7472  ta-analysis-attr
+00000340: 6962 7574 652d 746f 6f6c 2d6a 6d73 3e3d  ibute-tool-jms>=
+00000350: 302e 302e 320d 0a09 6461 7461 2d61 6e61  0.0.2...data-ana
+00000360: 6c79 7369 732d 746f 6f6c 732d 6a6d 732d  lysis-tools-jms-
+00000370: 7365 673e 3d30 2e30 2e32 0d0a 0d0a 5b65  seg>=0.0.2....[e
+00000380: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
+00000390: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
+000003a0: 203d 2030 0d0a 0d0a                       = 0....
```

