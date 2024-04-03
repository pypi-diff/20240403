# Comparing `tmp/pandas-dataset-0.1.2.tar.gz` & `tmp/pandas-dataset-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-dataset-0.1.2.tar", last modified: Tue Mar 26 07:07:17 2024, max compression
+gzip compressed data, was "pandas-dataset-0.1.3.tar", last modified: Wed Apr  3 09:37:20 2024, max compression
```

## Comparing `pandas-dataset-0.1.2.tar` & `pandas-dataset-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-03-26 07:07:17.831213 pandas-dataset-0.1.2/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      485 2024-03-26 06:54:27.000000 pandas-dataset-0.1.2/LICENSE.txt
--rw-r--r--   0 mihai     (1000) mihai     (1000)      560 2024-03-26 07:07:17.831213 pandas-dataset-0.1.2/PKG-INFO
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      192 2024-03-26 07:02:14.000000 pandas-dataset-0.1.2/README.md
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-03-26 07:07:17.827213 pandas-dataset-0.1.2/pandas_dataset/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      174 2024-03-26 06:54:27.000000 pandas-dataset-0.1.2/pandas_dataset/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4654 2024-03-26 07:05:35.000000 pandas-dataset-0.1.2/pandas_dataset/column_types.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    20718 2024-03-26 06:54:27.000000 pandas-dataset-0.1.2/pandas_dataset/dataset.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1713 2024-03-26 06:57:03.000000 pandas-dataset-0.1.2/pandas_dataset/dataset_hash_check.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2059 2024-03-26 06:54:27.000000 pandas-dataset-0.1.2/pandas_dataset/indexes.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-03-26 07:07:17.831213 pandas-dataset-0.1.2/pandas_dataset/input_output/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      184 2024-03-26 06:54:27.000000 pandas-dataset-0.1.2/pandas_dataset/input_output/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4490 2024-03-26 06:54:27.000000 pandas-dataset-0.1.2/pandas_dataset/input_output/csv_read.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1503 2024-03-26 06:54:27.000000 pandas-dataset-0.1.2/pandas_dataset/input_output/csv_write.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4220 2024-03-26 06:54:27.000000 pandas-dataset-0.1.2/pandas_dataset/input_output/parquet_read.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1337 2024-03-26 06:54:27.000000 pandas-dataset-0.1.2/pandas_dataset/input_output/parquet_write.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     5894 2024-03-26 06:57:17.000000 pandas-dataset-0.1.2/pandas_dataset/internal.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1635 2024-03-26 06:54:27.000000 pandas-dataset-0.1.2/pandas_dataset/merge.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3109 2024-03-26 06:54:27.000000 pandas-dataset-0.1.2/pandas_dataset/stats.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-03-26 07:07:17.831213 pandas-dataset-0.1.2/pandas_dataset.egg-info/
--rw-r--r--   0 mihai     (1000) mihai     (1000)      560 2024-03-26 07:07:17.000000 pandas-dataset-0.1.2/pandas_dataset.egg-info/PKG-INFO
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      651 2024-03-26 07:07:17.000000 pandas-dataset-0.1.2/pandas_dataset.egg-info/SOURCES.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        1 2024-03-26 07:07:17.000000 pandas-dataset-0.1.2/pandas_dataset.egg-info/dependency_links.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       36 2024-03-26 07:07:17.000000 pandas-dataset-0.1.2/pandas_dataset.egg-info/requires.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       15 2024-03-26 07:07:17.000000 pandas-dataset-0.1.2/pandas_dataset.egg-info/top_level.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       38 2024-03-26 07:07:17.831213 pandas-dataset-0.1.2/setup.cfg
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      719 2024-03-26 07:06:41.000000 pandas-dataset-0.1.2/setup.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-03 09:37:20.385761 pandas-dataset-0.1.3/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      485 2024-03-26 06:54:27.000000 pandas-dataset-0.1.3/LICENSE.txt
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     2591 2024-04-03 09:37:20.385761 pandas-dataset-0.1.3/PKG-INFO
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2120 2024-03-26 10:13:59.000000 pandas-dataset-0.1.3/README.md
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-03 09:37:20.381761 pandas-dataset-0.1.3/pandas_dataset/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      271 2024-04-03 09:37:06.000000 pandas-dataset-0.1.3/pandas_dataset/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4665 2024-04-03 06:54:48.000000 pandas-dataset-0.1.3/pandas_dataset/column_types.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    20684 2024-04-03 06:39:08.000000 pandas-dataset-0.1.3/pandas_dataset/dataset.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1713 2024-03-26 06:57:03.000000 pandas-dataset-0.1.3/pandas_dataset/dataset_hash_check.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2068 2024-04-03 06:38:16.000000 pandas-dataset-0.1.3/pandas_dataset/indexes.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-03 09:37:20.385761 pandas-dataset-0.1.3/pandas_dataset/input_output/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      184 2024-03-26 06:54:27.000000 pandas-dataset-0.1.3/pandas_dataset/input_output/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4493 2024-04-03 06:36:08.000000 pandas-dataset-0.1.3/pandas_dataset/input_output/csv_read.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1503 2024-04-03 06:36:11.000000 pandas-dataset-0.1.3/pandas_dataset/input_output/csv_write.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4260 2024-04-03 09:37:06.000000 pandas-dataset-0.1.3/pandas_dataset/input_output/parquet_read.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1337 2024-03-26 06:54:27.000000 pandas-dataset-0.1.3/pandas_dataset/input_output/parquet_write.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     5272 2024-04-03 06:32:49.000000 pandas-dataset-0.1.3/pandas_dataset/internal.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1639 2024-04-03 06:35:12.000000 pandas-dataset-0.1.3/pandas_dataset/merge.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3120 2024-04-03 06:35:24.000000 pandas-dataset-0.1.3/pandas_dataset/stats.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    10336 2024-04-03 09:37:06.000000 pandas-dataset-0.1.3/pandas_dataset/torch_dataset.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      739 2024-04-03 06:38:50.000000 pandas-dataset-0.1.3/pandas_dataset/utils.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-03 09:37:20.385761 pandas-dataset-0.1.3/pandas_dataset.egg-info/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     2591 2024-04-03 09:37:20.000000 pandas-dataset-0.1.3/pandas_dataset.egg-info/PKG-INFO
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      707 2024-04-03 09:37:20.000000 pandas-dataset-0.1.3/pandas_dataset.egg-info/SOURCES.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        1 2024-04-03 09:37:20.000000 pandas-dataset-0.1.3/pandas_dataset.egg-info/dependency_links.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      109 2024-04-03 09:37:20.000000 pandas-dataset-0.1.3/pandas_dataset.egg-info/requires.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       15 2024-04-03 09:37:20.000000 pandas-dataset-0.1.3/pandas_dataset.egg-info/top_level.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       38 2024-04-03 09:37:20.385761 pandas-dataset-0.1.3/setup.cfg
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      810 2024-04-03 09:37:06.000000 pandas-dataset-0.1.3/setup.py
```

### Comparing `pandas-dataset-0.1.2/pandas_dataset/column_types.py` & `pandas-dataset-0.1.3/pandas_dataset/column_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Fundamental column types to Dataset library"""
 # pylint: disable=protected-access
-from typing import Dict, Optional
+from __future__ import annotations
+from typing import Dict
 import numpy as np
 import pandas as pd
 from loguru import logger
 
 ColumnType = str
 # { users: {client_id: str, total_number_of_sessions: int}, sessions: {...}, ... }
 DatasetDgTypes = Dict[str, Dict[str, ColumnType]]
@@ -36,17 +37,17 @@
 
 def _dtype_to_column_type(col_data: pd.Series, dtype: type) -> ColumnType:
     """Converts a regular dtype from a backend (i.e. pandas) to a dataet type, which is represented as string"""
     # This is first checked because it's not a numpy type, but a pandas type. All the other ones are numpy dtypes
     # used by pandas in their series.
     if isinstance(dtype, pd.CategoricalDtype):
         return "categorical"
-    if isinstance(dtype, int) or np.issubdtype(dtype, np.dtype("int")):
+    if isinstance(dtype, int) or np.issubdtype(dtype, np.integer):
         return "int"
-    if isinstance(dtype, float) or np.issubdtype(dtype, np.dtype("float")):
+    if isinstance(dtype, float) or np.issubdtype(dtype, np.floating):
         return "float"
     if isinstance(dtype, bool) or np.issubdtype(dtype, np.dtype("bool")):
         return "bool"
     if np.issubdtype(dtype, np.dtype("datetime64")):
         return "datetime64[ns]"
     if np.issubdtype(dtype, np.dtype("timedelta64")):
         return "timedelta64[ns]"
@@ -88,13 +89,13 @@
         raise KeyError(f"Provided data types: {column_types.keys()}. Dataset: {dataset._data.keys()}")
     for dg in dataset._data.keys():
         for col in dataset._data[dg].columns:
             assert column_types[dg][col] in VALID_COLUMN_TYPES, f"{column_types[dg][col]} & {VALID_COLUMN_TYPES}"
             _check_col_data(dataset._data[dg][col], column_types[dg][col])
     return column_types
 
-def build_column_types(dataset: "Dataset", column_types: Optional[DatasetDgTypes]) -> DatasetDgTypes:
+def build_column_types(dataset: "Dataset", column_types: DatasetDgTypes | None) -> DatasetDgTypes:
     """Returns a properly verified dictionary of dg => {col: data type} for all data groups"""
     if column_types is None:
         column_types = _auto_detect_column_types(dataset)
 
     return check_column_types(dataset, column_types)
```

### Comparing `pandas-dataset-0.1.2/pandas_dataset/dataset.py` & `pandas-dataset-0.1.3/pandas_dataset/dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """Dataset class module."""
 from __future__ import annotations
-from typing import Dict, List, Optional, Union, Tuple, Callable, Any, overload
+from typing import Callable, Any, overload
 from copy import copy, deepcopy
 from pathlib import Path
 import json
 from natsort import natsorted
 import pandas as pd
 import numpy as np
 
 from loguru import logger
 
 from .indexes import compute_indexes
 from .stats import compute_stats
 from .column_types import ColumnType, build_column_types, check_column_types
-from .internal import check_data_groups_consistency, check_nans, build_data, build_data_groups, flatten_list, StrOrPath
+from .internal import check_data_groups_consistency, check_nans, build_data, build_data_groups
 from .merge import merge_datasets
 from .input_output import csv_read, csv_write, csv_peek, parquet_read, parquet_write, parquet_peek
+from .utils import StrOrPath, flatten_list
 
 class Dataset:
     """
     A `Dataset` represents a nested group of dataframes and contains the underlying data as a dict
     with string keys and `pd.DataFrame` values and the nested lists of indexes
     which help locating the corresponding data throughout the path.
     Notes:
@@ -56,54 +57,54 @@
         data_groups: The dict of lists representing the nested data groups.
         tables: The list of tables from which data_groups are formed.
         keys: The keys of the dataset (used as compatibility with dict).
         values: The values of the dataset (used as compatibility with dict).
         items: The items of the dataset (used as compatibility with dict).
     """
     def __init__(self,
-                 data: Dict[str, Union[pd.DataFrame, pd.Series]],
-                 column_types: Optional[Dict[str, List[ColumnType]]] = None,
+                 data: dict[str, pd.DataFrame | pd.Series],
+                 column_types: dict[str, list[ColumnType]] | None = None,
                  check_consistency: bool = False,
                  ):
         assert isinstance(data, dict), f"Datasets can only be constructed out of dicts of dataframes. Got {type(data)}"
         assert len(data.keys()) > 0, "No data groups were provided"
-        self._data: Dict[str, pd.DataFrame] = build_data(data)
+        self._data: dict[str, pd.DataFrame] = build_data(data)
         self._column_types = build_column_types(self, column_types)
-        self._data_groups: List[List[str]] = build_data_groups(self)
-        self._indexes: Optional[Dict[str, List]] = None
-        self._stats: Dict[str, Dict[str, Dict]] = None
-        self._metadata: Dict[str, Any] = {}
+        self._data_groups: list[list[str]] = build_data_groups(self)
+        self._indexes: dict[str, list] | None = None
+        self._stats: dict[str, dict[str, dict]] | None = None
+        self._metadata: dict[str, Any] = {}
         if check_consistency:
             self.check_consistency()
 
     @property
     def data(self):
         """Returns the underlying data of this dataset."""
         return self._data
 
     @property
-    def column_types(self) -> Dict[str, Dict[str, ColumnType]]:
+    def column_types(self) -> dict[str, dict[str, ColumnType]]:
         """Returns the dataset's data types dictionary"""
         assert self._column_types is not None, "Data types is not constructed. Call the constructor properly."
         return {dg: self._column_types[dg] for dg in self.tables}
 
     @property
-    def dtypes(self) -> Dict[str, Dict[str, ColumnType]]:
+    def dtypes(self) -> dict[str, dict[str, ColumnType]]:
         """same as self.column_types"""
         return self.column_types
 
     @property
-    def indexes(self) -> Dict[str, List]:
+    def indexes(self) -> dict[str, list]:
         """Returns the nested indexes of the dataset."""
         if self._indexes is None:
             self._indexes = compute_indexes(self)
         return self._indexes
 
     @property
-    def stats(self) -> Dict[str, Dict[str, np.ndarray]]:
+    def stats(self) -> dict[str, dict[str, np.ndarray]]:
         """
         Returns the statistics (min, max) of each column in the dataset
         Return format:
         {
             "dg1": {
                 "col1": np.array([
                     min_x, # can be also an array if dataset_type of col is categorical/vector
@@ -113,83 +114,83 @@
         }
         """
         if self._stats is None:
             self._stats = compute_stats(self)
         return self._stats
 
     @property
-    def metadata(self) -> Dict[str, Any]:
+    def metadata(self) -> dict[str, Any]:
         """Returns the metadata. It is guaranteed that it can be converted to a json representation"""
         return self._metadata
 
     @metadata.setter
-    def metadata(self, metadata: Dict[str, Any]):
+    def metadata(self, metadata: dict[str, Any]):
         assert isinstance(metadata, dict), f"Expected a dictionary metadata, got {metadata}"
         assert json.loads(json.dumps(metadata)) == metadata, f"Metadata doesn't seem JSON-able: {metadata}"
         self._metadata = metadata
 
     @property
-    def join_keys(self) -> Dict[str, List[str]]:
+    def join_keys(self) -> dict[str, list[str]]:
         """
         Returns the join keys of the dataset as a dict {data_group: [join keys]}. We assume that each nested group
         contains the primary key of its parent.
         """
         res = {}
         for dg in self.data_groups:
             dg_keys = []
             for tb in dg:
                 res[tb] = copy(dg_keys)
                 dg_keys.append(self.primary_keys[tb])
         return res
 
     @property
-    def primary_keys(self) -> Dict[str, str]:
+    def primary_keys(self) -> dict[str, str]:
         """Returns the primary keys of the dataset as a dict {table: primary key}."""
         return {dg: self._data[dg].index.name for dg in self.tables}
 
     @property
-    def columns(self) -> Dict[str, List[str]]:
+    def columns(self) -> dict[str, list[str]]:
         """Returns the columns of the dataset as a dict {table: [columns]}."""
         return {dg: self._data[dg].columns.tolist() for dg in self.tables}
 
     @property
-    def all_column_names(self) -> List[str]:
+    def all_column_names(self) -> list[str]:
         """Returns the values of all column names + primary keys + join keys for all data groups."""
         all_cols = flatten_list(self.columns.values())
         all_keys = flatten_list(self.primary_keys.values())
         return list(set(all_cols + all_keys))
 
     @property
-    def hash(self) -> Dict[str, pd.Series]:
+    def hash(self) -> dict[str, pd.Series]:
         """Returns the pandas hash of the dataset as a dict {data_group: hash}."""
         res = {}
         for tb in self.tables:
             hashable_df = self[tb].select_dtypes(exclude=[object])
             res[tb] = pd.util.hash_pandas_object(hashable_df, index=True)
         return res
 
     @property
-    def shape(self) -> Dict[str, Tuple[int, int]]:
+    def shape(self) -> dict[str, tuple[int, int]]:
         """Returns the shapes of the dataset as a dict {data_group: dataframe_shape}."""
         return {dg: tuple(self._data[dg].shape) for dg in self.tables}
 
     @property
-    def data_groups(self) -> List[List[str]]:
+    def data_groups(self) -> list[list[str]]:
         """
         Returns the data groups as a list of lists. It is assumed that the data groups are designed as a forest of
         linear trees (1 child only). So, we might have [ [products], [users, sessions] ] as two data groups. Each inner
         data group is guaranteed to be returned from root to leaf, so no [ [products], [sessions (X), users] ].
         However, since all data groups are equal at top level, we may get them in any order, so
         [ [users, sessions], [products] ] and [ [products], [users, sessions] ]
         are both fine, because only the data groups are shuffled.
         """
         return self._data_groups
 
     @property
-    def tables(self) -> List[str]:
+    def tables(self) -> list[str]:
         """Returns all the tables as a flattened list"""
         return flatten_list(self.data_groups)
 
     def keys(self):
         """Returns the data groups of the dataset. Used as compatibility to dicts. No guarantees on dg order!"""
         return self._data.keys()
 
@@ -222,26 +223,26 @@
     def sort_columns(self):
         """Sorts the columns of the dataset by name, inplace"""
         for dg in self.tables:
             cols = self.columns[dg]
             sorted_cols = natsorted(cols)
             self._data[dg] = self._data[dg][sorted_cols]
 
-    def get_column(self, col_name: str) -> Tuple[str, pd.Series]:
+    def get_column(self, col_name: str) -> tuple[str, pd.Series]:
         """Gets the data of a column, if it exists in this dataset, alongside the data group it is part of"""
         assert isinstance(col_name, str), f"Expected a string, got {col_name}"
         for k, v in self.items():
             if col_name == v.index.name:  # pragma: no cover
                 return k, v.index
             if col_name in v.columns:
                 return k, v[col_name]
         raise KeyError(f"Column '{col_name}' not found in dataset.")
 
-    def merge(self, other: Union[Dataset, Dict[str, Union[pd.DataFrame, pd.Series]]],
-              *args, must_be_disjoint: bool=False, **kwargs) -> Dataset:
+    def merge(self, other: Dataset | dict[str, pd.DataFrame | pd.Series],
+              *args, must_be_disjoint: bool = False, **kwargs) -> Dataset:
         """Given another dataset, merge using the underlying pandas.merge method for each data group."""
         if isinstance(other, dict):
             logger.warning("Merge was called with a dionary of dataframes. Converting to Dataset.")
             other = Dataset(other)
         assert isinstance(other, Dataset), f"Can only merge two datasets together. Got '{type(other)}'"
         new_data, new_column_types = merge_datasets(self, other, *args, must_be_disjoint=must_be_disjoint, **kwargs)
         res = Dataset(new_data, new_column_types)
@@ -272,16 +273,16 @@
             check_nans(self)
         if column_types:
             check_column_types(self, self.column_types)
 
     # I/O operations
 
     @staticmethod
-    def read(path: StrOrPath, data_format: str, tables_pk: Dict[str, str],
-             columns: Dict[str, List[str]] = None, **kwargs) -> Dataset:
+    def read(path: StrOrPath, data_format: str, tables_pk: dict[str, str],
+             columns: dict[str, list[str]] = None, **kwargs) -> Dataset:
         """
         Loads the dataset from a path given a mapping {data group => primary key} for all data groups and a list
         of columns for each data-groups. If columns is not set, it will read all the columns.
         Supported formats: "csv", "parquet". If indexes are provided, they will be used to set the index of the data.
 
         Usage: Datset.read("/path/to/disk_dir", "csv", tables_pk={"users": "client_id"}, [columns=col]}
 
@@ -314,15 +315,15 @@
             dataset._indexes = np.load(path / "indexes.npy", allow_pickle=True).item()
         if (path / "metadata.json").exists():
             with open(path / "metadata.json", "r", encoding="utf-8") as f:
                 dataset.metadata = json.load(f)
         return dataset
 
     @staticmethod
-    def peek(path: StrOrPath, data_format: str, tables_pk: Dict[str, str]) -> Dict[str, Dict[str, str]]:
+    def peek(path: StrOrPath, data_format: str, tables_pk: dict[str, str]) -> dict[str, dict[str, str]]:
         """
         Reads only the header and the dataset types from a path given a mapping {data group => primary key}.
         Supported formats: "csv", "parquet".
 
         Usage: Dataset.peek("/path/to/disk_dir", "parquet", {"users": "client_id", "sessions": "session_id"})
         """
         if data_format == "csv":
@@ -360,22 +361,22 @@
             np.save(path / "dataset_stats.npy", self.stats)
 
     @overload
     def __getitem__(self, index: str) -> pd.DataFrame:
         ...
 
     @overload
-    def __getitem__(self, index: Dict) -> Dataset:
+    def __getitem__(self, index: dict) -> Dataset:
         ...
 
     @overload
-    def __getitem__(self, index: List) -> Dataset:
+    def __getitem__(self, index: list) -> Dataset:
         ...
 
-    def __getitem__(self, index: Union[Dict, List, str]) -> Union[Dataset, pd.DataFrame]:
+    def __getitem__(self, index: dict | list | str) -> Dataset | pd.DataFrame:
         if isinstance(index, dict):
             res, res_dtypes = {}, {}
             # We can also index a dataset with a subset of columns {"dg": [cols], "dg2": [cols2]}
             for dg, v in index.items():
                 assert isinstance(v, (tuple, set, list)), f"Expeted a list to index columns using a dict, got {v}"
                 _v = sorted(list(set([*[(f.name if hasattr(f, "name") else f) for f in v], *self.join_keys[dg]])))
                 res[dg] = self._data[dg][_v]
@@ -395,15 +396,15 @@
         try:
             return super().__getattribute__(name)
         except AttributeError as ex:
             # this enables syntax like dataset.users if 'users' is a table in the dataset.
             # Alternative to dataset["users"], similarily to how it's done in pandas as well for columns.
             try:
                 return self._data[name]
-            except:
+            except Exception:
                 raise AttributeError(ex)
 
     def __setitem__(self, item, value):
         raise ValueError("Setting values to data groups is not allowed. Use dataset.merge() or Dataset() constructor.")
 
     def __contains__(self, key):
         return key in self.tables
```

### Comparing `pandas-dataset-0.1.2/pandas_dataset/dataset_hash_check.py` & `pandas-dataset-0.1.3/pandas_dataset/dataset_hash_check.py`

 * *Files identical despite different names*

### Comparing `pandas-dataset-0.1.2/pandas_dataset/indexes.py` & `pandas-dataset-0.1.3/pandas_dataset/indexes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Indexes internal module to compute the indexes of a dataset"""
-from typing import Dict, List
+from __future__ import annotations
 import pandas as pd
 import numpy as np
 
-def compute_indexes(data: "Dataset") -> Dict[str, List]:
+def compute_indexes(data: "Dataset") -> dict[str, list]:
     """
     Computes a nested lists of indexes that helps to locate the data throughout a path:
     indexes from the `k`-th list help to locate the top node data points in the dataframe associated
     to the `k`-th node of the path.
     All the lists have the same length, equal to the length of the top node dataframe.
 
     Example:
@@ -16,22 +16,22 @@
         dataframe that correspond to users in the `users` dataframe.
         Thus, for each user in the top dataframe we know exactly where to find its sessions in the `sessions`
         dataframe.
 
     Returns a dict whose keys are the nodes in `path` and whose values are the correspondingly nested lists of
     indexes.
     """
-    res: Dict[str, List[List[int]]] = {}
+    res: dict[str, list[list[int]]] = {}
     for dg in data.data_groups:
         # we start with the top-level data group. Since it is unique, it will a simple mapping: [ [0], [1], .., [n] ]
         assert len(pd.unique(data[dg[0]].index)) == len(data[dg[0]]), f"Index of data group '{dg[0]}' is not unique"
         res[dg[0]] = [ [i] for i in range(len(data[dg[0]])) ]
 
-        for i in range(len(dg)-1):
+        for i in range(len(dg) - 1):
             parent: pd.DataFrame = data[dg[i]]
-            child: pd.DataFrame = data[dg[i+1]]
+            child: pd.DataFrame = data[dg[i + 1]]
             assert len(pd.unique(child.index)) == len(child), f"Index of data group '{dg[i+1]}' is not unique"
             # Example: groupby dg='sessions' by 'Client ID', or dg='hits' by 'Session ID'
-            indices: Dict[str, np.ndarray] = child.groupby(parent.index.name).indices
+            indices: dict[str, np.ndarray] = child.groupby(parent.index.name).indices
             # turn the {index1: array([ix1]), index2: array([ix2])} into [ [ix1], [ix2] ]
             res[f"{dg[i]}-{dg[i+1]}"] = [x.tolist() for x in indices.values()]
     return res
```

### Comparing `pandas-dataset-0.1.2/pandas_dataset/input_output/csv_read.py` & `pandas-dataset-0.1.3/pandas_dataset/input_output/csv_read.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Reads a (Typed) CSV dataset from a directory"""
 # pylint: disable=consider-iterating-dictionary
-from typing import Dict, List, Callable, Tuple, Optional
+from __future__ import annotations
+from typing import Callable
 from pathlib import Path
 import json
 import ast
 import numpy as np
 import pandas as pd
 from loguru import logger
 from ..column_types import VALID_COLUMN_TYPES, ColumnType, column_type_to_dtype
 
-def _build_converters(dg_column_types: Dict[str, Dict[str, ColumnType]],
-                      object_converters: Dict[str, Callable]) -> Dict[str, Dict[str, Callable]]:
+def _build_converters(dg_column_types: dict[str, dict[str, ColumnType]],
+                      object_converters: dict[str, Callable]) -> dict[str, dict[str, Callable]]:
     """Special types that must be explicitly converted after reading them with pd.read_csv"""
     converters = {}
     for tb in dg_column_types.keys():
         converters[tb] = {}
         for k, v in dg_column_types[tb].items():
             if v == "vector":
                 converters[tb][k] = lambda x: np.array(ast.literal_eval(x), dtype=np.float32)
@@ -23,41 +24,41 @@
             if v == "object":
                 if k not in object_converters:
                     logger.warning(f"Column '{k}' is object and has no object converter callback. Reading as string.")
                     continue
                 converters[tb][k] = object_converters[k]
     return converters
 
-def _read_column_types(path: Path, columns: Dict[str, List[str]]) -> Dict[str, Dict[str, ColumnType]]:
+def _read_column_types(path: Path, columns: dict[str, list[str]]) -> dict[str, dict[str, ColumnType]]:
     """Reads dataset types from types.json expected in the same dir as the csv files"""
     col_types_file = path / "types.json"
     with open(col_types_file, "r", encoding="utf8") as json_file:
-        raw_dtypes: Dict[str, Dict[str, str]] = json.load(json_file)
+        raw_dtypes: dict[str, dict[str, str]] = json.load(json_file)
 
     col_types_file = {}
     for tb, tb_columns in columns.items():
         col_types_file[tb] = {}
         for column in tb_columns:
             assert column in raw_dtypes[tb], f"'{tb}/{column}' not in {raw_dtypes[tb]} (path: '{col_types_file}')"
             column_dtype = raw_dtypes[tb][column]
             assert column_dtype in VALID_COLUMN_TYPES, f"Got '{column_dtype}'. Valid: {VALID_COLUMN_TYPES}"
             col_types_file[tb][column] = column_dtype
 
     return col_types_file
 
-def csv_peek(path: Path, tables_pk: Dict[str, str]) -> Dict[str, Dict[str, str]]:
+def csv_peek(path: Path, tables_pk: dict[str, str]) -> dict[str, dict[str, str]]:
     """Reads just the first row of all csv files given a path. Then, reads the types.json file and returns it."""
     cols = {}
     for tb in tables_pk.keys():
         cols[tb] = pd.read_csv(f"{path}/{tb}.csv", nrows=0).columns.tolist()
     res = _read_column_types(path, cols)
     return res
 
-def csv_read(path: Path, tables_pk: Dict[str, str], columns: Dict[str, List[str]],
-             object_converters: Optional[Dict[str, Callable]] = None) -> Tuple[Dict, Dict]:
+def csv_read(path: Path, tables_pk: dict[str, str], columns: dict[str, list[str]],
+             object_converters: dict[str, Callable] | None = None) -> tuple[dict, dict]:
     """Reads data from a path of CSVs, given a list of columns and a list of data-groups plus their primary keys"""
     assert path.is_dir(), f"Path must be a directory. Got '{path}'."
     assert isinstance(columns, dict), f"Expected dict, got {columns}"
 
     object_converters = object_converters if object_converters is not None else {}
     column_types = _read_column_types(path, columns)
     converters = _build_converters(column_types, object_converters)
```

### Comparing `pandas-dataset-0.1.2/pandas_dataset/input_output/csv_write.py` & `pandas-dataset-0.1.3/pandas_dataset/input_output/csv_write.py`

 * *Files identical despite different names*

### Comparing `pandas-dataset-0.1.2/pandas_dataset/input_output/parquet_read.py` & `pandas-dataset-0.1.3/pandas_dataset/input_output/parquet_read.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Reads a parquet dataset from a directory"""
-from typing import Dict, List, Tuple
+# pylint: disable=c-extension-no-member
+from __future__ import annotations
 from pathlib import Path
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 from pyarrow import parquet as pq
 from loguru import logger
 from ..column_types import ColumnType
@@ -15,15 +16,15 @@
     NOTE: this doesn't protect you from invalid parquet files (having different headers) inside the directory
     """
     try:
         schema = pq.read_schema(path)
     except OSError:
         all_files = list(path.iterdir())
         assert len(all_files) > 0, f"Found dir at '{path}' but with no parquet files inside"
-        pq_files = [x for x in all_files if x.suffix==".parquet" and x.is_file()]
+        pq_files = [x for x in all_files if x.suffix == ".parquet" and x.is_file()]
         assert len(pq_files) == len(all_files), f"Found other type of files at '{path}' except parquet: {all_files}"
         return _peek_one_file_only(pq_files[0])
     return schema
 
 def _pq_to_dataset_type(pq_type) -> ColumnType:
     """Maps parquet types to Dataset types"""
     if pq_type == "string":
@@ -35,42 +36,42 @@
     if pq_type in ("int64", "int32"):
         return "int"
     if isinstance(pq_type, pa.lib.ListType):
         # Both vectors and objects are stored as lists, so we need to look at the inner type to differnetiate
         if pq_type.value_type == "float":
             return "vector"
         return "object"
-    if isinstance(pq_type, pa.lib.DictionaryType):
+    if isinstance(pq_type, pa.lib.dictionaryType):
         return "categorical"
     if isinstance(pq_type, pa.lib.TimestampType):
         assert pq_type.to_pandas_dtype() == np.dtype("datetime64[ns]"), f"Unknown datetime format: {pq_type}"
         return "datetime64[ns]"
     if isinstance(pq_type, pa.lib.DurationType):
         assert pq_type.unit == "ns", f"Unknown timedelta format: {pq_type}"
         return "timedelta64[ns]"
     if isinstance(pq_type, pa.lib.DataType):
         if pq_type == "date32[day]":
             assert pq_type.to_pandas_dtype() == np.dtype("datetime64[ns]"), f"Unknown datetime format: {pq_type}"
             return "datetime64[ns]"
 
     raise TypeError(f"Unknown parquet type: {pq_type} found in the dataset.")
 
-def parquet_peek(path: Path, tables_pk: Dict[str, str]) -> Dict[str, Dict[str, str]]:
+def parquet_peek(path: Path, tables_pk: dict[str, str]) -> dict[str, dict[str, str]]:
     """Reads just the first row of all pq files given a path. Then, reads the types.json file and returns it."""
     column_types = {}
     for tb, pk in tables_pk.items():
         column_types[tb] = {}
         schema = _peek_one_file_only(path / f"{tb}.parquet")
         assert pk in schema.names, f"Primary key '{tb}/{pk}' not found in the parquet file!"
         for col, pq_type in zip(schema.names, schema.types):
             column_type = _pq_to_dataset_type(pq_type)
             column_types[tb][col] = column_type
     return column_types
 
-def parquet_read(path: Path, tables_pk: Dict[str, str], columns: Dict[str, List[str]]) -> Tuple[Dict, Dict]:
+def parquet_read(path: Path, tables_pk: dict[str, str], columns: dict[str, list[str]]) -> tuple[dict, dict]:
     """Reads data from a path of parquets, given a list of columns and a list of data-groups plus their primary keys"""
     assert path.is_dir(), f"Path must be a directory. Got '{path}'."
     assert isinstance(columns, dict), f"Expected dict, got {columns}"
 
     logger.info(f"Reading Dataset from parquet files. Path: '{path}'. Data groups: {list(tables_pk)}")
     header = parquet_peek(path, tables_pk)
     data = {}
```

### Comparing `pandas-dataset-0.1.2/pandas_dataset/input_output/parquet_write.py` & `pandas-dataset-0.1.3/pandas_dataset/input_output/parquet_write.py`

 * *Files identical despite different names*

### Comparing `pandas-dataset-0.1.2/pandas_dataset/internal.py` & `pandas-dataset-0.1.3/pandas_dataset/internal.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,17 @@
 """Various checks done on the dataset to ensure its consistency. Called explicitly only for efficiency purposes"""
 # pylint: disable=protected-access, consider-iterating-dictionary
-from typing import Dict, Union, List, Iterable, T
-from pathlib import Path
+from __future__ import annotations
 from copy import copy
 from collections import Counter
 import pandas as pd
-import numpy as np
 
 from loguru import logger
 
-StrOrPath = Union[Path, str]
-
-def get_project_root() -> Path:
-    """gets the root of the project for tests"""
-    return Path(__file__).absolute().parents[1]
-
-def flatten_list(x: Iterable[T]) -> List[T]:
-    """Flattens a list of lists. Also flattens np arrays of object type, tuples and sets."""
-    if x is None or len(x) == 0:
-        return []
-    res = []
-    for item in x:
-        if isinstance(item, (tuple, list, set)) or (isinstance(item, np.ndarray) and item.dtype == object):
-            res.extend(flatten_list(item))
-        else:
-            res.append(item)
-    return res
+from .utils import flatten_list
 
 def _check_one_path(dataset: "Dataset", path):
     # Do a .unique() on each join key and check that data frames are perfectly inner joinable
     for i in range(len(path) - 1):
         parent: pd.DataFrame = dataset[path[i]]
         child: pd.DataFrame = dataset[path[i + 1]]
         index_col = parent.index
@@ -53,18 +35,18 @@
     """Checks if the dataset has nans. Will throw an error if true"""
     logger.debug("Checking for nans inside the dataset")
     for tb in dataset.tables:
         nans = dataset[tb].isna().any() if len(dataset[tb]) > 0 else []
         if sum(nans):
             raise ValueError(f"NaNs or Infinities were found in the table '{tb}': {nans}")
 
-def build_data(data: Dict[str, Union[pd.Series, pd.DataFrame]]) -> Dict[str, pd.DataFrame]:
+def build_data(data: dict[str, pd.Series | pd.DataFrame]) -> dict[str, pd.DataFrame]:
     """Returns a proper dictionary of dataframes. Does basic checks as well."""
     # Convert series to dataframes if the case
-    df_data: Dict[str, pd.DataFrame] = {}
+    df_data: dict[str, pd.DataFrame] = {}
     all_cols = []
     pks = []
     for dg, v in data.items():
         if isinstance(v, pd.Series):
             assert v.name, f"The value of data group '{dg}' is a `pd.Series` without name."
             data[dg] = v.to_frame()
 
@@ -76,21 +58,21 @@
             data[dg].index.name = dg
 
         df_data[dg] = data[dg]
         all_cols.extend(df_data[dg].columns.tolist())
         pks.append(df_data[dg].index.name)
 
     all_cols_except_pks = [col for col in all_cols if col not in pks]
-    duplicates = {k: v for k,v in Counter(all_cols_except_pks).items() if v > 1}
+    duplicates = {k: v for k, v in Counter(all_cols_except_pks).items() if v > 1}
     if len(duplicates) > 0:
         raise ValueError(f"There are duplicate column names across tables: {duplicates}")
 
     return df_data
 
-def build_data_groups(dataset: "Dataset") -> List[List[str]]:
+def build_data_groups(dataset: "Dataset") -> list[list[str]]:
     """
     Builds the nested data groups for all top-levels.
     Example: for users>sessions and products, we will get [[users, sessions], [products]]
     Cycles are ot allowed. Children with 2 parents are not allowed. One parent with 2 children are not allowed.
      - [tb1, tb2, tb3, tb1] -> wrong (rule 1)
      - tb1 => [tb2, tb3] -> wrong (rule 2)
      - [tb1, tb2] => tb3 -> wrong (rule 3)
```

### Comparing `pandas-dataset-0.1.2/pandas_dataset/merge.py` & `pandas-dataset-0.1.3/pandas_dataset/merge.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """"Merge module for dataset objects"""
-from typing import Dict, Tuple
+from __future__ import annotations
 import pandas as pd
 from .column_types import ColumnType
 
-def merge_datasets(dataset1: "Dataset", dataset2: "Dataset", *args, must_be_disjoint: bool, **kwargs
-                  ) -> Tuple[Dict[str, pd.DataFrame], Dict[str, Dict[str, ColumnType]]]:
+def merge_datasets(dataset1: "Dataset", dataset2: "Dataset", *args, must_be_disjoint: bool,
+                   **kwargs) -> tuple[dict[str, pd.DataFrame], dict[str, dict[str, ColumnType]]]:
     """Merges two datasets together. Calls underlying pd.merge only on needed data groups"""
-    new_data: Dict[str, pd.DataFrame] = {}
-    new_column_types: Dict[str, Dict[str, ColumnType]] = {}
+    new_data: dict[str, pd.DataFrame] = {}
+    new_column_types: dict[str, dict[str, ColumnType]] = {}
     tbs_together = set(dataset1.tables).union(dataset2.tables)
     for tb in tbs_together:
         if tb not in dataset1.tables:
             new_data[tb] = dataset2[tb]
             new_column_types[tb] = dataset2.column_types[tb]
             continue
```

### Comparing `pandas-dataset-0.1.2/pandas_dataset/stats.py` & `pandas-dataset-0.1.3/pandas_dataset/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Statistics for the given dataset. Only applies for numerical columns, plus vetors and categoricals"""
-from typing import Dict
+from __future__ import annotations
 
 import numpy as np
 import pandas as pd
 
 from loguru import logger
 
 from .column_types import ColumnType
 
-def compute_stats(dataset: "Dataset") -> Dict[str, Dict[str, np.ndarray]]:
+def compute_stats(dataset: "Dataset") -> dict[str, dict[str, np.ndarray]]:
     """computes the mins/maxs of all columns of all data groups and returns them as a dict"""
     res = {}
     for dg in dataset.keys():
         res[dg] = {}
         for col in dataset[dg].columns:
             res[dg][col] = _compute_col_stats(dataset[dg][col], dataset.column_types[dg][col])
     return res
```

### Comparing `pandas-dataset-0.1.2/pandas_dataset.egg-info/SOURCES.txt` & `pandas-dataset-0.1.3/pandas_dataset.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 pandas_dataset/column_types.py
 pandas_dataset/dataset.py
 pandas_dataset/dataset_hash_check.py
 pandas_dataset/indexes.py
 pandas_dataset/internal.py
 pandas_dataset/merge.py
 pandas_dataset/stats.py
+pandas_dataset/torch_dataset.py
+pandas_dataset/utils.py
 pandas_dataset.egg-info/PKG-INFO
 pandas_dataset.egg-info/SOURCES.txt
 pandas_dataset.egg-info/dependency_links.txt
 pandas_dataset.egg-info/requires.txt
 pandas_dataset.egg-info/top_level.txt
 pandas_dataset/input_output/__init__.py
 pandas_dataset/input_output/csv_read.py
```

### Comparing `pandas-dataset-0.1.2/setup.py` & `pandas-dataset-0.1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup, find_packages
 from os import path
 
 name = "pandas-dataset"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python Datasets on top of Pandas"
 url = "https://gitlab.com/meehai/pandas-dataset"
 
 loc = path.abspath(path.dirname(__file__))
 with open(f"{loc}/README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-required = ["pandas", "numpy", "loguru", "pyarrow", "natsort"]
+required = ["pandas==2.0.1", "numpy==1.24.1", "loguru==0.7.2", "pyarrow==11.0.0", "natsort==8.4.0",
+            "lovely-tensors==0.1.15", "torch==2.1.1"]
 
 setup(
     name=name,
     version=version,
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
```

