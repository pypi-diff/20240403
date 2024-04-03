# Comparing `tmp/kso_utils-0.1.0.tar.gz` & `tmp/kso_utils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kso_utils-0.1.0.tar", max compression
+gzip compressed data, was "kso_utils-0.2.0.tar", max compression
```

## Comparing `kso_utils-0.1.0.tar` & `kso_utils-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,25 @@
--rw-r--r--   0        0        0     1082 2023-04-04 08:07:54.094605 kso_utils-0.1.0/LICENSE
--rw-r--r--   0        0        0     3301 2022-03-22 14:40:29.745222 kso_utils-0.1.0/README.md
--rw-r--r--   0        0        0        0 2022-02-07 18:38:40.947472 kso_utils-0.1.0/kso_utils/__init__.py
--rw-r--r--   0        0        0      807 2023-03-28 14:48:37.378828 kso_utils-0.1.0/kso_utils/db_csv_info/movies_example.csv
--rw-r--r--   0        0        0      279 2023-03-28 14:48:37.379066 kso_utils-0.1.0/kso_utils/db_csv_info/sites_example.csv
--rw-r--r--   0        0        0     6375 2023-03-28 14:48:37.379259 kso_utils-0.1.0/kso_utils/db_csv_info/species_example.csv
--rw-r--r--   0        0        0        0 2022-11-16 15:24:33.417505 kso_utils-0.1.0/kso_utils/db_starter/__init__.py
--rw-r--r--   0        0        0      126 2022-11-23 09:26:11.841199 kso_utils-0.1.0/kso_utils/db_starter/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2291 2023-03-15 10:22:56.546589 kso_utils-0.1.0/kso_utils/db_starter/__pycache__/schema.cpython-38.pyc
--rwxr-xr-x   0        0        0     1079 2023-03-17 08:31:12.045288 kso_utils-0.1.0/kso_utils/db_starter/projects_list.csv
--rwxr-xr-x   0        0        0     2110 2023-03-15 10:12:07.026156 kso_utils-0.1.0/kso_utils/db_starter/schema.py
--rw-r--r--   0        0        0     6413 2023-03-28 12:58:06.209794 kso_utils-0.1.0/kso_utils/db_utils.py
--rw-r--r--   0        0        0     3397 2023-03-28 13:00:50.764117 kso_utils-0.1.0/kso_utils/frame_utils.py
--rw-r--r--   0        0        0    13339 2023-03-28 12:58:06.362518 kso_utils-0.1.0/kso_utils/koster_utils.py
--rw-r--r--   0        0        0    16439 2023-03-28 12:58:06.420614 kso_utils-0.1.0/kso_utils/movie_utils.py
--rw-r--r--   0        0        0    47244 2023-03-28 14:14:08.940051 kso_utils-0.1.0/kso_utils/project.py
--rw-r--r--   0        0        0     2706 2023-04-04 08:30:59.501500 kso_utils-0.1.0/kso_utils/project_utils.py
--rw-r--r--   0        0        0    19525 2023-04-04 08:23:05.079121 kso_utils-0.1.0/kso_utils/server_utils.py
--rw-r--r--   0        0        0     6525 2023-03-15 10:12:07.028960 kso_utils-0.1.0/kso_utils/sgu_utils.py
--rw-r--r--   0        0        0    18792 2023-03-28 12:58:06.426179 kso_utils-0.1.0/kso_utils/spyfish_utils.py
--rw-r--r--   0        0        0     7454 2023-03-15 10:12:07.029335 kso_utils-0.1.0/kso_utils/t11_utils.py
--rw-r--r--   0        0        0       91 2023-03-15 10:12:07.029574 kso_utils-0.1.0/kso_utils/t15_utils.py
--rw-r--r--   0        0        0    46152 2023-03-28 12:58:06.951592 kso_utils-0.1.0/kso_utils/t1_utils.py
--rw-r--r--   0        0        0    65466 2023-04-04 08:25:35.826910 kso_utils-0.1.0/kso_utils/t2_utils.py
--rw-r--r--   0        0        0    39759 2023-04-04 08:26:36.650146 kso_utils-0.1.0/kso_utils/t3_utils.py
--rw-r--r--   0        0        0    29108 2023-04-04 08:27:25.301642 kso_utils-0.1.0/kso_utils/t4_utils.py
--rw-r--r--   0        0        0    10673 2023-03-23 11:07:56.808963 kso_utils-0.1.0/kso_utils/t5_utils.py
--rw-r--r--   0        0        0    34147 2023-03-27 15:56:02.892496 kso_utils-0.1.0/kso_utils/t6_utils.py
--rw-r--r--   0        0        0     2668 2023-03-06 15:51:52.506981 kso_utils-0.1.0/kso_utils/t7_utils.py
--rw-r--r--   0        0        0    55389 2023-04-04 08:27:54.176432 kso_utils-0.1.0/kso_utils/t8_utils.py
--rw-r--r--   0        0        0    10765 2023-03-28 12:58:06.735739 kso_utils-0.1.0/kso_utils/tutorials_utils.py
--rw-r--r--   0        0        0    29969 2023-03-28 13:05:47.871693 kso_utils-0.1.0/kso_utils/yolo_utils.py
--rw-r--r--   0        0        0     3340 2023-04-03 14:30:42.060244 kso_utils-0.1.0/kso_utils/zenodo_utils.py
--rw-r--r--   0        0        0    18850 2023-03-28 12:58:06.888020 kso_utils-0.1.0/kso_utils/zooniverse_utils.py
--rw-r--r--   0        0        0      954 2023-03-28 14:13:13.523925 kso_utils-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4639 1970-01-01 00:00:00.000000 kso_utils-0.1.0/setup.py
--rw-r--r--   0        0        0     4858 1970-01-01 00:00:00.000000 kso_utils-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35126 2023-09-21 14:24:50.986126 kso_utils-0.2.0/LICENSE
+-rw-r--r--   0        0        0    14312 2024-04-02 13:24:27.140946 kso_utils-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-09-21 14:24:50.996729 kso_utils-0.2.0/kso_utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-21 14:24:50.996795 kso_utils-0.2.0/kso_utils/db_starter/__init__.py
+-rw-r--r--   0        0        0     1079 2024-04-02 13:24:18.424978 kso_utils-0.2.0/kso_utils/db_starter/cdn_projects_list.csv
+-rw-r--r--   0        0        0     1461 2024-02-28 09:49:51.234739 kso_utils-0.2.0/kso_utils/db_starter/projects_list.csv
+-rw-r--r--   0        0        0     1994 2024-04-02 13:24:18.425126 kso_utils-0.2.0/kso_utils/db_starter/schema.py
+-rw-r--r--   0        0        0    17893 2024-04-02 13:24:18.425340 kso_utils-0.2.0/kso_utils/db_utils.py
+-rw-r--r--   0        0        0     6741 2024-04-02 13:24:18.426034 kso_utils-0.2.0/kso_utils/frame_utils.py
+-rw-r--r--   0        0        0     4091 2023-09-22 19:06:03.217864 kso_utils-0.2.0/kso_utils/general.py
+-rw-r--r--   0        0        0    13317 2024-04-02 13:24:18.426336 kso_utils-0.2.0/kso_utils/koster_utils.py
+-rw-r--r--   0        0        0    31563 2024-04-02 13:24:18.426758 kso_utils-0.2.0/kso_utils/movie_utils.py
+-rw-r--r--   0        0        0    95930 2024-04-02 13:24:18.427610 kso_utils-0.2.0/kso_utils/project.py
+-rw-r--r--   0        0        0     3606 2024-04-02 13:24:18.428216 kso_utils-0.2.0/kso_utils/project_utils.py
+-rw-r--r--   0        0        0    14924 2024-04-02 13:24:18.428542 kso_utils-0.2.0/kso_utils/server_utils.py
+-rw-r--r--   0        0        0     6295 2024-04-02 13:24:18.429109 kso_utils-0.2.0/kso_utils/sgu_utils.py
+-rw-r--r--   0        0        0    10031 2024-04-02 13:24:18.429517 kso_utils-0.2.0/kso_utils/spyfish_utils.py
+-rw-r--r--   0        0        0    13795 2024-04-02 13:24:18.430086 kso_utils-0.2.0/kso_utils/video_reader.py
+-rw-r--r--   0        0        0    76147 2024-04-02 13:24:18.430796 kso_utils-0.2.0/kso_utils/widgets.py
+-rw-r--r--   0        0        0    80905 2024-04-02 15:03:44.770676 kso_utils-0.2.0/kso_utils/yolo_utils.py
+-rw-r--r--   0        0        0     3347 2023-09-21 14:24:50.998838 kso_utils-0.2.0/kso_utils/zenodo_utils.py
+-rw-r--r--   0        0        0    85468 2024-04-02 13:24:18.432485 kso_utils-0.2.0/kso_utils/zooniverse_utils.py
+-rw-r--r--   0        0        0     2527 2024-04-02 13:29:54.856409 kso_utils-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    15776 1970-01-01 00:00:00.000000 kso_utils-0.2.0/setup.py
+-rw-r--r--   0        0        0    15871 1970-01-01 00:00:00.000000 kso_utils-0.2.0/PKG-INFO
```

### Comparing `kso_utils-0.1.0/kso_utils/db_starter/__pycache__/schema.cpython-38.pyc` & `kso_utils-0.2.0/kso_utils/db_starter/schema.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,144 +1,125 @@
-00000000: 550d 0d0a 0000 0000 f799 1164 3e08 0000  U..........d>...
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0001 0000 0040 0000 0073 0800 0000 6400  .....@...s....d.
-00000030: 5a00 6401 5300 2902 6131 0800 0043 5245  Z.d.S.).a1...CRE
-00000040: 4154 4520 5441 424c 4520 4946 204e 4f54  ATE TABLE IF NOT
-00000050: 2045 5849 5354 5320 7369 7465 730a 280a   EXISTS sites.(.
-00000060: 6964 2069 6e74 6567 6572 2050 5249 4d41  id integer PRIMA
-00000070: 5259 204b 4559 2c0a 7369 7465 4e61 6d65  RY KEY,.siteName
-00000080: 2074 6578 7420 4e55 4c4c 2c0a 6465 6369   text NULL,.deci
-00000090: 6d61 6c4c 6174 6974 7564 6520 7661 7263  malLatitude varc
-000000a0: 6861 7228 3235 3529 204e 554c 4c2c 0a64  har(255) NULL,.d
-000000b0: 6563 696d 616c 4c6f 6e67 6974 7564 6520  ecimalLongitude 
-000000c0: 7661 7263 6861 7228 3235 3529 204e 554c  varchar(255) NUL
-000000d0: 4c2c 0a67 656f 6465 7469 6344 6174 756d  L,.geodeticDatum
-000000e0: 2076 6172 6368 6172 2832 3535 2920 4e55   varchar(255) NU
-000000f0: 4c4c 2c0a 636f 756e 7472 7943 6f64 6520  LL,.countryCode 
-00000100: 7661 7263 6861 7228 3235 3529 204e 554c  varchar(255) NUL
-00000110: 4c2c 0a55 4e49 5155 4520 2873 6974 654e  L,.UNIQUE (siteN
-00000120: 616d 6529 0a29 3b0a 0a43 5245 4154 4520  ame).);..CREATE 
-00000130: 5441 424c 4520 4946 204e 4f54 2045 5849  TABLE IF NOT EXI
-00000140: 5354 5320 6d6f 7669 6573 0a28 0a69 6420  STS movies.(.id 
-00000150: 696e 7465 6765 7220 5052 494d 4152 5920  integer PRIMARY 
-00000160: 4b45 592c 0a66 696c 656e 616d 6520 7465  KEY,.filename te
-00000170: 7874 204e 4f54 204e 554c 4c2c 0a63 7265  xt NOT NULL,.cre
-00000180: 6174 6564 5f6f 6e20 6461 7465 7469 6d65  ated_on datetime
-00000190: 204e 554c 4c2c 0a66 7073 2072 6561 6c20   NULL,.fps real 
-000001a0: 4e55 4c4c 2c0a 6475 7261 7469 6f6e 2064  NULL,.duration d
-000001b0: 6174 6574 696d 6520 4e55 4c4c 2c0a 7361  atetime NULL,.sa
-000001c0: 6d70 6c69 6e67 5f73 7461 7274 2072 6561  mpling_start rea
-000001d0: 6c20 4e55 4c4c 2c0a 7361 6d70 6c69 6e67  l NULL,.sampling
-000001e0: 5f65 6e64 2072 6561 6c20 4e55 4c4c 2c0a  _end real NULL,.
-000001f0: 6175 7468 6f72 2074 6578 7420 4e55 4c4c  author text NULL
-00000200: 2c0a 7369 7465 5f69 6420 696e 7465 6765  ,.site_id intege
-00000210: 7220 4e55 4c4c 2c0a 6670 6174 6820 7465  r NULL,.fpath te
-00000220: 7874 204e 554c 4c2c 0a55 4e49 5155 4520  xt NULL,.UNIQUE 
-00000230: 2866 696c 656e 616d 6529 2c0a 464f 5245  (filename),.FORE
-00000240: 4947 4e20 4b45 5920 2873 6974 655f 6964  IGN KEY (site_id
-00000250: 2920 5245 4645 5245 4e43 4553 2073 6974  ) REFERENCES sit
-00000260: 6573 2028 6964 290a 293b 0a0a 4352 4541  es (id).);..CREA
-00000270: 5445 2054 4142 4c45 2049 4620 4e4f 5420  TE TABLE IF NOT 
-00000280: 4558 4953 5453 2070 686f 746f 730a 280a  EXISTS photos.(.
-00000290: 6964 2069 6e74 6567 6572 2050 5249 4d41  id integer PRIMA
-000002a0: 5259 204b 4559 2c0a 6669 6c65 6e61 6d65  RY KEY,.filename
-000002b0: 2074 6578 7420 4e4f 5420 4e55 4c4c 2c0a   text NOT NULL,.
-000002c0: 5068 6f74 6f50 6f73 6974 696f 6e20 696e  PhotoPosition in
-000002d0: 7420 4e55 4c4c 2c0a 7369 7465 4e61 6d65  t NULL,.siteName
-000002e0: 2074 6578 7420 4e55 4c4c 2c0a 5375 7276   text NULL,.Surv
-000002f0: 6579 4944 2069 6e74 204e 554c 4c2c 0a55  eyID int NULL,.U
-00000300: 4e49 5155 4520 2866 696c 656e 616d 6529  NIQUE (filename)
-00000310: 0a29 3b20 0a0a 4352 4541 5445 2054 4142  .); ..CREATE TAB
-00000320: 4c45 2049 4620 4e4f 5420 4558 4953 5453  LE IF NOT EXISTS
-00000330: 2073 7562 6a65 6374 730a 280a 6964 2069   subjects.(.id i
-00000340: 6e74 6567 6572 2050 5249 4d41 5259 204b  nteger PRIMARY K
-00000350: 4559 2c0a 7375 626a 6563 745f 7479 7065  EY,.subject_type
-00000360: 2076 6172 6368 6172 2832 3535 2920 4e55   varchar(255) NU
-00000370: 4c4c 2c0a 6669 6c65 6e61 6d65 2074 6578  LL,.filename tex
-00000380: 7420 4e55 4c4c 2c0a 636c 6970 5f73 7461  t NULL,.clip_sta
-00000390: 7274 5f74 696d 6520 6461 7465 7469 6d65  rt_time datetime
-000003a0: 204e 554c 4c2c 0a63 6c69 705f 656e 645f   NULL,.clip_end_
-000003b0: 7469 6d65 2064 6174 6574 696d 6520 4e55  time datetime NU
-000003c0: 4c4c 2c0a 6672 616d 655f 6578 705f 7370  LL,.frame_exp_sp
-000003d0: 5f69 6420 696e 7465 6765 7220 4e55 4c4c  _id integer NULL
-000003e0: 2c0a 6672 616d 655f 6e75 6d62 6572 2069  ,.frame_number i
-000003f0: 6e74 6567 6572 204e 554c 4c2c 0a77 6f72  nteger NULL,.wor
-00000400: 6b66 6c6f 775f 6964 2076 6172 6368 6172  kflow_id varchar
-00000410: 2832 3535 2920 4e55 4c4c 2c0a 7375 626a  (255) NULL,.subj
-00000420: 6563 745f 7365 745f 6964 2076 6172 6368  ect_set_id varch
-00000430: 6172 2832 3535 292c 0a63 6c61 7373 6966  ar(255),.classif
-00000440: 6963 6174 696f 6e73 5f63 6f75 6e74 2069  ications_count i
-00000450: 6e74 6567 6572 204e 554c 4c2c 0a72 6574  nteger NULL,.ret
-00000460: 6972 6564 5f61 7420 6461 7465 7469 6d65  ired_at datetime
-00000470: 204e 554c 4c2c 0a72 6574 6972 656d 656e   NULL,.retiremen
-00000480: 745f 7265 6173 6f6e 2074 6578 7420 4e55  t_reason text NU
-00000490: 4c4c 2c0a 6372 6561 7465 645f 6174 2064  LL,.created_at d
-000004a0: 6174 6574 696d 652c 0a68 7474 7073 5f6c  atetime,.https_l
-000004b0: 6f63 6174 696f 6e20 7465 7874 204e 554c  ocation text NUL
-000004c0: 4c2c 0a6d 6f76 6965 5f69 6420 696e 7465  L,.movie_id inte
-000004d0: 6765 7220 4e55 4c4c 2c0a 464f 5245 4947  ger NULL,.FOREIG
-000004e0: 4e20 4b45 5920 286d 6f76 6965 5f69 6429  N KEY (movie_id)
-000004f0: 2052 4546 4552 454e 4345 5320 6d6f 7669   REFERENCES movi
-00000500: 6573 2028 6964 290a 293b 0a0a 4352 4541  es (id).);..CREA
-00000510: 5445 2054 4142 4c45 2049 4620 4e4f 5420  TE TABLE IF NOT 
-00000520: 4558 4953 5453 2073 7065 6369 6573 0a28  EXISTS species.(
-00000530: 0a69 6420 696e 7465 6765 7220 5052 494d  .id integer PRIM
-00000540: 4152 5920 4b45 592c 0a6c 6162 656c 2074  ARY KEY,.label t
-00000550: 6578 7420 4e4f 5420 4e55 4c4c 2c0a 7363  ext NOT NULL,.sc
-00000560: 6965 6e74 6966 6963 4e61 6d65 2074 6578  ientificName tex
-00000570: 7420 4e4f 5420 4e55 4c4c 2c0a 7461 786f  t NOT NULL,.taxo
-00000580: 6e52 616e 6b20 7465 7874 204e 4f54 204e  nRank text NOT N
-00000590: 554c 4c2c 0a6b 696e 6764 6f6d 2074 6578  ULL,.kingdom tex
-000005a0: 7420 4e4f 5420 4e55 4c4c 2c0a 554e 4951  t NOT NULL,.UNIQ
-000005b0: 5545 2028 6c61 6265 6c29 0a29 3b0a 0a43  UE (label).);..C
-000005c0: 5245 4154 4520 5441 424c 4520 4946 204e  REATE TABLE IF N
-000005d0: 4f54 2045 5849 5354 5320 6167 675f 616e  OT EXISTS agg_an
-000005e0: 6e6f 7461 7469 6f6e 735f 636c 6970 0a28  notations_clip.(
-000005f0: 0a69 6420 696e 7465 6765 7220 5052 494d  .id integer PRIM
-00000600: 4152 5920 4b45 5920 4155 544f 494e 4352  ARY KEY AUTOINCR
-00000610: 454d 454e 542c 0a73 7065 6369 6573 5f69  EMENT,.species_i
-00000620: 6420 696e 7465 6765 722c 0a68 6f77 5f6d  d integer,.how_m
-00000630: 616e 7920 696e 7465 6765 722c 0a66 6972  any integer,.fir
-00000640: 7374 5f73 6565 6e20 696e 7465 6765 722c  st_seen integer,
-00000650: 0a73 7562 6a65 6374 5f69 6420 696e 7465  .subject_id inte
-00000660: 6765 722c 0a55 4e49 5155 4528 7370 6563  ger,.UNIQUE(spec
-00000670: 6965 735f 6964 2c20 7375 626a 6563 745f  ies_id, subject_
-00000680: 6964 290a 464f 5245 4947 4e20 4b45 5920  id).FOREIGN KEY 
-00000690: 2873 7562 6a65 6374 5f69 6429 2052 4546  (subject_id) REF
-000006a0: 4552 454e 4345 5320 7375 626a 6563 7473  ERENCES subjects
-000006b0: 2028 6964 292c 0a46 4f52 4549 474e 204b   (id),.FOREIGN K
-000006c0: 4559 2028 7370 6563 6965 735f 6964 2920  EY (species_id) 
-000006d0: 5245 4645 5245 4e43 4553 2073 7065 6369  REFERENCES speci
-000006e0: 6573 2028 6964 290a 293b 0a0a 4352 4541  es (id).);..CREA
-000006f0: 5445 2054 4142 4c45 2049 4620 4e4f 5420  TE TABLE IF NOT 
-00000700: 4558 4953 5453 2061 6767 5f61 6e6e 6f74  EXISTS agg_annot
-00000710: 6174 696f 6e73 5f66 7261 6d65 0a28 0a69  ations_frame.(.i
-00000720: 6420 696e 7465 6765 7220 5052 494d 4152  d integer PRIMAR
-00000730: 5920 4b45 5920 4155 544f 494e 4352 454d  Y KEY AUTOINCREM
-00000740: 454e 542c 0a73 7065 6369 6573 5f69 6420  ENT,.species_id 
-00000750: 696e 7465 6765 7220 4e55 4c4c 2c0a 785f  integer NULL,.x_
-00000760: 706f 7369 7469 6f6e 2072 6561 6c20 4e55  position real NU
-00000770: 4c4c 2c0a 795f 706f 7369 7469 6f6e 2072  LL,.y_position r
-00000780: 6561 6c20 4e55 4c4c 2c0a 7769 6474 6820  eal NULL,.width 
-00000790: 7265 616c 204e 554c 4c2c 0a68 6569 6768  real NULL,.heigh
-000007a0: 7420 7265 616c 204e 554c 4c2c 0a73 7562  t real NULL,.sub
-000007b0: 6a65 6374 5f69 6420 696e 7465 6765 722c  ject_id integer,
-000007c0: 0a55 4e49 5155 4528 7370 6563 6965 735f  .UNIQUE(species_
-000007d0: 6964 2c20 785f 706f 7369 7469 6f6e 2c20  id, x_position, 
-000007e0: 795f 706f 7369 7469 6f6e 2c20 7769 6474  y_position, widt
-000007f0: 682c 2068 6569 6768 742c 2073 7562 6a65  h, height, subje
-00000800: 6374 5f69 6429 0a46 4f52 4549 474e 204b  ct_id).FOREIGN K
-00000810: 4559 2028 7370 6563 6965 735f 6964 2920  EY (species_id) 
-00000820: 5245 4645 5245 4e43 4553 2073 7065 6369  REFERENCES speci
-00000830: 6573 2028 6964 292c 0a46 4f52 4549 474e  es (id),.FOREIGN
-00000840: 204b 4559 2028 7375 626a 6563 745f 6964   KEY (subject_id
-00000850: 2920 5245 4645 5245 4e43 4553 2073 7562  ) REFERENCES sub
-00000860: 6a65 6374 7320 2869 6429 0a29 3b0a 4e29  jects (id).);.N)
-00000870: 01da 0373 716c a900 7202 0000 0072 0200  ...sql..r....r..
-00000880: 0000 fa5c 2f55 7365 7273 2f6a 7572 6965  ...\/Users/jurie
-00000890: 2e67 6572 6d69 7368 7579 732f 576f 726b  .germishuys/Work
-000008a0: 7370 6163 652f 6f64 662f 6b6f 7374 6572  space/odf/koster
-000008b0: 2d75 772f 6d6f 6465 6c73 2f79 6f6c 6f76  -uw/models/yolov
-000008c0: 352f 6b73 6f5f 7574 696c 732f 6462 5f73  5/kso_utils/db_s
-000008d0: 7461 7274 6572 2f73 6368 656d 612e 7079  tarter/schema.py
-000008e0: da08 3c6d 6f64 756c 653e 0100 0000 f300  ..<module>......
-000008f0: 0000 00                                  ...
+00000000: 7371 6c20 3d20 2222 2243 5245 4154 4520  sql = """CREATE 
+00000010: 5441 424c 4520 4946 204e 4f54 2045 5849  TABLE IF NOT EXI
+00000020: 5354 5320 7369 7465 730a 280a 6964 2069  STS sites.(.id i
+00000030: 6e74 6567 6572 2050 5249 4d41 5259 204b  nteger PRIMARY K
+00000040: 4559 2c0a 7369 7465 4e61 6d65 2074 6578  EY,.siteName tex
+00000050: 7420 4e55 4c4c 2c0a 6465 6369 6d61 6c4c  t NULL,.decimalL
+00000060: 6174 6974 7564 6520 7661 7263 6861 7228  atitude varchar(
+00000070: 3235 3529 204e 554c 4c2c 0a64 6563 696d  255) NULL,.decim
+00000080: 616c 4c6f 6e67 6974 7564 6520 7661 7263  alLongitude varc
+00000090: 6861 7228 3235 3529 204e 554c 4c2c 0a67  har(255) NULL,.g
+000000a0: 656f 6465 7469 6344 6174 756d 2076 6172  eodeticDatum var
+000000b0: 6368 6172 2832 3535 2920 4e55 4c4c 2c0a  char(255) NULL,.
+000000c0: 636f 756e 7472 7943 6f64 6520 7661 7263  countryCode varc
+000000d0: 6861 7228 3235 3529 204e 554c 4c2c 0a55  har(255) NULL,.U
+000000e0: 4e49 5155 4520 2873 6974 654e 616d 6529  NIQUE (siteName)
+000000f0: 0a29 3b0a 0a43 5245 4154 4520 5441 424c  .);..CREATE TABL
+00000100: 4520 4946 204e 4f54 2045 5849 5354 5320  E IF NOT EXISTS 
+00000110: 6d6f 7669 6573 0a28 0a69 6420 696e 7465  movies.(.id inte
+00000120: 6765 7220 5052 494d 4152 5920 4b45 592c  ger PRIMARY KEY,
+00000130: 0a66 696c 656e 616d 6520 7465 7874 204e  .filename text N
+00000140: 4f54 204e 554c 4c2c 0a63 7265 6174 6564  OT NULL,.created
+00000150: 5f6f 6e20 6461 7465 7469 6d65 204e 554c  _on datetime NUL
+00000160: 4c2c 0a66 7073 2072 6561 6c20 4e55 4c4c  L,.fps real NULL
+00000170: 2c0a 6475 7261 7469 6f6e 2064 6174 6574  ,.duration datet
+00000180: 696d 6520 4e55 4c4c 2c0a 7361 6d70 6c69  ime NULL,.sampli
+00000190: 6e67 5f73 7461 7274 2072 6561 6c20 4e55  ng_start real NU
+000001a0: 4c4c 2c0a 7361 6d70 6c69 6e67 5f65 6e64  LL,.sampling_end
+000001b0: 2072 6561 6c20 4e55 4c4c 2c0a 6175 7468   real NULL,.auth
+000001c0: 6f72 2074 6578 7420 4e55 4c4c 2c0a 7369  or text NULL,.si
+000001d0: 7465 5f69 6420 7465 7874 204e 554c 4c2c  te_id text NULL,
+000001e0: 0a66 7061 7468 2074 6578 7420 4e55 4c4c  .fpath text NULL
+000001f0: 2c0a 554e 4951 5545 2028 6669 6c65 6e61  ,.UNIQUE (filena
+00000200: 6d65 292c 0a46 4f52 4549 474e 204b 4559  me),.FOREIGN KEY
+00000210: 2028 7369 7465 5f69 6429 2052 4546 4552   (site_id) REFER
+00000220: 454e 4345 5320 7369 7465 7320 2869 6429  ENCES sites (id)
+00000230: 0a29 3b0a 0a43 5245 4154 4520 5441 424c  .);..CREATE TABL
+00000240: 4520 4946 204e 4f54 2045 5849 5354 5320  E IF NOT EXISTS 
+00000250: 7068 6f74 6f73 0a28 0a69 6420 696e 7465  photos.(.id inte
+00000260: 6765 7220 5052 494d 4152 5920 4b45 592c  ger PRIMARY KEY,
+00000270: 0a66 696c 656e 616d 6520 7465 7874 204e  .filename text N
+00000280: 4f54 204e 554c 4c2c 0a50 686f 746f 506f  OT NULL,.PhotoPo
+00000290: 7369 7469 6f6e 2069 6e74 204e 554c 4c2c  sition int NULL,
+000002a0: 0a73 6974 654e 616d 6520 7465 7874 204e  .siteName text N
+000002b0: 554c 4c2c 0a53 7572 7665 7949 4420 696e  ULL,.SurveyID in
+000002c0: 7420 4e55 4c4c 2c0a 554e 4951 5545 2028  t NULL,.UNIQUE (
+000002d0: 6669 6c65 6e61 6d65 290a 293b 0a0a 4352  filename).);..CR
+000002e0: 4541 5445 2054 4142 4c45 2049 4620 4e4f  EATE TABLE IF NO
+000002f0: 5420 4558 4953 5453 2073 7562 6a65 6374  T EXISTS subject
+00000300: 730a 280a 6964 2069 6e74 6567 6572 2050  s.(.id integer P
+00000310: 5249 4d41 5259 204b 4559 2c0a 7375 626a  RIMARY KEY,.subj
+00000320: 6563 745f 7479 7065 2076 6172 6368 6172  ect_type varchar
+00000330: 2832 3535 2920 4e55 4c4c 2c0a 6669 6c65  (255) NULL,.file
+00000340: 6e61 6d65 2074 6578 7420 4e55 4c4c 2c0a  name text NULL,.
+00000350: 636c 6970 5f73 7461 7274 5f74 696d 6520  clip_start_time 
+00000360: 6461 7465 7469 6d65 204e 554c 4c2c 0a63  datetime NULL,.c
+00000370: 6c69 705f 656e 645f 7469 6d65 2064 6174  lip_end_time dat
+00000380: 6574 696d 6520 4e55 4c4c 2c0a 6672 616d  etime NULL,.fram
+00000390: 655f 6578 705f 7370 5f69 6420 696e 7465  e_exp_sp_id inte
+000003a0: 6765 7220 4e55 4c4c 2c0a 6672 616d 655f  ger NULL,.frame_
+000003b0: 6e75 6d62 6572 2069 6e74 6567 6572 204e  number integer N
+000003c0: 554c 4c2c 0a73 7562 6a65 6374 5f73 6574  ULL,.subject_set
+000003d0: 5f69 6420 7661 7263 6861 7228 3235 3529  _id varchar(255)
+000003e0: 2c0a 6372 6561 7465 645f 6174 2064 6174  ,.created_at dat
+000003f0: 6574 696d 652c 0a68 7474 7073 5f6c 6f63  etime,.https_loc
+00000400: 6174 696f 6e20 7465 7874 204e 554c 4c2c  ation text NULL,
+00000410: 0a6d 6f76 6965 5f69 6420 696e 7465 6765  .movie_id intege
+00000420: 7220 4e55 4c4c 2c0a 464f 5245 4947 4e20  r NULL,.FOREIGN 
+00000430: 4b45 5920 286d 6f76 6965 5f69 6429 2052  KEY (movie_id) R
+00000440: 4546 4552 454e 4345 5320 6d6f 7669 6573  EFERENCES movies
+00000450: 2028 6964 290a 293b 0a0a 4352 4541 5445   (id).);..CREATE
+00000460: 2054 4142 4c45 2049 4620 4e4f 5420 4558   TABLE IF NOT EX
+00000470: 4953 5453 2073 7065 6369 6573 0a28 0a69  ISTS species.(.i
+00000480: 6420 696e 7465 6765 7220 5052 494d 4152  d integer PRIMAR
+00000490: 5920 4b45 592c 0a63 6f6d 6d6f 6e4e 616d  Y KEY,.commonNam
+000004a0: 6520 7465 7874 204e 4f54 204e 554c 4c2c  e text NOT NULL,
+000004b0: 0a73 6369 656e 7469 6669 634e 616d 6520  .scientificName 
+000004c0: 7465 7874 204e 4f54 204e 554c 4c2c 0a74  text NOT NULL,.t
+000004d0: 6178 6f6e 5261 6e6b 2074 6578 7420 4e4f  axonRank text NO
+000004e0: 5420 4e55 4c4c 2c0a 6b69 6e67 646f 6d20  T NULL,.kingdom 
+000004f0: 7465 7874 204e 4f54 204e 554c 4c2c 0a55  text NOT NULL,.U
+00000500: 4e49 5155 4520 2863 6f6d 6d6f 6e4e 616d  NIQUE (commonNam
+00000510: 6529 0a29 3b0a 0a43 5245 4154 4520 5441  e).);..CREATE TA
+00000520: 424c 4520 4946 204e 4f54 2045 5849 5354  BLE IF NOT EXIST
+00000530: 5320 6167 675f 616e 6e6f 7461 7469 6f6e  S agg_annotation
+00000540: 735f 636c 6970 0a28 0a69 6420 696e 7465  s_clip.(.id inte
+00000550: 6765 7220 5052 494d 4152 5920 4b45 5920  ger PRIMARY KEY 
+00000560: 4155 544f 494e 4352 454d 454e 542c 0a73  AUTOINCREMENT,.s
+00000570: 7065 6369 6573 5f69 6420 696e 7465 6765  pecies_id intege
+00000580: 722c 0a68 6f77 5f6d 616e 7920 696e 7465  r,.how_many inte
+00000590: 6765 722c 0a66 6972 7374 5f73 6565 6e20  ger,.first_seen 
+000005a0: 696e 7465 6765 722c 0a73 7562 6a65 6374  integer,.subject
+000005b0: 5f69 6420 696e 7465 6765 722c 0a55 4e49  _id integer,.UNI
+000005c0: 5155 4528 7370 6563 6965 735f 6964 2c20  QUE(species_id, 
+000005d0: 7375 626a 6563 745f 6964 290a 464f 5245  subject_id).FORE
+000005e0: 4947 4e20 4b45 5920 2873 7562 6a65 6374  IGN KEY (subject
+000005f0: 5f69 6429 2052 4546 4552 454e 4345 5320  _id) REFERENCES 
+00000600: 7375 626a 6563 7473 2028 6964 292c 0a46  subjects (id),.F
+00000610: 4f52 4549 474e 204b 4559 2028 7370 6563  OREIGN KEY (spec
+00000620: 6965 735f 6964 2920 5245 4645 5245 4e43  ies_id) REFERENC
+00000630: 4553 2073 7065 6369 6573 2028 6964 290a  ES species (id).
+00000640: 293b 0a0a 4352 4541 5445 2054 4142 4c45  );..CREATE TABLE
+00000650: 2049 4620 4e4f 5420 4558 4953 5453 2061   IF NOT EXISTS a
+00000660: 6767 5f61 6e6e 6f74 6174 696f 6e73 5f66  gg_annotations_f
+00000670: 7261 6d65 0a28 0a69 6420 696e 7465 6765  rame.(.id intege
+00000680: 7220 5052 494d 4152 5920 4b45 5920 4155  r PRIMARY KEY AU
+00000690: 544f 494e 4352 454d 454e 542c 0a73 7065  TOINCREMENT,.spe
+000006a0: 6369 6573 5f69 6420 696e 7465 6765 7220  cies_id integer 
+000006b0: 4e55 4c4c 2c0a 785f 706f 7369 7469 6f6e  NULL,.x_position
+000006c0: 2072 6561 6c20 4e55 4c4c 2c0a 795f 706f   real NULL,.y_po
+000006d0: 7369 7469 6f6e 2072 6561 6c20 4e55 4c4c  sition real NULL
+000006e0: 2c0a 7769 6474 6820 7265 616c 204e 554c  ,.width real NUL
+000006f0: 4c2c 0a68 6569 6768 7420 7265 616c 204e  L,.height real N
+00000700: 554c 4c2c 0a73 7562 6a65 6374 5f69 6420  ULL,.subject_id 
+00000710: 696e 7465 6765 722c 0a55 4e49 5155 4528  integer,.UNIQUE(
+00000720: 7370 6563 6965 735f 6964 2c20 785f 706f  species_id, x_po
+00000730: 7369 7469 6f6e 2c20 795f 706f 7369 7469  sition, y_positi
+00000740: 6f6e 2c20 7769 6474 682c 2068 6569 6768  on, width, heigh
+00000750: 742c 2073 7562 6a65 6374 5f69 6429 0a46  t, subject_id).F
+00000760: 4f52 4549 474e 204b 4559 2028 7370 6563  OREIGN KEY (spec
+00000770: 6965 735f 6964 2920 5245 4645 5245 4e43  ies_id) REFERENC
+00000780: 4553 2073 7065 6369 6573 2028 6964 292c  ES species (id),
+00000790: 0a46 4f52 4549 474e 204b 4559 2028 7375  .FOREIGN KEY (su
+000007a0: 626a 6563 745f 6964 2920 5245 4645 5245  bject_id) REFERE
+000007b0: 4e43 4553 2073 7562 6a65 6374 7320 2869  NCES subjects (i
+000007c0: 6429 0a29 3b0a 2222 220a                 d).);.""".
```

### Comparing `kso_utils-0.1.0/kso_utils/koster_utils.py` & `kso_utils-0.2.0/kso_utils/koster_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,118 @@
 # -*- coding: utf-8 -*-
 # base imports
-import json
 import logging
+import sqlite3
+import ftfy
 import pandas as pd
-import numpy as np
-from sklearn.cluster import DBSCAN
 from pathlib import Path
-from collections import Counter
-
-# util imports
-from kso_utils.project_utils import Project
-from kso_utils.db_utils import get_movies_id
 
 # Logging
 logging.basicConfig()
 logging.getLogger().setLevel(logging.INFO)
 
 
-# Function to extract metadata from subjects
-def extract_metadata(subj_df: pd.DataFrame):
-    # Reset index of df
-    subj_df = subj_df.reset_index(drop=True).reset_index()
-
-    # Flatten the metadata information
-    meta_df = pd.json_normalize(subj_df.metadata.apply(json.loads))
-
-    # Drop metadata and index columns from original df
-    subj_df = subj_df.drop(
-        columns=[
-            "metadata",
-            "index",
-        ]
-    )
+def fix_text_encoding(string: str):
+    """This function corrects for text encoding errors, which occur when there is
+    for example an ä,å,ö present."""
+    return ftfy.fix_text(string)
+
+
+def fix_text_encoding_folder(folder_name):
+    """
+    This function corrects for text encoding errors, which occur when there is
+    for example an ä,å,ö present. It runs through all the file and folder names
+    of the directory you give it. It uses the package ftfy, which recognizes
+    which encoding the text has based on the text itself, and it encodes/decodes
+    it to utf8.
+    This function was tested on a Linux and Windows device with package version
+    6.1.1. With package version 5.8 it did not work.
+
+    This function can replace the unswedify and reswedify functions from
+    koster_utils, but this is not implemented yet.
+    """
+    for item in Path(folder_name).iterdir():
+        if item.is_dir():
+            for sub_item in item.iterdir():
+                old_path = sub_item
+                new_path = sub_item.parent / ftfy.fix_text(sub_item.name)
+                old_path.rename(new_path)
+
+
+def get_koster_col_names(table_name: str):
+    """Return a dictionary with the project-specific column names of a csv of interest
+    This function helps matching the schema format without modifying the column names of the original csv.
+
+    :param table_name: a string of the name of the schema table of interest
+    :return: a dictionary with the names of the columns
+    """
+
+    if table_name == "movies":
+        # Save the column names of interest in a dict
+        col_names_dic = {
+            "SamplingStart": "sampling_start",
+            "SamplingEnd": "sampling_end",
+        }
+    else:
+        # Create empty data frame as there are no project-specific
+        # columns for this table
+        col_names_dic = {}
 
-    return subj_df, meta_df
+    return col_names_dic
 
 
 # Function to process subjects uploaded automatically
 def auto_subjects(subjects_df: pd.DataFrame, auto_date: str):
+    """
+    The function `auto_subjects` selects and extracts metadata from subjects that were automatically
+    uploaded after a specified date.
+
+    :param subjects_df: `subjects_df` is a pandas DataFrame containing information about subjects, such
+    as their IDs, project IDs, and creation dates
+    :type subjects_df: pd.DataFrame
+    :param auto_date: auto_date is a string parameter that represents the date from which the function
+    should select automatically uploaded frames. The function will only select frames that were created
+    after this date
+    :type auto_date: str
+    :return: The function `auto_subjects` returns a pandas DataFrame containing metadata information
+    extracted from subjects that were automatically uploaded after a specified date.
+    """
     # Select automatically uploaded frames
     auto_subjects_df = subjects_df[(subjects_df["created_at"] > auto_date)]
 
+    from kso_utils.zooniverse_utils import extract_metadata
+
     # Extract metadata from automatically uploaded subjects
     auto_subjects_df, auto_subjects_meta = extract_metadata(auto_subjects_df)
 
     # Combine metadata info with the subjects df
     auto_subjects_df = pd.concat([auto_subjects_df, auto_subjects_meta], axis=1)
 
     return auto_subjects_df
 
 
 # Function to process subjects uploaded manually
 def manual_subjects(subjects_df: pd.DataFrame, manual_date: str, auto_date: str):
+    """
+    The function extracts metadata from manually uploaded clips and processes it to combine with the
+    subjects dataframe.
+
+    :param subjects_df: A pandas DataFrame containing information about subjects, including metadata and
+    creation dates
+    :type subjects_df: pd.DataFrame
+    :param manual_date: The date from which to start selecting clips uploaded manually
+    :type manual_date: str
+    :param auto_date: It seems like the parameter auto_date is missing from the code snippet. Can you
+    provide more information on what this parameter represents?
+    :type auto_date: str
+    :return: a pandas DataFrame containing information about clips that were uploaded manually, along
+    with their metadata and processed information.
+    """
+    from kso_utils.zooniverse_utils import extract_metadata
+
     # Select clips uploaded manually
     man_clips_df = (
         subjects_df[
             (subjects_df["metadata"].str.contains(".mp4"))
             & (subjects_df["created_at"].between(manual_date, auto_date))
         ]
         .reset_index(drop=True)
@@ -64,25 +121,39 @@
 
     # Specify the type of subject
     man_clips_df["subject_type"] = "clip"
 
     # Extract metadata from manually uploaded clips
     man_clips_df, man_clips_meta = extract_metadata(man_clips_df)
 
-    # Process the metadata of manually uploaded clips
-    man_clips_meta = process_manual_clips(man_clips_meta)
+    if len(man_clips_meta) > 0:
+        # Process the metadata of manually uploaded clips
+        man_clips_meta = process_manual_clips(man_clips_meta)
 
-    # Combine metadata info with the subjects df
-    man_clips_df = pd.concat([man_clips_df, man_clips_meta], axis=1)
+        # Combine metadata info with the subjects df
+        man_clips_df = pd.concat([man_clips_df, man_clips_meta], axis=1)
 
     return man_clips_df
 
 
 # Function to process the metadata of clips that were uploaded manually
 def process_manual_clips(meta_df: pd.DataFrame):
+    """
+    The function processes metadata of manual clips by extracting relevant information such as clip
+    start and end times and the filename of the original movie.
+
+    :param meta_df: The input parameter `meta_df` is a Pandas DataFrame containing metadata information
+    about video clips. It is assumed that the DataFrame has a column named "filename" which contains the
+    name of the video clip file in the format "original_movie_name_start_time.mp4". The function
+    processes this information to extract
+    :type meta_df: pd.DataFrame
+    :return: a pandas DataFrame containing the filename of the clips, the filename of the original
+    movie, the starting time of the clips in relation to the original movie, and the end time of the
+    clips in relation to the original movie.
+    """
     # Select the filename of the clips and remove extension type
     clip_filenames = meta_df["filename"].str.replace(".mp4", "", regex=True)
 
     # Get the starting time of clips in relation to the original movie
     # split the filename and select the last section
     meta_df["clip_start_time"] = clip_filenames.str.rsplit("_", 1).str[-1]
 
@@ -104,132 +175,102 @@
     meta_df = meta_df[
         ["filename", "movie_filename", "clip_start_time", "clip_end_time"]
     ]
 
     return meta_df
 
 
-# Function to get the list of duplicated subjects
-def get_duplicatesdf(project: Project):
-    # Define the path to the csv files with initial info to build the db
-    db_csv_info = project.csv_folder
-
-    # Define the path to the csv file with ids of the duplicated subjects
-    for file in Path(db_csv_info).rglob("*.csv"):
-        if "duplicat" in file.name:
-            duplicates_csv = file
-
-    # Load the csv with information about duplicated subjects
-    duplicatesdf = pd.read_csv(duplicates_csv)
-
-    return duplicatesdf
-
-
-# Function to select the first subject of those that are duplicated
-def clean_duplicated_subjects(subjects: pd.DataFrame, project: Project):
-    # Get the duplicates df
-    duplicatesdf = get_duplicatesdf(project)
-
-    # Include a column with unique ids for duplicated subjects
-    subjects = pd.merge(
-        subjects,
-        duplicatesdf,
-        how="left",
-        left_on="subject_id",
-        right_on="dupl_subject_id",
-    )
+def get_movies_id(df: pd.DataFrame, conn: sqlite3.Connection):
+    """
+    This function retrieves movie IDs based on movie filenames from a database and merges them with a
+    given DataFrame.
+
+    :param df: A pandas DataFrame containing information about movie filenames and clip subjects
+    :type df: pd.DataFrame
+    :param conn: SQL connection object
+    :return: a pandas DataFrame with the movie_ids added to the input DataFrame based on matching movie
+    filenames with the movies table in a SQLite database. The function drops the movie_filename column
+    before returning the DataFrame.
+    """
+    from kso_utils.db_utils import get_df_from_db_table
 
-    # Replace the id of duplicated subjects for the id of the first subject
-    subjects.subject_id = np.where(
-        subjects.single_subject_id.isnull(),
-        subjects.subject_id,
-        subjects.single_subject_id,
+    # Query id and filenames from the movies table
+    movies_df = get_df_from_db_table(conn, "movies")[["id", "filename"]]
+    movies_df = movies_df.rename(
+        columns={"id": "movie_id", "filename": "movie_filename"}
     )
 
-    # Select only unique subjects
-    subjects = subjects.drop_duplicates(subset="subject_id", keep="first")
+    # Check all the movies have a unique ID
+    df_unique = df.movie_filename.unique()
+    movies_df_unique = movies_df.movie_filename.unique()
+    diff_filenames = set(df_unique).difference(movies_df_unique)
 
-    return subjects
+    if diff_filenames:
+        raise ValueError(
+            f"There are clip subjects that don't have movie_id. The movie filenames are {diff_filenames}"
+        )
+
+    # Reference the manually uploaded subjects with the movies table
+    df = pd.merge(df, movies_df, how="left", on="movie_filename")
+
+    # Drop the movie_filename column
+    df = df.drop(columns=["movie_filename"])
+
+    return df
 
 
-def process_koster_subjects(subjects: pd.DataFrame, db_path: str):
+def process_koster_subjects(subjects: pd.DataFrame, conn: sqlite3.Connection):
     """
     This function takes in a dataframe of subjects and a path to the database and returns a dataframe of
     subjects with updated metadata
 
     :param subjects: the dataframe of subjects from the database
     :type subjects: pd.DataFrame
-    :param db_path: the path to the database
-    :type db_path: str
+    :param conn: SQL connection object
     :return: A dataframe with all the subjects that have been uploaded to the database.
     """
 
-    ## Set the date when the metadata of subjects uploaded matches/doesn't match schema.py requirements
-
+    # Set the date when the metadata of subjects uploaded matches/doesn't match schema.py requirements
     # Specify the date when the metadata of subjects uploaded matches schema.py
     auto_date = "2020-05-29 00:00:00 UTC"
 
     # Specify the starting date when clips were manually uploaded
     manual_date = "2019-11-17 00:00:00 UTC"
 
-    ## Update subjects automatically uploaded
-
     # Select automatically uploaded subjects
     auto_subjects_df = auto_subjects(subjects, auto_date=auto_date)
 
-    ## Update subjects manually uploaded
     # Select manually uploaded subjects
     manual_subjects_df = manual_subjects(
         subjects, manual_date=manual_date, auto_date=auto_date
     )
 
-    # Include movie_ids to the metadata
-    manual_subjects_df = get_movies_id(manual_subjects_df, db_path)
+    if len(manual_subjects_df) > 0:
+        # Include movie_ids to the metadata
+        manual_subjects_df = get_movies_id(manual_subjects_df, conn=conn)
 
-    # Combine all uploaded subjects
-    subjects = pd.merge(manual_subjects_df, auto_subjects_df, how="outer")
-
-    return subjects
-
-
-# Function to combine classifications received on duplicated subjects
-def combine_annot_from_duplicates(annot_df: pd.DataFrame, project: Project):
-    # Get the duplicates df
-    duplicatesdf = get_duplicatesdf(project)
-
-    # Include a column with unique ids for duplicated subjects
-    annot_df = pd.merge(
-        annot_df,
-        duplicatesdf,
-        how="left",
-        left_on="subject_ids",
-        right_on="dupl_subject_id",
-    )
+        # Combine all uploaded subjects
+        subjects = pd.merge(manual_subjects_df, auto_subjects_df, how="outer")
 
-    # Replace the id of duplicated subjects for the id of the first subject
-    annot_df["subject_ids"] = np.where(
-        annot_df.single_subject_id.isnull(),
-        annot_df.subject_ids,
-        annot_df.single_subject_id,
-    )
+    else:
+        subjects = auto_subjects_df
 
-    return annot_df
+    return subjects
 
 
 def process_clips_koster(annotations, row_class_id: str, rows_list: list):
     """
     For each annotation, if the task is T4, then for each species annotated, flatten the relevant
     answers and save the species of choice, class and subject id
 
     :param annotations: the list of annotations for a given classification
     :param row_class_id: the classification id of the row
     :param rows_list: list
     :type rows_list: list
-    :return: A list of dictionaries, each dictionary containing the classification id, the label, the
-    first time seen and how many individuals were seen.
+    :return: A list of dictionaries, each dictionary containing the classification id, the label, the first time seen and how many individuals were seen.
     """
 
     nothing_values = [
         "NOANIMALSPRESENT",
         "ICANTRECOGNISEANYTHING",
         "ISEENOTHING",
         "NOTHINGHERE",
@@ -286,110 +327,24 @@
         - fpath
         - sampling_start
         - sampling_end
     """
     # Standarise the filename
     movies_df["filename"] = movies_df["filename"].str.normalize("NFD")
 
-    # Unswedify the filename
-    movies_df["filename"] = movies_df["filename"].apply(lambda x: unswedify(x))
+    # Ensure the filename has standard characters
+    movies_df["filename"] = movies_df["filename"].apply(lambda x: fix_text_encoding(x))
 
     # TO DO Include server's path to the movie files
-    movies_df["fpath"] = movies_df["filename"]
+    movies_df["fpath"] = (
+        movies_df["filename"].replace(".MP4", ".mp4").replace(".mov", ".mp4")
+    )
 
     # Rename relevant fields
     movies_df = movies_df.rename(
         columns={
             "SamplingStart": "sampling_start",
             "SamplingEnd": "sampling_end",
         }
     )
 
     return movies_df
-
-
-def bb_iou(boxA, boxB):
-    """
-    The function takes two bounding boxes, computes the area of intersection, and divides it by the area
-    of the union of the two boxes
-
-    :param boxA: The first bounding box
-    :param boxB: The ground truth box
-    :return: The IOU value
-    """
-
-    # Compute edges
-    temp_boxA = boxA.copy()
-    temp_boxB = boxB.copy()
-    temp_boxA[2], temp_boxA[3] = (
-        temp_boxA[0] + temp_boxA[2],
-        temp_boxA[1] + temp_boxA[3],
-    )
-    temp_boxB[2], temp_boxB[3] = (
-        temp_boxB[0] + temp_boxB[2],
-        temp_boxB[1] + temp_boxB[3],
-    )
-
-    # determine the (x, y)-coordinates of the intersection rectangle
-    xA = max(temp_boxA[0], temp_boxB[0])
-    yA = max(temp_boxA[1], temp_boxB[1])
-    xB = min(temp_boxA[2], temp_boxB[2])
-    yB = min(temp_boxA[3], temp_boxB[3])
-
-    # compute the area of intersection rectangle
-    interArea = abs(max((xB - xA, 0)) * max((yB - yA), 0))
-    if interArea == 0:
-        return 1
-    # compute the area of both the prediction and ground-truth
-    # rectangles
-    boxAArea = abs((temp_boxA[2] - temp_boxA[0]) * (temp_boxA[3] - temp_boxA[1]))
-    boxBArea = abs((temp_boxB[2] - temp_boxB[0]) * (temp_boxB[3] - temp_boxB[1]))
-
-    # compute the intersection over union by taking the intersection
-    # area and dividing it by the sum of prediction + ground-truth
-    # areas - the intersection area
-    iou = interArea / float(boxAArea + boxBArea - interArea)
-
-    # return the intersection over union value
-    return 1 - iou
-
-
-def filter_bboxes(
-    total_users: int, users: list, bboxes: list, obj: float, eps: float, iua: float
-):
-    """
-    If at least half of the users who saw this frame decided that there was an object, then we cluster
-    the bounding boxes based on the IoU criterion. If at least 80% of users agree on the annotation,
-    then we accept the cluster assignment
-
-    :param total_users: total number of users who saw this frame
-    :param users: list of user ids
-    :param bboxes: list of bounding boxes
-    :param obj: the minimum fraction of users who must have seen an object in order for it to be
-    considered
-    :param eps: The maximum distance between two samples for them to be considered as in the same
-    neighborhood
-    :param iua: the minimum percentage of users who must agree on a bounding box for it to be accepted
-    """
-
-    # If at least half of those who saw this frame decided that there was an object
-    user_count = pd.Series(users).nunique()
-    if user_count / total_users >= obj:
-        # Get clusters of annotation boxes based on iou criterion
-        cluster_ids = DBSCAN(min_samples=1, metric=bb_iou, eps=eps).fit_predict(bboxes)
-        # Count the number of users within each cluster
-        counter_dict = Counter(cluster_ids)
-        # Accept a cluster assignment if at least 80% of users agree on annotation
-        passing_ids = [k for k, v in counter_dict.items() if v / user_count >= iua]
-
-        indices = np.isin(cluster_ids, passing_ids)
-
-        final_boxes = []
-        for i in passing_ids:
-            # Compute median over all accepted bounding boxes
-            boxes = np.median(np.array(bboxes)[np.where(cluster_ids == i)], axis=0)
-            final_boxes.append(boxes)
-
-        return indices, final_boxes
-
-    else:
-        return [], bboxes
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `kso_utils-0.1.0/kso_utils/movie_utils.py` & `kso_utils-0.2.0/kso_utils/server_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,510 +1,480 @@
 # base imports
 import os
-import cv2
+import getpass
+import gdown
+import zipfile
+import boto3
 import logging
-import subprocess
-import urllib
-import pandas as pd
-import numpy as np
+from tqdm import tqdm
 from pathlib import Path
-from urllib.request import pathname2url
 
 # util imports
-from kso_utils.server_utils import (
-    upload_movie_server,
-    get_snic_files,
-    get_matching_s3_keys,
-)
 from kso_utils.project_utils import Project
-from kso_utils.tutorials_utils import is_url
-from kso_utils.db_utils import create_connection
 
 # Logging
 logging.basicConfig()
 logging.getLogger().setLevel(logging.INFO)
 
-# Function to prevent issues with Swedish characters
-# Converting the Swedish characters ä and ö to utf-8.
-def unswedify(string: str):
-    """Convert ä and ö to utf-8"""
-    return (
-        string.encode("utf-8")
-        .replace(b"\xc3\xa4", b"a\xcc\x88")
-        .replace(b"\xc3\xb6", b"o\xcc\x88")
-        .decode("utf-8")
-    )
 
+######################################
+# ###### Supported servers ###########
+# #####################################
+# Specify the names of the KSO supported servers
+class ServerType:
+    TEMPLATE = "TEMPLATE"
+    LOCAL = "LOCAL"
+    SNIC = "SNIC"
+    AWS = "AWS"
+
+
+# Store a list of ServerType values
+server_types = [
+    getattr(ServerType, attr)
+    for attr in dir(ServerType)
+    if not callable(getattr(ServerType, attr)) and not attr.startswith("__")
+]
+
+######################################
+# ###### Common server functions ######
+# #####################################
 
-# Function to prevent issues with Swedish characters
-def reswedify(string: str):
-    """Convert ä and ö to utf-8"""
-    return (
-        string.encode("utf-8")
-        .replace(b"a\xcc\x88", b"\xc3\xa4")
-        .replace(b"o\xcc\x88", b"\xc3\xb6")
-        .decode("utf-8")
-    )
 
+def connect_to_server(project: Project):
+    """
+    > This function connects to the server specified in the project object and returns a dictionary with
+    the client and sftp client
 
-def get_fps_duration(movie_path: str):
-    '''
-    This function takes the path (or url) of a movie and returns its fps and duration information
-
-    :param movie_path: a string containing the path (or url) where the movie of interest can be access from
-    :return: Two integers, the fps and duration of the movie
-    """
-    '''
-    cap = cv2.VideoCapture(movie_path)
-    fps = cap.get(cv2.CAP_PROP_FPS)
-    frame_count = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
+    :param project: the project object
+    :return: A dictionary with the client and sftp_client
+    """
+    # Get project-specific server info
+    if project is None or not hasattr(project, "server"):
+        logging.error("No server information found, edit projects_list.csv")
+        return {}
+
+    # Create an empty dictionary to host the server connections
+    server_connection = {}
+
+    if project.server == ServerType.TEMPLATE:
+        # Set client as Wildlife.ai
+        server_connection["client"] = "Wildlife.ai"
+
+    elif project.server in [ServerType.LOCAL, ServerType.SNIC]:
+        logging.info("Running locally, no external connection to server needed.")
+
+    elif project.server == ServerType.AWS:
+        # Connect to AWS as a client
+        server_connection["client"] = get_aws_client()
 
-    # Roadblock to prevent issues with missing movies
-    if int(frame_count) | int(fps) == 0:
+    else:
         raise ValueError(
-            f"{movie_path} doesn't have any frames, check the path/link is correct."
+            f"Unsupported server type: {project.server}. Supported servers are {server_types}."
         )
-    else:
-        duration = frame_count / fps
 
-    return fps, duration
+    return server_connection
 
 
-def get_movie_path(f_path: str, db_info_dict: dict, project: Project):
+def download_init_csv(project: Project, init_keys: list, server_connection: dict):
     """
-    Function to get the path (or url) of a movie
+    > This function connects to the server of the project and downloads the csv files of interest
 
-    :param f_path: string with the original path of a movie
-    :param db_info_dict: a dictionary with the initial information of the project
     :param project: the project object
-    :return: a string containing the path (or url) where the movie of interest can be access from
-
-    """
-    # Get the project-specific server
-    server = project.server
-
-    if server == "AWS":
-        # Extract the key from the orignal path of the movie
-        movie_key = urllib.parse.unquote(f_path).split("/", 3)[3]
+    :param init_keys: list of potential names of the csv files
+    :param server_connection: A dictionary with the client and sftp_client
+    :return: A dictionary with the server paths of the csv files
+    """
+
+    # Create empty dictionary to save the server paths of the csv files
+    db_initial_info = {}
+
+    if project.server == ServerType.TEMPLATE:
+        gdrive_id = "1PZGRoSY_UpyLfMhRphMUMwDXw4yx1_Fn"
+        download_gdrive(
+            gdrive_id=gdrive_id, folder_name=project.csv_folder, fix_encoding=False
+        )
+
+    elif project.server in [ServerType.LOCAL, ServerType.SNIC]:
+        logging.info("Running locally so no csv files were downloaded from the server.")
+
+    elif project.server == ServerType.AWS:
+        # Retrieve a list with all the csv files in the folder with initival csvs
+        server_csv_files = get_matching_s3_keys(
+            client=server_connection["client"],
+            bucket=project.bucket,
+            suffix="csv",
+        )
+
+        # Select only csv files that are relevant to start the db
+        server_csvs_db = [
+            s
+            for s in server_csv_files
+            if any(server_csv_files in s for server_csv_files in init_keys)
+        ]
+
+        # Download each csv file locally and store the path of the server csv
+        for server_csv in server_csvs_db:
+            # Specify the key of the csv
+            init_key = [key for key in init_keys if key in server_csv][0]
+
+            # Save the server path of the csv in a dict
+            db_initial_info[str("server_" + init_key + "_csv")] = server_csv
+
+            # Specify the local path for the csv
+            local_i_csv = Path(project.csv_folder, Path(server_csv).name)
+
+            # Download the csv
+            download_object_from_s3(
+                client=server_connection["client"],
+                bucket=project.bucket,
+                key=server_csv,
+                filename=str(local_i_csv),
+            )
 
-        # Generate presigned url
-        movie_url = db_info_dict["client"].generate_presigned_url(
-            "get_object",
-            Params={"Bucket": db_info_dict["bucket"], "Key": movie_key},
-            ExpiresIn=86400,
+    else:
+        raise ValueError(
+            f"Unsupported server type: {project.server}. Supported servers are {server_types}."
         )
-        return movie_url
 
-    elif server == "SNIC":
-        logging.error("Getting the path of the movies is still work in progress")
-        return f_path
+    return db_initial_info
 
-    else:
-        return f_path
 
+def get_ml_data(project: Project, test: bool = False):
+    """
+    It downloads the training data from Google Drive.
+    Currently only applies to the Template Project as other projects do not have prepared
+    training data.
 
-def get_movie_extensions():
-    # Specify the formats of the movies to select
-    return tuple(["wmv", "mpg", "mov", "avi", "mp4", "MOV", "MP4"])
+    :param project: The project object that contains all the information about the project
+    :type project: Project
+    """
+    if project.ml_folder is not None:
+        # Download the folder containing the training data
+        if project.server == ServerType.TEMPLATE:
+            gdrive_id = "1xknKGcMnHJXu8wFZTAwiKuR3xCATKco9"
+            ml_folder = project.ml_folder
 
+            # Download template training files from Gdrive
+            if test:
+                download_gdrive(gdrive_id, Path("../test/test_output") / ml_folder)
+            else:
+                download_gdrive(gdrive_id, Path(ml_folder))
+            logging.info("Template data downloaded successfully")
+        else:
+            logging.info("No download method implemented for this data")
+    else:
+        logging.info("No prepared data to be downloaded.")
 
-def standarise_movie_format(
-    movie_path: str,
-    movie_filename: str,
-    f_path: str,
-    db_info_dict: dict,
+
+def update_csv_server(
     project: Project,
-    gpu_available: bool = False,
+    csv_paths: dict,
+    server_connection: dict,
+    orig_csv: str,
+    updated_csv: str,
 ):
     """
-    This function reviews the movie metadata. If the movie is not in the correct format, frame rate or codec,
-    it is converted using ffmpeg.
+    > This function updates the original csv file with the updated csv file in the server
 
-    :param movie_path: The local path- or url to the movie file you want to convert
-    :type movie_path: str
-    :param movie_filename: The filename of the movie file you want to convert
-    :type movie_filename: str
-    :param f_path: The server or storage path of the original movie you want to convert
-    :type f_path: str
-    :param db_info_dict: a dictionary with the initial information of the project
     :param project: the project object
-    :param gpu_available: Boolean, whether or not a GPU is available
-    :type gpu_available: bool
-    """
-
-    ##### Check movie format ######
-    ext = Path(movie_filename).suffix
+    :param csv_paths: a dictionary with the paths of the csv files with info to initiate the db
+    :param server_connection: a dictionary with the connection to the server
+    :param orig_csv: the original csv file name
+    :type orig_csv: str
+    :param updated_csv: the updated csv file
+    :type updated_csv: str
+    """
+    if project.server == ServerType.TEMPLATE:
+        logging.error(
+            f"The server {orig_csv} can't be updated for template project without admin permissions."
+        )
+
+    elif project.server in [ServerType.LOCAL, ServerType.SNIC]:
+        logging.error(
+            "The project doesn't have csv files in the server so only the local csv files have been updated"
+        )
+
+    elif project.server == ServerType.AWS:
+        logging.info("Updating csv file in AWS server")
+        # Update csv to AWS
+        upload_file_to_s3(
+            client=server_connection["client"],
+            bucket=project.bucket,
+            key=str(csv_paths[orig_csv]),
+            filename=str(csv_paths[updated_csv]),
+        )
+        logging.info(f"{orig_csv} updated to the {ServerType.AWS} server.")
 
-    if not ext.lower() == "mp4":
-        logging.info(f"Extension of {movie_filename} not supported.")
-        # Set conversion to True
-        convert_video_T_F = True
-
-    ##### Check frame rate #######
-    cap = cv2.VideoCapture(movie_path)
-    fps = cap.get(cv2.CAP_PROP_FPS)
-
-    if not float(fps).is_integer():
-        logging.info(f"Variable frame rate of {movie_filename} not supported.")
-        # Set conversion to True
-        convert_video_T_F = True
-
-    ##### Check codec info ########
-    h = int(cap.get(cv2.CAP_PROP_FOURCC))
-    codec = (
-        chr(h & 0xFF)
-        + chr((h >> 8) & 0xFF)
-        + chr((h >> 16) & 0xFF)
-        + chr((h >> 24) & 0xFF)
-    )
+    else:
+        raise ValueError(
+            f"Unsupported server type: {project.server}. Supported servers are {server_types}."
+        )
 
-    if not codec == "h264":
-        logging.info(
-            f"The codecs of {movie_filename} are not supported (only h264 is supported)."
-        )
-        # Set conversion to True
-        convert_video_T_F = True
-
-    ##### Check movie file #######
-    ##### (not needed in Spyfish) #####
-    # Create a list of the project where movie compression is not needed
-    project_no_compress = ["Spyfish_Aotearoa"]
-
-    if project.Project_name in project_no_compress:
-        # Set movie compression to false
-        compress_video = False
 
-    else:
-        # Check movie filesize in relation to its duration
-        frame_count = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
-        duration = frame_count / fps
-        duration_mins = duration / 60
-
-        # Check if the movie is accessible locally
-        if os.path.exists(movie_path):
-            # Store the size of the movie
-            size = os.path.getsize(movie_path)
-
-        # Check if the path to the movie is a url
-        elif is_url(movie_path):
-            # Store the size of the movie
-            size = urllib.request.urlopen(movie_path).length
+def upload_file_server(
+    project: Project, server_connection: dict, conv_mov_path: str, f_path: str
+):
+    """
+    Takes the file path of a file and uploads/saves it to the server.
 
-        else:
-            logging.error(f"The path to {movie_path} is invalid")
+    :param project: the project object
+    :param conv_mov_path: The local path to the converted movie file you want to upload
+    :type conv_mov_path: str
+    :param f_path: The server or storage path of the movie you want to upload to
+    :type f_path: str
 
-        # Calculate the size:duration ratio
-        sizeGB = size / (1024 * 1024 * 1024)
-        size_duration = sizeGB / duration_mins
-
-        if size_duration > 0.16:
-            # Compress the movie if file size is too large
-            logging.info(
-                "File size of movie is too large (+5GB per 30 mins of footage)."
-            )
+    """
+    if project.server == ServerType.TEMPLATE:
+        logging.error(
+            f"{conv_mov_path} not uploaded to the server as project is template"
+        )
 
-            # Specify to compress the video
-            compress_video = True
-        else:
-            # Set movie compression to false
-            compress_video = False
+    elif project.server in [ServerType.LOCAL, ServerType.SNIC]:
+        logging.error(f"{conv_mov_path} not uploaded to the server as project is local")
 
-    # Start converting/compressing video if movie didn't pass any of the checks
-    if convert_video_T_F or compress_video:
-        conv_mov_path = convert_video(
-            movie_path, movie_filename, gpu_available, compress_video
+    elif project.server == ServerType.AWS:
+        # Update csv to AWS
+        upload_file_to_s3(
+            client=server_connection["client"],
+            bucket=project.bucket,
+            key=f_path,
+            filename=conv_mov_path,
         )
 
-        # Upload the converted movie to the server
-        upload_movie_server(conv_mov_path, f_path, db_info_dict, project)
+        logging.info(f"{f_path} standarised and uploaded to the server.")
 
     else:
-        logging.info(f"{movie_filename} format is standard.")
+        raise ValueError(
+            f"Unsupported server type: {project.server}. Supported servers are {server_types}."
+        )
 
 
-def retrieve_movie_info_from_server(project: Project, db_info_dict: dict):
-    """
-    This function uses the project information and the database information, and returns a dataframe with the
-    movie information
+#####################
+# ## AWS functions ###
+# ####################
 
-    :param project: the project object
-    :param db_info_dict: a dictionary containing the path to the database and the client to the server
-    :type db_info_dict: dict
-    :return: A dataframe with the following columns:
-    - index
-    - movie_id
-    - fpath
-    - spath
-    - exists
-    - filename_ext
-    """
-
-    server = project.server
-    bucket_i = project.bucket
-    movie_folder = project.movie_folder
-
-    if server == "AWS":
-        logging.info("Retrieving movies from AWS server")
-        # Retrieve info from the bucket
-        server_df = get_matching_s3_keys(
-            client=db_info_dict["client"],
-            bucket=bucket_i,
-            suffix=get_movie_extensions(),
-        )
-        # Get the fpath(html) from the key
-        server_df["spath"] = server_df["Key"].apply(
-            lambda x: "http://marine-buv.s3.ap-southeast-2.amazonaws.com/"
-            + urllib.parse.quote(x, safe="://").replace("\\", "/")
-        )
-
-    elif server == "SNIC":
-        if "client" in db_info_dict:
-            server_df = get_snic_files(
-                client=db_info_dict["client"], folder=movie_folder
-            )
-        else:
-            logging.error("No database connection could be established.")
-            return pd.DataFrame(columns=["filename"])
-
-    elif server == "LOCAL":
-        if [movie_folder, bucket_i] == ["None", "None"]:
-            logging.info(
-                "No movies to be linked. If you do not have any movie files, please use Tutorial 4 instead."
-            )
-            return pd.DataFrame(columns=["filename"])
-        else:
-            server_files = os.listdir(movie_folder)
-            server_df = pd.Series(server_files, name="spath").to_frame()
-    elif server == "TEMPLATE":
-        # Combine wildlife.ai storage and filenames of the movie examples
-        server_df = pd.read_csv(db_info_dict["local_movies_csv"])[["filename"]]
 
-        # Get the fpath(html) from the key
-        server_df = server_df.rename(columns={"filename": "fpath"})
+def aws_credentials():
+    # Save your access key for the s3 bucket.
+    aws_access_key_id = getpass.getpass("Enter the key id for the aws server")
+    aws_secret_access_key = getpass.getpass(
+        "Enter the secret access key for the aws server"
+    )
 
-        server_df["spath"] = server_df["fpath"].apply(
-            lambda x: "https://www.wildlife.ai/wp-content/uploads/2022/06/" + str(x), 1
-        )
+    return aws_access_key_id, aws_secret_access_key
 
-        # Remove fpath values
-        server_df.drop(columns=["fpath"], axis=1, inplace=True)
 
-    else:
-        raise ValueError("The server type you selected is not currently supported.")
+def connect_s3(aws_access_key_id: str, aws_secret_access_key: str):
+    # Connect to the s3 bucket
+    client = boto3.client(
+        "s3",
+        aws_access_key_id=aws_access_key_id,
+        aws_secret_access_key=aws_secret_access_key,
+    )
+    return client
 
-    # Create connection to db
-    conn = create_connection(db_info_dict["db_path"])
 
-    # Query info about the movie of interest
-    movies_df = pd.read_sql_query("SELECT * FROM movies", conn)
-    movies_df = movies_df.rename(columns={"id": "movie_id"})
-
-    # Find closest matching filename (may differ due to Swedish character encoding)
-    movies_df["fpath"] = movies_df["fpath"].apply(
-        lambda x: urllib.parse.quote(reswedify(x).replace("\\", "/"), safe="://")
-        if urllib.parse.quote(reswedify(x).replace("\\", "/"), safe="://")
-        in server_df["spath"].unique()
-        else unswedify(x)
+def get_aws_client():
+    # Set aws account credentials
+    aws_access_key_id, aws_secret_access_key = os.getenv("SPY_KEY"), os.getenv(
+        "SPY_SECRET"
     )
+    if aws_access_key_id is None or aws_secret_access_key is None:
+        aws_access_key_id, aws_secret_access_key = aws_credentials()
 
-    # Merge the server path to the filepath
-    movies_df = movies_df.merge(
-        server_df,
-        left_on=["fpath"],
-        right_on=["spath"],
-        how="left",
-        indicator=True,
-    )
+    # Connect to S3
+    client = connect_s3(aws_access_key_id, aws_secret_access_key)
 
-    # Check that movies can be mapped
-    movies_df["exists"] = np.where(movies_df["_merge"] == "left_only", False, True)
+    return client
 
-    # Drop _merge columns to match sql schema
-    movies_df = movies_df.drop("_merge", axis=1)
 
-    # Select only those that can be mapped
-    available_movies_df = movies_df[movies_df["exists"]].copy()
+def get_matching_s3_objects(
+    client: boto3.client, bucket: str, prefix: str = "", suffix: str = ""
+):
+    """
+    ## Code modified from alexwlchan (https://alexwlchan.net/2019/07/listing-s3-keys/)
+    Generate objects in an S3 bucket.
 
-    # Create a filename with ext column
-    available_movies_df["filename_ext"] = available_movies_df["spath"].apply(
-        lambda x: x.split("/")[-1], 1
-    )
+    :param client: S3 client.
+    :param bucket: Name of the S3 bucket.
+    :param prefix: Only fetch objects whose key starts with
+        this prefix (optional).
+    :param suffix: Only fetch objects whose keys end with
+        this suffix (optional).
+    """
 
-    # Add movie folder for SNIC
-    if server == "SNIC":
-        available_movies_df["spath"] = movie_folder + available_movies_df["spath"]
+    paginator = client.get_paginator("list_objects_v2")
 
-    logging.info(
-        f"{available_movies_df.shape[0]} out of {len(movies_df)} movies are mapped from the server"
-    )
+    kwargs = {"Bucket": bucket}
 
-    return available_movies_df
+    # We can pass the prefix directly to the S3 API.  If the user has passed
+    # a tuple or list of prefixes, we go through them one by one.
+    if isinstance(prefix, str):
+        prefixes = (prefix,)
+    else:
+        prefixes = prefix
 
+    for key_prefix in prefixes:
+        kwargs["Prefix"] = key_prefix
 
-def convert_video(
-    movie_path: str,
-    movie_filename: str,
-    gpu_available: bool = False,
-    compression: bool = False,
+        for page in paginator.paginate(**kwargs):
+            try:
+                contents = page["Contents"]
+            except KeyError:
+                break
+
+            for obj in contents:
+                key = obj["Key"]
+                if key.endswith(suffix):
+                    yield obj
+
+
+def get_matching_s3_keys(
+    client: boto3.client, bucket: str, prefix: str = "", suffix: str = ""
 ):
     """
-    It takes a movie file path and a boolean indicating whether a GPU is available, and returns a new
-    movie file path.
+    ## Code from alexwlchan (https://alexwlchan.net/2019/07/listing-s3-keys/)
+    Generate the keys in an S3 bucket.
 
-    :param movie_path: The local path- or url to the movie file you want to convert
-    :type movie_path: str
-    :param movie_filename: The filename of the movie file you want to convert
-    :type movie_path: str
-    :param gpu_available: Boolean, whether or not a GPU is available
-    :type gpu_available: bool
-    :param compression: Boolean, whether or not movie compression is required
-    :type compression: bool
-    :return: The path to the converted video file.
-    """
-    movie_filename = Path(movie_path).name
-    conv_filename = "conv_" + movie_filename
-
-    # Check the movie is accessible locally
-    if os.path.exists(movie_path):
-        # Store the directory and filename of the movie
-        movie_fpath = os.path.dirname(movie_path)
-        conv_fpath = os.path.join(movie_fpath, conv_filename)
-
-    # Check if the path to the movie is a url
-    elif is_url(movie_path):
-        # Specify the directory to store the converted movie
-        conv_fpath = os.path.join(conv_filename)
+    :param client: S3 client.
+    :param bucket: Name of the S3 bucket.
+    :param prefix: Only fetch keys that start with this prefix (optional).
+    :param suffix: Only fetch keys that end with this suffix (optional).
+    return a list of the matching objects
+    """
+
+    # Select the relevant bucket
+    s3_keys = [
+        obj["Key"] for obj in get_matching_s3_objects(client, bucket, prefix, suffix)
+    ]
+
+    return s3_keys
+
+
+def download_object_from_s3(
+    client: boto3.client,
+    *,
+    bucket: str,
+    key: str,
+    version_id: str = None,
+    filename: str,
+):
+    """
+    Download an object from S3 with a progress bar.
 
+    From https://alexwlchan.net/2021/04/s3-progress-bars/
+    """
+
+    # First get the size, so we know what tqdm is counting up to.
+    # Theoretically the size could change between this HeadObject and starting
+    # to download the file, but this would only affect the progress bar.
+    kwargs = {"Bucket": bucket, "Key": key}
+
+    if version_id is not None:
+        kwargs["VersionId"] = version_id
+
+    object_size = client.head_object(**kwargs)["ContentLength"]
+
+    if version_id is not None:
+        ExtraArgs = {"VersionId": version_id}
     else:
-        logging.error("The path to", movie_path, " is invalid")
+        ExtraArgs = None
 
-    if gpu_available and compression:
-        subprocess.call(
-            [
-                "ffmpeg",
-                "-hwaccel",
-                "cuda",
-                "-hwaccel_output_format",
-                "cuda",
-                "-i",
-                str(movie_path),
-                "-c:v",
-                "h264_nvenc",  # ensures correct codec
-                "-crf",
-                "22",  # compresses the video
-                str(conv_fpath),
-            ]
-        )
-
-    elif gpu_available and not compression:
-        subprocess.call(
-            [
-                "ffmpeg",
-                "-hwaccel",
-                "cuda",
-                "-hwaccel_output_format",
-                "cuda",
-                "-i",
-                str(movie_path),
-                "-c:v",
-                "h264_nvenc",  # ensures correct codec
-                str(conv_fpath),
-            ]
-        )
-
-    elif not gpu_available and compression:
-        subprocess.call(
-            [
-                "ffmpeg",
-                "-i",
-                str(movie_path),
-                "-c:v",
-                "h264",  # ensures correct codec
-                "-crf",
-                "22",  # compresses the video
-                str(conv_fpath),
-            ]
-        )
-
-    elif not gpu_available and not compression:
-        subprocess.call(
-            [
-                "ffmpeg",
-                "-i",
-                str(movie_path),
-                "-c:v",
-                "h264",  # ensures correct codec
-                str(conv_fpath),
-            ]
+    with tqdm(
+        total=object_size,
+        unit="B",
+        unit_scale=True,
+        desc=filename,
+        position=0,
+        leave=True,
+    ) as pbar:
+        client.download_file(
+            Bucket=bucket,
+            Key=key,
+            ExtraArgs=ExtraArgs,
+            Filename=filename,
+            Config=boto3.s3.transfer.TransferConfig(use_threads=False),
+            Callback=lambda bytes_transferred: pbar.update(bytes_transferred),
         )
+
+
+def upload_file_to_s3(client: boto3.client, *, bucket: str, key: str, filename: str):
+    """
+    > Upload a file to S3, and show a progress bar if the file is large enough
+
+    :param client: The boto3 client to use
+    :param bucket: The name of the bucket to upload to
+    :param key: The name of the file in S3
+    :param filename: The name of the file to upload
+    """
+
+    # Get the size of the file to upload
+    file_size = os.stat(filename).st_size
+
+    # Prevent issues with small files (<1MB) and tqdm
+    if file_size > 1000000:
+        with tqdm(
+            total=file_size,
+            unit="B",
+            unit_scale=True,
+            desc=filename,
+            position=0,
+            leave=True,
+        ) as pbar:
+            client.upload_file(
+                Filename=filename,
+                Bucket=bucket,
+                Key=key,
+                Config=boto3.s3.transfer.TransferConfig(use_threads=False),
+                Callback=lambda bytes_transferred: pbar.update(bytes_transferred),
+            )
     else:
-        raise ValueError(f"{movie_path} not modified")
+        client.upload_file(
+            Filename=filename,
+            Bucket=bucket,
+            Key=key,
+        )
 
-    # Ensure open permissions on file (for now)
-    os.chmod(conv_fpath, 0o777)
-    logging.info("Movie file successfully converted and stored locally.")
-    return conv_fpath
 
+def delete_file_from_s3(client: boto3.client, *, bucket: str, key: str):
+    """
+    > Delete a file from S3.
 
-# Function to preview underwater movies
-def preview_movie(
-    project: Project,
-    db_info_dict: dict,
-    available_movies_df: pd.DataFrame,
-    movie_i: str,
-):
+    :param client: boto3.client - the client object that you created in the previous step
+    :type client: boto3.client
+    :param bucket: The name of the bucket that contains the object to delete
+    :type bucket: str
+    :param key: The name of the file
+    :type key: str
     """
-    It takes a movie filename and returns a HTML object that can be displayed in the notebook
+    client.delete_object(Bucket=bucket, Key=key)
 
-    :param project: the project object
-    :param db_info_dict: a dictionary containing the database information
-    :param available_movies_df: a dataframe with all the movies in the database
-    :param movie_i: the filename of the movie you want to preview
-    :return: A tuple of two elements:
-        1. HTML object
-        2. Movie path
-    """
-
-    # Select the movie of interest
-    movie_selected = available_movies_df[
-        available_movies_df["filename"] == movie_i
-    ].reset_index(drop=True)
-    movie_selected_view = movie_selected.T
-    movie_selected_view.columns = ["Movie summary"]
-
-    # Make sure only one movie is selected
-    if len(movie_selected.index) > 1:
-        logging.info(
-            "There are several movies with the same filename. This should be fixed!"
-        )
-        return None
 
-    else:
-        # Generate temporary path to the movie select
-        if project.server == "SNIC":
-            movie_path = get_movie_path(
-                project=project,
-                db_info_dict=db_info_dict,
-                f_path=movie_selected["spath"].values[0],
-            )
-            url = (
-                "https://portal.c3se.chalmers.se/pun/sys/dashboard/files/fs/"
-                + pathname2url(movie_path)
-            )
-        else:
-            url = get_movie_path(
-                f_path=movie_selected["fpath"].values[0],
-                db_info_dict=db_info_dict,
-                project=project,
-            )
-            movie_path = url
-        html_code = f"""<html>
-                <div style="display: flex; justify-content: space-around; align-items: center">
-                <div>
-                  <video width=500 controls>
-                  <source src={url}>
-                  </video>
-                </div>
-                <div>{movie_selected_view.to_html()}</div>
-                </div>
-                </html>"""
-        return HTML(html_code), movie_path
+#####################
+# ## Google Drive functions ###
+# ####################
+
+
+def download_gdrive(gdrive_id: str, folder_name: str, fix_encoding: bool = True):
+    # Specify the url of the file to download
+    url_input = f"https://drive.google.com/uc?&confirm=s5vl&id={gdrive_id}"
+
+    logging.info(f"Retrieving the file from {url_input}")
+
+    # Specify the output of the file
+    zip_file = f"{folder_name}.zip"
+
+    # Download the zip file
+    gdown.download(url_input, zip_file, quiet=False)
+
+    # Unzip the folder with the files
+    with zipfile.ZipFile(zip_file, "r") as zip_ref:
+        zip_ref.extractall(Path(folder_name).parent)
+
+    # Remove the zipped file
+    Path(zip_file).unlink()
+
+    if fix_encoding:
+        from kso_utils.koster_utils import fix_text_encoding_folder
+
+        # Correct the file names by using correct encoding
+        fix_text_encoding_folder(folder_name)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `kso_utils-0.1.0/kso_utils/project_utils.py` & `kso_utils-0.2.0/kso_utils/project_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,79 +1,96 @@
 # base imports
 import os
+from pathlib import Path
 import logging
 import pandas as pd
 from dataclasses import dataclass
-from dataclass_csv import DataclassReader, DataclassWriter, exceptions
+from dataclass_csv import DataclassReader, exceptions
 
 # Logging
 logging.basicConfig()
 logging.getLogger().setLevel(logging.DEBUG)
 
+
 @dataclass
 class Project:
+    # This is defining a data class called `Project` with several attributes including `Project_name`,
+    # `Zooniverse_number`, `db_path`, `server`, `bucket`, `key`, `csv_folder`, `movie_folder`,
+    # `photo_folder`, and `ml_folder`. The `@dataclass` decorator is used to automatically generate
+    # several special methods such as `__init__`, `__repr__`, and `__eq__` for the class. This makes it
+    # easier to create and work with instances of the `Project` class.
     Project_name: str
     Zooniverse_number: int = 0
     db_path: str = None
     server: str = None
     bucket: str = None
     key: str = None
     csv_folder: str = None
     movie_folder: str = None
     photo_folder: str = None
     ml_folder: str = None
 
 
-def find_project(project_name: str = ""):
+def find_project(
+    project_name: str = "", project_csv: str = "db_starter/projects_list.csv"
+):
     """Find project information using
     project csv path and project name"""
     # Specify the path to the list of projects
-    tut_path = os.getcwd()
-    abspath = os.path.abspath(__file__)
-    dname = os.path.dirname(abspath)
+    tut_path = Path.cwd()
+    abspath = Path(__file__).resolve()
+    dname = abspath.parent
     os.chdir(dname)
-    project_path = "db_starter/projects_list.csv"
+
+    # Switch to cdn project list (temporary fix)
+    if Path("/buckets").exists():
+        project_csv = "db_starter/cdn_projects_list.csv"
 
     # Check path to the list of projects is a csv
-    if os.path.exists(project_path) and not project_path.endswith(".csv"):
+    if Path(project_csv).exists() and not project_csv.endswith(".csv"):
         logging.error("A csv file was not selected. Please try again.")
 
     # If list of projects doesn't exist retrieve it from github
-    elif not os.path.exists(project_path):
-        github_path = "https://github.com/ocean-data-factory-sweden/kso_utils/blob/main/kso_utils/db_starter/projects_list.csv?raw=true"
+    elif not Path(project_csv).exists():
+        if Path("/buckets").exists():
+            github_path = "https://github.com/ocean-data-factory-sweden/kso_utils/blob/main/kso_utils/db_starter/cdn_projects_list.csv?raw=true"
+        else:
+            github_path = "https://github.com/ocean-data-factory-sweden/kso_utils/blob/main/kso_utils/db_starter/projects_list.csv?raw=true"
         read_file = pd.read_csv(github_path)
-        read_file.to_csv(project_path, index=None)
+        read_file.to_csv(project_csv, index=None)
 
-    with open(project_path) as csv:
+    with open(project_csv) as csv:
         reader = DataclassReader(csv, Project)
         try:
             for row in reader:
                 if row.Project_name == project_name:
                     logging.info(f"{project_name} loaded succesfully")
+                    os.chdir(tut_path)
                     return row
         except exceptions.CsvValueError:
             logging.error(
                 f"This project {project_name} does not contain any csv information. Please select another."
             )
     os.chdir(tut_path)
+    return
 
 
-def add_project(project_info: dict = {}):
-    """Add new project information to
-    project csv using a project_info dictionary
-    """
-    tut_path = os.getcwd()
-    abspath = os.path.abspath(__file__)
-    dname = os.path.dirname(abspath)
-    os.chdir(dname)
-    # Specify standard project list location
-    project_path = "db_starter/projects_list.csv"
-    # Specify volume allocated by SNIC
-    snic_path = "/mimer/NOBACKUP/groups/snic2021-6-9"
-
-    if not os.path.exists(project_path) and os.path.exists(snic_path):
-        project_path = os.path.join(snic_path, "db_starter/projects_list.csv")
-    with open(project_path, "a") as f:
-        project = [Project(*list(project_info.values()))]
-        w = DataclassWriter(f, project, Project)
-        w.write(skip_header=True)
-    os.chdir(tut_path)
+# def add_project(project_info: dict = {}):
+#     """Add new project information to
+#     project csv using a project_info dictionary
+#     """
+#     tut_path = os.getcwd()
+#     abspath = os.path.abspath(__file__)
+#     dname = os.path.dirname(abspath)
+#     os.chdir(dname)
+#     # Specify standard project list location
+#     project_path = "db_starter/projects_list.csv"
+#     # Specify volume allocated by SNIC
+#     snic_path = "/mimer/NOBACKUP/groups/snic2021-6-9"
+
+#     if not os.path.exists(project_path) and os.path.exists(snic_path):
+#         project_path = os.path.join(snic_path, "db_starter/projects_list.csv")
+#     with open(project_path, "a") as f:
+#         project = [Project(*list(project_info.values()))]
+#         w = DataclassWriter(f, project, Project)
+#         w.write(skip_header=True)
+#     os.chdir(tut_path)
```

### Comparing `kso_utils-0.1.0/kso_utils/sgu_utils.py` & `kso_utils-0.2.0/kso_utils/sgu_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,26 +7,32 @@
 from tqdm import tqdm
 from pathlib import Path
 import splitfolders
 import glob
 
 tqdm.pandas()
 
+# util imports
+import kso_utils.project_utils as project_utils
+
 # Logging
 logging.basicConfig()
 logging.getLogger().setLevel(logging.INFO)
 
 
 def create_classification_dataset(
     data_path: str, out_path: str, test_size: float, seed: int = 1337
 ):
-    if not os.path.exists(out_path):
-        Path(out_path).mkdir(parents=True, exist_ok=True)
+    out_path = Path(out_path)
+    if not out_path.exists():
+        out_path.mkdir(parents=True, exist_ok=True)
         # Recursively add permissions to folders created
-        [os.chmod(root, 0o777) for root, dirs, files in os.walk(out_path)]
+        for root, dirs, files in out_path.iterdir():
+            root.chmod(0o777)
+
     splitfolders.ratio(
         data_path, output=out_path, seed=seed, ratio=(1 - test_size, 0, test_size)
     )
     logging.info(f"Training and test datasets saved at {out_path}")
 
 
 def get_patch(row, out_path: str, pixels: int = 224, label_col: str = "sub_type"):
@@ -39,24 +45,20 @@
 
     for ix, (pos_X, pos_Y) in enumerate(zip(row.pos_X, row.pos_Y)):
         # Use conversion between current XY position and actual pixel values
         coord = (pos_X / 15, pos_Y / 15)
 
         # Discard images where pos_X is negative
         if coord[0] < 0:
-            logging.error(
-                f"Negative X value in {os.path.basename(row.fpath)}. Skipping..."
-            )
+            logging.error(f"Negative X value in {Path(row.fpath).name}. Skipping...")
             return
 
         # Discard images where label is NA
         if not isinstance(row[label_col][ix], str):
-            logging.error(
-                f"Invalid label in {os.path.basename(row.fpath)}. Skipping..."
-            )
+            logging.error(f"Invalid label in {Path(row.fpath).name}. Skipping...")
             return
 
         cropped_ys, cropped_ye = int(coord[1] - pixels / 2), int(coord[1] + pixels / 2)
         cropped_xs, cropped_xe = int(coord[0] - pixels / 2), int(coord[0] + pixels / 2)
 
         if cropped_ys < 0:
             y_diff = -1 * cropped_ys
@@ -72,27 +74,24 @@
         cropped_image = img[
             cropped_ys:cropped_ye,
             cropped_xs:cropped_xe,
         ]
 
         # Get label
         label = row[label_col][ix]
-        if not os.path.exists(Path(out_path, label)):
-            Path(out_path, label).mkdir(parents=True, exist_ok=True)
-            # Recursively add permissions to folders created
-            [
-                os.chmod(root, 0o777)
-                for root, dirs, files in os.walk(str(Path(out_path, label)))
-            ]
+        label_path = Path(out_path, label)
+        label_path.mkdir(parents=True, exist_ok=True)
+
+        # Recursively add permissions to folders created
+        for root, dirs, files in label_path.iterdir():
+            root.chmod(0o777)
 
         # Write patches to a folder
-        cv2.imwrite(
-            f"{Path(out_path, label)}/{Path(row.fpath).stem}_patch_{row.point[ix]}.jpg",
-            cropped_image,
-        )
+        patch_filename = f"{Path(row.fpath).stem}_patch_{row.point[ix]}.jpg"
+        cv2.imwrite(str(label_path / patch_filename), cropped_image)
 
 
 def get_patches(
     root_path: str,
     meta_filename: str,
     pixels: int,
     out_path: str,
@@ -161,29 +160,27 @@
         [os.chmod(root, 0o777) for root, dirs, files in os.walk(out_path)]
     df.progress_apply(lambda x: get_patch(x, out_path, pixels, label_col), axis=1)
     logging.info(
         f"Patch creation completed successfully. Total patches: {len(glob.glob(out_path + '/**/*.jpg', recursive=True))}"
     )
 
 
-def process_sgu_photos_csv(db_initial_info: dict):
+def process_sgu_photos_csv(project: project_utils.Project):
     """
     It takes the local csv files with photos and surveys information and returns a dataframe with the
     photos information
 
-    :param db_initial_info: a dictionary with the following keys:
+    :param project: The project object
     :return: A dataframe with the photos information
     """
-    # Load the csv with photos and survey information
-    photos_df = pd.read_csv(db_initial_info["local_photos_csv"])
-    surveys_df = pd.read_csv(db_initial_info["local_surveys_csv"])
-
     # Add survey info to the photos information
-    photos_df = photos_df.merge(
-        surveys_df.rename(columns={"ID": "SurveyID"}), on="SurveyID", how="left"
+    photos_df = project.local_photos_csv.merge(
+        project.local_surveys_csv.rename(columns={"ID": "SurveyID"}),
+        on="SurveyID",
+        how="left",
     )
 
     # TO DO Include server's path to the photo files
     photos_df["fpath"] = photos_df["filename"]
 
     # Rename to match schema format
     photos_df = photos_df.rename(
```

### Comparing `kso_utils-0.1.0/kso_utils/t4_utils.py` & `kso_utils-0.2.0/kso_utils/movie_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,366 +1,364 @@
-# t4 utils
 # base imports
 import os
-import sqlite3
-import ffmpeg as ffmpeg_python
-import re
+import sys
+import cv2
+import logging
+import ffmpeg
+import subprocess
+import urllib
+import unicodedata
 import pandas as pd
 import numpy as np
-import shutil
-import logging
-import cv2
-
-# widget imports
+from pathlib import Path
 from tqdm import tqdm
-from IPython.display import display, clear_output
+from ultralytics.utils.downloads import is_url
+from IPython.display import display
 import ipywidgets as widgets
-from ipyfilechooser import FileChooser
-from pathlib import Path
-from datetime import date
-from panoptes_client import (
-    SubjectSet,
-    Subject,
-)
 
 # util imports
-from kso_utils.zooniverse_utils import populate_agg_annotations
-import kso_utils.db_utils as db_utils
-import kso_utils.server_utils as s_utils
-
-# import kso_utils.spyfish_utils as spyfish_utils
-import kso_utils.project_utils as project_utils
-import kso_utils.movie_utils as movie_utils
-import kso_utils.t8_utils as t8
+from kso_utils.project_utils import Project
+
+# server imports
+from kso_utils.server_utils import ServerType, get_matching_s3_keys, upload_file_server
+
 
 # Logging
 logging.basicConfig()
 logging.getLogger().setLevel(logging.INFO)
 
 
-def choose_species(db_info_dict: dict):
-    """
-    This function generates a widget to select the species of interest
+# Function to check if ffmpeg is available in the system's PATH.
+def check_ffmpeg_availability():
+    try:
+        # Try to import the ffmpeg module from ffmpeg-python
+        import ffmpeg
+
+        return True
+    except ImportError:
+        return False
 
-    :param db_info_dict: a dictionary containing the path to the database
-    :type db_info_dict: dict
+
+def get_fps_duration(movie_path: str):
     """
-    # Create connection to db
-    conn = db_utils.create_connection(db_info_dict["db_path"])
+    This function takes the path (or url) of a movie and returns its fps and duration information
 
-    # Get a list of the species available
-    species_list = pd.read_sql_query("SELECT label from species", conn)[
-        "label"
-    ].tolist()
+    :param movie_path: a string containing the path (or url) where the movie of interest can be access from
+    :return: Two integers, the fps and duration of the movie
+    """
+    cap = cv2.VideoCapture(movie_path)
+    fps = cap.get(cv2.CAP_PROP_FPS)
+    frame_count = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
 
-    # Roadblock to check if species list is empty
-    if len(species_list) == 0:
+    # Roadblock to prevent issues with missing movies
+    if int(frame_count) | int(fps) == 0:
         raise ValueError(
-            "Your database contains no species, please add at least one species before continuing."
+            f"{movie_path} doesn't have any frames, check the path/link is correct."
         )
+    else:
+        duration = frame_count / fps
 
-    # Generate the widget
-    w = widgets.SelectMultiple(
-        options=species_list,
-        value=[species_list[0]],
-        description="Species",
-        disabled=False,
-    )
-
-    display(w)
-    return w
+    return fps, duration
 
 
-# Function to choose a folder path
-def choose_folder():
-    fc = FileChooser(".")
-    display(fc)
-    return fc
-
-
-# Function to clean label (no non-alpha characters)
-def clean_label(label_string: str):
-    label_string = label_string.upper()
-    label_string = label_string.replace(" ", "")
-    pattern = r"[^A-Za-z0-9]+"
-    cleaned_string = re.sub(pattern, "", label_string)
-    return cleaned_string
-
-
-# Function to match species selected to species id
-def get_species_ids(project: project_utils.Project, species_list: list):
-    """
-    # Get ids of species of interest
-    """
-    db_path = project.db_path
-    conn = db_utils.create_connection(db_path)
-    if len(species_list) == 1:
-        species_ids = pd.read_sql_query(
-            f'SELECT id FROM species WHERE label=="{species_list[0]}"', conn
-        )["id"].tolist()
-    else:
-        species_ids = pd.read_sql_query(
-            f"SELECT id FROM species WHERE label IN {tuple(species_list)}", conn
-        )["id"].tolist()
-    return species_ids
-
-
-def get_species_frames(
-    agg_clips_df: pd.DataFrame,
-    species_ids: list,
-    server_dict: dict,
-    conn: sqlite3.Connection,
-    project: project_utils.Project,
-    n_frames_subject: int,
-):
+def get_movie_path(f_path: str, project: Project, server_connection: dict = None):
     """
-    # Function to identify up to n number of frames per classified clip
-    # that contains species of interest after the first time seen
+    Function to get the path (or url) of a movie
+
+    :param f_path: string with the original path of a movie
+    :param project: the project object
+    :param server_connection: a dictionary with the connection to the server
+    :return: a string containing the path (or url) where the movie of interest can be access from
 
-    # Find classified clips that contain the species of interest
     """
+    if project.server == ServerType.AWS:
+        # Generate presigned url
+        movie_url = server_connection["client"].generate_presigned_url(
+            "get_object",
+            Params={"Bucket": project.bucket, "Key": f_path},
+            ExpiresIn=86400,
+        )
+        return movie_url
 
-    # Retrieve list of subjects
-    subjects_df = pd.read_sql_query(
-        "SELECT id, clip_start_time, movie_id FROM subjects WHERE subject_type='clip'",
-        conn,
-    )
+    else:
+        logging.info(f"Returning the fpath {f_path}")
+        return f_path
 
-    agg_clips_df["subject_ids"] = agg_clips_df["subject_ids"].copy().astype(int)
-    subjects_df["id"] = subjects_df["id"].copy().astype(int)
 
-    # Combine the aggregated clips and subjects dataframes
-    frames_df = pd.merge(
-        agg_clips_df, subjects_df, how="left", left_on="subject_ids", right_on="id"
-    ).drop(columns=["id"])
-
-    # Identify the second of the original movie when the species first appears
-    frames_df["first_seen_movie"] = (
-        frames_df["clip_start_time"] + frames_df["first_seen"]
-    )
+def movies_in_movie_folder(project: Project, db_connection, server_connection: dict):
+    """
+    This function uses the project information and the database information, and returns
+    a dataframe of the movies in the "movie_folder".
 
-    server = project.server
+    :param project: the project object
+    :param server_connection: a dictionary with the connection to the server
+    :param db_connection: SQL connection object
+    :return: A dataframe with the following columns (index, movie_id, fpath, exists, filename_ext)
 
-    if server in ["SNIC", "TEMPLATE"]:
-        movies_df = s_utils.retrieve_movie_info_from_server(project, server_dict)
+    """
 
-        # Include movies' filepath and fps to the df
-        frames_df = frames_df.merge(movies_df, left_on="movie_id", right_on="movie_id")
-        frames_df["fpath"] = frames_df["spath"]
+    # Retrieve the list of movies available in Wildlife.ai
+    if project.server == ServerType.TEMPLATE:
+        # Combine wildlife.ai storage and filenames of the movie examples
+        available_movies_list = [
+            "https://www.wildlife.ai/wp-content/uploads/2022/06/" + filename
+            for filename in [f"movie_{i}.mp4" for i in range(1, 6)]
+        ]
 
-        if len(frames_df[~frames_df.exists]) > 0:
-            logging.error(
-                f"There are {len(frames_df) - frames_df.exists.sum()} out of {len(frames_df)} frames with a missing movie"
-            )
+        # Save the list of movies as a pd df
+        mov_folder_df = pd.Series(available_movies_list, name="fpath").to_frame()
 
-        # Select only frames from movies that can be found
-        frames_df = frames_df[frames_df.exists]
-        if len(frames_df) == 0:
-            logging.error(
-                "There are no frames for this species that meet your aggregation criteria."
-                "Please adjust your aggregation criteria / species choice and try again."
-            )
+    # Retrieve the list of local movies available
+    elif project.server in [ServerType.LOCAL, ServerType.SNIC]:
+        logging.info("Retrieving movies that are available locally")
+        # Read the movie files from the movie_path folder
+        local_files = list(Path(project.movie_folder).rglob("*"))
+        available_movies_list = [
+            str(f) for f in local_files if f.suffix.endswith(get_movie_extensions())
+        ]
+
+        # Save the list of movies as a pd df
+        mov_folder_df = pd.Series(available_movies_list, name="fpath").to_frame()
 
-        ##### Add species_id info ####
-        # Retrieve species info
-        species_df = pd.read_sql_query(
-            "SELECT id, label, scientificName FROM species",
-            conn,
+    # Retrieve the list of movies available in AWS
+    elif project.server == ServerType.AWS:
+        logging.info("Retrieving movies that are available in AWS")
+        # List all the movies available from the S3 bucket
+        available_movies_list = get_matching_s3_keys(
+            client=server_connection["client"],
+            bucket=project.bucket,
+            suffix=get_movie_extensions(),
         )
 
-        # Retrieve species info
-        species_df = species_df.rename(columns={"id": "species_id"})
+        # Save the list of movies as a pd df
+        mov_folder_df = pd.Series(available_movies_list, name="fpath").to_frame()
 
-        # Match format of species name to Zooniverse labels
-        species_df["label"] = species_df["label"].apply(clean_label)
+    else:
+        raise ValueError(f"Unsupported server type: {project.server}")
 
-        # Combine the aggregated clips and subjects dataframes
-        frames_df = pd.merge(frames_df, species_df, how="left", on="label")
+    return mov_folder_df
 
-    if server == "AWS":
-        # Include movies' filepath and fps to the df
-        # TODO: Define fpaths?
-        frames_df = frames_df.merge(f_paths, left_on="movie_id", right_on="id")
 
-        ##### Add species_id info ####
-        # Retrieve species info
-        species_df = pd.read_sql_query(
-            "SELECT id, label, scientificName FROM species",
-            conn,
-        )
+def retrieve_movie_info_from_server(
+    project: Project, db_connection, server_connection: dict
+):
+    """
+    This function uses the project information and the database information, and returns a dataframe with the
+    movie information
 
-        # Retrieve species info
-        species_df = species_df.rename(columns={"id": "species_id"})
+    :param project: the project object
+    :param server_connection: a dictionary with the connection to the server
+    :param db_connection: SQL connection object
+    :return: A dataframe with the following columns (index, movie_id, fpath, exists, filename_ext)
 
-        # Match format of species name to Zooniverse labels
-        species_df["label"] = species_df["label"].apply(clean_label)
+    """
 
-        # Combine the aggregated clips and subjects dataframes
-        frames_df = pd.merge(frames_df, species_df, how="left", on="label").drop(
-            columns=["id"]
-        )
+    # Create a dataframe of the movies in the "movie_folder"
+    mov_folder_df = movies_in_movie_folder(project, db_connection, server_connection)
+
+    from kso_utils.db_utils import get_df_from_db_table
+
+    # Temporarily retrieve the movies info from the db
+    movies_df = get_df_from_db_table(conn=db_connection, table_name="movies")
+
+    # Query info about the movie of interest
+    movies_df = movies_df.rename(columns={"id": "movie_id"})
+
+    if project.server == ServerType.SNIC:
+
+        def get_match(string, string_options):
+            normalized_string = unicodedata.normalize("NFC", string)
+            for s in string_options:
+                normalized_s = unicodedata.normalize("NFC", s)
+                if normalized_string in normalized_s:
+                    return s
+            return None
 
-    # Identify the ordinal number of the frames expected to be extracted
-    if len(frames_df) == 0:
-        raise ValueError("No frames. Workflow stopped.")
+        movies_df["fpath"] = movies_df["fpath"].apply(
+            lambda x: get_match(x, mov_folder_df["fpath"].unique()),
+            1,
+        )
 
-    frames_df["frame_number"] = frames_df[["first_seen_movie", "fps"]].apply(
-        lambda x: [
-            int((x["first_seen_movie"] + j) * x["fps"]) for j in range(n_frames_subject)
-        ],
-        1,
+    # Merge the server path to the filepath
+    all_movies_df = movies_df.merge(
+        mov_folder_df,
+        on=["fpath"],
+        how="outer",
+        indicator=True,
     )
 
-    # Reshape df to have each frame as rows
-    lst_col = "frame_number"
+    # Select only movies without information in the movies.csv
+    no_info_movies_df = all_movies_df[all_movies_df["_merge"] == "right_only"].copy()
 
-    frames_df = pd.DataFrame(
-        {
-            col: np.repeat(frames_df[col].values, frames_df[lst_col].str.len())
-            for col in frames_df.columns.difference([lst_col])
-        }
-    ).assign(**{lst_col: np.concatenate(frames_df[lst_col].values)})[
-        frames_df.columns.tolist()
-    ]
-
-    # Drop unnecessary columns
-    frames_df.drop(["subject_ids"], inplace=True, axis=1)
-
-    return frames_df
-
-
-# Function to gather information of frames already uploaded
-def check_frames_uploaded(
-    frames_df: pd.DataFrame,
-    project: project_utils.Project,
-    species_ids: list,
-    conn: sqlite3.Connection,
-):
-    if project.server == "SNIC":
-        # Get info of frames of the species of interest already uploaded
-        if len(species_ids) <= 1:
-            uploaded_frames_df = pd.read_sql_query(
-                f"SELECT movie_id, frame_number, \
-            frame_exp_sp_id FROM subjects WHERE frame_exp_sp_id=='{species_ids[0]}' AND subject_type='frame'",
-                conn,
-            )
+    # Select only movies without information in the movies.csv
+    no_available_movies_df = all_movies_df[
+        all_movies_df["_merge"] == "left_only"
+    ].copy()
+
+    # Check that movies can be mapped
+    all_movies_df["exists"] = np.where(all_movies_df["_merge"] == "both", True, False)
+
+    # Drop _merge columns to match sql schema
+    all_movies_df = all_movies_df.drop("_merge", axis=1)
+
+    # Select only those that can be mapped
+    available_movies_df = all_movies_df[all_movies_df["exists"]].copy()
+
+    # Create a filename with ext column
+    available_movies_df["filename_ext"] = available_movies_df["fpath"].apply(
+        lambda x: x.split("/")[-1], 1
+    )
 
-        else:
-            uploaded_frames_df = pd.read_sql_query(
-                f"SELECT movie_id, frame_number, frame_exp_sp_id FROM subjects WHERE frame_exp_sp_id IN \
-            {tuple(species_ids)} AND subject_type='frame'",
-                conn,
-            )
+    # log the available movies
+    n_movies = movies_df.shape[0]
 
-        # Filter out frames that have already been uploaded
-        if (
-            len(uploaded_frames_df) > 0
-            and not uploaded_frames_df["frame_number"].isnull().any()
-        ):
-            logging.info(
-                "There are some frames already uploaded in Zooniverse for the species selected. \
-                  Checking if those are the frames you are trying to upload"
-            )
-            # Ensure that frame_number is an integer
-            uploaded_frames_df["frame_number"] = uploaded_frames_df[
-                "frame_number"
-            ].astype(int)
-            frames_df["frame_number"] = frames_df["frame_number"].astype(int)
-            merge_df = (
-                pd.merge(
-                    frames_df,
-                    uploaded_frames_df,
-                    left_on=["movie_id", "frame_number"],
-                    right_on=["movie_id", "frame_number"],
-                    how="left",
-                    indicator=True,
-                )["_merge"]
-                == "both"
-            )
-
-            # Exclude frames that have already been uploaded
-            # trunk-ignore(flake8/E712)
-            frames_df = frames_df[merge_df == False]
-            if len(frames_df) == 0:
-                logging.error(
-                    "All of the frames you have selected are already uploaded."
-                )
-            else:
-                logging.info(
-                    "There are",
-                    len(frames_df),
-                    "frames with the species of interest not uploaded to Zooniverse yet.",
-                )
+    n_available_movies = available_movies_df.shape[0]
 
-        else:
-            logging.info(
-                "There are no frames uploaded in Zooniverse for the species selected."
-            )
+    if n_movies == n_available_movies:
+        logging.info(f"All {n_movies} movies are mapped from the server")
+
+    else:
+        logging.info(
+            f"{n_available_movies} out of {n_movies} movies are available."
+            f"The missing movies are: {no_available_movies_df.fpath.unique()}"
+        )
 
-    return frames_df
+    return available_movies_df, no_available_movies_df, no_info_movies_df
 
 
-def write_movie_frames(key_movie_df: pd.DataFrame, url: str):
+def preview_movie(
+    movie_path: str,
+    movie_metadata: pd.DataFrame,
+):
     """
-    Function to get a frame from a movie
+    It takes a movie filename and its associated metadata and returns a widget object that can be displayed in the notebook
+
+    :param movie_path: the filename of the movie you want to preview
+    :param movie_metadata: the metadata of the movie you want to preview
+    :return: Widget object
     """
-    # Read the movie on cv2 and prepare to extract frames
-    cap = cv2.VideoCapture(url)
 
-    if cap.isOpened():
-        # Get the frame numbers for each movie the fps and duration
-        for index, row in tqdm(key_movie_df.iterrows(), total=key_movie_df.shape[0]):
-            # Create the folder to store the frames if not exist
-            if not os.path.exists(row["frame_path"]):
-                cap.set(1, row["frame_number"])
-                ret, frame = cap.read()
-                if frame is not None:
-                    cv2.imwrite(row["frame_path"], frame)
-                    os.chmod(row["frame_path"], 0o777)
-                else:
-                    cv2.imwrite(row["frame_path"], np.zeros((100, 100, 3), np.uint8))
-                    os.chmod(row["frame_path"], 0o777)
-                    logging.info(
-                        f"No frame was extracted for {url} at frame {row['frame_number']}"
-                    )
+    # Adjust the width of the video and metadata sections based on your preference
+    video_width = "60%"  # Adjust as needed
+    metadata_width = "40%"  # Adjust as needed
+
+    if "http" in movie_path:
+        video_widget = widgets.Video.from_url(movie_path, width=video_width)
     else:
-        logging.info("Missing movie", url)
+        video_widget = widgets.Video.from_file(movie_path, width=video_width)
+
+    metadata_html = movie_metadata.T.to_html()
+
+    metadata_widget = widgets.HTML(
+        value=metadata_html,
+        layout=widgets.Layout(width=metadata_width, overflow="auto"),
+    )
+
+    # Create a horizontal box layout to display video and metadata side by side
+    display_widget = widgets.HBox([video_widget, metadata_widget])
+
+    display(display_widget)
+
+    return display_widget
+
+
+def get_info_selected_movies(
+    selected_movies: list,
+    footage_source: str,
+    df: pd.DataFrame,
+    project: Project,
+    server_connection: dict,
+):
+    """
+    > This function takes the selected movies and source of the footage (already in the system or new) and return the df, paths and ids of the movies selected.
+    :param selected_movies: TBC
+    :param footage_source: a string specifying whether the footage is already in the system or is new
+    :param project: the project object
+    :param server_connection: a dictionary with the connection to the server
+    :param df: the dataframe of available movies
+    """
+
+    if footage_source == "Existing Footage":
+        # Create a df with the selected movies
+        selected_movies_df = df[df["filename"].isin(selected_movies)].reset_index(
+            drop=True
+        )
+
+        # Retrieve the paths of the movies selected
+        selected_movies_paths = [
+            get_movie_path(
+                project=project,
+                f_path=f_path,
+                server_connection=server_connection,
+            )
+            for f_path in selected_movies_df["fpath"]
+        ]
+
+        # Remove movie extension to match yolo_format labels
+        selected_movies_no_ext = tuple(
+            filename.rsplit(".", 1)[0] for filename in selected_movies
+        )
+
+        selected_movies_ids = {
+            key: value
+            for key, value in zip(
+                selected_movies_no_ext,
+                selected_movies_df["movie_id"].to_list(),
+            )
+        }
+
+    elif footage_source == "New Footage":
+        selected_movies_paths = selected_movies
+        selected_movies_ids = {}
+        selected_movies_df = pd.DataFrame()
+
+    return (
+        selected_movies_paths,
+        selected_movies,
+        selected_movies_df,
+        selected_movies_ids,
+    )
 
 
 # Function to extract selected frames from videos
 def extract_frames(
-    project: project_utils.Project,
+    project: Project,
+    server_connection: dict,
     df: pd.DataFrame,
-    server_dict: dict,
     frames_folder: str,
 ):
     """
     Extract frames and save them in chosen folder.
+    :param project: the project object
+    :param server_connection: a dictionary with the connection to the server
+    :param df: a dataframe of the frames to be extracted
+    :param frames_folder: a string with the path of the folder to store the frames
+
     """
 
     # Set the filename of the frames
-    df["frame_path"] = (
-        frames_folder
-        + df["filename"].astype(str)
-        + "_frame_"
-        + df["frame_number"].astype(str)
-        + "_"
-        + df["label"].astype(str)
-        + ".jpg"
+    df["frame_path"] = df.apply(
+        lambda row: str(
+            Path(frames_folder)
+            / f"{row['filename']}_{row['frame_number']}_{row['label']}.jpg"
+        ),
+        axis=1,
     )
 
     # Create the folder to store the frames if not exist
-    if not os.path.exists(frames_folder):
-        Path(frames_folder).mkdir(parents=True, exist_ok=True)
+    frames_folder_path = Path(frames_folder)
+    if not frames_folder_path.exists():
+        frames_folder_path.mkdir(parents=True, exist_ok=True)
         # Recursively add permissions to folders created
-        [os.chmod(root, 0o777) for root, dirs, files in os.walk(frames_folder)]
+        for root, dirs, files in frames_folder_path.iterdir():
+            Path(root).chmod(0o777)
 
     for movie in df["fpath"].unique():
-        url = movie_utils.get_movie_path(
-            project=project, db_info_dict=server_dict, f_path=movie
+        url = get_movie_path(
+            f_path=movie, project=project, server_connection=server_connection
         )
 
         if url is None:
             logging.error(f"Movie {movie} couldn't be found in the server.")
         else:
             # Select the frames to download from the movie
             key_movie_df = df[df["fpath"] == movie].reset_index()
@@ -369,494 +367,542 @@
             write_movie_frames(key_movie_df, url)
 
         logging.info("Frames extracted successfully")
 
     return df
 
 
-# Function to the provide drop-down options to select the frames to be uploaded
-def get_frames(
-    species_names: list,
-    db_path: str,
-    zoo_info_dict: dict,
-    server_dict: dict,
-    project: project_utils.Project,
-    n_frames_subject=3,
-    subsample_up_to=100,
-):
-    # Roadblock to check if species list is empty
-    if len(species_names) == 0:
-        raise ValueError(
-            "No species were selected. Please select at least one species before continuing."
-        )
-
-    # Transform species names to species ids
-    species_ids = get_species_ids(project, species_names)
-    conn = db_utils.create_connection(db_path)
-
-    if project.movie_folder is None:
-        # Extract frames of interest from a folder with frames
-        if project.server == "SNIC":
-            # Specify volume allocated by SNIC
-            snic_path = "/mimer/NOBACKUP/groups/snic2021-6-9"
-            df = FileChooser(str(Path(snic_path, "tmp_dir")))
-        else:
-            df = FileChooser(".")
-        df.title = "<b>Select frame folder location</b>"
+def write_movie_frames(key_movie_df: pd.DataFrame, url: str):
+    """
+    Function to get a frame from a movie
+    :param key_movie_df: a df with the information of the movie
+    :param url: a string with the url of the movie
 
-        # Callback function
-        def build_df(chooser):
-            frame_files = os.listdir(chooser.selected)
-            frame_paths = [os.path.join(chooser.selected, i) for i in frame_files]
-            chooser.df = pd.DataFrame(frame_paths, columns=["frame_path"])
+    """
+    # Read the movie on cv2 and prepare to extract frames
+    cap = cv2.VideoCapture(url)
 
-            if isinstance(species_ids, list):
-                chooser.df["species_id"] = str(species_ids)
-            else:
-                chooser.df["species_id"] = species_ids
+    if cap.isOpened():
+        # Get the frame numbers for each movie the fps and duration
+        for index, row in tqdm(key_movie_df.iterrows(), total=key_movie_df.shape[0]):
+            # Create the folder to store the frames if not exist
+            frame_path = Path(row["frame_path"])
+            if not frame_path.exists():
+                cap.set(1, row["frame_number"])
+                ret, frame = cap.read()
+                if frame is not None:
+                    cv2.imwrite(str(frame_path), frame)
+                    frame_path.chmod(0o777)
+                else:
+                    cv2.imwrite(str(frame_path), np.zeros((100, 100, 3), np.uint8))
+                    frame_path.chmod(0o777)
+                    logging.info(
+                        f"No frame was extracted for {url} at frame {row['frame_number']}"
+                    )
+    else:
+        logging.info(f"Missing movie {url}")
 
-        # Register callback function
-        df.register_callback(build_df)
-        display(df)
-
-    else:
-        ## Choose the Zooniverse workflow/s with classified clips to extract the frames from ####
-        # Select the Zooniverse workflow/s of interest
-        workflows_out = t8.WidgetMaker(zoo_info_dict["workflows"])
-        display(workflows_out)
-
-        # Select the agreement threshold to aggregrate the responses
-        agg_params = t8.choose_agg_parameters("clip")
-
-        # Select the temp location to store frames before uploading them to Zooniverse
-        if project.server == "SNIC":
-            # Specify volume allocated by SNIC
-            snic_path = "/mimer/NOBACKUP/groups/snic2021-6-9"
-            df = FileChooser(str(Path(snic_path, "tmp_dir")))
-        else:
-            df = FileChooser(".")
-        df.title = "<b>Choose location to store frames</b>"
 
-        # Callback function
-        def extract_files(chooser):
-            # Get the aggregated classifications based on the specified agreement threshold
-            clips_df = t8.get_classifications(
-                workflows_out.checks,
-                zoo_info_dict["workflows"],
-                "clip",
-                zoo_info_dict["classifications"],
-                db_path,
-                project,
-            )
-
-            agg_clips_df, raw_clips_df = t8.aggregate_classifications(
-                clips_df, "clip", project, agg_params=agg_params
-            )
-
-            # Match format of species name to Zooniverse labels
-            species_names_zoo = [
-                clean_label(species_name) for species_name in species_names
-            ]
+def get_movie_extensions():
+    # Specify the formats of the movies to select
+    return tuple(["wmv", "mpg", "mov", "avi", "mp4", "MOV", "MP4"])
 
-            # Select only aggregated classifications of species of interest:
-            sp_agg_clips_df = agg_clips_df[
-                agg_clips_df["label"].isin(species_names_zoo)
-            ]
 
-            # Subsample up to desired sample
-            if sp_agg_clips_df.shape[0] >= subsample_up_to:
-                logging.info("Subsampling up to " + str(subsample_up_to))
-                sp_agg_clips_df = sp_agg_clips_df.sample(subsample_up_to)
-
-            # Populate the db with the aggregated classifications
-            populate_agg_annotations(sp_agg_clips_df, "clip", project)
-
-            # Get df of frames to be extracted
-            frame_df = get_species_frames(
-                sp_agg_clips_df,
-                species_ids,
-                server_dict,
-                conn,
-                project,
-                n_frames_subject,
-            )
-
-            # Check the frames haven't been uploaded to Zooniverse
-            frame_df = check_frames_uploaded(frame_df, project, species_ids, conn)
-
-            # Extract the frames from the videos and store them in the temp location
-            if project.server == "SNIC":
-                folder_name = chooser.selected
-                frames_folder = Path(
-                    folder_name, "_".join(species_names_zoo) + "_frames/"
-                )
-            else:
-                frames_folder = "_".join(species_names_zoo) + "_frames/"
-            chooser.df = extract_frames(project, frame_df, server_dict, frames_folder)
+def convert_video(
+    movie_path: str,
+    movie_filename: str,
+    fps_output: str,
+    gpu_available: bool = False,
+    compression: bool = False,
+):
+    """
+    It takes a movie file path and a boolean indicating whether a GPU is available, and returns a new
+    movie file path.
 
-        # Register callback function
-        df.register_callback(extract_files)
-        display(df)
-
-    return df
+    :param movie_path: The local path- or url to the movie file you want to convert
+    :type movie_path: str
+    :param movie_filename: The filename of the movie file you want to convert
+    :type movie_filename: str
+    :param gpu_available: Boolean, whether or not a GPU is available
+    :type gpu_available: bool
+    :param compression: Boolean, whether or not movie compression is required
+    :type compression: bool
+    :param fps_output: String, argument used to force integer fps for movies
+    :type fps_output: str
+    :return: The path to the converted video file.
+    """
+
+    # Set the name of the converted movie
+    conv_filename = "conv_" + movie_filename
+
+    # Check the movie is accessible locally
+    if Path(movie_path).exists():
+        # Store the directory and filename of the movie
+        movie_fpath = Path(movie_path).parent
+        conv_fpath = movie_fpath / conv_filename
+
+    # Check if the path to the movie is a url
+    elif is_url(movie_path):
+        # Specify the directory to store the converted movie
+        conv_fpath = Path(conv_filename)
 
+    else:
+        logging.error(f"The path to {conv_fpath} is invalid")
 
-# Function to specify the frame modification
-def select_modification():
-    # Widget to select the frame modification
-
-    frame_modifications = {
-        "Color_correction": {
-            "filter": ".filter('curves', '0/0 0.396/0.67 1/1', \
-                                        '0/0 0.525/0.451 1/1', \
-                                        '0/0 0.459/0.517 1/1')"
-        }
-        # borrowed from https://www.element84.com/blog/color-correction-in-space-and-at-sea
-        ,
-        "Zoo_low_compression": {
-            "crf": "25",
-        },
-        "Zoo_medium_compression": {
-            "crf": "27",
-        },
-        "Zoo_high_compression": {
-            "crf": "30",
-        },
-        "Blur_sensitive_info": {
-            "filter": ".drawbox(0, 0, 'iw', 'ih*(15/100)', color='black' \
-                            ,thickness='fill').drawbox(0, 'ih*(95/100)', \
-                            'iw', 'ih*(15/100)', color='black', thickness='fill')",
-            "None": {},
-        },
-    }
-
-    select_modification_widget = widgets.Dropdown(
-        options=[(a, b) for a, b in frame_modifications.items()],
-        description="Select modification:",
-        ensure_option=True,
-        disabled=False,
-        style={"description_width": "initial"},
-    )
+    # Set up input and output default prompts
+    input_path = movie_path
+    output_path = str(conv_fpath)
+
+    input_options = {}
+    output_options = {}
+
+    # Add GPU-related options if available
+    if gpu_available:
+        input_options["hwaccel"] = "cuda"
+
+    output_options["filter:v"] = fps_output
+    output_options["pix_fmt"] = "yuv420p"
+
+    if compression:
+        output_options["crf"] = "22"
+
+    # Run the ffmpeg movie convertion code
+    try:
+        ffmpeg.input(input_path, **input_options).output(
+            output_path, **output_options
+        ).run(overwrite_output=True)
+
+    except ffmpeg.Error as e:
+        logging.error("ffmpeg error occurred.")
+        logging.error(f"stderr: {e}")
+        if e.stdout is not None:
+            logging.error(f"stdout: {e.stdout.decode('utf8')}")
+        if e.stderr is not None:
+            logging.error(f"stderr: {e.stderr.decode('utf8')}")
+        raise e
+
+    # Ensure the movie was extracted
+    if not conv_fpath.exists():
+        raise FileNotFoundError(f"{conv_fpath} was not converted and stored locally.")
 
-    display(select_modification_widget)
-    return select_modification_widget
+    else:
+        # Ensure open permissions on file
+        conv_fpath.chmod(0o777)
+        logging.info(f"{conv_fpath} successfully converted and stored locally.")
+
+    return str(conv_fpath)
 
 
-def check_frame_size(frame_paths: list):
+def standarise_movie_format(
+    project: Project,
+    server_connection: dict,
+    movie_path: str,
+    movie_filename: str,
+    f_path: str,
+    gpu_available: bool = False,
+):
     """
-    It takes a list of file paths, gets the size of each file, and returns a dataframe with the file
-    path and size of each file
+    This function reviews the movie metadata. If the movie is not in the correct format, frame rate or codec,
+    it is converted using ffmpeg.
 
-    :param frame_paths: a list of paths to the frames you want to check
-    :return: A dataframe with the file path and size of each frame.
-    """
+    :param project: the project object
+    :param movie_path: The local path- or url to the movie file you want to convert
+    :type movie_path: str
+    :param movie_filename: The filename of the movie file you want to convert
+    :type movie_filename: str
+    :param f_path: The server or storage path of the original movie you want to convert
+    :type f_path: str
+    :param gpu_available: Boolean, whether or not a GPU is available
+    :type gpu_available: bool
+    """
+
+    # Check movie format ######
+    ext = Path(movie_filename).suffix
+
+    # Set video conversion to false as default
+    convert_video_T_F = False
+
+    if not ext.lower() == ".mp4":
+        logging.info(f"Extension of {movie_filename} not supported.")
+        # Set conversion to True
+        convert_video_T_F = True
+
+    # Check frame rate #######
+    cap = cv2.VideoCapture(movie_path)
+    fps = cap.get(cv2.CAP_PROP_FPS)
 
-    # Get list of files with size
-    files_with_size = [
-        (file_path, os.stat(file_path).st_size) for file_path in frame_paths
-    ]
+    if not float(fps).is_integer():
+        logging.info(
+            f"Variable frame rate {float(fps)} of {movie_filename} not supported."
+        )
+        # Set conversion to True
+        convert_video_T_F = True
 
-    df = pd.DataFrame(files_with_size, columns=["File_path", "Size"])
+    # Check codec info ########
+    def get_fourcc(cap: cv2.VideoCapture) -> str:
+        """Return the 4-letter string of the codec of a video."""
+        return (
+            int(cap.get(cv2.CAP_PROP_FOURCC))
+            .to_bytes(4, byteorder=sys.byteorder)
+            .decode()
+        )
 
-    # Change bytes to MB
-    df["Size"] = df["Size"] / 1000000
+    codec = get_fourcc(cap)
 
-    if df["Size"].ge(1).any():
-        logging.info(
-            "Frames are too large (over 1 MB) to be uploaded to Zooniverse. Compress them!"
-        )
-        return df
-    else:
+    if codec not in ["h264", "avc1"]:
         logging.info(
-            "Frames are a good size (below 1 MB). Ready to be uploaded to Zooniverse"
+            f"The codecs of {movie_filename} are not supported (only h264 is supported)."
         )
-        return df
+        # Set conversion to True
+        convert_video_T_F = True
 
+    #  Check movie file #######
+    # Create a list of the project where movie compression is not needed
+    project_no_compress = ["Spyfish_Aotearoa"]
+
+    if project.Project_name in project_no_compress:
+        # Set movie compression to false
+        compress_video = False
 
-# Function to compare original to modified frames
-def compare_frames(df):
-    if not isinstance(df, pd.DataFrame):
-        df = df.df
+    else:
+        # Check movie filesize in relation to its duration
+        frame_count = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
+        duration = frame_count / fps
+        duration_mins = duration / 60
+
+        # Check if the movie is accessible locally
+        if Path(movie_path).exists():
+            # Store the size of the movie
+            size = Path(movie_path).stat().st_size
+
+        # Check if the path to the movie is a url
+        elif is_url(movie_path):
+            # Store the size of the movie
+            size = urllib.request.urlopen(movie_path).length
 
-    # Save the paths of the clips
-    original_frame_paths = df["frame_path"].unique()
+        else:
+            logging.error(f"The path to {movie_path} is invalid")
 
-    # Add "no movie" option to prevent conflicts
-    original_frame_paths = np.append(original_frame_paths, "No frame")
+        # Calculate the size:duration ratio
+        sizeGB = size / (1024 * 1024 * 1024)
+        size_duration = sizeGB / duration_mins
 
-    clip_path_widget = widgets.Dropdown(
-        options=tuple(np.sort(original_frame_paths)),
-        description="Select original frame:",
-        ensure_option=True,
-        disabled=False,
-        layout=widgets.Layout(width="50%"),
-        style={"description_width": "initial"},
-    )
+        if size_duration > 0.16:
+            # Compress the movie if file size is too large
+            logging.info(
+                "File size of movie is too large (+5GB per 30 mins of footage)."
+            )
 
-    main_out = widgets.Output()
-    display(clip_path_widget, main_out)
+            # Specify to compress the video
+            compress_video = True
+        else:
+            # Set movie compression to false
+            compress_video = False
 
-    # Display the original and modified clips
-    def on_change(change):
-        with main_out:
-            clear_output()
-            if change["new"] == "No frame":
-                print("It is OK to modify the frames again")
-            else:
-                a = view_frames(df, change["new"])
-                display(a)
+    # Start converting/compressing video if movie didn't pass any of the checks
+    if convert_video_T_F or compress_video:
+        # Specify the desired fps of the movie
+        fps_output = "fps=" + str(round(fps))
+
+        conv_mov_path = convert_video(
+            movie_path=movie_path,
+            movie_filename=movie_filename,
+            fps_output=fps_output,
+            gpu_available=gpu_available,
+            compression=compress_video,
+        )
+
+        # Upload the converted movie to the server
+        upload_file_server(
+            conv_mov_path=conv_mov_path,
+            f_path=f_path,
+            project=project,
+            server_connection=server_connection,
+        )
 
-    clip_path_widget.observe(on_change, names="value")
+    else:
+        logging.info(f"No modification needed for {movie_filename}")
 
 
-# Display the frames using html
-def view_frames(df: pd.DataFrame, frame_path: str):
-    # Get path of the modified clip selected
-    modified_frame_path = df[df["frame_path"] == frame_path].modif_frame_path.values[0]
-    extension = os.path.splitext(frame_path)[1]
-
-    img1 = open(frame_path, "rb").read()
-    wi1 = widgets.Image(value=img1, format=extension, width=400, height=500)
-    img2 = open(modified_frame_path, "rb").read()
-    wi2 = widgets.Image(value=img2, format=extension, width=400, height=500)
-    a = [wi1, wi2]
-    wid = widgets.HBox(a)
-
-    return wid
-
-
-# Function modify the frames
-def modify_frames(
-    frames_to_upload_df: pd.DataFrame,
-    species_i: list,
-    modification_details: dict,
-    project: project_utils.Project,
+def check_movies_meta(
+    project: Project,
+    csv_paths: dict,
+    db_connection,
+    available_movies_df: pd.DataFrame,
+    no_info_movies_df: pd.DataFrame,
+    server_connection: dict,
+    review_method: str,
+    gpu_available: bool = False,
 ):
-    server = project.server
+    """
+    > This function loads the csv with movies information, checks and updates missing info
 
-    # Specify the folder to host the modified frames
-    if server == "SNIC":
-        # Specify volume allocated by SNIC
-        snic_path = "/mimer/NOBACKUP/groups/snic2021-6-9"
-        folder_name = f"{snic_path}/tmp_dir/frames/"
-        mod_frames_folder = Path(
-            folder_name, "modified_" + "_".join(species_i) + "_frames/"
-        )
-    else:
-        mod_frames_folder = "modified_" + "_".join(species_i) + "_frames/"
-
-    # Specify the path of the modified frames
-    frames_to_upload_df["modif_frame_path"] = (
-        mod_frames_folder
-        + "_modified_"
-        + frames_to_upload_df["frame_path"].apply(lambda x: os.path.basename(x))
+    :param project: the project object
+    :param db_connection: the sql connection to the db
+    :param available_movies_df: a df with the information about the filepaths and "existance" of the movies
+    :param csv_paths: a dictionary with the paths of the csv files with info to initiate the db
+    :param server_connection: a dictionary with the connection to the server
+    :param review_method: The method used to review the movies
+    :param gpu_available: Boolean, whether or not a GPU is available
+    """
+
+    # Load the csv with movies information
+    df = pd.read_csv(csv_paths["local_movies_csv"])
+
+    from kso_utils.db_utils import cols_rename_to_schema
+
+    # Rename the project-specific column names
+    # that match schema standard names
+    df = cols_rename_to_schema(
+        project=project,
+        table_name="movies",
+        df=df,
     )
 
-    # Remove existing modified clips
-    if os.path.exists(mod_frames_folder):
-        shutil.rmtree(mod_frames_folder)
-
-    if len(modification_details.values()) > 0:
-        # Save the modification details to include as subject metadata
-        frames_to_upload_df["frame_modification_details"] = str(modification_details)
-
-        # Create the folder to store the videos if not exist
-        if not os.path.exists(mod_frames_folder):
-            Path(mod_frames_folder).mkdir(parents=True, exist_ok=True)
-            # Recursively add permissions to folders created
-            [os.chmod(root, 0o777) for root, dirs, files in os.walk(mod_frames_folder)]
-
-        #### Modify the clips###
-        # Read each clip and modify them (printing a progress bar)
-        for index, row in tqdm(
-            frames_to_upload_df.iterrows(), total=frames_to_upload_df.shape[0]
-        ):
-            if not os.path.exists(row["modif_frame_path"]):
-                # Set up input prompt
-                init_prompt = f"ffmpeg_python.input('{row['frame_path']}')"
-                full_prompt = init_prompt
-                # Set up modification
-                for transform in modification_details.values():
-                    if "filter" in transform:
-                        mod_prompt = transform["filter"]
-                        full_prompt += mod_prompt
-                # Setup output prompt
-                crf_value = [
-                    transform["crf"] if "crf" in transform else None
-                    for transform in modification_details.values()
-                ]
-                crf_value = [i for i in crf_value if i is not None]
+    # Check all available movies in the server/storage have information in the movies.csv
+    # Get a list of all the available movies
+    if not no_info_movies_df.empty:
+        logging.info(
+            f"There are {no_info_movies_df.shape[0]} movies in the movie_folder"
+            f" that are not in the movies.csv. Their paths are: {no_info_movies_df.fpath.unique()}"
+        )
 
-                if len(crf_value) > 0:
-                    # Note: now using q option as crf not supported by ffmpeg build
-                    crf_prompt = str(max([int(i) for i in crf_value]))
-                    full_prompt += f".output('{row['modif_frame_path']}', q={crf_prompt}, pix_fmt='yuv420p')"
-                else:
-                    full_prompt += (
-                        f".output('{row['modif_frame_path']}', q=20, pix_fmt='yuv420p')"
-                    )
-                # Run the modification
-                try:
-                    print(full_prompt)
-                    eval(full_prompt).run(capture_stdout=True, capture_stderr=True)
-                    os.chmod(row["modif_frame_path"], 0o777)
-                except ffmpeg_python.Error as e:
-                    logging.info("stdout:", e.stdout.decode("utf8"))
-                    logging.info("stderr:", e.stderr.decode("utf8"))
-                    raise e
+    # Add information about whether the movies are available in the movie_folder
+    df_temp = df.copy().drop(columns=["fpath"])
+    df_toreview = df_temp.merge(
+        available_movies_df[["filename", "fpath", "exists"]],
+        on=["filename"],
+        how="left",
+    )
 
-        logging.info("Frames modified successfully")
+    if df_toreview.exists.isnull().values.any():
+        # Replace na with False
+        df_toreview["exists"] = df_toreview["exists"].fillna(False)
+
+        logging.warn(
+            f"Only # {df_toreview[df_toreview['exists']].shape[0]} out of"
+            f"# {df_toreview[~df_toreview['exists']].shape[0]} movies with missing information are available."
+            f" Proceeding to retrieve information for only those {df_toreview[df_toreview['exists']].shape[0]} available movies."
+        )
+
+        # Select only available movies
+        df_toreview = df_toreview[df_toreview["exists"]].reset_index(drop=True)
+
+    if df_toreview.empty:
+        logging.info("There are no movies available to review.")
+        return
 
     else:
-        # Save the modification details to include as subject metadata
-        frames_to_upload_df["modif_frame_path"] = frames_to_upload_df["frame_path"]
+        if review_method.startswith("Advanced"):
+            logging.info("Checking the format, frame rate and codec of the movies")
 
-    return frames_to_upload_df
+            # Convert movies to the right format, frame rate or codec and upload them to the project's server/storage
+            [
+                standarise_movie_format(
+                    project=project,
+                    server_connection=server_connection,
+                    movie_path=get_movie_path(j, project, server_connection),
+                    movie_filename=i,
+                    f_path=j,
+                    gpu_available=gpu_available,
+                )
+                for i, j in tqdm(
+                    zip(df_toreview["filename"], df_toreview["fpath"]),
+                    total=df_toreview.shape[0],
+                )
+            ]
 
+            # Specify to check the fps
+            check_fps = True
 
-# Function to set the metadata of the frames to be uploaded to Zooniverse
-def set_zoo_metadata(
-    df, species_list: list, project: project_utils.Project, db_info_dict: dict
-):
-    project_name = project.Project_name
+        if review_method.startswith("Basic"):
+            # Check if fps or duration is missing from any movie
+            if not df_toreview[["fps", "duration"]].isna().any().any():
+                # Specify to not check the fps
+                check_fps = False
 
-    if not isinstance(df, pd.DataFrame):
-        df = df.df
+            else:
+                # Create a df with only those rows with missing fps/duration
+                df_toreview = df_toreview[
+                    df_toreview["fps"].isna() | df_toreview["duration"].isna()
+                ].reset_index(drop=True)
 
-    if (
-        "modif_frame_path" in df.columns
-        and "no_modification" not in df["modif_frame_path"].values
-    ):
-        df["frame_path"] = df["modif_frame_path"]
-
-    # Set project-specific metadata
-    if project.Zooniverse_number == 9747:
-        conn = db_utils.create_connection(project.db_path)
-        sites_df = pd.read_sql_query("SELECT id, siteName FROM sites", conn)
-        df = df.merge(sites_df, left_on="site_id", right_on="id")
-        upload_to_zoo = df[
-            [
-                "frame_path",
-                "frame_number",
-                "species_id",
-                "movie_id",
-                "created_on",
-                "siteName",
+                logging.info(
+                    "There are empty entries for fps, duration and sampling information"
+                )
+                # Specify to check the fps
+                check_fps = True
+
+        if check_fps:
+            logging.info("Checking the fps and duration of the movies")
+            # Retrieve the path of the movie (wheter the local path or a url),
+            # get the fps/duration and overwrite the existing fps and duration info
+            df_toreview[["fps", "duration"]] = pd.DataFrame(
+                [
+                    get_fps_duration(get_movie_path(i, project, server_connection))
+                    for i in tqdm(df_toreview["fpath"], total=df_toreview.shape[0])
+                ],
+                columns=["fps", "duration"],
+            )
+
+        # Check if there are missing sampling starts
+        empty_sampling_start = df_toreview["sampling_start"].isna()
+
+        # Check if there are missing sampling ends
+        empty_sampling_end = df_toreview["sampling_end"].isna()
+
+        # Fill out missing sampling start information
+        if empty_sampling_start.any():
+            df_toreview.loc[empty_sampling_start, "sampling_start"] = 0.0
+            mov_list = df_toreview[empty_sampling_start].filename.unique()
+            logging.info(f"Added sampling_start of the movies {mov_list}")
+
+        # Fill out missing sampling end information
+        if empty_sampling_end.any():
+            df_toreview.loc[empty_sampling_end, "sampling_end"] = df_toreview[
+                "duration"
             ]
-        ]
+            mov_list = df_toreview[empty_sampling_end].filename.unique()
+            logging.info(f"Added sampling_end of the movies {mov_list}")
 
-    elif project_name == "SGU":
-        upload_to_zoo = df[["frame_path", "species_id", "filename"]]
+        # Prevent sampling end times longer than actual movies
+        if (df_toreview["sampling_end"] > df_toreview["duration"]).any():
+            mov_list = df_toreview[
+                df_toreview["sampling_end"] > df_toreview["duration"]
+            ].filename.unique()
+            raise ValueError(
+                f"The sampling_end times of the following movies are longer than the actual movies {mov_list}"
+            )
 
-    elif project_name == "Spyfish_Aotearoa":
-        upload_to_zoo = spyfish_utils.spyfish_subject_metadata(df, db_info_dict)
-    else:
-        logging.error("This project is not a supported Zooniverse project.")
+        # if there have not been any changes, report that movies are OK, else update the csv files
+        if (
+            not check_fps
+            and not empty_sampling_end.any()
+            and not empty_sampling_start.any()
+        ):
+            logging.info(
+                f"{df_toreview[df_toreview['exists']].shape[0]} available movies"
+                f" have been checked and no action was required."
+            )
 
-    # Add information about the type of subject
-    upload_to_zoo = upload_to_zoo.copy()
-    upload_to_zoo.loc[:, "subject_type"] = "frame"
-    upload_to_zoo = upload_to_zoo.rename(columns={"species_id": "frame_exp_sp_id"})
+            return
 
-    # Check there are no empty values (prevent issues uploading subjects)
-    if upload_to_zoo.isnull().values.any():
-        logging.error(
-            "There are some values missing from the data you are trying to upload."
-        )
+        else:
+            # Add the missing info to the original df based on movie ids
+            df.set_index("movie_id", inplace=True)
+            df_toreview.set_index("movie_id", inplace=True)
+            df.update(df_toreview)
+            df.reset_index(drop=False, inplace=True)
+
+            # Rename back the project-specific column names
+            # that don't match schema standard names
+            df = cols_rename_to_schema(
+                project=project,
+                table_name="movies",
+                df=df,
+                reverse_lookup=True,
+            )
+
+            # Save the updated df locally
+            if os.access(csv_paths["local_movies_csv"], os.W_OK):
+                df.to_csv(csv_paths["local_movies_csv"], index=False)
+            else:
+                logging.info(
+                    "Unable to update local movies.csv file automatically, please do this manually with the given output."
+                )
+                return df
+            logging.info(
+                f"The local movies.csv file {csv_paths['local_movies_csv']} has been updated"
+            )
+
+            from kso_utils.server_utils import update_csv_server
+
+            # Save the updated df in the server
+            update_csv_server(
+                project=project,
+                csv_paths=csv_paths,
+                server_connection=server_connection,
+                orig_csv="server_movies_csv",
+                updated_csv="local_movies_csv",
+            )
+
+
+def concatenate_local_movies(csv_paths):
+    # Load the csv with movies information
+    df = pd.read_csv(csv_paths["local_movies_csv"])
+
+    # Select only the path of the folder
+    df["Path"] = df["fpath"].apply(lambda x: Path(x).parent)
+
+    # Function to merge directory path and multiple filenames into a list
+    def merge_paths(row):
+        directory_path = row["Path"]
+        filenames = row["go_pro_files"].split("; ")
+        merged_paths = [directory_path / filename.strip() for filename in filenames]
+        return merged_paths
+
+    # Combine the path of the folder with the go_profiles inside the folder
+    df["path_go_pros"] = df.apply(merge_paths, axis=1)
+
+    # Loop through each classification submitted by the users
+    for index, row in tqdm(df.iterrows(), total=df.shape[0]):
+        # Start text file and list to keep track of the videos to concatenate
+        textfile_name = "a_file.txt"
+        with open(textfile_name, "w") as textfile:
+            video_list = []
+
+            for movie_i in sorted(row["path_go_pros"]):
+                # Keep track of the videos to concatenate
+                textfile.write("file '" + str(movie_i) + "'" + "\n")
+                video_list.append(movie_i)
+
+        # Concatenate the files
+        if Path(row["fpath"]).exists():
+            logging.info(f"{row['fpath']} not concatenated because it already exists")
+        else:
+            logging.info(f"Concatenating {row['fpath']}")
+
+            # Concatenate the videos
+            subprocess.call(
+                [
+                    "ffmpeg",
+                    "-f",
+                    "concat",
+                    "-safe",
+                    "0",
+                    "-i",
+                    "a_file.txt",
+                    "-c",
+                    "copy",
+                    str(row["fpath"]),
+                ]
+            )
 
-    return upload_to_zoo
+        logging.info(f"{row['fpath']} concatenated successfully")
 
+        # Delete the text file
+        Path(textfile_name).unlink()
 
-# Function to upload frames to Zooniverse
-def upload_frames_to_zooniverse(
-    upload_to_zoo: dict,
-    species_list: list,
-    db_info_dict: dict,
-    project: project_utils.Project,
+
+def select_project_movies(
+    project: Project,
+    movies_df: pd.DataFrame,
 ):
-    # Retireve zooniverse project name and number
-    project_name = project.Project_name
-    project_number = project.Zooniverse_number
-
-    # Estimate the number of frames
-    n_frames = upload_to_zoo.shape[0]
-
-    if project_name == "Koster_Seafloor_Obs":
-        created_on = upload_to_zoo["created_on"].unique()[0]
-        sitename = upload_to_zoo["siteName"].unique()[0]
-
-        # Name the subject set
-        subject_set_name = (
-            "frames_"
-            + str(int(n_frames))
-            + "_"
-            + "_".join(species_list)
-            + "_"
-            + sitename
-            + "_"
-            + created_on
-        )
-
-    elif project_name == "SGU":
-        surveys_df = pd.read_csv(db_info_dict["local_surveys_csv"])
-        created_on = surveys_df["SurveyDate"].unique()[0]
-        folder_name = os.path.split(
-            os.path.dirname(upload_to_zoo["frame_path"].iloc[0])
-        )[1]
-        sitename = folder_name
-
-        # Name the subject set
-        subject_set_name = (
-            "frames_"
-            + str(int(n_frames))
-            + "_"
-            + "_".join(species_list)
-            + "_"
-            + sitename
-            + "_"
-            + created_on
-        )
-
-    else:
-        # Name the subject for frames from multiple sites/movies
-        subject_set_name = (
-            "frames_"
-            + str(int(n_frames))
-            + "_"
-            + "_".join(species_list)
-            + date.today().strftime("_%d_%m_%Y")
-        )
-
-    # Create a new subject set to host the frames
-    subject_set = SubjectSet()
-    subject_set.links.project = project_number
-    subject_set.display_name = subject_set_name
-    subject_set.save()
-
-    logging.info(subject_set_name, "subject set created")
-
-    # Save the df as the subject metadata
-    subject_metadata = upload_to_zoo.set_index("frame_path").to_dict("index")
-
-    # Upload the clips to Zooniverse (with metadata)
-    new_subjects = []
-
-    logging.info("Uploading subjects to Zooniverse...")
-    for frame_path, metadata in tqdm(
-        subject_metadata.items(), total=len(subject_metadata)
-    ):
-        subject = Subject()
-
-        subject.links.project = project_number
-        subject.add_location(frame_path)
-
-        logging.info(frame_path)
-        subject.metadata.update(metadata)
-
-        logging.info(metadata)
-        subject.save()
-        logging.info("Subject saved")
-        new_subjects.append(subject)
-
-    # Upload videos
-    subject_set.add(new_subjects)
-    logging.info("Subjects uploaded to Zooniverse")
+    """
+    > This function filters a df of movies to select only those movies that are relevant to the project (e.g. good visibity)
+
+    :param project: the project object
+    :param movies_df: a df with the information about the filepaths and "existance" of the movies
+    """
+
+    # Select only movies that are a good deployment
+    if project.Project_name in ["Spyfish_Aotearoa"]:
+        # Check for missing values in IsBadDeployment column
+        if movies_df["IsBadDeployment"].isnull().any():
+            raise ValueError(
+                "The 'IsBadDeployment' column contains missing values. Please handle missing values before proceeding."
+            )
+
+        else:
+            movies_df = movies_df.loc[~movies_df.IsBadDeployment]
+
+    return movies_df
```

### Comparing `kso_utils-0.1.0/kso_utils/zenodo_utils.py` & `kso_utils-0.2.0/kso_utils/zenodo_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import wandb
 import requests
-import os, json
+import os
+import json
 import logging
 from pathlib import Path
 
 # Logging
 logging.basicConfig()
 logging.getLogger().setLevel(logging.INFO)
 
@@ -94,16 +94,16 @@
     r = requests.put(
         f"https://zenodo.org/api/deposit/depositions/{deposition_id}",
         params={"access_token": access_token},
         data=json.dumps(data),
         headers=headers,
     )
     if r.status_code == 200:
-        print("Upload successful")
+        logging.info("Upload successful")
         r = requests.post(
             f"https://zenodo.org/api/deposit/depositions/{deposition_id}/actions/publish",
             params={"access_token": access_token},
         )
         return r.status_code
 
     else:
-        print("Upload failed")
+        logging.info("Upload failed")
```

### Comparing `kso_utils-0.1.0/kso_utils/zooniverse_utils.py` & `kso_utils-0.2.0/kso_utils/db_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,541 +1,561 @@
-## Zooniverse utils
-
 # base imports
-import io
-import getpass
-import pandas as pd
-import json
+import sqlite3
 import logging
-import numpy as np
-from panoptes_client import Project, Panoptes, panoptes
-from ast import literal_eval
+from pathlib import Path
+import pandas as pd
 
 # util imports
-from kso_utils.koster_utils import (
-    process_koster_subjects,
-    clean_duplicated_subjects,
-    combine_annot_from_duplicates,
-)
-
-# from kso_utils.spyfish_utils import process_spyfish_subjects
-import kso_utils.project_utils as project_utils
-import kso_utils.db_utils as db_utils
+import kso_utils.db_starter.schema as schema
+from kso_utils.project_utils import Project
 
 
 # Logging
 logging.basicConfig()
 logging.getLogger().setLevel(logging.INFO)
 
 
-def zoo_credentials():
-    zoo_user = getpass.getpass("Enter your Zooniverse user")
-    zoo_pass = getpass.getpass("Enter your Zooniverse password")
-    return zoo_user, zoo_pass
+# SQL specific functions
+def create_connection(db_file: str):
+    """create a database connection to the SQLite database
+        specified by db_file
 
+    :param db_file: database file
+    :return: Connection object or None
+    """
+    conn = None
+    db_path = Path(db_file)
+    try:
+        if not db_path.parent.exists():
+            if not db_path.parent == Path(""):
+                db_path.parent.mkdir(parents=True)
+                db_path.parent.chmod(0o777)
+        conn = sqlite3.connect(db_file)
+        conn.execute("PRAGMA foreign_keys = 1")
+        db_path.chmod(0o777)
+        return conn
+    except sqlite3.Error as e:
+        logging.error(e)
 
-class AuthenticationError(Exception):
-    pass
+    return conn
 
 
-def connect_zoo_project(project: project_utils.Project):
+def drop_table(conn: sqlite3.Connection, table_name: str):
     """
-    It takes a project name as input, and returns a Zooniverse project object
+    Safely remove a table from a Sql db
 
-    :param project: the project you want to connect to
-    :return: A Zooniverse project object.
+    :param conn: the Connection object
+    :param table_name: table of interest
     """
-    # Save your Zooniverse user name and password.
-    zoo_user, zoo_pass = zoo_credentials()
+    # Creating a cursor object using the cursor() method
+    cursor = conn.cursor()
+
+    try:
+        cursor.execute(f"DELETE FROM {table_name}")
+    except Exception as e:
+        logging.info(f"Table doesn't exist, {e}")
+        return
+    logging.debug(f"Previous content from the {table_name} table have been cleared.")
 
-    # Get the project-specific zooniverse number
-    project_n = project.Zooniverse_number
+    # Commit your changes in the database
+    conn.commit()
 
-    # Connect to the Zooniverse project
-    project = auth_session(zoo_user, zoo_pass, project_n)
 
-    logging.info("Connected to Zooniverse")
+def insert_many(conn: sqlite3.Connection, data: list, table: str, count: int):
+    """
+    Insert multiple rows into table
 
-    return project
+    :param conn: the Connection object
+    :param data: data to be inserted into table
+    :param table: table of interest
+    :param count: number of fields
+    :return:
+    """
 
+    values = (1,) * count
+    values = str(values).replace("1", "?")
 
-# Function to authenticate to Zooniverse
-def auth_session(username: str, password: str, project_n: int):
+    cur = conn.cursor()
+    cur.executemany(f"INSERT INTO {table} VALUES {values}", data)
+
+
+def retrieve_query(conn: sqlite3.Connection, query: str):
     """
-    It connects to the Zooniverse with your username and password, and then returns the project number
-    you specify
+    Execute SQL query and returns output
 
-    :param username: Your Zooniverse username
-    :param password: your Zooniverse password
-    :param project_n: The project number of the project you want to download data from
-    :return: The project number of the koster lab
+    :param conn: the Connection object
+    :param query: a SQL query
+    :return:
     """
+    try:
+        cur = conn.cursor()
+        cur.execute(query)
+    except sqlite3.Error as e:
+        logging.error(e)
+
+    rows = cur.fetchall()
 
-    # Connect to Zooniverse with your username and password
-    auth = Panoptes.connect(username=username, password=password)
+    return rows
 
-    if not auth.logged_in:
-        raise AuthenticationError("Your credentials are invalid. Please try again.")
 
-    # Specify the project number of the koster lab
+def execute_sql(conn: sqlite3.Connection, sql: str):
+    """Execute multiple SQL statements without return
+
+    :param conn: Connection object
+    :param sql: a string of SQL statements
+    :return:
+    """
     try:
-        project = Project(int(float(project_n)))
-        return project
-    except Exception as e:
+        c = conn.cursor()
+        c.executescript(sql)
+    except sqlite3.Error as e:
         logging.error(e)
 
 
-# Function to retrieve information from Zooniverse
-def retrieve_zoo_info(
-    project: project_utils.Project,
-    zoo_project: Project,
-    zoo_info: str,
-    generate_export: bool = False,
+def add_to_table(
+    conn: sqlite3.Connection, table_name: str, values: list, num_fields: int
 ):
     """
-    This function retrieves the information of interest from Zooniverse and saves it as a pandas data
-    frame
+    This function adds multiple rows of data to a specified table in a SQLite database.
 
-    :param project: the project object
-    :param zoo_project: the Zooniverse project object
-    :param zoo_info: a list of the info you want to retrieve from Zooniverse
-    :type zoo_info: str
-    :param generate_export: boolean determining whether to generate a new export and wait for it to be ready or to just download the latest export
-    :return: A dictionary of dataframes.
-    """
-    if hasattr(project, "info_df"):
-        if project.info_df is not None:
-            logging.info(
-                "Zooniverse info retrieved from cache, to force retrieval set project.info_df = None"
-            )
-            return project.info_df
+    :param conn: SQL connection object
+    :param table_name: The name of the table in the database where the values will be added
+    :type table_name: str
+    :param values: The `values` parameter is a list of tuples, where each tuple represents a row of data
+    to be inserted into the specified table. The number of values in each tuple should match the
+    `num_fields` parameter, which specifies the number of columns in the table
+    :type values: list
+    :param num_fields: The parameter `num_fields` is an integer that represents the number of fields or
+    columns in the table where the values will be inserted. This parameter is used to ensure that the
+    correct number of values are being inserted into the table
+    :type num_fields: int
+    """
 
-    # Create an empty dictionary to host the dfs of interest
-    info_df = {}
+    try:
+        insert_many(
+            conn,
+            values,
+            table_name,
+            num_fields,
+        )
+    except sqlite3.Error as e:
+        logging.error(e)
 
-    for info_n in zoo_info:
-        logging.info(f"Retrieving {info_n} from Zooniverse")
+    conn.commit()
 
-        # Get the information of interest from Zooniverse
-        if generate_export:
-            try:
-                export = zoo_project.get_export(
-                    info_n, generate=generate_export, wait=True, wait_timeout=1800
-                )
-            except panoptes.PanoptesAPIException:
-                logging.error(
-                    "Export generation time out, retrieving the last available information..."
-                )
-                export = zoo_project.get_export(info_n, generate=False)
-        else:
-            export = zoo_project.get_export(info_n, generate=generate_export)
+    logging.info(f"Updated {table_name} table from the temporary database")
 
-        # Save the info as pandas data frame
-        try:
-            export_df = pd.read_csv(io.StringIO(export.content.decode("utf-8")))
-        except pd.errors.ParserError:
-            logging.error(
-                "Export retrieval time out, please try again in 1 minute or so."
-            )
-            export_df = {}
 
-        if len(export_df) > 0:
-            # If KSO deal with duplicated subjects
-            if project.Project_name == "Koster_Seafloor_Obs":
-                # Clear duplicated subjects
-                if info_n == "subjects":
-                    export_df = clean_duplicated_subjects(export_df, project)
-
-                # Combine classifications from duplicated subjects to unique subject id
-                if info_n == "classifications":
-                    export_df = combine_annot_from_duplicates(export_df, project)
+def test_table(df: pd.DataFrame, table_name: str, keys: list = ["id"]):
+    """
+    The function checks if a given DataFrame has any NULL values in the specified key columns and logs
+    an error message if it does.
 
-        else:
-            raise ValueError(
-                "The export is empty. This may be due to a "
-                "request time out, please try again in 1 minute."
-            )
+    :param df: A pandas DataFrame that represents a table in a database
+    :type df: pd.DataFrame
+    :param table_name: The name of the table being tested, which is a string
+    :type table_name: str
+    :param keys: The `keys` parameter is a list of column names that are used as keys to uniquely
+    identify each row in the DataFrame `df`. The function `test_table` checks that there are no NULL
+    values in these key columns, which would indicate that some rows were not properly matched
+    :type keys: list
+    """
+    try:
+        # check that there are no id columns with a NULL value, which means that they were not matched
+        assert len(df[df[keys].isnull().any(axis=1)]) == 0
+    except AssertionError:
+        logging.error(
+            f"The table {table_name} has invalid entries, please ensure that all columns are non-zero"
+        )
+        logging.error(f"The invalid entries are {df[df[keys].isnull().any(axis=1)]}")
+
+
+def get_df_from_db_table(conn: sqlite3.Connection, table_name: str):
+    """
+    This function connects to a specific table from the sql database
+    and returns it as a pd DataFrame.
+
+    :param conn: SQL connection object
+    :param table_name: The name of the table you want to get from the database
+    :return: A dataframe
+    """
+
+    if conn is not None:
+        cursor = conn.cursor()
+    else:
+        return
+    # Get column names
+    cursor.execute(f"SELECT * FROM {table_name}")
+    rows = cursor.fetchall()
 
-        # Ensure subject_ids match db format
-        if info_n == "classifications":
-            export_df["subject_ids"] = export_df["subject_ids"].astype(np.int64)
+    # Get column names
+    cursor.execute(f"PRAGMA table_info('{table_name}')")
+    columns = [col[1] for col in cursor.fetchall()]
 
-        # Add df to dictionary
-        info_df[info_n] = export_df
-        project.info_df = info_df
-        logging.info(f"{info_n} retrieved successfully")
+    # Create a DataFrame from the data
+    df = pd.DataFrame(rows, columns=columns)
 
-    return info_df
+    return df
 
 
-# Function to extract metadata from subjects
-def extract_metadata(subj_df: pd.DataFrame):
+def get_schema_table_names(conn: sqlite3.Connection):
     """
-    > The function takes a dataframe with a column called `metadata` that contains a JSON string. It
-    then flattens the JSON string into a dataframe and returns the original dataframe with the
-    `metadata` column removed and the flattened dataframe
+    > This function retrieves a list with table names of the sql db
 
-    :param subj_df: The dataframe containing the subject data
-    :return: A tuple of two dataframes.
+    :param conn: SQL connection object
     """
 
-    # Reset index of df
-    subj_df = subj_df.reset_index(drop=True).reset_index()
+    cursor = conn.cursor()
+    cursor.execute("SELECT name FROM sqlite_master WHERE type='table'")
+    tables = cursor.fetchall()
+    table_names = [table[0] for table in tables]
 
-    # Flatten the metadata information
-    meta_df = pd.json_normalize(subj_df.metadata.apply(json.loads))
+    return table_names
 
-    # Drop metadata and index columns from original df
-    subj_df = subj_df.drop(
-        columns=[
-            "metadata",
-            "index",
-        ]
-    )
 
-    return subj_df, meta_df
+def get_column_names_db(conn: sqlite3.Connection, table_i: str):
+    """
+    > This function returns the "column" names of the sql table of interest
+
+    :param conn: SQL connection object
+    :param table_i: a string of the name of the table of interest
+    :return: A list of column names of the table of interest
+    """
+
+    # Get the data of the table of interest
+    data = conn.execute(f"SELECT * FROM {table_i}")
+
+    # Save in a dictionary the column names of the table
+    field_names = {}
+    for i in data.description:
+        field_names[i[0]] = i[0]
+
+    return field_names
 
 
-def populate_subjects(
-    subjects: pd.DataFrame, project: project_utils.Project, db_path: str
+def cols_rename_to_schema(
+    project: Project,
+    table_name: str,
+    df: pd.DataFrame,
+    reverse_lookup: bool = False,
 ):
     """
-    Populate the subjects table with the subject metadata
+    > This function renames columns of a df (of one of the three intial project csv files)
+    to match the names used in the schema. This deals with csv files having different
+    project-specific column names
+
+    :param project: The project object
+    :param df: a dataframe with the information of the local csv
+    :param table_name: The name of the table in the database where the data is stored
+    :param reverse_lookup: a boolean value to reverse the dict if formatting from schema to csv
+    """
+
+    # Get the spyfish-specific column names and their correspondent
+    # schema fields
+    if project.Project_name in ["Spyfish_Aotearoa", "Spyfish_BOPRC"]:
+        from kso_utils.spyfish_utils import get_spyfish_col_names
+
+        col_names_lookup = get_spyfish_col_names(table_name)
+
+    # Get the koster-specific column names and their correspondent
+    # schema fields
+    if project.Project_name == "Koster_Seafloor_Obs":
+        from kso_utils.koster_utils import get_koster_col_names
+
+        col_names_lookup = get_koster_col_names(table_name)
+
+    # Rename project-specific columns using the dictionary
+    if "col_names_lookup" in locals():
+        if reverse_lookup:
+            # Reverse the dictionaries if formatting from schema to csv
+            col_names_lookup = dict(
+                zip(col_names_lookup.values(), col_names_lookup.keys())
+            )
 
-    :param subjects: the subjects dataframe
-    :param project_path: The path to the projects.csv file
-    :param project_name: The name of the Zooniverse project
-    :param db_path: the path to the database
-    """
+        df = df.rename(columns=col_names_lookup)
 
-    project_name = project.Project_name
-    server = project.server
-    movie_folder = project.movie_folder
+    return df
 
-    # Check if the Zooniverse project is the KSO
-    if project_name == "Koster_Seafloor_Obs":
-        subjects = process_koster_subjects(subjects, db_path)
 
-    else:
-        # Extract metadata from uploaded subjects
-        subjects_df, subjects_meta = extract_metadata(subjects)
+# Utility functions for common database operations
+def create_db(db_path: str):
+    """Create a new database for the project
 
-        # Combine metadata info with the subjects df
-        subjects = pd.concat([subjects_df, subjects_meta], axis=1)
+    :param db_path: path of the database file
+    :return:
+    """
+    db_file = Path(db_path)
 
-        # Check if the Zooniverse project is the Spyfish
-        if project_name == "Spyfish_Aotearoa":
-            subjects = process_spyfish_subjects(subjects, db_path)
+    # Delete previous database versions if exists
+    if db_file.exists():
+        db_file.unlink()
 
-        # If project is not KSO or Spyfish standardise subject info
-        else:
-            # Create columns to match schema if they don't exist
-            subjects["frame_exp_sp_id"] = subjects.get("frame_exp_sp_id", np.nan)
-            subjects["frame_number"] = subjects.get("frame_number", np.nan)
-
-            # Select only relevant metadata columns
-            subjects = subjects[
-                [
-                    "subject_id",
-                    "project_id",
-                    "workflow_id",
-                    "subject_set_id",
-                    "locations",
-                    "movie_id",
-                    "frame_number",
-                    "frame_exp_sp_id",
-                    "upl_seconds",
-                    "Subject_type",
-                    "subject_type",
-                    "#VideoFilename",
-                    "#clip_length",
-                    "classifications_count",
-                    "retired_at",
-                    "retirement_reason",
-                    "created_at",
-                ]
-            ]
-
-            # Fix weird bug where Subject_type is used instead of subject_type for the column name for some clips
-            if "Subject_type" in subjects.columns:
-                subjects["subject_type"] = subjects[
-                    ["subject_type", "Subject_type"]
-                ].apply(lambda x: x[1] if isinstance(x[1], str) else x[0], 1)
-                subjects.drop(columns=["Subject_type"], inplace=True)
-
-            # Rename columns to match the db format
-            subjects = subjects.rename(
-                columns={
-                    "#VideoFilename": "filename",
-                    "upl_seconds": "clip_start_time",
-                    "#frame_number": "frame_number",
-                }
-            )
+    # Get sql command for db setup
+    sql_setup = schema.sql
 
-            # Remove clip subjects with no clip_start_time info (from different projects)
-            subjects = subjects[
-                ~(
-                    (subjects["subject_type"] == "clip")
-                    & (subjects["clip_start_time"].isna())
-                )
-            ]
-
-            # Calculate the clip_end_time
-            subjects["clip_end_time"] = (
-                subjects["clip_start_time"] + subjects["#clip_length"]
-            )
+    # create a database connection
+    conn = create_connection(str(db_file))
+
+    # create tables
+    if conn is not None:
+        # execute sql
+        execute_sql(conn, sql_setup)
+        return "Database creation success"
+    else:
+        return "Database creation failure"
 
-    # Set subject_id information as id
-    subjects = subjects.rename(columns={"subject_id": "id"})
 
-    # Extract the html location of the subjects
-    subjects["https_location"] = subjects["locations"].apply(
-        lambda x: literal_eval(x)["0"]
-    )
+def populate_db(
+    conn: sqlite3.Connection, project: Project, local_df: pd.DataFrame, init_key=str
+):
+    """
+    > This function processes and tests the initial csv files compatibility with sql db
+    and populates the table of interest
+
+    :param conn: SQL connection object
+    :param project: The project object
+    :param local_df: a dataframe with the information of the local csv to populate from
+    :param init_key: a string of the initial key of the local csv and the name of the db table to populate
+    """
 
-    # Set movie_id column to None if no movies are linked to the subject
-    if movie_folder == "None" and server in ["LOCAL", "SNIC"]:
-        subjects["movie_id"] = None
-
-    # Fix subjects where clip_start_time is not provided but upl_seconds is
-    if "clip_start_time" in subjects.columns and "upl_seconds" in subjects.columns:
-        subjects["clip_start_time"] = subjects[
-            ["clip_start_time", "upl_seconds"]
-        ].apply(lambda x: x[0] if not np.isnan(x[0]) else x[1], 1)
-
-    # Set the columns in the right order
-    subjects = subjects[
-        [
-            "id",
-            "subject_type",
-            "filename",
-            "clip_start_time",
-            "clip_end_time",
-            "frame_exp_sp_id",
-            "frame_number",
-            "workflow_id",
-            "subject_set_id",
-            "classifications_count",
-            "retired_at",
-            "retirement_reason",
-            "created_at",
-            "https_location",
-            "movie_id",
-        ]
-    ]
-
-    # Ensure that subject_ids are not duplicated by workflow
-    subjects = subjects.drop_duplicates(subset="id")
-
-    # Test table validity
-    db_utils.test_table(subjects, "subjects", keys=["id"])
-
-    # Add values to subjects
-    db_utils.add_to_table(db_path, "subjects", [tuple(i) for i in subjects.values], 15)
-
-    ##### Print how many subjects are in the db
-    # Create connection to db
-    conn = db_utils.create_connection(db_path)
-
-    # Query id and subject type from the subjects table
-    subjects_df = pd.read_sql_query("SELECT id, subject_type FROM subjects", conn)
-    frame_subjs = subjects_df[subjects_df["subject_type"] == "frame"].shape[0]
-    clip_subjs = subjects_df[subjects_df["subject_type"] == "clip"].shape[0]
-
-    logging.info(
-        f"The database has a total of "
-        f"{frame_subjs}"
-        f" frame subjects and "
-        f"{clip_subjs}"
-        f" clip subjects"
+    # Process the csv of interest and tests for compatibility with sql table
+    local_df = process_test_csv(
+        conn=conn,
+        project=project,
+        local_df=local_df,
+        init_key=init_key,
     )
 
+    # Only populate the tables if df is not empty
+    if not local_df.empty:
+        # Add values of the processed csv to the sql table of interest
+        add_to_table(
+            conn=conn,
+            table_name=init_key,
+            values=[tuple(i) for i in local_df.values],
+            num_fields=len(local_df.columns),
+        )
+
 
-# Relevant for ML and upload frames tutorials
-def populate_agg_annotations(
-    annotations: pd.DataFrame, subj_type: str, project: project_utils.Project
+def process_test_csv(
+    conn: sqlite3.Connection, project: Project, local_df: pd.DataFrame, init_key=str
 ):
     """
-    It takes in a list of annotations, the subject type, and the project, and adds the annotations to
-    the database
+    > This function process a csv of interest and tests for compatibility with the
+    respective sql table of interest
 
-    :param annotations: a dataframe containing the annotations
-    :param subj_type: "clip" or "frame"
-    :param project: the project object
-    """
-
-    # Get the project-specific name of the database
-    db_path = project.db_path
-
-    conn = db_utils.create_connection(db_path)
-
-    # Query id and subject type from the subjects table
-    subjects_df = pd.read_sql_query("SELECT id, frame_exp_sp_id FROM subjects", conn)
-
-    # Combine annotation and subject information
-    annotations_df = pd.merge(
-        annotations,
-        subjects_df,
-        how="left",
-        left_on="subject_ids",
-        right_on="id",
-        validate="many_to_one",
+    :param conn: SQL connection object
+    :param project: The project object
+    :param local_df: a dataframe with the information of the local csv to populate from
+    :param init_key: a string corresponding to the name of the initial key of the local csv
+    :return: a string of the category of interest and the processed dataframe
+    """
+
+    # Rename potential project-specific column names to "standard" schema names
+    local_df = cols_rename_to_schema(
+        project=project,
+        table_name=init_key,
+        df=local_df,
     )
 
-    # Update agg_annotations_clip table
-    if subj_type == "clip":
-        # Set the columns in the right order
-        species_df = pd.read_sql_query(
-            "SELECT id as species_id, label FROM species", conn
-        )
-        species_df["label"] = species_df["label"].apply(
-            lambda x: x.replace(" ", "").replace(")", "").replace("(", "").upper()
-        )
+    # Set the id of the df of interest
+    if init_key == "sites":
+        table_id = "site_id"
 
-        # Combine annotation and subject information
-        annotations_df = pd.merge(annotations_df, species_df, how="left", on="label")
+    elif init_key == "movies":
+        table_id = "movie_id"
 
-        annotations_df = annotations_df[
-            ["species_id", "how_many", "first_seen", "subject_ids"]
-        ]
-        annotations_df["species_id"] = annotations_df["species_id"].apply(
-            lambda x: int(x) if not np.isnan(x) else x
-        )
+        from kso_utils.movie_utils import select_project_movies
 
-        # Test table validity
-        db_utils.test_table(
-            annotations_df, "agg_annotations_clip", keys=["subject_ids"]
-        )
+        # Select only the movies that are relevant to the project
+        local_df = select_project_movies(project, local_df)
 
-        # Add annotations to the agg_annotations_clip table
-        db_utils.add_to_table(
-            db_path,
-            "agg_annotations_clip",
-            [(None,) + tuple(i) for i in annotations_df.values],
-            5,
+        # Reference movies with their respective sites
+        sites_df = get_df_from_db_table(conn, "sites")[["id", "siteName"]].rename(
+            columns={"id": "site_id"}
         )
 
-    # Update agg_annotations_frame table
-    if subj_type == "frame":
-        # Select relevant columns
-        annotations_df = annotations_df[["label", "x", "y", "w", "h", "subject_ids"]]
-
-        # Set the columns in the right order
-        species_df = pd.read_sql_query(
-            "SELECT id as species_id, label FROM species", conn
-        )
-        species_df["label"] = species_df["label"].apply(
-            lambda x: x[:-1] if x == "Blue mussels" else x
+        # Merge df (aka movies) and sites dfs
+        local_df = pd.merge(local_df, sites_df, how="left", on="siteName")
+
+    elif init_key == "species":
+        table_id = "species_id"
+
+    elif init_key == "photos":
+        table_id = "ID"
+
+    else:
+        logging.error(
+            f"{init_key} has not been processed because the db schema does not have a table for it"
         )
 
-        # Combine annotation and subject information
-        annotations_df = pd.merge(annotations_df, species_df, how="left", on="label")
+    # Create a dictionary with the table-specific column id and its schema match
+    id_lookup = {table_id: "id"}
 
-        annotations_df = annotations_df[
-            ["species_id", "x", "y", "w", "h", "subject_ids"]
-        ].dropna()
+    # Rename id columns using the dictionary
+    local_df = local_df.rename(columns=id_lookup)
 
-        # Test table validity
+    # Roadblock to ensure cols match schema
+    ##################
+    # Get the "standard" schema column names of the table of interest
+    col_names_dic = get_column_names_db(conn, init_key)
 
-        db_utils.test_table(
-            annotations_df, "agg_annotations_frame", keys=["species_id"]
-        )
+    # Check the column names of the df are standard
+    column_names = local_df.columns
+    required_columns = col_names_dic.values()
 
-        # Add values to agg_annotations_frame
-        db_utils.add_to_table(
-            db_path,
-            "agg_annotations_frame",
-            [(None,) + tuple(i) for i in annotations_df.values],
-            7,
+    # Modify the dictionary if the df has different column names
+    if not all(col in column_names for col in required_columns):
+        missing_cols = [col for col in required_columns if col not in column_names]
+        # Log the issue
+        logging.error(
+            f"{missing_cols} column(s) not found and"
+            f" are required for the {init_key}'s schema table"
+            f" The col names are:{column_names}"
         )
 
+    # Select only columns that have fields in the sql table
+    local_df = local_df[[c for c in required_columns if c in local_df.columns]]
+
+    # Roadblock to prevent empty rows in id_columns
+    test_table(local_df, init_key, [local_df.columns[0]])
+
+    return local_df
+
 
-def process_clips_template(annotations, row_class_id, rows_list: list):
+def check_species_meta(csv_paths: dict, conn: sqlite3.Connection):
     """
-    For each annotation, if the task is T0, then for each species annotated, flatten the relevant
-    answers and save the species of choice, class and subject id.
+    > The function `check_species_meta` loads the csv with species information and checks if it is empty
 
-    :param annotations: the list of annotations for a given subject
-    :param row_class_id: the classification id
-    :param rows_list: a list of dictionaries, each dictionary is a row in the output dataframe
-    :return: A list of dictionaries, each dictionary containing the classification id, the label, the
-    first seen time and the number of individuals.
-    """
-
-    for ann_i in annotations:
-        if ann_i["task"] == "T0":
-            # Select each species annotated and flatten the relevant answers
-            for value_i in ann_i["value"]:
-                choice_i = {}
-                # If choice = 'nothing here', set follow-up answers to blank
-                if value_i["choice"] == "NOTHINGHERE":
-                    f_time = ""
-                    inds = ""
-                # If choice = species, flatten follow-up answers
-                else:
-                    answers = value_i["answers"]
-                    for k in answers.keys():
-                        if "EARLIESTPOINT" in k:
-                            f_time = answers[k].replace("S", "")
-                        if "HOWMANY" in k:
-                            inds = answers[k]
-                            # Deal with +20 fish options
-                            if inds == "2030":
-                                inds = "25"
-                            if inds == "3040":
-                                inds = "35"
-                        elif "EARLIESTPOINT" not in k and "HOWMANY" not in k:
-                            f_time, inds = None, None
-
-                # Save the species of choice, class and subject id
-                choice_i.update(
-                    {
-                        "classification_id": row_class_id,
-                        "label": value_i["choice"],
-                        "first_seen": f_time,
-                        "how_many": inds,
-                    }
-                )
-
-                rows_list.append(choice_i)
-
-    return rows_list
-
-
-def retrieve__populate_zoo_info(
-    project: project_utils.Project,
-    db_info_dict: dict,
-    zoo_project: Project,
-    zoo_info: list,
-    generate_export: bool = False,
-):
+    :param csv_paths: a dictionary with the paths of the csv files with info to initiate the db
+    :param conn: SQL connection object
     """
-    It retrieves the information of the subjects uploaded to Zooniverse and populates the SQL database
-    with the information
 
-    :param project: the project you want to retrieve information for
-    :param db_info_dict: a dictionary containing the path to the database and the name of the database
-    :param zoo_project: The name of the Zooniverse project you created
-    :param zoo_info: a list containing the information of the Zooniverse project you would like to retrieve
-    :param generate_export: boolean determining whether to generate a new export and wait for it to be ready or to just download the latest export
+    # Load the csv with movies information
+    species_df = pd.read_csv(csv_paths["local_species_csv"])
+
+    # Retrieve the names of the basic columns in the sql db
+    field_names = list(get_column_names_db(conn, "species").values())
+
+    # Select the basic fields for the db check
+    df_to_db = species_df[[c for c in species_df.columns if c in field_names]]
+
+    # Roadblock to prevent empty lat/long/datum/countrycode
+    test_table(df_to_db, "species", df_to_db.columns)
 
-    :return: The zoo_info_dict is being returned.
+    logging.info("The species dataframe is complete")
+
+
+def add_db_info_to_df(
+    project: Project,
+    conn: sqlite3.Connection,
+    csv_paths: dict,
+    df: pd.DataFrame,
+    table_name: str,
+    cols_interest: str = "*",
+):
     """
+    > This function retrieves information from a sql table and adds it to
+    the df
+
+    :param project: The project object
+    :param conn: SQL connection object
+    :param csv_paths: a dictionary with the paths of the csv files with info to initiate the db
+    :param df: a dataframe with the information of the local csv to populate from
+    :param table_name: The name of the table in the database where the data is stored
+    :param cols_interest: list,
+    """
+    # Retrieve the sql as a df
+    query = f"SELECT {cols_interest} FROM {table_name}"
+    sql_df = pd.read_sql_query(query, conn)
+
+    # Set the column to merge dfs on right to "id" as default
+    right_on_col = "id"
+
+    # Set movies table
+    if table_name == "movies":
+        # Add survey information as part of the movie info
+        if "local_surveys_csv" in csv_paths.keys():
+            from kso_utils.spyfish_utils import add_spyfish_survey_info
+
+            sql_df = add_spyfish_survey_info(sql_df, csv_paths)
+
+        # Save the name of the column to merge dfs on
+        left_on_col = "movie_id"
+
+    # Set subjects table
+    elif table_name == "subjects":
+        # Save the name of the columns to merge dfs on
+        left_on_col = "subject_ids"
+
+    # Set sites table
+    elif table_name == "sites":
+        # Save the name of the columns to merge dfs on
+        left_on_col = "site_id"
+
+    # Set species table
+    elif table_name == "species":
+        # Save the name of the columns to merge dfs on
+        left_on_col = "commonName"
+        right_on_col = "commonName"
+
+        if "label" in df.columns:
+            df[right_on_col] = df["label"]
+
+        from kso_utils.zooniverse_utils import clean_label
+
+        # Match format of species name to Zooniverse labels
+        sql_df[right_on_col] = sql_df[right_on_col].apply(clean_label)
+        df[left_on_col] = df[left_on_col].apply(clean_label)
 
-    if zoo_project is None:
-        logging.error(
-            "This project is not linked to a Zooniverse project. Please create one and add the required fields to proceed with this tutorial."
-        )
     else:
-        # Retrieve and store the information of subjects uploaded to zooniverse
-        zoo_info_dict = retrieve_zoo_info(
-            project, zoo_project, zoo_info, generate_export
+        logging.error(
+            f"The table_name specified ({table_name}) doesn't have a merging option"
         )
 
-        # Populate the sql with subjects uploaded to Zooniverse
-        if "db_path" in db_info_dict:
-            populate_subjects(
-                zoo_info_dict["subjects"], project, db_info_dict["db_path"]
+    # Ensure id columns that are going to be used to merge are int
+    if "id" in left_on_col:
+        # Ensure there are no NaN values found in the column id column
+        if df[left_on_col].isna().any() or (df[left_on_col] == "None").any():
+            logging.error(
+                f"Error: NaN values found in the {left_on_col} column of {table_name}."
             )
+
         else:
-            logging.info("No database path found. Subjects have not been added to db")
-        return zoo_info_dict
+            df[left_on_col] = df[left_on_col].astype(float).astype(int)
+
+    # Combine the original and sqldf dfs
+    comb_df = pd.merge(
+        df, sql_df, how="left", left_on=left_on_col, right_on=right_on_col
+    )
+
+    # Check for rows with NaN values in the merged DataFrame
+    missing_values = comb_df[right_on_col].isnull()
+
+    # If there are missing values, raise an issue
+    if missing_values.any():
+        # Log a warning or raise an exception with relevant information
+        logging.error(
+            f"Some rows in df do not have corresponding values in sql_df. Rows with missing values are: {comb_df[missing_values]}"
+        )
+
+    # Drop the id column to prevent duplicated column issues
+    comb_df = comb_df.drop(columns=["id"], errors="ignore")
+
+    return comb_df
+
+
+# Function to match species selected to species id
+def get_species_ids(conn: sqlite3.Connection, species_list: list):
+    """
+    # Get ids of species of interest
+    """
+    if len(species_list) == 1:
+        species_ids = pd.read_sql_query(
+            f'SELECT id FROM species WHERE commonName=="{species_list[0]}"', conn
+        )["id"].tolist()
+    else:
+        species_ids = pd.read_sql_query(
+            f"SELECT id FROM species WHERE commonName IN {tuple(species_list)}", conn
+        )["id"].tolist()
+
+    return species_ids
```

