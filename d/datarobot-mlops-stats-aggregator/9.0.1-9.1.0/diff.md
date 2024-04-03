# Comparing `tmp/datarobot_mlops_stats_aggregator-9.0.1-py2.py3-none-any.whl.zip` & `tmp/datarobot_mlops_stats_aggregator-9.1.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 17011 bytes, number of entries: 11
--rw-r--r--  2.0 unx      812 b- defN 23-Jun-09 20:57 datarobot/mlops/stats_aggregator/__init__.py
--rw-r--r--  2.0 unx    15046 b- defN 23-Jun-09 20:57 datarobot/mlops/stats_aggregator/aggregation.py
--rw-r--r--  2.0 unx      888 b- defN 23-Jun-09 20:57 datarobot/mlops/stats_aggregator/constants.py
--rw-r--r--  2.0 unx     6528 b- defN 23-Jun-09 20:57 datarobot/mlops/stats_aggregator/histogram.py
--rw-r--r--  2.0 unx    12097 b- defN 23-Jun-09 20:57 datarobot/mlops/stats_aggregator/merging.py
--rw-r--r--  2.0 unx     9370 b- defN 23-Jun-09 20:57 datarobot/mlops/stats_aggregator/type_conversion.py
--rw-r--r--  2.0 unx     2982 b- defN 23-Jun-09 20:57 datarobot/mlops/stats_aggregator/types.py
--rw-r--r--  2.0 unx     2201 b- defN 23-Jun-09 20:58 datarobot_mlops_stats_aggregator-9.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-09 20:58 datarobot_mlops_stats_aggregator-9.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-09 20:58 datarobot_mlops_stats_aggregator-9.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1114 b- defN 23-Jun-09 20:58 datarobot_mlops_stats_aggregator-9.0.1.dist-info/RECORD
-11 files, 51158 bytes uncompressed, 15065 bytes compressed:  70.6%
+Zip file size: 17031 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      812 b- defN 23-Jun-27 20:23 datarobot/mlops/stats_aggregator/__init__.py
+-rw-r--r--  2.0 unx    15101 b- defN 23-Jun-27 20:23 datarobot/mlops/stats_aggregator/aggregation.py
+-rw-r--r--  2.0 unx      888 b- defN 23-Jun-27 20:23 datarobot/mlops/stats_aggregator/constants.py
+-rw-r--r--  2.0 unx     6528 b- defN 23-Jun-27 20:23 datarobot/mlops/stats_aggregator/histogram.py
+-rw-r--r--  2.0 unx    12097 b- defN 23-Jun-27 20:23 datarobot/mlops/stats_aggregator/merging.py
+-rw-r--r--  2.0 unx     9370 b- defN 23-Jun-27 20:23 datarobot/mlops/stats_aggregator/type_conversion.py
+-rw-r--r--  2.0 unx     2982 b- defN 23-Jun-27 20:23 datarobot/mlops/stats_aggregator/types.py
+-rw-r--r--  2.0 unx     2201 b- defN 23-Jun-27 20:25 datarobot_mlops_stats_aggregator-9.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-27 20:25 datarobot_mlops_stats_aggregator-9.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-27 20:25 datarobot_mlops_stats_aggregator-9.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1114 b- defN 23-Jun-27 20:25 datarobot_mlops_stats_aggregator-9.1.0.dist-info/RECORD
+11 files, 51213 bytes uncompressed, 15085 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: datarobot/mlops/stats_aggregator/type_conversion.py
 Comment: 
 
 Filename: datarobot/mlops/stats_aggregator/types.py
 Comment: 
 
-Filename: datarobot_mlops_stats_aggregator-9.0.1.dist-info/METADATA
+Filename: datarobot_mlops_stats_aggregator-9.1.0.dist-info/METADATA
 Comment: 
 
-Filename: datarobot_mlops_stats_aggregator-9.0.1.dist-info/WHEEL
+Filename: datarobot_mlops_stats_aggregator-9.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: datarobot_mlops_stats_aggregator-9.0.1.dist-info/top_level.txt
+Filename: datarobot_mlops_stats_aggregator-9.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: datarobot_mlops_stats_aggregator-9.0.1.dist-info/RECORD
+Filename: datarobot_mlops_stats_aggregator-9.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datarobot/mlops/stats_aggregator/__init__.py

```diff
@@ -1,10 +1,10 @@
 #  --------------------------------------------------------------------------------
 #  Copyright (c) 2021 DataRobot, Inc. and its affiliates. All rights reserved.
-#  Last updated 2022.
+#  Last updated 2023.
 #
 #  DataRobot, Inc. Confidential.
 #  This is proprietary source code of DataRobot, Inc. and its affiliates.
 #
 #  This file and its contents are subject to DataRobot Tool and Utility Agreement.
 #  For details, see
 #  https://www.datarobot.com/wp-content/uploads/2021/07/DataRobot-Tool-and-Utility-Agreement.pdf.
@@ -14,8 +14,8 @@
 from __future__ import absolute_import
 
 from .aggregation import aggregate_stats
 from .merging import merge_stats
 from .types import FeatureType
 
 __all__ = ["aggregate_stats", "merge_stats", "FeatureType"]
-__version__ = '9.0.1'
+__version__ = '9.1.0'
```

## datarobot/mlops/stats_aggregator/aggregation.py

```diff
@@ -1,10 +1,10 @@
 #  --------------------------------------------------------------------------------
 #  Copyright (c) 2021 DataRobot, Inc. and its affiliates. All rights reserved.
-#  Last updated 2022.
+#  Last updated 2023.
 #
 #  DataRobot, Inc. Confidential.
 #  This is proprietary source code of DataRobot, Inc. and its affiliates.
 #
 #  This file and its contents are subject to DataRobot Tool and Utility Agreement.
 #  For details, see
 #  https://www.datarobot.com/wp-content/uploads/2021/07/DataRobot-Tool-and-Utility-Agreement.pdf.
@@ -147,15 +147,20 @@
 
 def aggregate_text_stats(series, feature_type, distinct_category_count):
     # type: (pd.Series, str, Optional[int]) -> CategoricalAggregate
     """Aggregate a text (words or characters) feature into statistics"""
     value_count, missing_count = compute_counts(series)
 
     # Remove numbers from the text (Port behavior of remove_numbers_from_text)
-    series = series.fillna("").astype(six.text_type).str.replace(digit_pattern, "").str.lower()
+    series = (
+        series.fillna("")
+        .astype(six.text_type)
+        .str.replace(digit_pattern, "", regex=True)
+        .str.lower()
+    )
 
     # Split each document into words or characters, depending on feature type
     # Original implementation is keyed off of language: If logographic, tokenize by characters.
     # Rather than passing in an extra map of languages, I chose to just split the feature type.
     pattern = word_pattern if feature_type == FeatureType.TEXT_WORDS else char_pattern
     series = series.str.findall(pattern)
```

## Comparing `datarobot_mlops_stats_aggregator-9.0.1.dist-info/METADATA` & `datarobot_mlops_stats_aggregator-9.1.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot-mlops-stats-aggregator
-Version: 9.0.1
+Version: 9.1.0
 Summary: datarobot-mlops-stats-aggregator library to compute statistics aggregations
 Home-page: http://datarobot.com
 Author: DataRobot
 Author-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `datarobot_mlops_stats_aggregator-9.0.1.dist-info/RECORD` & `datarobot_mlops_stats_aggregator-9.1.0.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-datarobot/mlops/stats_aggregator/__init__.py,sha256=khSs_eRhD2_Q2jiczwWsVbMqqcJMLltncA_uZ7ZlfPY,812
-datarobot/mlops/stats_aggregator/aggregation.py,sha256=X5am7_M0vqqX3ZmnkPjhv286FW7U2Z1FRu701dXIKGc,15046
+datarobot/mlops/stats_aggregator/__init__.py,sha256=v-YCzQ8Msh2ueRyhSfMz8kBxvxnPdoJYa9uDJLAsVNk,812
+datarobot/mlops/stats_aggregator/aggregation.py,sha256=BjBiVoGq1FMT3PRVd_PqXv-qMhUiWJ4tDpAPwMzjAN0,15101
 datarobot/mlops/stats_aggregator/constants.py,sha256=e-pqtDD2dlXXTfcUYz4AL5GgkrMrOP3XChklh9iRB8g,888
 datarobot/mlops/stats_aggregator/histogram.py,sha256=KtA0hwIyT9wG-3LjFYnixqBlFMgywWjuhrXPgxIopwE,6528
 datarobot/mlops/stats_aggregator/merging.py,sha256=wr-2MZunpk-iR4UTsNX1ivEieZbkadNOhMU4YT7oWQw,12097
 datarobot/mlops/stats_aggregator/type_conversion.py,sha256=9qBpD8zV_Hx3ZDX80h_DPnsYr0kzy0dYJ7O2iiWKNUA,9370
 datarobot/mlops/stats_aggregator/types.py,sha256=zdCg-5lDIH2MhbgRFt-Mlt6wvnm9oPGJngydJOlPSy8,2982
-datarobot_mlops_stats_aggregator-9.0.1.dist-info/METADATA,sha256=HvtGk7AwBugZP23HD3ih0qRvlWVaVUOew_YshstCobw,2201
-datarobot_mlops_stats_aggregator-9.0.1.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-datarobot_mlops_stats_aggregator-9.0.1.dist-info/top_level.txt,sha256=RTK5ZHErXe7mZUlXWQRjQpqFdWw3qmpF95Lz7ViL2Lc,10
-datarobot_mlops_stats_aggregator-9.0.1.dist-info/RECORD,,
+datarobot_mlops_stats_aggregator-9.1.0.dist-info/METADATA,sha256=9qyX1NccjcwBbCL_pO0bSmROJkYCpDkunYN3EOHcCpg,2201
+datarobot_mlops_stats_aggregator-9.1.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+datarobot_mlops_stats_aggregator-9.1.0.dist-info/top_level.txt,sha256=RTK5ZHErXe7mZUlXWQRjQpqFdWw3qmpF95Lz7ViL2Lc,10
+datarobot_mlops_stats_aggregator-9.1.0.dist-info/RECORD,,
```

