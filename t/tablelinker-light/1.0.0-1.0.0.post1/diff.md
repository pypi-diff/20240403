# Comparing `tmp/tablelinker_light-1.0.0.tar.gz` & `tmp/tablelinker_light-1.0.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablelinker_light-1.0.0.tar", max compression
+gzip compressed data, was "tablelinker_light-1.0.0.post1.tar", max compression
```

## Comparing `tablelinker_light-1.0.0.tar` & `tablelinker_light-1.0.0.post1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1095 2024-04-02 06:09:18.460912 tablelinker_light-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0     1697 2024-04-03 02:07:42.118076 tablelinker_light-1.0.0/README.md
--rw-r--r--   0        0        0     1599 2024-04-02 05:01:20.711727 tablelinker_light-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      548 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/__init__.py
--rw-r--r--   0        0        0      204 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/__main__.py
--rw-r--r--   0        0        0     8735 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/cli.py
--rw-r--r--   0        0        0     1003 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/convertors/basics/__init__.py
--rw-r--r--   0        0        0     6188 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/convertors/basics/calc_col.py
--rw-r--r--   0        0        0    11511 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/convertors/basics/concat_col.py
--rw-r--r--   0        0        0     8521 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/convertors/basics/concat_title.py
--rw-r--r--   0        0        0     5169 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/convertors/basics/delete_col.py
--rw-r--r--   0        0        0     8535 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/convertors/basics/delete_row.py
--rw-r--r--   0        0        0    10113 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/convertors/basics/generate_pk.py
--rw-r--r--   0        0        0    10139 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/convertors/basics/insert_col.py
--rw-r--r--   0        0        0     5628 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/convertors/basics/mapping_col.py
--rw-r--r--   0        0        0     4205 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/convertors/basics/move_col.py
--rw-r--r--   0        0        0     6054 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/convertors/basics/rename_col.py
--rw-r--r--   0        0        0     4081 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/convertors/basics/reorder_col.py
--rw-r--r--   0        0        0     4349 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/convertors/basics/round.py
--rw-r--r--   0        0        0     7894 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/convertors/basics/select_row.py
--rw-r--r--   0        0        0    10194 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/convertors/basics/split_col.py
--rw-r--r--   0        0        0     5302 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/convertors/basics/truncate.py
--rw-r--r--   0        0        0    13389 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/convertors/basics/update_col.py
--rw-r--r--   0        0        0    10385 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/convertors/basics/zenkaku.py
--rw-r--r--   0        0        0     1003 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/convertors/extras/__init__.py
--rw-r--r--   0        0        0    14364 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/convertors/extras/date_extract.py
--rw-r--r--   0        0        0    41601 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/convertors/extras/geocoder.py
--rw-r--r--   0        0        0     8168 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/convertors/extras/mapping_col.py
--rw-r--r--   0        0        0     9884 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/convertors/extras/wareki.py
--rw-r--r--   0        0        0      176 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/core/__init__.py
--rw-r--r--   0        0        0     4497 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/core/context.py
--rw-r--r--   0        0        0    25582 2024-04-02 06:44:38.766295 tablelinker_light-1.0.0/tablelinker/core/convertors.py
--rw-r--r--   0        0        0     6922 2024-04-02 04:49:06.714540 tablelinker_light-1.0.0/tablelinker/core/csv_cleaner.py
--rw-r--r--   0        0        0     4212 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/core/data_type.py
--rw-r--r--   0        0        0    27004 2024-04-02 05:01:34.252123 tablelinker_light-1.0.0/tablelinker/core/date_extractor.py
--rw-r--r--   0        0        0      951 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/core/fieldtypes.py
--rw-r--r--   0        0        0     8764 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/core/input.py
--rw-r--r--   0        0        0    15928 2024-04-02 03:39:36.502828 tablelinker_light-1.0.0/tablelinker/core/mapping.py
--rw-r--r--   0        0        0     2306 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/core/output.py
--rw-r--r--   0        0        0    13941 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/core/params.py
--rw-r--r--   0        0        0    36652 2024-04-02 04:23:53.712614 tablelinker_light-1.0.0/tablelinker/core/table.py
--rw-r--r--   0        0        0     8030 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/core/task.py
--rw-r--r--   0        0        0     3692 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0/tablelinker/core/validators.py
--rw-r--r--   0        0        0       52 2024-04-02 06:44:44.206363 tablelinker_light-1.0.0/tablelinker/exceptions.py
--rw-r--r--   0        0        0     3093 1970-01-01 00:00:00.000000 tablelinker_light-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-04-02 06:09:18.460912 tablelinker_light-1.0.0.post1/LICENSE.txt
+-rw-r--r--   0        0        0     1697 2024-04-03 02:07:42.118076 tablelinker_light-1.0.0.post1/README.md
+-rw-r--r--   0        0        0     1607 2024-04-03 05:13:46.250500 tablelinker_light-1.0.0.post1/pyproject.toml
+-rw-r--r--   0        0        0      554 2024-04-03 05:14:01.098762 tablelinker_light-1.0.0.post1/tablelinker/__init__.py
+-rw-r--r--   0        0        0      204 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/__main__.py
+-rw-r--r--   0        0        0     8735 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/cli.py
+-rw-r--r--   0        0        0     1003 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/__init__.py
+-rw-r--r--   0        0        0     6188 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/calc_col.py
+-rw-r--r--   0        0        0    11511 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/concat_col.py
+-rw-r--r--   0        0        0     8521 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/concat_title.py
+-rw-r--r--   0        0        0     5169 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/delete_col.py
+-rw-r--r--   0        0        0     8535 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/delete_row.py
+-rw-r--r--   0        0        0    10113 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/generate_pk.py
+-rw-r--r--   0        0        0    10139 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/insert_col.py
+-rw-r--r--   0        0        0     5628 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/mapping_col.py
+-rw-r--r--   0        0        0     4205 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/move_col.py
+-rw-r--r--   0        0        0     6054 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/rename_col.py
+-rw-r--r--   0        0        0     4081 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/reorder_col.py
+-rw-r--r--   0        0        0     4349 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/round.py
+-rw-r--r--   0        0        0     7894 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/select_row.py
+-rw-r--r--   0        0        0    10194 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/split_col.py
+-rw-r--r--   0        0        0     5302 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/truncate.py
+-rw-r--r--   0        0        0    13389 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/update_col.py
+-rw-r--r--   0        0        0    10385 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/zenkaku.py
+-rw-r--r--   0        0        0     1003 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/convertors/extras/__init__.py
+-rw-r--r--   0        0        0    14364 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/convertors/extras/date_extract.py
+-rw-r--r--   0        0        0    41601 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/convertors/extras/geocoder.py
+-rw-r--r--   0        0        0     8168 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/convertors/extras/mapping_col.py
+-rw-r--r--   0        0        0     9884 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/convertors/extras/wareki.py
+-rw-r--r--   0        0        0      176 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/core/__init__.py
+-rw-r--r--   0        0        0     4497 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/core/context.py
+-rw-r--r--   0        0        0    25582 2024-04-02 06:44:38.766295 tablelinker_light-1.0.0.post1/tablelinker/core/convertors.py
+-rw-r--r--   0        0        0     6922 2024-04-02 04:49:06.714540 tablelinker_light-1.0.0.post1/tablelinker/core/csv_cleaner.py
+-rw-r--r--   0        0        0     4212 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/core/data_type.py
+-rw-r--r--   0        0        0    27004 2024-04-02 05:01:34.252123 tablelinker_light-1.0.0.post1/tablelinker/core/date_extractor.py
+-rw-r--r--   0        0        0      951 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/core/fieldtypes.py
+-rw-r--r--   0        0        0     8764 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/core/input.py
+-rw-r--r--   0        0        0    15928 2024-04-02 03:39:36.502828 tablelinker_light-1.0.0.post1/tablelinker/core/mapping.py
+-rw-r--r--   0        0        0     2306 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/core/output.py
+-rw-r--r--   0        0        0    13941 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/core/params.py
+-rw-r--r--   0        0        0    36652 2024-04-02 04:23:53.712614 tablelinker_light-1.0.0.post1/tablelinker/core/table.py
+-rw-r--r--   0        0        0     8030 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/core/task.py
+-rw-r--r--   0        0        0     3692 2023-03-31 11:50:20.000000 tablelinker_light-1.0.0.post1/tablelinker/core/validators.py
+-rw-r--r--   0        0        0       52 2024-04-02 06:44:44.206363 tablelinker_light-1.0.0.post1/tablelinker/exceptions.py
+-rw-r--r--   0        0        0     3103 1970-01-01 00:00:00.000000 tablelinker_light-1.0.0.post1/PKG-INFO
```

### Comparing `tablelinker_light-1.0.0/LICENSE.txt` & `tablelinker_light-1.0.0.post1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/README.md` & `tablelinker_light-1.0.0.post1/README.md`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/pyproject.toml` & `tablelinker_light-1.0.0.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "tablelinker-light"
-version = "1.0.0"
+version = "1.0.0.post1"
 description = "TableLinker: CSV data processing library (light version)"
 authors = ["Takeshi Sagara <sagara@info-proto.com>", "Akiko Aizawa <akiko@nii.ac.jp>"]
 readme = "README.md"
 maintainers = ["Takeshi Sagara <sagara@info-proto.com>"]
-repository = "https://github.com/KMCS-NII/tablelinker-lib"
+repository = "https://github.com/KMCS-NII/tablelinker-light"
 documentation = "https://tablelinker-light.readthedocs.io/"
 keywords = ["CSV", "tabular", "cleansing", "batch processing"]
 packages = [{include = "tablelinker"}]
 classifiers = [
     "Operating System :: Microsoft :: Windows :: Windows 11",
     "Operating System :: POSIX :: Linux",
     "License :: OSI Approved :: MIT License",
```

### Comparing `tablelinker_light-1.0.0/tablelinker/__init__.py` & `tablelinker_light-1.0.0.post1/tablelinker/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from logging import getLogger
 
 from .core.table import Table
 from .core.task import Task
 
-__version__ = "1.0.0"  # pyproject.toml と git tag も変更すること
+__version__ = "1.0.0.post1"  # pyproject.toml と git tag も変更すること
 
 logger = getLogger(__name__)
 
 
 def useExtraConvertors() -> None:
     """
     拡張コンバータを利用することを宣言する。
```

### Comparing `tablelinker_light-1.0.0/tablelinker/cli.py` & `tablelinker_light-1.0.0.post1/tablelinker/cli.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/convertors/basics/__init__.py` & `tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/__init__.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/convertors/basics/calc_col.py` & `tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/calc_col.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/convertors/basics/concat_col.py` & `tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/concat_col.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/convertors/basics/concat_title.py` & `tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/concat_title.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/convertors/basics/delete_col.py` & `tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/delete_col.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/convertors/basics/delete_row.py` & `tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/delete_row.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/convertors/basics/generate_pk.py` & `tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/generate_pk.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/convertors/basics/insert_col.py` & `tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/insert_col.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/convertors/basics/mapping_col.py` & `tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/mapping_col.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/convertors/basics/move_col.py` & `tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/move_col.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/convertors/basics/rename_col.py` & `tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/rename_col.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/convertors/basics/reorder_col.py` & `tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/reorder_col.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/convertors/basics/round.py` & `tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/round.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/convertors/basics/select_row.py` & `tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/select_row.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/convertors/basics/split_col.py` & `tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/split_col.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/convertors/basics/truncate.py` & `tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/truncate.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/convertors/basics/update_col.py` & `tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/update_col.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/convertors/basics/zenkaku.py` & `tablelinker_light-1.0.0.post1/tablelinker/convertors/basics/zenkaku.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/convertors/extras/__init__.py` & `tablelinker_light-1.0.0.post1/tablelinker/convertors/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/convertors/extras/date_extract.py` & `tablelinker_light-1.0.0.post1/tablelinker/convertors/extras/date_extract.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/convertors/extras/geocoder.py` & `tablelinker_light-1.0.0.post1/tablelinker/convertors/extras/geocoder.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/convertors/extras/mapping_col.py` & `tablelinker_light-1.0.0.post1/tablelinker/convertors/extras/mapping_col.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/convertors/extras/wareki.py` & `tablelinker_light-1.0.0.post1/tablelinker/convertors/extras/wareki.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/core/context.py` & `tablelinker_light-1.0.0.post1/tablelinker/core/context.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/core/convertors.py` & `tablelinker_light-1.0.0.post1/tablelinker/core/convertors.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/core/csv_cleaner.py` & `tablelinker_light-1.0.0.post1/tablelinker/core/csv_cleaner.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/core/data_type.py` & `tablelinker_light-1.0.0.post1/tablelinker/core/data_type.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/core/date_extractor.py` & `tablelinker_light-1.0.0.post1/tablelinker/core/date_extractor.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/core/fieldtypes.py` & `tablelinker_light-1.0.0.post1/tablelinker/core/fieldtypes.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/core/input.py` & `tablelinker_light-1.0.0.post1/tablelinker/core/input.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/core/mapping.py` & `tablelinker_light-1.0.0.post1/tablelinker/core/mapping.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/core/output.py` & `tablelinker_light-1.0.0.post1/tablelinker/core/output.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/core/params.py` & `tablelinker_light-1.0.0.post1/tablelinker/core/params.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/core/table.py` & `tablelinker_light-1.0.0.post1/tablelinker/core/table.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/core/task.py` & `tablelinker_light-1.0.0.post1/tablelinker/core/task.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/tablelinker/core/validators.py` & `tablelinker_light-1.0.0.post1/tablelinker/core/validators.py`

 * *Files identical despite different names*

### Comparing `tablelinker_light-1.0.0/PKG-INFO` & `tablelinker_light-1.0.0.post1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: tablelinker-light
-Version: 1.0.0
+Version: 1.0.0.post1
 Summary: TableLinker: CSV data processing library (light version)
-Home-page: https://github.com/KMCS-NII/tablelinker-lib
+Home-page: https://github.com/KMCS-NII/tablelinker-light
 Keywords: CSV,tabular,cleansing,batch processing
 Author: Takeshi Sagara
 Author-email: sagara@info-proto.com
 Maintainer: Takeshi Sagara
 Maintainer-email: sagara@info-proto.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -27,15 +27,15 @@
 Requires-Dist: munkres (>=1.1.4,<2.0.0)
 Requires-Dist: openpyxl
 Requires-Dist: pandas
 Requires-Dist: regex (>=2023.12.25,<2024.0.0)
 Requires-Dist: requests
 Requires-Dist: xlrd
 Project-URL: Documentation, https://tablelinker-light.readthedocs.io/
-Project-URL: Repository, https://github.com/KMCS-NII/tablelinker-lib
+Project-URL: Repository, https://github.com/KMCS-NII/tablelinker-light
 Description-Content-Type: text/markdown
 
 # tablelinker-light
 
 ![Python 3.7](https://github.com/InfoProto/tablelinker-light/actions/workflows/python-3.7.yml/badge.svg)
 ![Python 3.8](https://github.com/InfoProto/tablelinker-light/actions/workflows/python-3.8.yml/badge.svg)
 ![Python 3.9](https://github.com/InfoProto/tablelinker-light/actions/workflows/python-3.9.yml/badge.svg)
```

