# Comparing `tmp/inference_schema-1.7-py3-none-any.whl.zip` & `tmp/inference_schema-1.7.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 21238 bytes, number of entries: 18
+Zip file size: 21282 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat      183 b- defN 22-Feb-04 18:09 inference_schema/__init__.py
 -rw-rw-rw-  2.0 fat      307 b- defN 22-Oct-28 16:24 inference_schema/_constants.py
--rw-rw-rw-  2.0 fat    12748 b- defN 23-Aug-28 21:08 inference_schema/schema_decorators.py
+-rw-rw-rw-  2.0 fat    12776 b- defN 23-Dec-29 20:35 inference_schema/schema_decorators.py
 -rw-rw-rw-  2.0 fat     4189 b- defN 22-Oct-28 16:24 inference_schema/schema_util.py
 -rw-rw-rw-  2.0 fat      421 b- defN 22-Feb-04 18:09 inference_schema/parameter_types/__init__.py
 -rw-rw-rw-  2.0 fat      642 b- defN 22-Feb-04 18:09 inference_schema/parameter_types/_constants.py
 -rw-rw-rw-  2.0 fat     4001 b- defN 22-Feb-04 18:09 inference_schema/parameter_types/_swagger_from_dtype.py
 -rw-rw-rw-  2.0 fat     4446 b- defN 22-Oct-28 16:24 inference_schema/parameter_types/_util.py
 -rw-rw-rw-  2.0 fat     5229 b- defN 22-Apr-14 14:38 inference_schema/parameter_types/abstract_parameter_type.py
 -rw-rw-rw-  2.0 fat     6953 b- defN 22-Feb-04 18:09 inference_schema/parameter_types/numpy_parameter_type.py
 -rw-rw-rw-  2.0 fat     9372 b- defN 23-Jul-21 21:43 inference_schema/parameter_types/pandas_parameter_type.py
 -rw-rw-rw-  2.0 fat     9647 b- defN 22-Feb-04 18:09 inference_schema/parameter_types/spark_parameter_type.py
 -rw-rw-rw-  2.0 fat     3456 b- defN 22-Mar-28 20:14 inference_schema/parameter_types/standard_py_parameter_type.py
--rw-rw-rw-  2.0 fat     1183 b- defN 23-Aug-28 21:08 inference_schema-1.7.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     2398 b- defN 23-Aug-28 21:08 inference_schema-1.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-28 21:08 inference_schema-1.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Aug-28 21:08 inference_schema-1.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1765 b- defN 23-Aug-28 21:08 inference_schema-1.7.dist-info/RECORD
-18 files, 67049 bytes uncompressed, 18248 bytes compressed:  72.8%
+-rw-rw-rw-  2.0 fat     1183 b- defN 23-Dec-29 20:36 inference_schema-1.7.1.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     2451 b- defN 23-Dec-29 20:36 inference_schema-1.7.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Dec-29 20:36 inference_schema-1.7.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Dec-29 20:36 inference_schema-1.7.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1775 b- defN 23-Dec-29 20:36 inference_schema-1.7.1.dist-info/RECORD
+18 files, 67140 bytes uncompressed, 18272 bytes compressed:  72.8%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: inference_schema/parameter_types/spark_parameter_type.py
 Comment: 
 
 Filename: inference_schema/parameter_types/standard_py_parameter_type.py
 Comment: 
 
-Filename: inference_schema-1.7.dist-info/LICENSE.txt
+Filename: inference_schema-1.7.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: inference_schema-1.7.dist-info/METADATA
+Filename: inference_schema-1.7.1.dist-info/METADATA
 Comment: 
 
-Filename: inference_schema-1.7.dist-info/WHEEL
+Filename: inference_schema-1.7.1.dist-info/WHEEL
 Comment: 
 
-Filename: inference_schema-1.7.dist-info/top_level.txt
+Filename: inference_schema-1.7.1.dist-info/top_level.txt
 Comment: 
 
-Filename: inference_schema-1.7.dist-info/RECORD
+Filename: inference_schema-1.7.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inference_schema/schema_decorators.py

```diff
@@ -50,15 +50,15 @@
                 decorators = _get_decorators(user_run)
                 arg_names = inspect.getfullargspec(decorators[-1]).args
                 if param_name not in arg_names:
                     raise Exception('Error, provided param_name "{}" '
                                     'is not in the decorated function.'.format(param_name))
                 param_position = arg_names.index(param_name)
                 args[param_position] = _deserialize_input_argument(args[param_position], param_type, param_name)
-            elif param_name not in kwargs.keys() and optional:
+            elif optional and (param_name not in kwargs.keys() or not kwargs[param_name]):
                 pass
             else:
                 kwargs[param_name] = _deserialize_input_argument(kwargs[param_name], param_type, param_name)
 
             args = tuple(args)
 
         return user_run(*args, **kwargs)
```

## Comparing `inference_schema-1.7.dist-info/LICENSE.txt` & `inference_schema-1.7.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `inference_schema-1.7.dist-info/METADATA` & `inference_schema-1.7.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inference-schema
-Version: 1.7
+Version: 1.7.1
 Summary: This package is intended to provide a uniform schema for common machine learning applications, as well as a set of decorators that can be used to aid in web based ML prediction applications.
 Author: Microsoft Corp
 License: MIT License        
             Copyright (c) Microsoft Corporation. All rights reserved.        
             Permission is hereby granted, free of charge, to any person obtaining a copy
             of this software and associated documentation files (the "Software"), to deal
             in the Software without restriction, including without limitation the rights
@@ -23,19 +23,20 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7,<3.11
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8,<3.12
 License-File: LICENSE.txt
 Requires-Dist: python-dateutil (>=2.5.3)
 Requires-Dist: pytz (>=2017.2)
-Requires-Dist: wrapt (<=1.12.1,>=1.11.1)
+Requires-Dist: wrapt (<=1.16.0,>=1.14.0)
 Provides-Extra: numpy-support
 Requires-Dist: numpy (>=1.13.0) ; extra == 'numpy-support'
 Provides-Extra: pandas-support
 Requires-Dist: pandas (>=0.20.2) ; extra == 'pandas-support'
 Provides-Extra: pyspark-support
 Requires-Dist: pyspark (>=2.3.2) ; extra == 'pyspark-support'
```

## Comparing `inference_schema-1.7.dist-info/RECORD` & `inference_schema-1.7.1.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 inference_schema/__init__.py,sha256=JlCCObuOLZyNhIZlsoL51KtFxiY4xKIIzIRDBcdeu6Y,183
 inference_schema/_constants.py,sha256=oyCqVS9IFFLmBZQ5pggUdPm1pmBHY35uYNpeOCKz_jw,307
-inference_schema/schema_decorators.py,sha256=e_fpPUU1dS6fSc13A7HIRHeIwLAFZZ3BB1kM41jYu6A,12748
+inference_schema/schema_decorators.py,sha256=VOCis5WX7un5CQnMRqXE8kpoL5KlUEyY_zG5ALZf6XM,12776
 inference_schema/schema_util.py,sha256=bWp6OSbeRcpmLWx1pmV8DD68ZPTOhoct1YUhx1eMf0M,4189
 inference_schema/parameter_types/__init__.py,sha256=ZZqhUutuAxCsQyDODYilPdx1miZx02jNdWmHVPhJt2k,421
 inference_schema/parameter_types/_constants.py,sha256=qnr_V7yT5xZJNNtt8_EqN1FfLyTqMUvJPJnbHo1_qt0,642
 inference_schema/parameter_types/_swagger_from_dtype.py,sha256=WWYVGo6-KiGoPg0CMmM3RBa_WTtbS33lTV9PS-dQ5T0,4001
 inference_schema/parameter_types/_util.py,sha256=vXKbnsTbVBpxrhBXpIHycKxYzBl1PE04dtWtQLY6G6M,4446
 inference_schema/parameter_types/abstract_parameter_type.py,sha256=qkdLkYgXlIHFA-NxGOTkYmG6FK-qdFgPenn9HMJrTzo,5229
 inference_schema/parameter_types/numpy_parameter_type.py,sha256=goBx3Vzti-9jlKvMPn55t4SS5FF416-tq-ZGEpAjb_Q,6953
 inference_schema/parameter_types/pandas_parameter_type.py,sha256=wPYgg7IlbJq6VAQB6wRQ_fj2Wvxfpu3RcJ9gpmMVjh4,9372
 inference_schema/parameter_types/spark_parameter_type.py,sha256=vVmYWZFRSNCReouZiS1cGoR30NGu5OJlPyvQ_flgY2g,9647
 inference_schema/parameter_types/standard_py_parameter_type.py,sha256=DO5Ty02A0D5zjt4ODodxw6WeOA7r2QyfK-NswN9yOzI,3456
-inference_schema-1.7.dist-info/LICENSE.txt,sha256=3qkmU0GCkALiwjpzcjk-su1uJghftiPzikugr4M_MKY,1183
-inference_schema-1.7.dist-info/METADATA,sha256=Eof_jpxfxUkS5KhTIwL-IGb3FSgWm6J_t3ic6bVDGno,2398
-inference_schema-1.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-inference_schema-1.7.dist-info/top_level.txt,sha256=VppQqI390J43UCHv4CcDtEGPp8EktkSEi5Q80wWYq9M,17
-inference_schema-1.7.dist-info/RECORD,,
+inference_schema-1.7.1.dist-info/LICENSE.txt,sha256=3qkmU0GCkALiwjpzcjk-su1uJghftiPzikugr4M_MKY,1183
+inference_schema-1.7.1.dist-info/METADATA,sha256=xeSs2JMLlY-zVxIA0c9Xm3swzZs8sZkbG_jVQmqtoiM,2451
+inference_schema-1.7.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+inference_schema-1.7.1.dist-info/top_level.txt,sha256=VppQqI390J43UCHv4CcDtEGPp8EktkSEi5Q80wWYq9M,17
+inference_schema-1.7.1.dist-info/RECORD,,
```

