# Comparing `tmp/revolve2_experimentation-1.0.2-py3-none-any.whl.zip` & `tmp/revolve2_experimentation-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,23 @@
-Zip file size: 18447 bytes, number of entries: 29
+Zip file size: 23089 bytes, number of entries: 37
 -rw-r--r--  2.0 unx       38 b- defN 80-Jan-01 00:00 revolve2/experimentation/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 revolve2/experimentation/_util/__init__.py
 -rw-r--r--  2.0 unx     1068 b- defN 80-Jan-01 00:00 revolve2/experimentation/_util/init_subclass_get_generic_args.py
 -rw-r--r--  2.0 unx      295 b- defN 80-Jan-01 00:00 revolve2/experimentation/database/__init__.py
 -rw-r--r--  2.0 unx      296 b- defN 80-Jan-01 00:00 revolve2/experimentation/database/_has_id.py
 -rw-r--r--  2.0 unx      235 b- defN 80-Jan-01 00:00 revolve2/experimentation/database/_open_method.py
 -rw-r--r--  2.0 unx     1930 b- defN 80-Jan-01 00:00 revolve2/experimentation/database/_sqlite.py
+-rw-r--r--  2.0 unx      150 b- defN 80-Jan-01 00:00 revolve2/experimentation/evolution/__init__.py
+-rw-r--r--  2.0 unx     2576 b- defN 80-Jan-01 00:00 revolve2/experimentation/evolution/_modular_robot_evolution.py
+-rw-r--r--  2.0 unx      310 b- defN 80-Jan-01 00:00 revolve2/experimentation/evolution/abstract_elements/__init__.py
+-rw-r--r--  2.0 unx      552 b- defN 80-Jan-01 00:00 revolve2/experimentation/evolution/abstract_elements/_evaluator.py
+-rw-r--r--  2.0 unx      614 b- defN 80-Jan-01 00:00 revolve2/experimentation/evolution/abstract_elements/_evolution.py
+-rw-r--r--  2.0 unx      637 b- defN 80-Jan-01 00:00 revolve2/experimentation/evolution/abstract_elements/_learner.py
+-rw-r--r--  2.0 unx      576 b- defN 80-Jan-01 00:00 revolve2/experimentation/evolution/abstract_elements/_reproducer.py
+-rw-r--r--  2.0 unx      696 b- defN 80-Jan-01 00:00 revolve2/experimentation/evolution/abstract_elements/_selector.py
 -rw-r--r--  2.0 unx     1245 b- defN 80-Jan-01 00:00 revolve2/experimentation/logging.py
 -rw-r--r--  2.0 unx       85 b- defN 80-Jan-01 00:00 revolve2/experimentation/optimization/__init__.py
 -rw-r--r--  2.0 unx      266 b- defN 80-Jan-01 00:00 revolve2/experimentation/optimization/ea/__init__.py
 -rw-r--r--  2.0 unx     3102 b- defN 80-Jan-01 00:00 revolve2/experimentation/optimization/ea/_generation.py
 -rw-r--r--  2.0 unx     4309 b- defN 80-Jan-01 00:00 revolve2/experimentation/optimization/ea/_individual.py
 -rw-r--r--  2.0 unx     1145 b- defN 80-Jan-01 00:00 revolve2/experimentation/optimization/ea/_parameters.py
 -rw-r--r--  2.0 unx     2344 b- defN 80-Jan-01 00:00 revolve2/experimentation/optimization/ea/_population.py
@@ -21,11 +29,11 @@
 -rw-r--r--  2.0 unx     1352 b- defN 80-Jan-01 00:00 revolve2/experimentation/optimization/ea/selection/_multiple_unique.py
 -rw-r--r--  2.0 unx     2642 b- defN 80-Jan-01 00:00 revolve2/experimentation/optimization/ea/selection/_pareto_frontier.py
 -rw-r--r--  2.0 unx      389 b- defN 80-Jan-01 00:00 revolve2/experimentation/optimization/ea/selection/_supports_lt.py
 -rw-r--r--  2.0 unx      694 b- defN 80-Jan-01 00:00 revolve2/experimentation/optimization/ea/selection/_topn.py
 -rw-r--r--  2.0 unx      707 b- defN 80-Jan-01 00:00 revolve2/experimentation/optimization/ea/selection/_tournament.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 revolve2/experimentation/py.typed
 -rw-r--r--  2.0 unx     1357 b- defN 80-Jan-01 00:00 revolve2/experimentation/rng.py
--rw-r--r--  2.0 unx     3119 b- defN 80-Jan-01 00:00 revolve2_experimentation-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 revolve2_experimentation-1.0.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx     3149 b- defN 16-Jan-01 00:00 revolve2_experimentation-1.0.2.dist-info/RECORD
-29 files, 33980 bytes uncompressed, 13077 bytes compressed:  61.5%
+-rw-r--r--  2.0 unx     3137 b- defN 80-Jan-01 00:00 revolve2_experimentation-1.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 revolve2_experimentation-1.1.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     4098 b- defN 16-Jan-01 00:00 revolve2_experimentation-1.1.1.dist-info/RECORD
+37 files, 41058 bytes uncompressed, 16111 bytes compressed:  60.8%
```

## zipnote {}

```diff
@@ -15,14 +15,38 @@
 
 Filename: revolve2/experimentation/database/_open_method.py
 Comment: 
 
 Filename: revolve2/experimentation/database/_sqlite.py
 Comment: 
 
+Filename: revolve2/experimentation/evolution/__init__.py
+Comment: 
+
+Filename: revolve2/experimentation/evolution/_modular_robot_evolution.py
+Comment: 
+
+Filename: revolve2/experimentation/evolution/abstract_elements/__init__.py
+Comment: 
+
+Filename: revolve2/experimentation/evolution/abstract_elements/_evaluator.py
+Comment: 
+
+Filename: revolve2/experimentation/evolution/abstract_elements/_evolution.py
+Comment: 
+
+Filename: revolve2/experimentation/evolution/abstract_elements/_learner.py
+Comment: 
+
+Filename: revolve2/experimentation/evolution/abstract_elements/_reproducer.py
+Comment: 
+
+Filename: revolve2/experimentation/evolution/abstract_elements/_selector.py
+Comment: 
+
 Filename: revolve2/experimentation/logging.py
 Comment: 
 
 Filename: revolve2/experimentation/optimization/__init__.py
 Comment: 
 
 Filename: revolve2/experimentation/optimization/ea/__init__.py
@@ -72,17 +96,17 @@
 
 Filename: revolve2/experimentation/py.typed
 Comment: 
 
 Filename: revolve2/experimentation/rng.py
 Comment: 
 
-Filename: revolve2_experimentation-1.0.2.dist-info/METADATA
+Filename: revolve2_experimentation-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: revolve2_experimentation-1.0.2.dist-info/WHEEL
+Filename: revolve2_experimentation-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: revolve2_experimentation-1.0.2.dist-info/RECORD
+Filename: revolve2_experimentation-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `revolve2_experimentation-1.0.2.dist-info/METADATA` & `revolve2_experimentation-1.1.1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: revolve2-experimentation
-Version: 1.0.2
+Version: 1.1.1
 Summary: Revolve2: Tools for experimentation.
 Home-page: https://github.com/ci-group/revolve2
 Author: Aart Stuurman
 Author-email: aartstuurman@hotmail.com
 Requires-Python: >=3.10,<3.12
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Provides-Extra: dev
 Requires-Dist: numpy (>=1.21.2,<2.0.0)
 Requires-Dist: sqlalchemy (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/ci-group/revolve2
 Description-Content-Type: text/markdown
 
-<img  align="right" width="150" height="150"  src="./docs/source/logo.png">
+<img align="right" width="150" height="150"  src="./docs/source/logo_light.png">
 
 # Revolve2
 
 Revolve2 is a collection of Python packages used for researching evolutionary algorithms and modular robotics.
 Its primary features are a modular robot framework, an abstraction layer around physics simulators, and evolutionary algorithms.
 
 **Documentation: [ci-group.github.io/revolve2](https://ci-group.github.io/revolve2)**
```

## Comparing `revolve2_experimentation-1.0.2.dist-info/RECORD` & `revolve2_experimentation-1.1.1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 revolve2/experimentation/__init__.py,sha256=fsaE15zGl4-G_qaVsMuEnEHC2hHXtTlRQRA9uSmoxcE,38
 revolve2/experimentation/_util/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 revolve2/experimentation/_util/init_subclass_get_generic_args.py,sha256=iCtpnbxz09UoiahUcGKOye-UNk7GlTu7SBgYqG-rtlo,1068
 revolve2/experimentation/database/__init__.py,sha256=R4fyarPysmfzBXBeApYVWBHSnon7CBq9-YLICd7pUqc,295
 revolve2/experimentation/database/_has_id.py,sha256=XKNxoZpx_6NAl4TfrAZwLjPhC3B21uLw2s7ot5yerUs,296
 revolve2/experimentation/database/_open_method.py,sha256=55oVAd4oxofkQtFVwKeRboajNyipNXki7mFMfdiRAYE,235
 revolve2/experimentation/database/_sqlite.py,sha256=F_q76i2heNuiOQ8GOvYkwVyPF1dmtOZFf8aijfQ_jhg,1930
+revolve2/experimentation/evolution/__init__.py,sha256=Iefj3fSoymkYtUSIJ65VTtSv2OfgmfFtw0eJP0bTbaU,150
+revolve2/experimentation/evolution/_modular_robot_evolution.py,sha256=y44HOQJy4jAnUv8KYDHD3LQBZqDpi31AWWr4R-7gXjM,2576
+revolve2/experimentation/evolution/abstract_elements/__init__.py,sha256=gJ1aTcYWsUgv9fgdu8ffwRDtgVsLof4orC-BTseTMH0,310
+revolve2/experimentation/evolution/abstract_elements/_evaluator.py,sha256=TupKDd2wU4JghfbKVKnV0tO062VcAgL5gHzHqlQYpUU,552
+revolve2/experimentation/evolution/abstract_elements/_evolution.py,sha256=xEJyMqAeTAqC8uzHmSZDaiQS5OBZ1zdHw_2lwSL7hb4,614
+revolve2/experimentation/evolution/abstract_elements/_learner.py,sha256=I8BvofG-enFge7WU6lQpz5tZVbgBWpii30Ee0q7spr4,637
+revolve2/experimentation/evolution/abstract_elements/_reproducer.py,sha256=10o_FEX3wiLM0KS3BZmIJ4jq5OXPSmTFG9-I6G0jOsk,576
+revolve2/experimentation/evolution/abstract_elements/_selector.py,sha256=pS9AwCZwPRqMpPhzwKLAJm8ostEfd_Qgiv_KwkMQAP8,696
 revolve2/experimentation/logging.py,sha256=3RgLCeQABKqQ9XpyXJY2IC3FR61yHtv3mr2klA-lU2E,1245
 revolve2/experimentation/optimization/__init__.py,sha256=b17HbcltS-dYHCECYF8UFVNm6n2wQG1pqu3METKgAE0,85
 revolve2/experimentation/optimization/ea/__init__.py,sha256=nx-s0wX_pAJfe736LQh0ebTXGj1f3hcnoN9B1lvfRec,266
 revolve2/experimentation/optimization/ea/_generation.py,sha256=-TbLMsTIAKSttyAiLHHCGiVqBcuv9QV9OZQGhwonv_M,3102
 revolve2/experimentation/optimization/ea/_individual.py,sha256=u1IqLIKYpyEF0n-R3ADAJajjdJ3j5KZppdJDuyTRjCE,4309
 revolve2/experimentation/optimization/ea/_parameters.py,sha256=IE2N4RmhGacchVcDrgl3_fQvNApS5tJPlDMYws0tAOU,1145
 revolve2/experimentation/optimization/ea/_population.py,sha256=ESwi04lhY1EW9sh_PFvhEch1-bON_AjmsecEy5MB6eU,2344
@@ -20,10 +28,10 @@
 revolve2/experimentation/optimization/ea/selection/_multiple_unique.py,sha256=b4BHnpdD6iVUQBbyVgGBWdVNqSAqVTQCh9RnO4GACN8,1352
 revolve2/experimentation/optimization/ea/selection/_pareto_frontier.py,sha256=5PvijjQQw9-zBdxZ5kyRybRPmMPlLcgux-WTHQZUSv4,2642
 revolve2/experimentation/optimization/ea/selection/_supports_lt.py,sha256=5zGObYyZzZ4M2n28wUgRXRvuBuvYzRmxqQzbIISQzJ4,389
 revolve2/experimentation/optimization/ea/selection/_topn.py,sha256=u7gkqYhfU0-Mshf9l9XD55glptboDSewpOnnETIcWnU,694
 revolve2/experimentation/optimization/ea/selection/_tournament.py,sha256=CRsaCfnyNzciJlD6hCI9W6atIbGKXhf-OYKvSXPAS1s,707
 revolve2/experimentation/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 revolve2/experimentation/rng.py,sha256=QmJBcevRmgq2TvpjJtyzej39eylPR9P490j0bugLtrw,1357
-revolve2_experimentation-1.0.2.dist-info/METADATA,sha256=fKc_i5LL88EZb4etC2xg5RfeICEpJJPhRuQfUpWC-8o,3119
-revolve2_experimentation-1.0.2.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-revolve2_experimentation-1.0.2.dist-info/RECORD,,
+revolve2_experimentation-1.1.1.dist-info/METADATA,sha256=zPI3vFKRh5wc0J_Op9GmmB7HKGlVMnkdtCuLf4XUuYw,3137
+revolve2_experimentation-1.1.1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+revolve2_experimentation-1.1.1.dist-info/RECORD,,
```

