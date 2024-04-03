# Comparing `tmp/cat_merge-0.2.0.tar.gz` & `tmp/cat_merge-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cat_merge-0.2.0.tar", max compression
+gzip compressed data, was "cat_merge-0.2.1.tar", max compression
```

## Comparing `cat_merge-0.2.0.tar` & `cat_merge-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        0 2023-09-26 18:25:54.185326 cat_merge-0.2.0/cat_merge/__init__.py
--rw-r--r--   0        0        0     1220 2023-09-26 18:25:54.185326 cat_merge-0.2.0/cat_merge/cli.py
--rw-r--r--   0        0        0     8647 2023-09-26 18:25:54.185326 cat_merge-0.2.0/cat_merge/file_utils.py
--rw-r--r--   0        0        0     1414 2023-09-26 18:25:54.185326 cat_merge-0.2.0/cat_merge/mapping_utils.py
--rw-r--r--   0        0        0     3268 2023-09-26 18:25:54.185326 cat_merge-0.2.0/cat_merge/merge.py
--rw-r--r--   0        0        0     3419 2023-09-26 18:25:54.185326 cat_merge-0.2.0/cat_merge/merge_utils.py
--rw-r--r--   0        0        0        0 2023-09-26 18:25:54.185326 cat_merge-0.2.0/cat_merge/model/__init__.py
--rw-r--r--   0        0        0      488 2023-09-26 18:25:54.185326 cat_merge-0.2.0/cat_merge/model/merged_kg.py
--rw-r--r--   0        0        0     2050 2023-09-26 18:25:54.185326 cat_merge-0.2.0/cat_merge/qc.py
--rw-r--r--   0        0        0    11135 2023-09-26 18:25:54.185326 cat_merge-0.2.0/cat_merge/qc_diff_utils.py
--rw-r--r--   0        0        0     2920 2023-09-26 18:25:54.185326 cat_merge-0.2.0/cat_merge/qc_stats.py
--rw-r--r--   0        0        0    15355 2023-09-26 18:25:54.185326 cat_merge-0.2.0/cat_merge/qc_utils.py
--rw-r--r--   0        0        0      659 2023-09-26 18:25:54.185326 cat_merge-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      454 1970-01-01 00:00:00.000000 cat_merge-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-03 19:51:15.417942 cat_merge-0.2.1/cat_merge/__init__.py
+-rw-r--r--   0        0        0     1220 2024-04-03 19:51:15.417942 cat_merge-0.2.1/cat_merge/cli.py
+-rw-r--r--   0        0        0     8833 2024-04-03 19:51:15.417942 cat_merge-0.2.1/cat_merge/file_utils.py
+-rw-r--r--   0        0        0     1414 2024-04-03 19:51:15.417942 cat_merge-0.2.1/cat_merge/mapping_utils.py
+-rw-r--r--   0        0        0     3268 2024-04-03 19:51:15.417942 cat_merge-0.2.1/cat_merge/merge.py
+-rw-r--r--   0        0        0     3448 2024-04-03 19:51:15.417942 cat_merge-0.2.1/cat_merge/merge_utils.py
+-rw-r--r--   0        0        0        0 2024-04-03 19:51:15.417942 cat_merge-0.2.1/cat_merge/model/__init__.py
+-rw-r--r--   0        0        0      488 2024-04-03 19:51:15.417942 cat_merge-0.2.1/cat_merge/model/merged_kg.py
+-rw-r--r--   0        0        0     2050 2024-04-03 19:51:15.417942 cat_merge-0.2.1/cat_merge/qc.py
+-rw-r--r--   0        0        0    11135 2024-04-03 19:51:15.417942 cat_merge-0.2.1/cat_merge/qc_diff_utils.py
+-rw-r--r--   0        0        0     2920 2024-04-03 19:51:15.417942 cat_merge-0.2.1/cat_merge/qc_stats.py
+-rw-r--r--   0        0        0    15355 2024-04-03 19:51:15.417942 cat_merge-0.2.1/cat_merge/qc_utils.py
+-rw-r--r--   0        0        0      659 2024-04-03 19:51:15.417942 cat_merge-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      505 1970-01-01 00:00:00.000000 cat_merge-0.2.1/PKG-INFO
```

### Comparing `cat_merge-0.2.0/cat_merge/cli.py` & `cat_merge-0.2.1/cat_merge/cli.py`

 * *Files identical despite different names*

### Comparing `cat_merge-0.2.0/cat_merge/file_utils.py` & `cat_merge-0.2.1/cat_merge/file_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,15 +80,22 @@
         add_source_col (str, optional): Name of column to add to the dataframe with the name of the file.
         source_col_value (Any, optional): Value to add to the source column.
         comment_character (str, optional): Character to ignore lines starting with, or anything after.
 
     Returns:
         pandas.DataFrame: Dataframe.
     """
-    df = pd.read_csv(fh, sep="\t", dtype="string", lineterminator="\n", quoting=csv.QUOTE_NONE, comment=comment_character)
+    df = pd.read_csv(fh,
+                     sep="\t",
+                     dtype="string",
+                     lineterminator="\n",
+                     quoting=csv.QUOTE_NONE,
+                     comment=comment_character,
+                     keep_default_na=False,
+                     na_values=[''])
     if add_source_col is not None:
         df[add_source_col] = source_col_value
     return df
 
 
 def write_df(df: pd.DataFrame, filename: str):
     """
```

### Comparing `cat_merge-0.2.0/cat_merge/mapping_utils.py` & `cat_merge-0.2.1/cat_merge/mapping_utils.py`

 * *Files identical despite different names*

### Comparing `cat_merge-0.2.0/cat_merge/merge.py` & `cat_merge-0.2.1/cat_merge/merge.py`

 * *Files identical despite different names*

### Comparing `cat_merge-0.2.0/cat_merge/merge_utils.py` & `cat_merge-0.2.1/cat_merge/merge_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     Clean nodes by dropping duplicates
 
     Args:
         nodes (pandas.DataFrame): Dataframe of nodes
     Returns:
         pandas.DataFrame: Dataframe of nodes with duplicates dropped
     """
-    nodes.drop_duplicates(inplace=True)
+    nodes.drop_duplicates(inplace=True, subset=['id'], keep='first')
     return nodes
 
 
 def clean_edges(edges: DataFrame, nodes: DataFrame) -> DataFrame:
     """
     Clean edges by dropping duplicate and dangling edges
```

### Comparing `cat_merge-0.2.0/cat_merge/qc.py` & `cat_merge-0.2.1/cat_merge/qc.py`

 * *Files identical despite different names*

### Comparing `cat_merge-0.2.0/cat_merge/qc_diff_utils.py` & `cat_merge-0.2.1/cat_merge/qc_diff_utils.py`

 * *Files identical despite different names*

### Comparing `cat_merge-0.2.0/cat_merge/qc_stats.py` & `cat_merge-0.2.1/cat_merge/qc_stats.py`

 * *Files identical despite different names*

### Comparing `cat_merge-0.2.0/cat_merge/qc_utils.py` & `cat_merge-0.2.1/cat_merge/qc_utils.py`

 * *Files identical despite different names*

### Comparing `cat_merge-0.2.0/pyproject.toml` & `cat_merge-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cat-merge"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = [
     "Monarch Initiative <info@monarchinitiative.org>",
     "Glass Elsarboukh <glass@tislab.org>",
     "Tim Putman <tim@tislab.org>",
     "Kevin Schaper <kevin@tislab.org>",
     "Victoria Soesanto <victoria@tislab.org",
```

