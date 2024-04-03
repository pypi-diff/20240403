# Comparing `tmp/odbc2deltalake-0.7.1.tar.gz` & `tmp/odbc2deltalake-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odbc2deltalake-0.7.1.tar", max compression
+gzip compressed data, was "odbc2deltalake-0.8.0.tar", max compression
```

## Comparing `odbc2deltalake-0.7.1.tar` & `odbc2deltalake-0.8.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1081 2024-03-27 11:24:41.612901 odbc2deltalake-0.7.1/LICENSE
--rw-r--r--   0        0        0     3073 2024-03-27 11:24:41.612901 odbc2deltalake-0.7.1/README.md
--rw-r--r--   0        0        0      126 2024-03-27 11:24:41.612901 odbc2deltalake-0.7.1/odbc2deltalake/__init__.py
--rw-r--r--   0        0        0    37686 2024-03-27 11:24:41.612901 odbc2deltalake-0.7.1/odbc2deltalake/db_to_delta.py
--rw-r--r--   0        0        0       38 2024-03-27 11:24:41.612901 odbc2deltalake-0.7.1/odbc2deltalake/destination/__init__.py
--rw-r--r--   0        0        0     2554 2024-03-27 11:24:41.612901 odbc2deltalake-0.7.1/odbc2deltalake/destination/azure.py
--rw-r--r--   0        0        0     2923 2024-03-27 11:24:41.612901 odbc2deltalake-0.7.1/odbc2deltalake/destination/azure_utils.py
--rw-r--r--   0        0        0     2541 2024-03-27 11:24:41.612901 odbc2deltalake-0.7.1/odbc2deltalake/destination/databricks.py
--rw-r--r--   0        0        0     1196 2024-03-27 11:24:41.612901 odbc2deltalake-0.7.1/odbc2deltalake/destination/destination.py
--rw-r--r--   0        0        0     1592 2024-03-27 11:24:41.612901 odbc2deltalake-0.7.1/odbc2deltalake/destination/file_system.py
--rw-r--r--   0        0        0     5609 2024-03-27 11:24:41.612901 odbc2deltalake-0.7.1/odbc2deltalake/metadata.py
--rw-r--r--   0        0        0     1221 2024-03-27 11:24:41.612901 odbc2deltalake-0.7.1/odbc2deltalake/odbc_utils.py
--rw-r--r--   0        0        0     1851 2024-03-27 11:24:41.612901 odbc2deltalake-0.7.1/odbc2deltalake/query.py
--rw-r--r--   0        0        0       38 2024-03-27 11:24:41.612901 odbc2deltalake-0.7.1/odbc2deltalake/reader/__init__.py
--rw-r--r--   0        0        0     5656 2024-03-27 11:24:41.612901 odbc2deltalake-0.7.1/odbc2deltalake/reader/odbc_reader.py
--rw-r--r--   0        0        0     1527 2024-03-27 11:24:41.612901 odbc2deltalake-0.7.1/odbc2deltalake/reader/reader.py
--rw-r--r--   0        0        0     3622 2024-03-27 11:24:41.612901 odbc2deltalake-0.7.1/odbc2deltalake/reader/spark_reader.py
--rw-r--r--   0        0        0     1976 2024-03-27 11:24:41.612901 odbc2deltalake-0.7.1/odbc2deltalake/sql_glot_utils.py
--rw-r--r--   0        0        0      951 2024-03-27 11:24:41.612901 odbc2deltalake-0.7.1/odbc2deltalake/sql_schema.py
--rw-r--r--   0        0        0        0 2024-03-27 11:24:41.612901 odbc2deltalake-0.7.1/odbc2deltalake/write_utils/__init__.py
--rw-r--r--   0        0        0     4591 2024-03-27 11:24:41.612901 odbc2deltalake-0.7.1/odbc2deltalake/write_utils/restore_pk.py
--rw-r--r--   0        0        0     1373 2024-03-27 11:24:41.612901 odbc2deltalake-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     4012 1970-01-01 00:00:00.000000 odbc2deltalake-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/LICENSE
+-rw-r--r--   0        0        0     3563 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/README.md
+-rw-r--r--   0        0        0      126 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/odbc2deltalake/__init__.py
+-rw-r--r--   0        0        0    41361 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/odbc2deltalake/db_to_delta.py
+-rw-r--r--   0        0        0       38 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/odbc2deltalake/destination/__init__.py
+-rw-r--r--   0        0        0     2554 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/odbc2deltalake/destination/azure.py
+-rw-r--r--   0        0        0     2923 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/odbc2deltalake/destination/azure_utils.py
+-rw-r--r--   0        0        0     2541 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/odbc2deltalake/destination/databricks.py
+-rw-r--r--   0        0        0     1196 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/odbc2deltalake/destination/destination.py
+-rw-r--r--   0        0        0     1592 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/odbc2deltalake/destination/file_system.py
+-rw-r--r--   0        0        0     5392 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/odbc2deltalake/metadata.py
+-rw-r--r--   0        0        0     1221 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/odbc2deltalake/odbc_utils.py
+-rw-r--r--   0        0        0     1851 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/odbc2deltalake/query.py
+-rw-r--r--   0        0        0       38 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/odbc2deltalake/reader/__init__.py
+-rw-r--r--   0        0        0     5656 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/odbc2deltalake/reader/odbc_reader.py
+-rw-r--r--   0        0        0     1527 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/odbc2deltalake/reader/reader.py
+-rw-r--r--   0        0        0     3622 2024-04-03 12:11:08.957293 odbc2deltalake-0.8.0/odbc2deltalake/reader/spark_reader.py
+-rw-r--r--   0        0        0     1976 2024-04-03 12:11:08.961293 odbc2deltalake-0.8.0/odbc2deltalake/sql_glot_utils.py
+-rw-r--r--   0        0        0      951 2024-04-03 12:11:08.961293 odbc2deltalake-0.8.0/odbc2deltalake/sql_schema.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:11:08.961293 odbc2deltalake-0.8.0/odbc2deltalake/write_utils/__init__.py
+-rw-r--r--   0        0        0     4757 2024-04-03 12:11:08.961293 odbc2deltalake-0.8.0/odbc2deltalake/write_utils/restore_pk.py
+-rw-r--r--   0        0        0     1373 2024-04-03 12:11:08.961293 odbc2deltalake-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     4497 1970-01-01 00:00:00.000000 odbc2deltalake-0.8.0/PKG-INFO
```

### Comparing `odbc2deltalake-0.7.1/LICENSE` & `odbc2deltalake-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.7.1/README.md` & `odbc2deltalake-0.8.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -68,13 +68,18 @@
     delta_col: str | None = None
     """The column to use for the delta load. If None, the column will be determined from the source. Should be mostly increasing to make load efficient"""
 
     load_mode: Literal["overwrite", "append", "force_full"] = "append"
     """The load mode to use. Attention: overwrite will not help you build scd2, the history is in the delta table only"""
 
     data_type_map: Mapping[str, ex.DATA_TYPE] = dataclasses.field(
-        default_factory=lambda: _default_type_map.copy()
+        default_factory=lambda: _default_type_map.copy() # defaults to some simple sql server related maps
     )
     """Set this if you want to map stuff like decimal to double before writing to delta. We recommend doing so later in ETL usually"""
 
+    get_target_name: Callable[[InformationSchemaColInfo], str] = dataclasses.field(
+        default_factory=lambda: compat_name # defaults to removing spaces and other characters not allowed by spark
+    )
+    """A method that returns the target name of a column. This is used to map the source column names to the target column names.
+    Use if you want to apply some naming convention or avoid special characters in the target. """
 
 ```
```

### Comparing `odbc2deltalake-0.7.1/odbc2deltalake/db_to_delta.py` & `odbc2deltalake-0.8.0/odbc2deltalake/db_to_delta.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from dataclasses import dataclass
 import dataclasses
 from datetime import datetime, timezone
 from pathlib import Path
-from typing import Iterable, Literal, Mapping, Sequence, TypeVar, cast
-import asyncio
-from pydantic import BaseModel
+from typing import Callable, Iterable, Literal, Mapping, Sequence, TypeVar, cast
 import sqlglot as sg
 from odbc2deltalake.destination.destination import (
     Destination,
 )
 from odbc2deltalake.reader import DataSourceReader
 from .query import sql_quote_name
 from .metadata import (
@@ -18,14 +16,17 @@
     InformationSchemaColInfo,
 )
 import json
 import time
 import sqlglot.expressions as ex
 from .sql_glot_utils import table_from_tuple, union, count_limit_one
 import logging
+import pydantic
+
+is_pydantic_2 = int(pydantic.__version__.split(".")[0]) > 1
 
 logger = logging.getLogger(__name__)
 
 IS_DELETED_COL_NAME = "__is_deleted"
 IS_DELETED_COL_INFO = InformationSchemaColInfo.from_name_type(
     IS_DELETED_COL_NAME, "bit"
 )
@@ -45,14 +46,22 @@
     "datetime2": ex.DataType(this="datetime2(6)"),
     "rowversion": ex.DataType.Type.BIGINT,
     "timestamp": ex.DataType.Type.BIGINT,
 }
 DEFAULT_DATA_TYPE_MAP: Mapping[str, ex.DATA_TYPE] = _default_type_map
 
 
+def compat_name(inf: InformationSchemaColInfo) -> str:
+    invalid_chars = " ,;{}()\n\t="
+    res = inf.column_name
+    for ic in invalid_chars:
+        res = res.replace(ic, "_")
+    return res
+
+
 @dataclass(frozen=True)
 class WriteConfig:
 
     dialect: str = "tsql"
     """The sqlglot dialect to use for the SQL generation against the source"""
 
     primary_keys: list[str] | None = None
@@ -73,14 +82,20 @@
         default_factory=lambda: _default_type_map.copy()
     )
     """Set this if you want to map stuff like decimal to double before writing to delta. We recommend doing so later in ETL usually"""
 
     no_complex_entries_load: bool = False
     """If true, will not load 'strange updates' via OPENJSON. Use if your db does not support OPENJSON or you're fine to get some additional updates in order to reduce complexity"""
 
+    get_target_name: Callable[[InformationSchemaColInfo], str] = dataclasses.field(
+        default_factory=lambda: compat_name
+    )
+    """A method that returns the target name of a column. This is used to map the source column names to the target column names.
+    Use if you want to apply some naming convention or avoid special characters in the target. """
+
 
 def _not_none(v: T | None) -> T:
     if v is None:
         raise ValueError("Value is None")
     return v
 
 
@@ -122,23 +137,26 @@
     *,
     is_deleted: bool | None = None,
     is_full: bool | None = None,
     with_valid_from: bool = False,
     table_alias: str | None = None,
     source_uses_compat: bool,
     data_type_map: Mapping[str, ex.DATA_TYPE] | None = None,
+    get_target_name: Callable[[InformationSchemaColInfo], str] | None,
 ) -> Sequence[ex.Expression]:
+    if get_target_name is None:
+        get_target_name = lambda c: c.column_name
     return (
         [
             _cast(
-                c.compat_name if source_uses_compat else c.column_name,
+                get_target_name(c) if source_uses_compat else c.column_name,
                 c.data_type,
                 table_alias=table_alias,
                 type_map=data_type_map,
-            ).as_(c.compat_name, quoted=True)
+            ).as_(get_target_name(c), quoted=True)
             for c in cols
         ]
         + ([valid_from_expr] if with_valid_from else [])
         + (
             [ex.cast(ex.convert(int(is_deleted)), "bit").as_(IS_DELETED_COL_NAME)]
             if is_deleted is not None
             else []
@@ -185,15 +203,17 @@
 
         source = ODBCReader(source)
     delta_path = destination / "delta"
     cols = get_columns(source, table, dialect=write_config.dialect)
 
     (destination / "meta").mkdir()
     (destination / "meta/schema.json").upload_str(
-        json.dumps([c.dict() for c in cols], indent=4)
+        json.dumps(
+            [c.model_dump() if is_pydantic_2 else c.dict() for c in cols], indent=4
+        )
     )
     if (destination / "delta_load" / DBDeltaPathConfigs.LATEST_PK_VERSION).exists():
         last_version_pk = source.get_local_delta_ops(
             destination / "delta_load" / DBDeltaPathConfigs.LATEST_PK_VERSION
         ).version()
     else:
         last_version_pk = None
@@ -206,25 +226,48 @@
                 datetime.now(tz=timezone.utc) - lock_file_path.modified_time()
             ).total_seconds()
             > 60 * 60
         ):
             lock_file_path.remove()
         lock_file_path.upload_str("")
 
-        delta_col = (
-            next((c for c in cols if c.column_name == write_config.delta_col))
-            if write_config.delta_col
-            else get_delta_col(cols)
-        )
+        if write_config.delta_col:
+            delta_col = next(
+                (c for c in cols if c.column_name == write_config.delta_col), None
+            )
+            if delta_col is None:
+                delta_col = next(
+                    (
+                        c
+                        for c in cols
+                        if write_config.get_target_name(c) == write_config.delta_col
+                    ),
+                    None,
+                )
+            if delta_col is None:
+                raise ValueError(
+                    f"Delta column {write_config.delta_col} not found in source"
+                )
+        else:
+            delta_col = get_delta_col(cols)
 
-        pks = write_config.primary_keys or get_primary_keys(
+        _pks = write_config.primary_keys or get_primary_keys(
             source, table, dialect=write_config.dialect
         )
-        pk_cols = [c for c in cols if c.column_name in pks]
-        assert len(pks) == len(pk_cols), f"Primary keys not found: {pks}"
+        pk_cols: list[InformationSchemaColInfo] = []
+        for pk in _pks:
+            pk_col = next((c for c in cols if c.column_name == pk), None)
+            if pk_col is None:
+                pk_col = next(
+                    (c for c in cols if write_config.get_target_name(c) == pk), None
+                )
+            if pk_col is None:
+                raise ValueError(f"Primary key {pk} not found in source")
+            pk_cols.append(pk_col)
+        assert len(_pks) == len(pk_cols), f"Primary keys not found: {_pks}"
         if (
             not (delta_path / "_delta_log").exists()
             or write_config.load_mode == "overwrite"
         ):
             delta_path.mkdir()
             logger.info(f"{table}: Start Full Load")
             do_full_load(
@@ -250,15 +293,15 @@
                 delta_col=delta_col,
                 cols=cols,
                 write_config=write_config,
             )
         else:
             if (
                 delta_col is None
-                or len(pks) == 0
+                or len(pk_cols) == 0
                 or write_config.load_mode == "force_full"
             ):
                 do_full_load(
                     source,
                     table,
                     delta_path,
                     mode="append",
@@ -334,65 +377,80 @@
     latest_pk_query = union(
         [
             ex.select(
                 *_get_cols_select(
                     cols=pks + [delta_col],
                     table_alias="au",
                     source_uses_compat=True,
+                    get_target_name=write_config.get_target_name,
                 )
             ).from_(table_from_tuple("delta_2", alias="au")),
             (
                 ex.select(
                     *_get_cols_select(
                         cols=pks + [delta_col],
                         table_alias="d1",
                         source_uses_compat=True,
+                        get_target_name=write_config.get_target_name,
                     )
                 )
                 .from_(ex.table_(DBDeltaPathConfigs.DELTA_1_NAME, alias="d1"))
                 .join(
                     ex.table_("delta_2", alias="au2"),
                     ex.and_(
                         *[
-                            ex.column(c.compat_name, "d1", quoted=True).eq(
-                                ex.column(c.compat_name, "au2", quoted=True)
+                            ex.column(
+                                write_config.get_target_name(c), "d1", quoted=True
+                            ).eq(
+                                ex.column(
+                                    write_config.get_target_name(c), "au2", quoted=True
+                                )
                             )
                             for c in pks
                         ]
                     ),
                     join_type="anti",
                 )
             ),
             (
                 ex.select(
                     *_get_cols_select(
                         cols=pks + [delta_col],
                         table_alias="cpk",
                         source_uses_compat=True,
+                        get_target_name=write_config.get_target_name,
                     )
                 )
                 .from_(ex.table_(DBDeltaPathConfigs.PRIMARY_KEYS_TS, alias="cpk"))
                 .join(
                     ex.table_("delta_2", alias="au3"),
                     ex.and_(
                         *[
-                            ex.column(c.compat_name, "cpk", quoted=True).eq(
-                                ex.column(c.compat_name, "au3", quoted=True)
+                            ex.column(
+                                write_config.get_target_name(c), "cpk", quoted=True
+                            ).eq(
+                                ex.column(
+                                    write_config.get_target_name(c), "au3", quoted=True
+                                )
                             )
                             for c in pks
                         ]
                     ),
                     join_type="anti",
                 )
                 .join(
                     ex.table_(DBDeltaPathConfigs.DELTA_1_NAME, alias="au4"),
                     ex.and_(
                         *[
-                            ex.column(c.compat_name, "cpk", quoted=True).eq(
-                                ex.column(c.compat_name, "au4", quoted=True)
+                            ex.column(
+                                write_config.get_target_name(c), "cpk", quoted=True
+                            ).eq(
+                                ex.column(
+                                    write_config.get_target_name(c), "au4", quoted=True
+                                )
                             )
                             for c in pks
                         ]
                     ),
                     join_type="anti",
                 )
             ),
@@ -467,15 +525,17 @@
         reader.get_local_delta_ops(
             destination / "delta_load" / DBDeltaPathConfigs.LATEST_PK_VERSION
         ).version()
         if not simple
         else None
     )
     delta_path = destination / "delta"
-    delta_load_value = _get_latest_delta_value(reader, delta_path, table, delta_col)
+    delta_load_value = _get_latest_delta_value(
+        reader, delta_path, table, delta_col, write_config
+    )
 
     if delta_load_value is None:
         logger.warning(f"{table}: No delta load value, do a full load")
         do_full_load(
             reader,
             table,
             delta_path,
@@ -561,15 +621,17 @@
     cols: list[InformationSchemaColInfo],
     write_config: WriteConfig,
 ):
     logger.info(
         f"{table}: Start Append Only Load with Delta Column {delta_col.column_name}"
     )
     delta_path = destination / "delta"
-    delta_load_value = _get_latest_delta_value(reader, delta_path, table, delta_col)
+    delta_load_value = _get_latest_delta_value(
+        reader, delta_path, table, delta_col, write_config
+    )
 
     criterion = (
         _cast(
             delta_col.column_name,
             delta_col.data_type,
             table_alias="t",
             type_map=write_config.data_type_map,
@@ -593,22 +655,23 @@
 
 
 def _get_latest_delta_value(
     reader: DataSourceReader,
     delta_path: Destination,
     table: table_name_type,
     delta_col: InformationSchemaColInfo,
+    write_config: WriteConfig,
 ):
     reader.local_register_update_view(delta_path, _temp_table(table))
     return reader.local_execute_sql_to_py(
         sg.from_(ex.to_identifier(_temp_table(table))).select(
             ex.func(
                 "MAX",
                 _cast(
-                    delta_col.compat_name,
+                    write_config.get_target_name(delta_col),
                     delta_col.data_type,
                 ),
             ).as_("max_ts")
         )
     )[0]["max_ts"]
 
 
@@ -633,41 +696,47 @@
     )
     delete_query = ex.except_(
         left=ex.select(
             *_get_cols_select(
                 pk_cols,
                 table_alias="lpk",
                 source_uses_compat=True,
+                get_target_name=write_config.get_target_name,
             )
         ).from_(table_from_tuple(LAST_PK_VERSION, alias="lpk")),
         right=ex.select(
             *_get_cols_select(
                 pk_cols,
                 table_alias="cpk",
                 source_uses_compat=True,
+                get_target_name=write_config.get_target_name,
             )
         ).from_(table_from_tuple(DBDeltaPathConfigs.LATEST_PK_VERSION, alias="cpk")),
     )
 
     non_pk_cols = [c for c in cols if c not in pk_cols]
-    non_pk_select = [ex.Null().as_(c.compat_name, quoted=True) for c in non_pk_cols]
+    non_pk_select = [
+        ex.Null().as_(write_config.get_target_name(c), quoted=True) for c in non_pk_cols
+    ]
     deletes_with_schema = union(
         [
             ex.select(
                 *_get_cols_select(
                     pk_cols,
                     table_alias="d1",
                     source_uses_compat=True,
+                    get_target_name=write_config.get_target_name,
                 )
             )
             .select(
                 *_get_cols_select(
                     non_pk_cols,
                     table_alias="d1",
                     source_uses_compat=True,
+                    get_target_name=write_config.get_target_name,
                 ),
                 append=True,
             )
             .select(
                 ex.AtTimeZone(
                     this=ex.CurrentTimestamp(),
                     zone=ex.Literal(this="UTC", is_string=True),
@@ -719,14 +788,15 @@
         *_get_cols_select(
             is_full=None,
             is_deleted=None,
             cols=pk_cols + [delta_col],
             with_valid_from=False,
             data_type_map=write_config.data_type_map,
             source_uses_compat=False,
+            get_target_name=write_config.get_target_name,
         )
     ).from_(table_from_tuple(table))
     pk_ts_reader_sql = pk_ts_col_select.sql(write_config.dialect)
 
     pk_path = destination / f"delta_load/{DBDeltaPathConfigs.PRIMARY_KEYS_TS}"
 
     reader.source_write_sql_to_delta(
@@ -776,55 +846,61 @@
     reader.local_register_view(
         ex.except_(
             left=ex.select(
                 *_get_cols_select(
                     cols=pk_ds_cols,
                     table_alias="pk",
                     source_uses_compat=True,
+                    get_target_name=write_config.get_target_name,
                 )
             ).from_(ex.table_(DBDeltaPathConfigs.PRIMARY_KEYS_TS, alias="pk")),
             right=ex.select(
                 *_get_cols_select(
                     cols=pk_ds_cols,
                     table_alias="lpk",
                     source_uses_compat=True,
+                    get_target_name=write_config.get_target_name,
                 )
             ).from_(table_from_tuple(LAST_PK_VERSION, alias="lpk")),
         ),
         "additional_updates",
     )
 
     sql_query = ex.except_(
         left=ex.select(
             *_get_cols_select(
                 cols=pk_cols,
                 table_alias="au",
                 source_uses_compat=True,
+                get_target_name=write_config.get_target_name,
             )
         ).from_(ex.table_("additional_updates", alias="au")),
         right=ex.select(
             *_get_cols_select(
                 cols=pk_cols,
                 table_alias="d1",
                 source_uses_compat=True,
+                get_target_name=write_config.get_target_name,
             )
         ).from_(table_from_tuple("delta_1", alias="d1")),
     )
     reader.local_register_view(sql_query, "real_additional_updates")
     update_count: int = reader.local_execute_sql_to_py(
         sg.from_("real_additional_updates").select(ex.Count(this=ex.Star()).as_("cnt"))
     )[0]["cnt"]
 
     from .sql_schema import get_sql_type
     from .query import sql_quote_value
 
     jsd = reader.local_execute_sql_to_py(
         sg.from_("real_additional_updates").select(
             *[
-                ex.column(c.compat_name).as_("p" + str(i), quoted=False)
+                ex.column(write_config.get_target_name(c)).as_(
+                    "p" + str(i), quoted=False
+                )
                 for i, c in enumerate(pk_cols)
             ]
         )
     )
 
     def _collate(c: InformationSchemaColInfo):
         if c.data_type.lower() in [
@@ -853,46 +929,50 @@
                 cols,
                 is_full=False,
                 is_deleted=False,
                 with_valid_from=True,
                 table_alias="t",
                 data_type_map=write_config.data_type_map,
                 source_uses_compat=False,
+                get_target_name=write_config.get_target_name,
             )
         )
         sql = (
             ex.select(*selects)
             .from_(table_from_tuple(table, alias="t"))
             .sql(write_config.dialect)
         )
         pk_map = ", ".join(
             [
-                "p" + str(i) + " as " + sql_quote_name(c.compat_name)
+                "p" + str(i) + " as " + sql_quote_name(write_config.get_target_name(c))
                 for i, c in enumerate(pk_cols)
             ]
         )
         return f"""{sql}
         inner join (SELECT {pk_map} FROM OPENJSON({sql_quote_value(js)}) with ({col_defs}) ) ttt
-             on {' AND '.join([f't.{sql_quote_name(c.column_name)} {_collate(c)} = ttt.{sql_quote_name(c.compat_name)}' for c in pk_cols])}
+             on {' AND '.join([f't.{sql_quote_name(c.column_name)} {_collate(c)} = ttt.{sql_quote_name(write_config.get_target_name(c))}' for c in pk_cols])}
         """
 
     if update_count == 0:
         reader.source_write_sql_to_delta(full_sql("[]"), delta_2_path, mode="overwrite")
     elif (
         update_count > 1000
     ) or write_config.no_complex_entries_load:  # many updates. get the smallest timestamp and do "normal" delta, even if there are too many records then
-        reader.source_write_sql_to_delta(full_sql("[]"), delta_2_path, mode="overwrite") # still need to create delta_2_path
+        reader.source_write_sql_to_delta(
+            full_sql("[]"), delta_2_path, mode="overwrite"
+        )  # still need to create delta_2_path
         logger.warning(
             f"{table}: Start delta step 3, load {update_count} strange updates via normal delta load"
         )
         delta_load_value = reader.local_execute_sql_to_py(
             ex.select(
-                ex.func("MIN", ex.column(delta_col.compat_name, quoted=True)).as_(
-                    "min_ts"
-                )
+                ex.func(
+                    "MIN",
+                    ex.column(write_config.get_target_name(delta_col), quoted=True),
+                ).as_("min_ts")
             ).from_(ex.table_("additional_updates", alias="rau"))
         )[0]["min_ts"]
         criterion = _cast(
             delta_col.column_name,
             delta_col.data_type,
             table_alias="t",
             type_map=write_config.data_type_map,
@@ -977,14 +1057,15 @@
                 cols,
                 is_full=False,
                 is_deleted=False,
                 with_valid_from=True,
                 table_alias="t",
                 data_type_map=write_config.data_type_map,
                 source_uses_compat=False,
+                get_target_name=write_config.get_target_name,
             )
         )
         .where(
             *(
                 criterion
                 if criterion is not None and not isinstance(criterion, str)
                 else []
@@ -1037,14 +1118,15 @@
             *_get_cols_select(
                 is_deleted=False,
                 is_full=True,
                 cols=cols,
                 with_valid_from=True,
                 data_type_map=write_config.data_type_map,
                 source_uses_compat=False,
+                get_target_name=write_config.get_target_name,
             )
         )
         .from_(table_from_tuple(table))
         .sql(write_config.dialect)
     )
     if (delta_path / "_delta_log").exists():
         reader.local_register_update_view(delta_path, _temp_table(table))
@@ -1062,16 +1144,20 @@
         return
     logger.info(f"{table}: Full Load done, write meta for delta load")
 
     reader.local_register_update_view(delta_path, _temp_table(table))
     (delta_path.parent / "delta_load").mkdir()
     query = sg.from_(ex.to_identifier(_temp_table(table))).select(
         *(
-            [ex.column(pk.compat_name, quoted=True) for pk in pk_cols]
-            + ([ex.column(delta_col.compat_name, quoted=True)] if delta_col else [])
+            [ex.column(write_config.get_target_name(pk), quoted=True) for pk in pk_cols]
+            + (
+                [ex.column(write_config.get_target_name(delta_col), quoted=True)]
+                if delta_col
+                else []
+            )
         )
     )
     if max_valid_from:
         query = query.where(
             ex.column(VALID_FROM_COL_NAME, quoted=True) > ex.convert(max_valid_from)
         )
     reader.local_execute_sql_to_delta(
```

### Comparing `odbc2deltalake-0.7.1/odbc2deltalake/destination/azure.py` & `odbc2deltalake-0.8.0/odbc2deltalake/destination/azure.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.7.1/odbc2deltalake/destination/azure_utils.py` & `odbc2deltalake-0.8.0/odbc2deltalake/destination/azure_utils.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.7.1/odbc2deltalake/destination/databricks.py` & `odbc2deltalake-0.8.0/odbc2deltalake/destination/databricks.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.7.1/odbc2deltalake/destination/destination.py` & `odbc2deltalake-0.8.0/odbc2deltalake/destination/destination.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.7.1/odbc2deltalake/destination/file_system.py` & `odbc2deltalake-0.8.0/odbc2deltalake/destination/file_system.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.7.1/odbc2deltalake/metadata.py` & `odbc2deltalake-0.8.0/odbc2deltalake/metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,38 +42,30 @@
     type: str
     max_str_length: int | None = None
 
 
 class InformationSchemaColInfo(BaseModel):
     column_name: str
 
-    @property
-    def compat_name(self):
-        invalid_chars = " ,;{}()\n\t="
-        res = self.column_name
-        for ic in invalid_chars:
-            res = res.replace(ic, "_")
-        return res
-
     data_type: str
     column_default: str | None = None
     is_nullable: bool = True
     character_maximum_length: int | None = None
     numeric_precision: int | None = None
     numeric_scale: int | None = None
     datetime_precision: int | None = None
     generated_always_type_desc: Literal[
         "NOT_APPLICABLE", "AS_ROW_START", "AS_ROW_END"
     ] = "NOT_APPLICABLE"
     is_identity: bool = False
 
-    def as_field_type(self, *, compat: bool):
+    def as_field_type(self, *, col_name: Optional[str] = None):
 
         return FieldWithType(
-            name=self.column_name if not compat else self.compat_name,
+            name=col_name or self.column_name,
             type=self.data_type,
             max_str_length=self.character_maximum_length,
         )
 
     @staticmethod
     def from_name_type(name: str, type: str) -> "InformationSchemaColInfo":
         if "(" in type:
```

### Comparing `odbc2deltalake-0.7.1/odbc2deltalake/odbc_utils.py` & `odbc2deltalake-0.8.0/odbc2deltalake/odbc_utils.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.7.1/odbc2deltalake/query.py` & `odbc2deltalake-0.8.0/odbc2deltalake/query.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.7.1/odbc2deltalake/reader/odbc_reader.py` & `odbc2deltalake-0.8.0/odbc2deltalake/reader/odbc_reader.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.7.1/odbc2deltalake/reader/reader.py` & `odbc2deltalake-0.8.0/odbc2deltalake/reader/reader.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.7.1/odbc2deltalake/reader/spark_reader.py` & `odbc2deltalake-0.8.0/odbc2deltalake/reader/spark_reader.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.7.1/odbc2deltalake/sql_glot_utils.py` & `odbc2deltalake-0.8.0/odbc2deltalake/sql_glot_utils.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.7.1/odbc2deltalake/sql_schema.py` & `odbc2deltalake-0.8.0/odbc2deltalake/sql_schema.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.7.1/odbc2deltalake/write_utils/restore_pk.py` & `odbc2deltalake-0.8.0/odbc2deltalake/write_utils/restore_pk.py`

 * *Files 11% similar despite different names*

```diff
@@ -41,16 +41,16 @@
     if sq_valid_from is None or len(sq_valid_from) == 0:
         return False
     latest_full_load_date = sq_valid_from[0][VALID_FROM_COL_NAME]
     reader.local_register_view(
         sg.from_(ex.table_(ex.to_identifier(_temp_table(table)), alias="tr"))
         .select(
             *(
-                [ex.column(c.compat_name, "tr") for c in pk_cols]
-                + [ex.column(delta_col.compat_name, "tr")]
+                [ex.column(write_config.get_target_name(c), "tr") for c in pk_cols]
+                + [ex.column(delta_col.column_name, "tr")]
             )
         )
         .where(
             ex.column(IS_FULL_LOAD_COL_NAME).eq(True)
             and ex.column(VALID_FROM_COL_NAME).eq(
                 ex.Subquery(
                     this=ex.select(ex.func("MAX", ex.column(VALID_FROM_COL_NAME)))
@@ -62,30 +62,32 @@
         "last_full_load",
     )
 
     sq = (
         sg.from_(ex.table_(_temp_table(table), alias="tr"))
         .select(
             *(
-                [ex.column(c.compat_name, "tr") for c in pk_cols]
-                + [ex.column(delta_col.compat_name, "tr")]
+                [ex.column(write_config.get_target_name(c), "tr") for c in pk_cols]
+                + [ex.column(write_config.get_target_name(delta_col), "tr")]
                 + [ex.column(IS_DELETED_COL_NAME, "tr")]
             )
         )
         .where(ex.column(VALID_FROM_COL_NAME) > ex.convert(latest_full_load_date))
     )
     sq = sq.qualify(
         ex.EQ(
             this=ex.Window(
                 this=ex.RowNumber(),
-                partition_by=[ex.column(pk.compat_name) for pk in pk_cols],
+                partition_by=[
+                    ex.column(write_config.get_target_name(pk)) for pk in pk_cols
+                ],
                 order=ex.Order(
                     expressions=[
                         ex.Ordered(
-                            this=ex.column(delta_col.compat_name),
+                            this=ex.column(write_config.get_target_name(delta_col)),
                             desc=True,
                             nulls_first=False,
                         )
                     ]
                 ),
                 over="OVER",
             ),
@@ -101,16 +103,16 @@
             as_=ex.union(
                 left=sq.from_("delta_after_full_load").select("*"),
                 right=sq.from_(ex.table_("last_full_load", "f")).join(
                     ex.table_("delta_after_full_load", "d"),
                     join_type="anti",
                     on=ex.and_(
                         *[
-                            ex.column(c.compat_name, "f").eq(
-                                ex.column(c.compat_name, "d")
+                            ex.column(write_config.get_target_name(c), "f").eq(
+                                ex.column(write_config.get_target_name(c), "d")
                             )
                             for c in pk_cols
                         ]
                     ),
                 ),
                 distinct=False,
             ),
```

### Comparing `odbc2deltalake-0.7.1/pyproject.toml` & `odbc2deltalake-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "odbc2deltalake"
-version = "0.7.1"
+version = "0.8.0"
 description = ""
 authors = ["Adrian Ehrsam <adrian.ehrsam@bmsuisse.ch>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = ">=1.10.0"
 pyodbc = { version = "^5.1.0", optional = true }
 deltalake2db = { version = ">=0.2.1", optional = true }
-arrow-odbc = { version = "^4.1.0", optional = true }
+arrow-odbc = { version = "^5.0.0", optional = true }
 deltalake = { version = ">=0.16.1", optional = true }
 duckdb = { version = ">=0.10.1", optional = true }
 azure-identity = { version = "^1.15.0", optional = true }
 adlfs = { version = "^2024.2.0", optional = true }
 sqlglot = "^23.0.5"
```

### Comparing `odbc2deltalake-0.7.1/PKG-INFO` & `odbc2deltalake-0.8.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: odbc2deltalake
-Version: 0.7.1
+Version: 0.8.0
 Summary: 
 License: MIT
 Author: Adrian Ehrsam
 Author-email: adrian.ehrsam@bmsuisse.ch
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: local
 Provides-Extra: local-azure
 Requires-Dist: adlfs (>=2024.2.0,<2025.0.0) ; extra == "local-azure"
-Requires-Dist: arrow-odbc (>=4.1.0,<5.0.0) ; extra == "local"
+Requires-Dist: arrow-odbc (>=5.0.0,<6.0.0) ; extra == "local"
 Requires-Dist: azure-identity (>=1.15.0,<2.0.0) ; extra == "local-azure"
 Requires-Dist: deltalake (>=0.16.1) ; extra == "local"
 Requires-Dist: deltalake2db (>=0.2.1) ; extra == "local"
 Requires-Dist: duckdb (>=0.10.1) ; extra == "local"
 Requires-Dist: pydantic (>=1.10.0)
 Requires-Dist: pyodbc (>=5.1.0,<6.0.0) ; extra == "local"
 Requires-Dist: sqlglot (>=23.0.5,<24.0.0)
@@ -94,14 +94,19 @@
     delta_col: str | None = None
     """The column to use for the delta load. If None, the column will be determined from the source. Should be mostly increasing to make load efficient"""
 
     load_mode: Literal["overwrite", "append", "force_full"] = "append"
     """The load mode to use. Attention: overwrite will not help you build scd2, the history is in the delta table only"""
 
     data_type_map: Mapping[str, ex.DATA_TYPE] = dataclasses.field(
-        default_factory=lambda: _default_type_map.copy()
+        default_factory=lambda: _default_type_map.copy() # defaults to some simple sql server related maps
     )
     """Set this if you want to map stuff like decimal to double before writing to delta. We recommend doing so later in ETL usually"""
 
+    get_target_name: Callable[[InformationSchemaColInfo], str] = dataclasses.field(
+        default_factory=lambda: compat_name # defaults to removing spaces and other characters not allowed by spark
+    )
+    """A method that returns the target name of a column. This is used to map the source column names to the target column names.
+    Use if you want to apply some naming convention or avoid special characters in the target. """
 
 ```
```

