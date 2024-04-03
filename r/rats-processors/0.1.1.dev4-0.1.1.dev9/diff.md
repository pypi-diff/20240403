# Comparing `tmp/rats_processors-0.1.1.dev4-py3-none-any.whl.zip` & `tmp/rats_processors-0.1.1.dev9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -62,12 +62,12 @@
 -rw-r--r--  2.0 unx     1570 b- defN 80-Jan-01 00:00 rats/processors/ux/_declash.py
 -rw-r--r--  2.0 unx     3585 b- defN 80-Jan-01 00:00 rats/processors/ux/_omegaconf.py
 -rw-r--r--  2.0 unx     9924 b- defN 80-Jan-01 00:00 rats/processors/ux/_ops.py
 -rw-r--r--  2.0 unx    15092 b- defN 80-Jan-01 00:00 rats/processors/ux/_pipeline.py
 -rw-r--r--  2.0 unx     5070 b- defN 80-Jan-01 00:00 rats/processors/ux/_session.py
 -rw-r--r--  2.0 unx     2805 b- defN 80-Jan-01 00:00 rats/processors/ux/_utils.py
 -rw-r--r--  2.0 unx     4794 b- defN 80-Jan-01 00:00 rats/processors/ux/_verification.py
--rw-r--r--  2.0 unx      906 b- defN 80-Jan-01 00:00 rats_processors-0.1.1.dev4.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 rats_processors-0.1.1.dev4.dist-info/WHEEL
--rw-r--r--  2.0 unx       87 b- defN 80-Jan-01 00:00 rats_processors-0.1.1.dev4.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     6773 b- defN 16-Jan-01 00:00 rats_processors-0.1.1.dev4.dist-info/RECORD
+-rw-r--r--  2.0 unx      906 b- defN 80-Jan-01 00:00 rats_processors-0.1.1.dev9.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 rats_processors-0.1.1.dev9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       87 b- defN 80-Jan-01 00:00 rats_processors-0.1.1.dev9.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     6773 b- defN 16-Jan-01 00:00 rats_processors-0.1.1.dev9.dist-info/RECORD
 71 files, 259053 bytes uncompressed, 67511 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -195,20 +195,20 @@
 
 Filename: rats/processors/ux/_utils.py
 Comment: 
 
 Filename: rats/processors/ux/_verification.py
 Comment: 
 
-Filename: rats_processors-0.1.1.dev4.dist-info/METADATA
+Filename: rats_processors-0.1.1.dev9.dist-info/METADATA
 Comment: 
 
-Filename: rats_processors-0.1.1.dev4.dist-info/WHEEL
+Filename: rats_processors-0.1.1.dev9.dist-info/WHEEL
 Comment: 
 
-Filename: rats_processors-0.1.1.dev4.dist-info/entry_points.txt
+Filename: rats_processors-0.1.1.dev9.dist-info/entry_points.txt
 Comment: 
 
-Filename: rats_processors-0.1.1.dev4.dist-info/RECORD
+Filename: rats_processors-0.1.1.dev9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `rats_processors-0.1.1.dev4.dist-info/METADATA` & `rats_processors-0.1.1.dev9.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rats-processors
-Version: 0.1.1.dev4
+Version: 0.1.1.dev9
 Summary: Rats Processors
 Home-page: https://github.com/microsoft/rats/
 License: MIT
 Keywords: pipelines,machine learning,research
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `rats_processors-0.1.1.dev4.dist-info/RECORD` & `rats_processors-0.1.1.dev9.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -61,11 +61,11 @@
 rats/processors/ux/_declash.py,sha256=aWMC1rAB8jV2992Uj3n6j76och8uzi-d6Bl-ITD_mGk,1570
 rats/processors/ux/_omegaconf.py,sha256=e3EzhRfnyj68FPLfHBu9vP_8fMIPA67g3SdpYHGtzrY,3585
 rats/processors/ux/_ops.py,sha256=lfZkSt9GJzIgPO8u00ncRAQ8KHQ7LM2EJj-mVYeQzpc,9924
 rats/processors/ux/_pipeline.py,sha256=m43u0m4GdJUfN-1q3-0pE4wBzbBTr0kUsLF0exhaufg,15092
 rats/processors/ux/_session.py,sha256=EsKhN9qw8j4Vivf8onAy37KMkU2g_8UtXPR60FchkvA,5070
 rats/processors/ux/_utils.py,sha256=6PbFczI6Qb7S-2z2gQi9Uqrje12UNm8fYMjBJ8bYLfU,2805
 rats/processors/ux/_verification.py,sha256=LRMert_Il_KEKF3MKnPkXO6da_SQfo2kJxgORbyylZ8,4794
-rats_processors-0.1.1.dev4.dist-info/METADATA,sha256=oguTLCkiMj66LC2YiNFP5XSKeXLMCOqrfaYAbWXU9-k,906
-rats_processors-0.1.1.dev4.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-rats_processors-0.1.1.dev4.dist-info/entry_points.txt,sha256=ZtyQNxiYP_NZNcvQlVHyGrIY5KI6AnqoQtO88_aYQmI,87
-rats_processors-0.1.1.dev4.dist-info/RECORD,,
+rats_processors-0.1.1.dev9.dist-info/METADATA,sha256=q2GFmRH7G5Uj_jZUWSWzm579QFFELOwGAJQfQN9K2Bc,906
+rats_processors-0.1.1.dev9.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+rats_processors-0.1.1.dev9.dist-info/entry_points.txt,sha256=ZtyQNxiYP_NZNcvQlVHyGrIY5KI6AnqoQtO88_aYQmI,87
+rats_processors-0.1.1.dev9.dist-info/RECORD,,
```

