# Comparing `tmp/tesseract_olap-0.9.1.tar.gz` & `tmp/tesseract_olap-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tesseract_olap-0.9.1.tar", max compression
+gzip compressed data, was "tesseract_olap-0.9.2.tar", max compression
```

## Comparing `tesseract_olap-0.9.1.tar` & `tesseract_olap-0.9.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     2589 2024-03-22 18:36:26.345984 tesseract_olap-0.9.1/PACKAGE.md
--rw-r--r--   0        0        0     1219 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/pyproject.toml
--rw-r--r--   0        0        0      449 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/__init__.py
--rw-r--r--   0        0        0      138 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/backend/__init__.py
--rw-r--r--   0        0        0       79 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/backend/clickhouse/__init__.py
--rw-r--r--   0        0        0     6347 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/backend/clickhouse/backend.py
--rw-r--r--   0        0        0     2714 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/backend/clickhouse/dialect.py
--rw-r--r--   0        0        0    21513 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/backend/clickhouse/sqlbuild.py
--rw-r--r--   0        0        0     1734 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/backend/exceptions.py
--rw-r--r--   0        0        0     3780 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/backend/models.py
--rw-r--r--   0        0        0      299 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/common/__init__.py
--rw-r--r--   0        0        0      219 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/common/exceptions.py
--rw-r--r--   0        0        0     1803 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/common/strings.py
--rw-r--r--   0        0        0      385 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/common/types.py
--rw-r--r--   0        0        0      380 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/exceptions.py
--rw-r--r--   0        0        0      511 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/logiclayer/__init__.py
--rw-r--r--   0        0        0     7684 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/logiclayer/dependencies.py
--rw-r--r--   0        0        0     5464 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/logiclayer/module.py
--rw-r--r--   0        0        0     4416 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/logiclayer/response.py
--rw-r--r--   0        0        0     1170 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/query/__init__.py
--rw-r--r--   0        0        0     2262 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/query/calculations.py
--rw-r--r--   0        0        0     3029 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/query/enums.py
--rw-r--r--   0        0        0     3589 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/query/exceptions.py
--rw-r--r--   0        0        0    10930 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/query/models.py
--rw-r--r--   0        0        0    14395 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/query/queries.py
--rw-r--r--   0        0        0    11555 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/query/requests.py
--rw-r--r--   0        0        0     1721 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/schema/__init__.py
--rw-r--r--   0        0        0     5646 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/schema/aggregators.py
--rw-r--r--   0        0        0     3551 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/schema/csv.py
--rw-r--r--   0        0        0     3697 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/schema/enums.py
--rw-r--r--   0        0        0     3839 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/schema/exceptions.py
--rw-r--r--   0        0        0     2542 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/schema/json.py
--rw-r--r--   0        0        0     9267 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/schema/models.py
--rw-r--r--   0        0        0    11992 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/schema/parser.py
--rw-r--r--   0        0        0     5065 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/schema/public.py
--rw-r--r--   0        0        0     4824 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/schema/schema.xsd
--rw-r--r--   0        0        0    23446 2024-03-22 18:36:26.349984 tesseract_olap-0.9.1/tesseract_olap/schema/traverse.py
--rw-r--r--   0        0        0    18482 2024-03-22 18:36:26.353984 tesseract_olap-0.9.1/tesseract_olap/schema/xml.py
--rw-r--r--   0        0        0       64 2024-03-22 18:36:26.353984 tesseract_olap-0.9.1/tesseract_olap/server/__init__.py
--rw-r--r--   0        0        0      898 2024-03-22 18:36:26.353984 tesseract_olap-0.9.1/tesseract_olap/server/exceptions.py
--rw-r--r--   0        0        0     4508 2024-03-22 18:36:26.353984 tesseract_olap-0.9.1/tesseract_olap/server/schema.py
--rw-r--r--   0        0        0     2968 2024-03-22 18:36:26.353984 tesseract_olap-0.9.1/tesseract_olap/server/server.py
--rw-r--r--   0        0        0     3881 1970-01-01 00:00:00.000000 tesseract_olap-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     2589 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/PACKAGE.md
+-rw-r--r--   0        0        0     1298 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0      478 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/__init__.py
+-rw-r--r--   0        0        0      320 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/backend/__init__.py
+-rw-r--r--   0        0        0     1806 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/backend/cache.py
+-rw-r--r--   0        0        0       79 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/backend/clickhouse/__init__.py
+-rw-r--r--   0        0        0     7219 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/backend/clickhouse/backend.py
+-rw-r--r--   0        0        0     2714 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/backend/clickhouse/dialect.py
+-rw-r--r--   0        0        0    20624 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/backend/clickhouse/sqlbuild.py
+-rw-r--r--   0        0        0     3743 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/backend/models.py
+-rw-r--r--   0        0        0     2731 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/backend/redis.py
+-rw-r--r--   0        0        0      571 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/common/__init__.py
+-rw-r--r--   0        0        0     2461 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/common/strings.py
+-rw-r--r--   0        0        0      385 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/common/types.py
+-rw-r--r--   0        0        0      787 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/exceptions/__init__.py
+-rw-r--r--   0        0        0     1596 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/exceptions/backend.py
+-rw-r--r--   0        0        0     3461 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/exceptions/query.py
+-rw-r--r--   0        0        0     3712 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/exceptions/schema.py
+-rw-r--r--   0        0        0      741 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/exceptions/server.py
+-rw-r--r--   0        0        0      511 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/logiclayer/__init__.py
+-rw-r--r--   0        0        0    10203 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/logiclayer/dependencies.py
+-rw-r--r--   0        0        0     5539 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/logiclayer/module.py
+-rw-r--r--   0        0        0     4468 2024-04-03 16:41:13.935447 tesseract_olap-0.9.2/tesseract_olap/logiclayer/response.py
+-rw-r--r--   0        0        0     1166 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/query/__init__.py
+-rw-r--r--   0        0        0     3318 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/query/enums.py
+-rw-r--r--   0        0        0    12543 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/query/models.py
+-rw-r--r--   0        0        0    12963 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/query/queries.py
+-rw-r--r--   0        0        0    10178 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/query/requests.py
+-rw-r--r--   0        0        0     1721 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/schema/__init__.py
+-rw-r--r--   0        0        0     5432 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/schema/aggregators.py
+-rw-r--r--   0        0        0     3587 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/schema/csv.py
+-rw-r--r--   0        0        0     4744 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/schema/enums.py
+-rw-r--r--   0        0        0     2542 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/schema/json.py
+-rw-r--r--   0        0        0     9528 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/schema/models.py
+-rw-r--r--   0        0        0    11992 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/schema/parser.py
+-rw-r--r--   0        0        0     5184 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/schema/public.py
+-rw-r--r--   0        0        0     4824 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/schema/schema.xsd
+-rw-r--r--   0        0        0    23758 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/schema/traverse.py
+-rw-r--r--   0        0        0    18520 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/schema/xml.py
+-rw-r--r--   0        0        0       64 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/server/__init__.py
+-rw-r--r--   0        0        0     4674 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/server/schema.py
+-rw-r--r--   0        0        0     3542 2024-04-03 16:41:13.939447 tesseract_olap-0.9.2/tesseract_olap/server/server.py
+-rw-r--r--   0        0        0     3960 1970-01-01 00:00:00.000000 tesseract_olap-0.9.2/PKG-INFO
```

### Comparing `tesseract_olap-0.9.1/PACKAGE.md` & `tesseract_olap-0.9.2/PACKAGE.md`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.1/pyproject.toml` & `tesseract_olap-0.9.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tesseract-olap"
-version = "0.9.1"
+version = "0.9.2"
 description = "A simple OLAP library."
 authors = [
   "Francisco Abarzua <francisco@datawheel.us>",
   "Jelmy Hermosilla <jelmy@datawheel.us>",
 ]
 maintainers = [
   "Francisco Abarzua <francisco@datawheel.us>",
@@ -16,32 +16,35 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 clickhouse-cityhash = { version = "^1.0.2.4", optional = true }
 clickhouse-driver = {extras = ["lz4"], version = "^0.2.0", optional = true}
 httpx = ">=0.18.0 <1.0"
 immutables = ">=0.16 <1.0"
 lxml = "^4.6.0"
+orjson = "^3.9.15"
 polars = "^0.20.0"
 PyPika = ">=0.48.0 <1.0"
+redis = {version="^5.0.0", optional = true}
 typing-extensions = ">=3.7.4"
 xlsxwriter = "^3.2.0"
-orjson = "^3.9.15"
 
 [tool.poetry.extras]
 clickhouse = ["clickhouse-driver", "clickhouse-cityhash"]
+redis = ["redis"]
 
 [tool.poetry.group.dev.dependencies]
 clickhouse-cityhash = "^1.0.2.4"
 clickhouse-driver = "^0.2.0"
 fastapi = ">=0.100.0"
+granian = {extras = ["reload"], version = "^1.1.2"}
 logiclayer = "^0.3.0"
 lxml-stubs = "^0.4.0"
 pytest = "^8.0.0"
 pytest-asyncio = "^0.20.0"
+redis = "^5.0.3"
 ruff = "^0.3.0"
 sqlparse = "^0.4.0"
 tomli = "^2.0.1"
-granian = {extras = ["reload"], version = "^1.1.2"}
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tesseract_olap-0.9.1/tesseract_olap/backend/clickhouse/backend.py` & `tesseract_olap-0.9.2/tesseract_olap/backend/clickhouse/backend.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 import logging
-from typing import List, Tuple, Union, overload
-from urllib.parse import urlparse
+from typing import List, Optional, Tuple, Union, overload
 
 import clickhouse_driver as chdr
 import polars as pl
 from clickhouse_driver.dbapi import DatabaseError, InterfaceError
 from clickhouse_driver.dbapi.extras import Cursor, DictCursor, NamedTupleCursor
 from pypika.queries import Selectable
 from typing_extensions import Literal
 
-from tesseract_olap.backend import Backend, ParamManager, Result, Session
-from tesseract_olap.backend.exceptions import UpstreamInternalError, UpstreamNotPrepared
-from tesseract_olap.common import AnyDict, AnyTuple
-from tesseract_olap.query import AnyQuery, DataQuery, MembersQuery
+from tesseract_olap.backend import (
+    Backend,
+    CacheProvider,
+    DummyProvider,
+    ParamManager,
+    Result,
+    Session,
+)
+from tesseract_olap.common import AnyDict, AnyTuple, hide_dsn_password
+from tesseract_olap.exceptions.backend import UpstreamInternalError, UpstreamNotPrepared
+from tesseract_olap.query import AnyQuery, DataQuery, MembersQuery, PaginationIntent
 from tesseract_olap.schema import InlineTable, SchemaTraverser
 
 from .dialect import ClickhouseDataType
 from .sqlbuild import dataquery_sql, membersquery_sql
 
 logger = logging.getLogger("tesseract_olap.backend.clickhouse")
 
@@ -33,16 +39,18 @@
     """
 
     dsn: str
 
     def __init__(self, dsn: str) -> None:
         self.dsn = dsn
 
-    def new_session(self):
-        return ClickhouseSession(self.dsn)
+    def new_session(self, cache: Optional["CacheProvider"] = None, **kwargs):
+        if cache is None:
+            cache = DummyProvider()
+        return ClickhouseSession(self.dsn, cache=cache, **kwargs)
 
     def ping(self) -> bool:
         """Checks if the current connection is working correctly."""
         with self.new_session() as session:
             with session.cursor() as cursor:
                 cursor.execute("SELECT 1")
                 result = cursor.fetchone()
@@ -75,74 +83,92 @@
 
         observed: dict[str, set[str]] = {item[0]: set(item[1]) for item in result}
 
         assert tables == observed
 
 
 class ClickhouseSession(Session):
-    def __init__(self, dsn: str) -> None:
+    def __init__(self, dsn: str, *, cache: "CacheProvider"):
+        self.cache = cache
         self.dsn = dsn
 
-    def __repr__(self) -> str:
-        dsn = urlparse(self.dsn)
-        if dsn.password is not None:
-            dsn = dsn._replace(password="***")
-        return f"{type(self).__name__}(dsn='{dsn.geturl()}')"
+    def __repr__(self):
+        return f"{type(self).__name__}(dsn='{hide_dsn_password(self.dsn)}')"
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         result = super().__exit__(exc_type, exc_val, exc_tb)
 
         if exc_type is InterfaceError:
             raise UpstreamNotPrepared(*exc_val.args).with_traceback(exc_tb)
         if exc_type is DatabaseError:
             raise UpstreamInternalError(*exc_val.args).with_traceback(exc_tb)
 
         return result
 
     def connect(self):
+        self._cache = self.cache.connect()
         self._connection = chdr.connect(dsn=self.dsn, compression="lz4")
 
     def close(self):
+        self._cache.close()
         self._connection.close()
+        delattr(self, "_cache")
+        delattr(self, "_connection")
 
     def fetch(self, query: AnyQuery, **kwargs) -> Result[List[AnyTuple]]:
         qbuilder, meta = _query_to_builder(query)
 
         with self.cursor() as cursor:
             _tables_into_cursor(cursor, meta.tables)
             cursor.execute(qbuilder.get_sql(), parameters=meta.params)
             data = cursor.fetchall()
-            columns = tuple(cursor.columns_with_types or [])
 
-        return Result(data or [], columns)
+        return Result(data or [], query.columns)
 
-    def fetch_dataframe(self, query: AnyQuery, **kwargs) -> Result[pl.DataFrame]:
+    def _fetch_dataframe(self, query: AnyQuery, **kwargs) -> Result[pl.DataFrame]:
         qbuilder, meta = _query_to_builder(query)
 
         with self.cursor() as cursor:
             _tables_into_cursor(cursor, meta.tables)
             data = pl.read_database(
                 query=qbuilder.get_sql(),
                 connection=cursor,
                 execute_options={"parameters": meta.params},
             )
-            columns = tuple(cursor.columns_with_types or [])
 
-        return Result(data, columns)
+        return Result(data, query.columns)
+
+    def fetch_dataframe(self, query: AnyQuery, **kwargs) -> Result[pl.DataFrame]:
+        pagi = query.pagination
+        if pagi.limit > 0 or pagi.offset > 0:
+            query.pagination = PaginationIntent(0, 0)
+
+        result = self._cache.retrieve(query)
+        if result is None:
+            logger.debug(f"Cache: {type(self.cache).__name__} MISS {query.key}")
+            result = self._fetch_dataframe(query, **kwargs)
+            self._cache.store(query, result)
+        else:
+            logger.debug(f"Cache: {type(self.cache).__name__} HIT {query.key}")
+
+        if pagi.limit > 0 or pagi.offset > 0:
+            query.pagination = pagi
+            result.data = result.data.slice(pagi.offset, pagi.limit or None)
+
+        return result
 
     def fetch_records(self, query: AnyQuery, **kwargs) -> Result[List[AnyDict]]:
         qbuilder, meta = _query_to_builder(query)
 
         with self.cursor("Dict") as cursor:
             _tables_into_cursor(cursor, meta.tables)
             cursor.execute(qbuilder.get_sql(), parameters=meta.params)
             data = cursor.fetchall()
-            columns = tuple(cursor.columns_with_types or [])
 
-        return Result(data, columns)
+        return Result(data, query.columns)
 
     @overload
     def cursor(self) -> "TypedCursor": ...
     @overload
     def cursor(self, format_: Literal["Tuple"]) -> "TypedCursor": ...
     @overload
     def cursor(self, format_: Literal["Dict"]) -> "TypedDictCursor": ...
```

### Comparing `tesseract_olap-0.9.1/tesseract_olap/backend/clickhouse/dialect.py` & `tesseract_olap-0.9.2/tesseract_olap/backend/clickhouse/dialect.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.1/tesseract_olap/backend/clickhouse/sqlbuild.py` & `tesseract_olap-0.9.2/tesseract_olap/backend/clickhouse/sqlbuild.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,20 +17,17 @@
     Field,
     Function,
     PyformatParameter,
     ValueWrapper,
 )
 
 from tesseract_olap.backend import ParamManager
-from tesseract_olap.common import shorthash
 from tesseract_olap.query import (
     Comparison,
     DataQuery,
-    HierarchyField,
-    LevelField,
     LogicOperator,
     MeasureField,
     MembersQuery,
     NumericConstraint,
     RestrictionAge,
 )
 from tesseract_olap.schema import Interpreter, MemberType, models
@@ -108,15 +105,15 @@
                 # apply cuts to fact table to reduce amount of data to aggregate later
                 caster = lvlfi.level.type_caster
                 members_include = sorted(caster(mem) for mem in lvlfi.members_include)
                 members_exclude = sorted(caster(mem) for mem in lvlfi.members_exclude)
 
                 lvl_columns = [
                     Field(column, table=table_dim, alias=f"lv_{alias}")
-                    for column, _, alias in _yield_lvlfi_columns(lvlfi, locale)
+                    for column, _, alias in lvlfi.iter_columns(locale)
                 ]
 
                 if table_dim is table_fact:
                     if len(members_include) > 0:
                         qb = qb.where(
                             table_fact.field(lvlfi.key_column).isin(members_include)
                         )
@@ -229,42 +226,46 @@
     def dataquery_tgroup_sql(tcore: Selectable) -> Selectable:
         """
         Builds the query which will perform the grouping by drilldown members, and
         then the aggregation over the resulting groups.
         """
         qb: QueryBuilder = ClickHouseQuery.from_(tcore)
 
-        select_fields = chain(
-            # Apply aggregations over quantitative fields to get measures
-            (_get_aggregate(tcore, item) for item in query.fields_quantitative if isinstance(item.measure, models.Measure)),
-
-            # Pass the representative level columns to later use to enrich
-            (Field(f"lv_{alias}", alias=name, table=tcore)
-            for hiefi in query.fields_qualitative
-            for _, name, alias in _yield_hiefi_columns(hiefi, locale)
-            if hiefi.has_drilldowns),
+        # Apply aggregations over quantitative fields to get measures
+        measure_fields = (
+            _get_aggregate(tcore, msrfi)
+            for msrfi in query.fields_quantitative
+            if isinstance(msrfi.measure, models.Measure)
         )
-        qb = qb.select(*select_fields)
 
         # Creates Ranking columns using window functions
         rank_fields = (
-            an.Rank(alias="%s Ranking" % item.name)\
-              .orderby(Field(item.name),
-                       order=Order.asc if item.with_ranking == "asc" else Order.desc)
-            for item in query.fields_quantitative
-            if item.with_ranking is not None
+            an.Rank(alias=f"{msrfi.name} Ranking")\
+              .orderby(Field(msrfi.name),
+                       order=Order.asc if msrfi.with_ranking == "asc" else Order.desc)
+            for msrfi in query.fields_quantitative
+            if msrfi.with_ranking is not None
         )
-        qb = qb.select(*rank_fields)
+
+        # Pass the representative level columns to later use to enrich
+        level_fields = chain(
+            (Field(f"lv_{alias}", alias=name, table=tcore)
+            for hiefi in query.fields_qualitative
+            for lvlfi in hiefi.drilldown_levels
+            for _, name, alias in lvlfi.iter_columns(locale)),
+        )
+
+        qb = qb.select(*measure_fields, *rank_fields, *level_fields)
 
         # Use the representative levels, so the data gets aggregated
         groupby_fields = (
             tcore.field(f"lv_{alias}")
             for hiefi in query.fields_qualitative
-            for _, _, alias in _yield_hiefi_columns(hiefi, locale)
-            if hiefi.has_drilldowns
+            for lvlfi in hiefi.drilldown_levels
+            for _, _, alias in lvlfi.iter_columns(locale)
         )
         qb = qb.groupby(*groupby_fields)
 
         # Default sorting directions
         # The results are sorted by the ID column of each drilldown
         order = Order.asc
         orderby = (
@@ -274,40 +275,41 @@
         )
         # Flag to know an user-defined sorting field hasn't been set
         sort_field = None
 
         # Apply user-defined filters on aggregated data
         for msrfi in query.fields_quantitative:
             # skip field if no filter is defined
-            if not msrfi.constraint1:
+            if not msrfi.constraint:
                 continue
 
             # create criterion for first constraint
             column = Field(msrfi.name)
-            criterion = _get_filter_criterion(column, msrfi.constraint1)
+            criterion = _get_filter_criterion(column, msrfi.constraint[0])
             # add second constraint to criterion if defined
-            if msrfi.constraint2:
-                criterion2 = _get_filter_criterion(column, msrfi.constraint2)
-                if msrfi.joint == LogicOperator.AND:
+            if len(msrfi.constraint) == 3:
+                criterion2 = _get_filter_criterion(column, msrfi.constraint[2])
+                if msrfi.constraint[1] == LogicOperator.AND:
                     criterion &= criterion2
-                elif msrfi.joint == LogicOperator.OR:
+                elif msrfi.constraint[1] == LogicOperator.OR:
                     criterion |= criterion2
             qb = qb.having(criterion)
 
         for hiefi in query.fields_qualitative:
             # skip field if is not a drilldown
             if not hiefi.has_drilldowns:
                 continue
 
             # User-defined sorting directions for Properties
             if sort_field is None and query.sorting:
                 sort_field, sort_order = query.sorting
                 # TODO: this method could still use a drilldown for sorting, check
                 field_finder = (tcore.field(f"lv_{alias}")
-                                for column, name, alias in _yield_hiefi_columns(hiefi, locale)
+                                for lvlfi in hiefi.drilldown_levels
+                                for _, name, alias in lvlfi.iter_columns(locale)
                                 if name == sort_field)
                 sort_field = next(field_finder, None)
                 if sort_field is not None:
                     order = Order.asc if sort_order == "asc" else Order.desc
                     orderby = chain((sort_field,), orderby)
 
         # User-defined sorting directions for Measures
@@ -521,31 +523,7 @@
         return field.lte(scalar)
     elif comparison == Comparison.EQ:
         return field.eq(scalar)
     elif comparison == Comparison.NEQ:
         return field.ne(scalar)
 
     raise NameError(f"Invalid criterion type: {comparison}")
-
-
-def _yield_hiefi_columns(hiefi: HierarchyField, locale: str):
-    """Generates pairs of (column name, column alias) for all fields related to
-    a HierarchyField object.
-
-    This comprises Drilldown Labels and IDs, and its requested Properties.
-    """
-    for lvlfi in hiefi.drilldown_levels:
-        yield from _yield_lvlfi_columns(lvlfi, locale)
-
-
-def _yield_lvlfi_columns(lvlfi: LevelField, locale: str):
-    name = lvlfi.level.name
-    key_column = lvlfi.level.key_column
-    name_column = lvlfi.level.get_name_column(locale)
-    if name_column is None:
-        yield key_column, name, shorthash(name + key_column)
-    else:
-        yield key_column, f"{name} ID", shorthash(name + key_column)
-        yield name_column, name, shorthash(name + name_column)
-    for propty in lvlfi.properties:
-        propty_column = propty.get_key_column(locale)
-        yield propty_column, propty.name, shorthash(propty.name + propty_column)
```

### Comparing `tesseract_olap-0.9.1/tesseract_olap/backend/exceptions.py` & `tesseract_olap-0.9.2/tesseract_olap/exceptions/backend.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 """Backend exceptions module.
 
 The errors in this module refer to problems during the retrieval of data from
 the backend, but happening at the backend plugin side of the code.
 These should be extended/raised from inside the Backend module.
 """
 
-from tesseract_olap.common import BaseError
-
-
-class BackendError(BaseError):
-    """Base class for exceptions in `tesseract_olap.backend` module."""
-
-    code = 500
+from . import BackendError
 
 
 class UpstreamNotPrepared(BackendError):
     """This error happens when there's a connection attempt done against a
     backend which is unable to accept connections.
 
     The user must avoid race conditions and ensure connections and cursors are
```

### Comparing `tesseract_olap-0.9.1/tesseract_olap/backend/models.py` & `tesseract_olap-0.9.2/tesseract_olap/backend/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,34 +3,31 @@
 This module contains abstract definitions for the interfaces of the Backend
 class. Tesseract is compatible with any kind of data source as long as there's a
 backend class that adapts the Query and the Results to the defined interface.
 """
 
 import abc
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Dict, Generic, List, Optional, Tuple
+from typing import TYPE_CHECKING, Dict, Generic, List, Optional
 
 import polars as pl
 
 from tesseract_olap.common import T, shorthash
+from tesseract_olap.schema import MemberType
 
 if TYPE_CHECKING:
     from tesseract_olap.common import AnyDict, AnyTuple
     from tesseract_olap.query import AnyQuery
     from tesseract_olap.schema import InlineTable, SchemaTraverser
 
 
-@dataclass(order=False, eq=False)
+@dataclass(eq=False, order=False)
 class Result(Generic[T]):
     data: T
-    columns: Tuple[Tuple[str, str], ...]
-
-    @property
-    def column_types(self):
-        return dict(self.columns)
+    columns: Dict[str, MemberType]
 
 
 class Backend(abc.ABC):
     """Base class for database backends compatible with Tesseract."""
 
     @abc.abstractmethod
     def new_session(self, **kwargs) -> "Session":
@@ -63,15 +60,15 @@
         self.connect()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
     @abc.abstractmethod
-    def connect(self):
+    def connect(self) -> None:
         """Establishes the connection to the backend server.
 
         This operation is called automatically when the Session instance is
         used within a context manager.
         """
         raise NotImplementedError()
```

### Comparing `tesseract_olap-0.9.1/tesseract_olap/common/strings.py` & `tesseract_olap-0.9.2/tesseract_olap/common/strings.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,50 @@
 from functools import lru_cache
 from hashlib import md5
-from typing import Mapping, Optional, Union, overload
+from typing import Any, Mapping, Optional, Union, overload
+from urllib.parse import urlparse
 
 from typing_extensions import Literal
 
-
-NAN_VALUES = frozenset((
-    '-1.#IND', '1.#QNAN', '1.#IND', '-1.#QNAN', '#N/A N/A', '#N/A', 'N/A',
-    'n/a', '#NA', 'NULL', 'null', 'NaN', '-NaN', 'nan', '-nan'
-))
+NAN_VALUES = frozenset(
+    (
+        "-1.#IND",
+        "1.#QNAN",
+        "1.#IND",
+        "-1.#QNAN",
+        "#N/A N/A",
+        "#N/A",
+        "N/A",
+        "n/a",
+        "#NA",
+        "NULL",
+        "null",
+        "NaN",
+        "-NaN",
+        "nan",
+        "-nan",
+    )
+)
 
 TRUTHY_STRINGS = frozenset(("1", "true", "on", "y", "yes"))
 FALSEY_STRINGS = frozenset(("0", "false", "off", "n", "no", "none", ""))
 
 
 @overload
 def get_localization(
     dictionary: Mapping[str, str],
     locale: str,
-) -> Optional[str]:
-    ...
+) -> Optional[str]: ...
 @overload
 def get_localization(
     dictionary: Mapping[str, str],
     locale: str,
     *,
     force: Literal[True],
-) -> str:
-    ...
+) -> str: ...
 def get_localization(
     dictionary: Mapping[str, str],
     locale: str,
     *,
     force: bool = False,
 ) -> Optional[str]:
     """Attempts to return the value from a dictionary of terms, where the locale
@@ -44,25 +57,45 @@
         locale = locale[0:2]
     if locale not in dictionary:
         locale = "xx"
     return dictionary[locale] if force else dictionary.get(locale)
 
 
 @lru_cache(128)
-def shorthash(string: str):
+def shorthash(string: str) -> str:
     return str(md5(string.encode("utf-8")).hexdigest())[:8]
 
 
 def numerify(string: Union[str, bytes]):
     string = string if isinstance(string, str) else str(string)
     if string in NAN_VALUES:
         return float("nan")
     _f = float(string)
     return int(string) if string.isnumeric() and int(string) == _f else _f
 
 
-def is_numeric(string: Union[str, bytes]):
+def is_numeric(string: Union[str, bytes]) -> bool:
     try:
         float(string)
         return True
     except ValueError:
         return string in NAN_VALUES
+
+
+def hide_dsn_password(dsn: str) -> str:
+    url = urlparse(dsn)
+    if url.password is not None:
+        url = url._replace(password="***")
+    return url.geturl()
+
+
+def stringify(obj: Any) -> str:
+    if isinstance(obj, (list, set, tuple)):
+        return repr(sorted(obj))
+
+    if isinstance(obj, Mapping):
+        return "{%s}" % ", ".join(
+            f"{repr(key)}: {repr(value)}"
+            for key, value in sorted(obj.items(), key=lambda x: x[0])
+        )
+
+    return repr(obj)
```

### Comparing `tesseract_olap-0.9.1/tesseract_olap/logiclayer/module.py` & `tesseract_olap-0.9.2/tesseract_olap/logiclayer/module.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,20 +41,20 @@
 
     def __init__(self, server: OlapServer, **kwargs):
         super().__init__(**kwargs)
         self.server = server
         self.debug = kwargs.get("debug", False)
 
     @classmethod
-    def new(cls, connection: str, schema: Union[str, Path]):
+    def new(cls, connection: str, schema: Union[str, Path], cache: str = ""):
         """Creates a new :class:`TesseractModule` instance from the strings with
         the path to the schema file (or the schema content itself), and with the
         connection string to the backend.
         """
-        server = OlapServer(connection, schema)
+        server = OlapServer(backend=connection, schema=schema, cache=cache)
         return cls(server)
 
     def get_debug_meta(self):
         """Generates some extra info if the app is running in debug mode."""
         if not self.debug:
             return False
 
@@ -136,11 +136,11 @@
     def debug_schema(self):
         """Returns the true internal schema, used to validate the requests."""
         return dataclasses.asdict(self.server.raw_schema)
 
     @ll.exception_handler(TesseractError)
     def exc_tesseracterror(self, request: Request, exc: TesseractError):
         if self.debug or isinstance(exc, QueryError):
-            content = {"type": type(exc).__name__, "detail": exc.message}
+            content = {"error": True, "type": type(exc).__name__, "detail": exc.message}
         else:
-            content = {"detail": "Backend error"}
+            content = {"error": True, "detail": "Backend error"}
         return JSONResponse(content, status_code=exc.code)
```

### Comparing `tesseract_olap-0.9.1/tesseract_olap/logiclayer/response.py` & `tesseract_olap-0.9.2/tesseract_olap/logiclayer/response.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from fastapi.responses import FileResponse, Response
 from starlette.background import BackgroundTask
 from typing_extensions import Literal
 
 from tesseract_olap.backend import Result
 from tesseract_olap.common import AnyDict
 from tesseract_olap.query import DataQuery, DataRequest, MembersQuery, MembersRequest
-from tesseract_olap.schema import Annotations, PublicProperty
+from tesseract_olap.schema import Annotations, MemberType, PublicProperty
 
 
 class ResponseFormat(str, Enum):
     csv = "csv"
     excel = "xlsx"
     jsonarrays = "jsonarrays"
     jsonrecords = "jsonrecords"
@@ -47,15 +47,15 @@
 @dataclass(eq=False, order=False)
 class MembersResModel:
     name: str
     caption: str
     depth: int
     annotations: Annotations
     properties: List["PublicProperty"]
-    dtypes: Mapping[str, str]
+    dtypes: Mapping[str, MemberType]
     members: List[AnyDict]
 
 
 def data_response(
     params: DataRequest,
     query: DataQuery,
     result: Result[pl.DataFrame],
@@ -92,37 +92,39 @@
         elif extension is ResponseFormat.parquet:
             df.write_parquet(tmp_file.name)
 
         else:
             raise HTTPException(406, f"Requested format is not supported: {extension}")
 
     kwargs["background"] = BackgroundTask(os.unlink, tmp_file.name)
-    kwargs["filename"] = f"data_{params.request_id}.{extension}"
+    kwargs["filename"] = f"data_{query.key}.{extension}"
 
     return FileResponse(tmp_file.name, **kwargs)
 
 
 def members_response(
     params: MembersRequest,
     query: MembersQuery,
     result: Result[List[AnyDict]],
 ):
+    locale = query.locale
     level = query.hiefield.deepest_level.level
+    with_parents = params.options["parents"]
 
     return MembersResModel(
         name=level.name,
-        caption=level.get_caption(query.locale),
+        caption=level.get_caption(locale),
         depth=level.depth,
         annotations=dict(level.annotations),
         properties=[
-            PublicProperty.from_entity(item, query.locale) for item in level.properties
+            PublicProperty.from_entity(item, locale) for item in level.properties
         ],
-        dtypes=result.column_types,
+        dtypes=result.columns,
         members=[nest_keys(row) for row in result.data]
-        if params.options["parents"]
+        if with_parents
         else result.data,
     )
 
 
 def nest_keys(item: dict):
     return build_member(
         key=item.pop("key"),
```

### Comparing `tesseract_olap-0.9.1/tesseract_olap/query/__init__.py` & `tesseract_olap-0.9.2/tesseract_olap/query/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .enums import (
+    AnyOrder,
     Comparison,
     LogicOperator,
     Membership,
     Order,
     RestrictionAge,
     RestrictionScale,
 )
@@ -15,28 +16,28 @@
     MeasureField,
     MembershipConstraint,
     NumericConstraint,
     PaginationIntent,
     SortingIntent,
     TimeRestriction,
 )
-from .queries import AnyQuery, ColumnEntity, DataQuery, MembersQuery
+from .queries import AnyQuery, DataQuery, MembersQuery
 from .requests import (
     AnyRequest,
     DataRequest,
     DataRequestParams,
     MembersRequest,
     MembersRequestParams,
     RequestWithRoles,
 )
 
 __all__ = (
+    "AnyOrder",
     "AnyQuery",
     "AnyRequest",
-    "ColumnEntity",
     "Comparison",
     "CutIntent",
     "DataQuery",
     "DataRequest",
     "DataRequestParams",
     "FilterCondition",
     "FilterIntent",
```

### Comparing `tesseract_olap-0.9.1/tesseract_olap/query/enums.py` & `tesseract_olap-0.9.2/tesseract_olap/query/enums.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 from enum import Enum
-from typing import Optional
+from typing import Optional, Union
+
+from typing_extensions import Literal
 
 
 class Comparison(str, Enum):
     """Comparison Enum.
 
     Defines the available value comparison operations.
     """
+
     GT = "gt"
     GTE = "gte"
     LT = "lt"
     LTE = "lte"
     EQ = "eq"
     NEQ = "neq"
 
     @classmethod
     def from_str(cls, value: str):
-        value = value.lower().strip()
+        value = value.strip().upper()
         try:
-            return next((item for item in cls if item == COMPARISON_SYMBOL.get(value, value)))
-        except StopIteration:
+            return COMPARISON_SYMBOL.get(value) or cls[value]
+        except KeyError:
             raise ValueError(f"Invalid Comparison value: {value}") from None
 
 
 COMPARISON_SYMBOL = {
     ">": Comparison.GT,
     ">=": Comparison.GTE,
     "<": Comparison.LT,
@@ -35,88 +38,112 @@
 
 
 class Order(str, Enum):
     """Order direction Enum.
 
     Defines a direction to use in a sorting operation.
     """
+
     ASC = "asc"
     DESC = "desc"
 
+    def __repr__(self):
+        return f"{type(self).__name__}.{self.name}"
+
+    def __str__(self):
+        return self.value
+
     @classmethod
     def from_str(cls, value: Optional[str]):
-        return next((item for item in cls if item == value), cls.ASC)
+        value = str(value).strip().upper()
+        try:
+            return cls[value]
+        except KeyError:
+            return cls.ASC
+
+
+AnyOrder = Union[Literal["asc", "desc"], "Order"]
 
 
 class Membership(Enum):
     """Membership Enum.
 
     Defines the membership of a value to a set."""
+
     IN = "in"
     NIN = "nin"
 
     @classmethod
     def from_str(cls, value: str):
+        value = value.strip().upper()
         try:
-            return next((item for item in cls if item.value == value))
-        except StopIteration:
+            return cls[value]
+        except KeyError:
             raise ValueError(f"Invalid Membership value: {value}") from None
 
 
 class LogicOperator(str, Enum):
     """Logical connector Enum.
 
     Defines logical operations between conditional predicates.
     """
+
     AND = "and"
     OR = "or"
     XOR = "xor"
 
-    def __str__(self) -> str:
-        return self.value
+    def __repr__(self):
+        return f"{type(self).__name__}.{self.name}"
 
-    def __repr__(self) -> str:
-        return f"LogicOperator.{self.name}"
+    def __str__(self):
+        return self.value
 
     @classmethod
     def from_str(cls, value: str):
+        value = value.strip().upper()
         try:
-            return next((item for item in cls if item.value == value))
-        except StopIteration:
+            return cls[value]
+        except KeyError:
             raise ValueError(f"Invalid LogicOperator value: {value}") from None
 
 
 class RestrictionScale(str, Enum):
     YEAR = "year"
     QUARTER = "quarter"
     MONTH = "month"
     WEEK = "week"
     DAY = "day"
 
-    def __str__(self) -> str:
+    def __repr__(self):
+        return f"{type(self).__name__}.{self.name}"
+
+    def __str__(self):
         return self.value
 
     @classmethod
     def from_str(cls, value: str):
-        assert value != "", "Invalid RestrictionScale: no value provided"
+        assert value, "Invalid RestrictionScale: no value provided"
         try:
-            value = value.lower()
-            return next((item for item in cls if item.value == value))
-        except StopIteration:
+            value = value.strip().upper()
+            return cls[value]
+        except KeyError:
             raise ValueError(f"Invalid RestrictionScale value: {value}") from None
 
 
 class RestrictionAge(str, Enum):
     LATEST = "latest"
     OLDEST = "oldest"
 
-    def __str__(self) -> str:
+    def __repr__(self):
+        return f"{type(self).__name__}.{self.name}"
+
+    def __str__(self):
         return self.value
 
     @classmethod
     def from_str(cls, value: str):
-        assert value != "", "Invalid RestrictionAge: no value provided"
+        assert value, "Invalid RestrictionAge: no value provided"
         try:
-            value = value.lower()
-            return next((item for item in cls if item.value == value))
-        except StopIteration:
+            value = value.strip().upper()
+            return cls[value]
+        except KeyError:
             raise ValueError(f"Invalid RestrictionAge value: {value}") from None
```

### Comparing `tesseract_olap-0.9.1/tesseract_olap/query/exceptions.py` & `tesseract_olap-0.9.2/tesseract_olap/exceptions/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,17 @@
 
 The errors in this module refer to problems during the retrieval of data from
 the backend, but happening at the core side of the code.
 """
 
 from typing import Optional
 
-from tesseract_olap.common import Array, BaseError
+from tesseract_olap.common import Array
 
-
-class QueryError(BaseError):
-    """Base class for exceptions in `tesseract_olap.query` module."""
-    code = 400
+from . import QueryError
 
 
 class InvalidQuery(QueryError):
     """This error occurs when a query is misconstructed.
 
     Can be raised before or after a request is made against a data server.
     """
@@ -27,22 +24,21 @@
 
     As this is entirely an user issue, should be informed to the user, but not
     necessarily to the administrator.
     """
 
     def __init__(self, param: str, detail: Optional[str]) -> None:
         super().__init__(
-            f"Query parameter '{param}' set incorrectly" +\
-            ("" if detail is None else f": {detail}")
+            f"Query parameter '{param}' set incorrectly"
+            + ("" if detail is None else f": {detail}")
         )
 
 
 class InvalidEntityName(InvalidQuery):
-    """This error occurs when a query asks for an object missing in the schema.
-    """
+    """This error occurs when a query asks for an object missing in the schema."""
 
     def __init__(self, node: str, name: str) -> None:
         super().__init__(
             f"Failed attempt to get a {node} object with name '{name}': "
             f"Entity doesn't exist"
         )
 
@@ -78,36 +74,35 @@
     """This error occurs when a format used to retrieve data is not supported by
     the upstream server.
 
     Should be raised before the query is executed against the upstream server.
     """
 
     def __init__(self, extension: str) -> None:
-        super().__init__(
-            f"Format '{extension}' is not supported by the server."
-        )
+        super().__init__(f"Format '{extension}' is not supported by the server.")
 
 
 class MissingMeasures(InvalidQuery):
     """This error occurs when a measure is being specified in part of the query,
     but it's not included in the list of measures for the query.
 
     Should be raised before the query is executed against the upstream server.
     """
 
     def __init__(self, feature: str, measures: Array[str]):
         super().__init__(
-            f"Requesting {feature} for measures not in the request: " +
-            ", ".join(measures)
+            f"Requesting {feature} for measures not in the request: "
+            + ", ".join(measures)
         )
 
 
 class NotAuthorized(InvalidQuery):
     """The roles provided don't match the roles needed to access some of the
     requested parameters.
 
     Should be raised before the query is executed against the upstream server.
     """
+
     code = 403
 
     def __init__(self) -> None:
         super().__init__("Request doesn't count with the necessary permissions.")
```

### Comparing `tesseract_olap-0.9.1/tesseract_olap/query/models.py` & `tesseract_olap-0.9.2/tesseract_olap/query/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """Query-related internal structs module.
 
 This module contains data-storing structs, used mainly on the query and backend
 modules.
 """
 
-import dataclasses
+import dataclasses as dcls
 from typing import Dict, FrozenSet, Iterable, NamedTuple, Optional, Set, Tuple, Union
 
 from typing_extensions import Literal
 
 from tesseract_olap.common import Array, Prim, shorthash
 from tesseract_olap.schema import (
     AnyMeasure,
     CalculatedMeasure,
     DimensionTraverser,
     HierarchyTraverser,
     LevelTraverser,
+    MemberType,
     PropertyTraverser,
 )
 
 from .enums import (
+    AnyOrder,
     Comparison,
     LogicOperator,
     Membership,
     Order,
     RestrictionAge,
     RestrictionScale,
 )
@@ -33,22 +35,23 @@
 MembershipConstraint = Tuple[Membership, Array[str]]
 
 SingleFilterCondition = Tuple[NumericConstraint]
 DoubleFilterCondition = Tuple[NumericConstraint, ConditionOperator, NumericConstraint]
 FilterCondition = Union[SingleFilterCondition, DoubleFilterCondition]
 
 
-@dataclasses.dataclass(eq=False, frozen=True, order=False)
+@dcls.dataclass(eq=False, frozen=True, order=False)
 class CutIntent:
     """Filtering instructions for a qualitative value.
 
     Instances of this class are used to define cut parameters.
     Its values are directly inputted by the user, so should never be considered
     valid by itself.
     """
+
     level: str
     include_members: Set[Prim]
     exclude_members: Set[Prim]
 
     @classmethod
     def new(cls, level: str, incl: Iterable[Prim], excl: Iterable[Prim]):
         # TODO: enable compatibility for ranged-type include/exclude
@@ -56,15 +59,15 @@
         # The include/exclude sets are intended to be used as rules for the
         # composition of the query, so it's not needed to resolve them here.
         include = set(incl).difference(null_values)
         exclude = set(excl).difference(null_values)
         return cls(level=level, include_members=include, exclude_members=exclude)
 
 
-@dataclasses.dataclass(eq=False, frozen=True, order=False)
+@dcls.dataclass(eq=False, frozen=True, order=False)
 class FilterIntent:
     """Filtering instructions for a quantitative value.
 
     Instances of this class are used to define filter parameters.
     Its values are directly inputted by the user, so should never be considered
     valid by itself.
     """
@@ -90,74 +93,83 @@
         else:
             constr = condition[0] if len(condition) == 1 else condition
             if and_ is not None:
                 cond = (_numconst(constr), LogicOperator.AND, _numconst(and_))
             elif or_ is not None:
                 cond = (_numconst(constr), LogicOperator.OR, _numconst(or_))
             else:
-                cond = (_numconst(constr), )
+                cond = (_numconst(constr),)
 
         return cls(field=field, condition=cond)
 
 
 class PaginationIntent(NamedTuple):
     """Pagination instructions for internal use."""
+
     limit: int = 0
     offset: int = 0
 
+    def __repr__(self):
+        return f"Pagination(limit={self.limit}, offset={self.offset})"
+
     @classmethod
     def from_str(cls, value: str):
         """Parses a string in format `int[,int]` into a Pagination tuple."""
-        if value == "":
+        if not value:
             raise ValueError("Invalid Pagination: no value provided")
         limit, offset = f"{value},0,0".split(",")[:2]
 
         if not limit.isnumeric():
-            raise ValueError("Provided \"limit\" parameter is not an integer")
+            raise ValueError('Provided "limit" parameter is not an integer')
         if not offset.isnumeric():
-            raise ValueError("Provided \"offset\" parameter is not an integer")
+            raise ValueError('Provided "offset" parameter is not an integer')
 
-        return cls(limit=0 if limit is None else int(limit),
-                   offset=0 if offset is None else int(offset))
+        return cls(
+            limit=0 if limit is None else int(limit),
+            offset=0 if offset is None else int(offset),
+        )
 
 
 class SortingIntent(NamedTuple):
     """Sorting instructions for internal use."""
+
     field: str
-    order: Order
+    order: AnyOrder
+
+    def __repr__(self):
+        return f"Sorting(field={repr(self.field)}, order='{self.order}')"
 
     @classmethod
     def new(cls, field: str, order: Union[Order, str, None]):
-        """Creates a new SortingIntent object, accepting more diverse parameters.
-        """
+        """Creates a new SortingIntent object, accepting more diverse parameters."""
         order = order if isinstance(order, Order) else Order.from_str(order)
         return cls(field=field, order=order)
 
     @classmethod
     def from_str(cls, value: str):
         """Parses a string into a SortingIntent object."""
-        if value == "":
+        if not value:
             raise ValueError("Invalid Sorting: no value provided")
         field, order = f"{value}..".split(".")[:2]
-        return cls.new(field, order)  # type: ignore
+        return cls.new(field, order)
 
 
-@dataclasses.dataclass(eq=True, frozen=True, order=False)
+@dcls.dataclass(eq=True, frozen=True, order=False, repr=False)
 class TimeRestriction:
     """Time-axis filtering instructions for internal use.
 
     Instances of this class are used to define a time restriction over the
     resulting data. It must always contain both fields."""
 
     level: Union[str, RestrictionScale]
     age: RestrictionAge
     amount: int = 1
     is_full: bool = False
 
-    def __str__(self) -> str:
+    def __repr__(self):
         return (
             f"TimeRestriction(level='{self.level}', age='{self.age}', "
             f"amount={self.amount}, is_full={self.is_full})"
         )
 
     @classmethod
     def from_str(cls, value: str):
@@ -181,19 +193,20 @@
             amount = 1
 
         full = "full" in params or "all" in params
 
         return cls(level, age, amount, full)
 
 
-@dataclasses.dataclass(eq=True, frozen=True, order=False)
+@dcls.dataclass(eq=True, frozen=True, order=False)
 class HierarchyField:
     """Contains the parameters associated to a slicing operation on the data,
     based on a single Hierarchy from a Cube's Dimension.
     """
+
     dimension: "DimensionTraverser"
     hierarchy: "HierarchyTraverser"
     levels: Tuple["LevelField", ...]
 
     @property
     def alias(self) -> str:
         """Returns a deterministic unique short ID for the entity."""
@@ -237,27 +250,39 @@
     @property
     def table(self):
         """Returns the table to use as source for the Dimension data. If not
         set, the data is stored directly in the fact table for the Cube."""
         return self.hierarchy.table
 
 
-@dataclasses.dataclass(eq=True, frozen=True, order=False)
+@dcls.dataclass(eq=True, frozen=True, order=False, repr=False)
 class LevelField:
     """Contains the parameters associated to the slice operation, specifying the
     columns each resulting group should provide to the output data.
     """
+
     level: "LevelTraverser"
     caption: Optional["PropertyTraverser"] = None
     is_drilldown: bool = False
-    members_exclude: Set[str] = dataclasses.field(default_factory=set)
-    members_include: Set[str] = dataclasses.field(default_factory=set)
-    properties: FrozenSet["PropertyTraverser"] = dataclasses.field(default_factory=frozenset)
+    members_exclude: Set[str] = dcls.field(default_factory=set)
+    members_include: Set[str] = dcls.field(default_factory=set)
+    properties: FrozenSet["PropertyTraverser"] = dcls.field(default_factory=frozenset)
     time_restriction: Optional[TimeRestriction] = None
 
+    def __repr__(self):
+        params = (
+            f"name={repr(self.level.name)}",
+            f"is_drilldown={repr(self.is_drilldown)}",
+            f"caption={repr(self.caption)}",
+            f"properties={repr(sorted(self.properties, key=lambda x: x.name))}",
+            f"cut_exclude={repr(sorted(self.members_exclude))}",
+            f"cut_include={repr(sorted(self.members_include))}",
+        )
+        return f"{type(self).__name__}({', '.join(params)})"
+
     @property
     def alias(self) -> str:
         """Returns a deterministic unique short ID for the entity."""
         return shorthash(self.level.name + self.level.key_column)
 
     @property
     def is_cut(self) -> bool:
@@ -267,28 +292,52 @@
     def key_column(self) -> str:
         return self.level.key_column
 
     @property
     def name(self) -> str:
         return self.level.name
 
+    def iter_columns(self, locale: str):
+        """Generates triads of (column name, column alias, pair hash) for all fields related to
+        a HierarchyField object.
 
-@dataclasses.dataclass(eq=True, frozen=True, order=False)
+        This comprises Drilldown Labels and IDs, and its requested Properties.
+        """
+        name = self.level.name
+        key_column = self.level.key_column
+        name_column = self.level.get_name_column(locale)
+        if name_column is None:
+            yield key_column, name, shorthash(name + key_column)
+        else:
+            yield key_column, f"{name} ID", shorthash(name + key_column)
+            yield name_column, name, shorthash(name + name_column)
+        for propty in self.properties:
+            propty_column = propty.get_key_column(locale)
+            yield propty_column, propty.name, shorthash(propty.name + propty_column)
+
+
+@dcls.dataclass(eq=True, frozen=True, order=False, repr=False)
 class MeasureField:
     """MeasureField dataclass.
 
     Contains the parameters needed to filter the data points returned by the
     query operation from the server.
     """
+
     measure: "AnyMeasure"
-    is_measure: bool = False
-    with_ranking: Literal["asc", "desc", None] = None
-    constraint1: Optional[NumericConstraint] = None
-    constraint2: Optional[NumericConstraint] = None
-    joint: LogicOperator = LogicOperator.AND
+    constraint: Optional[FilterCondition] = None
+    with_ranking: Optional[Literal["asc", "desc"]] = None
+
+    def __repr__(self):
+        params = (
+            f"name={repr(self.measure.name)}",
+            f"constraint={repr(self.constraint)}",
+            f"with_ranking={repr(self.with_ranking)}",
+        )
+        return f"{type(self).__name__}({', '.join(params)})"
 
     @property
     def alias_name(self):
         """Returns a deterministic short hash of the name of the entity."""
         return shorthash(self.measure.name)
 
     @property
@@ -297,18 +346,14 @@
         return shorthash(
             repr(self.measure.formula)
             if isinstance(self.measure, CalculatedMeasure)
             else self.measure.key_column
         )
 
     @property
-    def is_filter(self) -> bool:
-        return self.constraint1 is not None
-
-    @property
     def name(self) -> str:
         """Quick method to return the measure name."""
         return self.measure.name
 
     @property
     def aggregator_params(self) -> Dict[str, str]:
         """Quick method to retrieve the measure aggregator params."""
@@ -319,7 +364,11 @@
         """Quick method to retrieve the measure aggregator type."""
         return str(self.measure.aggregator)
 
     def get_source(self):
         # TODO add locale compatibility
         """Quick method to obtain the source information of the measure."""
         return self.measure.annotations.get("source")
+
+    @property
+    def datatype(self):
+        return MemberType.FLOAT64
```

### Comparing `tesseract_olap-0.9.1/tesseract_olap/query/queries.py` & `tesseract_olap-0.9.2/tesseract_olap/query/queries.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,67 +1,112 @@
 """Query-related data-handling models module.
 
 This module contains data structs used to carry and compose objects used during
 a Query. The elements are agnostic to the type of backend used, and its primary
 purpose is organize and easily obtain the data needed for later steps.
 """
 
+import hashlib
 from collections import defaultdict
 from dataclasses import dataclass, field
 from itertools import chain
-from typing import Iterable, List, Mapping, Optional, Set, Tuple, Union
+from typing import Dict, List, Mapping, Optional, Tuple, Union
 
 import immutables as immu
 from typing_extensions import Literal
 
-from tesseract_olap.common import AnyDict
+from tesseract_olap.common import stringify
+from tesseract_olap.exceptions.query import (
+    InvalidEntityName,
+    MissingMeasures,
+    NotAuthorized,
+)
 from tesseract_olap.schema import (
-    AnyMeasure,
-    ColumnEntity,
     CubeTraverser,
     DimensionTraverser,
     HierarchyTraverser,
     LevelTraverser,
+    MemberType,
     SchemaTraverser,
 )
 
-from .enums import LogicOperator, RestrictionScale
-from .exceptions import InvalidEntityName, MissingMeasures, NotAuthorized
+from .enums import RestrictionScale
 from .models import (
     CutIntent,
     HierarchyField,
     LevelField,
     MeasureField,
     PaginationIntent,
     SortingIntent,
 )
 from .requests import DataRequest, MembersRequest
 
 AnyQuery = Union["DataQuery", "MembersQuery"]
 
 
-@dataclass(eq=False, order=False)
+@dataclass(eq=False, order=False, repr=False)
 class DataQuery:
     """Internal DataQuery class.
 
     Contains all the schema-hydrated elements corresponding to a
     :class:`DataRequest`, but also joining properties related to the same
     columnar entities.
     """
 
     cube: "CubeTraverser"
     locale: str
     fields_qualitative: Tuple["HierarchyField", ...] = field(default_factory=tuple)
     fields_quantitative: Tuple["MeasureField", ...] = field(default_factory=tuple)
     options: Mapping[str, bool] = field(default_factory=dict)
     pagination: "PaginationIntent" = field(default_factory=PaginationIntent)
-    parents: Union[bool, Set[str]] = False
-    ranking: Mapping[str, Literal["asc", "desc"]] = field(default_factory=dict)
     sorting: Optional["SortingIntent"] = None
 
+    def __repr__(self):
+        gen_levels = (
+            repr(lvlfi)
+            for hiefi in sorted(self.fields_qualitative, key=lambda x: x.dimension.name)
+            for lvlfi in hiefi.levels
+        )
+        gen_measures = (
+            repr(msrfi)
+            for msrfi in sorted(self.fields_quantitative, key=lambda x: x.name)
+        )
+        params = (
+            f"cube={repr(self.cube.name)}",
+            f"locale={repr(self.locale)}",
+            f"fields=({', '.join(chain(gen_levels, gen_measures))})",
+            f"options={stringify(self.options)}",
+            f"pagination={repr(self.pagination)}",
+            f"sorting={repr(self.sorting)}",
+        )
+        return f"{type(self).__name__}({', '.join(params)})"
+
+    @property
+    def key(self) -> str:
+        return hashlib.md5(repr(self).encode("utf-8")).hexdigest()
+
+    @property
+    def columns(self) -> Dict[str, MemberType]:
+        locale = self.locale
+        gen_measure = (
+            (msrfi.name, msrfi.datatype) for msrfi in self.fields_quantitative
+        )
+        gen_ranking = (
+            (f"{msrfi.name} Ranking", MemberType.UINT32)
+            for msrfi in self.fields_quantitative
+            if msrfi.with_ranking
+        )
+        gen_level = (
+            (name, lvlfi.level.key_type)
+            for hiefi in self.fields_qualitative
+            for lvlfi in hiefi.drilldown_levels
+            for _, name, _ in lvlfi.iter_columns(locale)
+        )
+        return dict(chain(gen_measure, gen_ranking, gen_level))
+
     @classmethod
     def from_request(cls, schema: "SchemaTraverser", request: "DataRequest"):
         """Generates a new :class:`Query` instance from the parameters defined
         in a :class:`DataRequest` object.
 
         If any of the parameters can't be found on the Schema, raises a derivate
         of the :class:`InvalidQuery` error.
@@ -71,85 +116,85 @@
 
         cube = schema.get_cube(request.cube)
 
         return cls(
             cube=cube,
             fields_qualitative=_get_data_hierarfields(cube, request),
             fields_quantitative=_get_data_measurefields(cube, request),
-            locale=schema.default_locale \
-                   if request.locale is None else \
-                   request.locale,
+            locale=schema.default_locale if request.locale is None else request.locale,
             options=request.options,
             pagination=request.pagination,
-            parents=request.parents,
-            ranking=_resolve_ranking(request),
             sorting=request.sorting,
         )
 
-    def get_entity_map(self) -> Mapping[str, ColumnEntity]:
-        return immu.Map(
-            _yield_column_entities(
-                self.fields_qualitative, self.fields_quantitative, self.locale
-            )
-        )
-
-    def get_sources(self) -> Tuple[AnyDict, ...]:
-        """Returns a sequence containing the sources for each measure in the Query.
 
-        Only measures with a properly declared source will appear in this dict.
-        """
-        source = {
-            "name": self.cube.name,
-            "measures": [item.name for item in self.fields_quantitative if item.is_measure],
-            "annotations": self.cube.annotations,
-        }
-        return (source,)
-
-
-@dataclass(eq=False, order=False)
+@dataclass(eq=False, order=False, repr=False)
 class MembersQuery:
     """Internal MembersQuery class."""
 
     cube: "CubeTraverser"
     hiefield: "HierarchyField"
     locale: str
     pagination: "PaginationIntent" = field(default_factory=PaginationIntent)
     search: Optional[str] = None
 
+    def __repr__(self):
+        fields = (
+            repr(item) for item in sorted(self.hiefield.levels, key=lambda x: x.name)
+        )
+        params = (
+            f'cube="{self.cube.name}"',
+            f'locale="{self.locale}"',
+            f'fields=({", ".join(fields)})',
+            f"pagination={repr(self.pagination)}",
+            f"search={repr(self.search)}",
+        )
+        return f"{type(self).__name__}({', '.join(params)})"
+
+    @property
+    def key(self) -> str:
+        return hashlib.md5(repr(self).encode("utf-8")).hexdigest()
+
+    @property
+    def columns(self) -> Dict[str, MemberType]:
+        locale = self.locale
+        return {
+            name: lvlfi.level.key_type
+            for lvlfi in self.hiefield.levels
+            for _, name, _ in lvlfi.iter_columns(locale)
+        }
+
     @classmethod
     def from_request(cls, schema: "SchemaTraverser", request: "MembersRequest"):
         """Generates a new :class:`MembersQuery` instance from a user-provided
         :class:`MembersRequest` instance.
         """
         if not schema.is_authorized(request):
             raise NotAuthorized()
 
         cube = schema.get_cube(request.cube)
 
         return cls(
             cube=cube,
             hiefield=_get_members_hierarfield(cube, request),
-            locale=schema.default_locale \
-                   if request.locale is None else \
-                   request.locale,
+            locale=schema.default_locale if request.locale is None else request.locale,
             pagination=request.pagination,
             search=request.search,
         )
 
-    def get_entity_map(self) -> Mapping[str, ColumnEntity]:
-        return immu.Map((lvlfi.name, lvlfi.level) for lvlfi in self.hiefield.levels)
-
 
 def _get_data_hierarfields(cube: "CubeTraverser", req: "DataRequest"):
     """Regroups query parameters related to a Level, to simplify later usage."""
     # we need a map with all possible levels, including the cube's shared dimensions
-    level_map = immu.Map((level.name, (dimension, hierarchy, level))
-                         for dimension in cube.dimensions
-                         for hierarchy in dimension.hierarchies
-                         for level in hierarchy.levels)
+    level_map = immu.Map(
+        (level.name, (dimension, hierarchy, level))
+        for dimension in cube.dimensions
+        for hierarchy in dimension.hierarchies
+        for level in hierarchy.levels
+    )
 
     drilldown_set = req.drilldowns
     property_set = req.properties
     caption_set = req.captions
     cut_map = {**req.cuts}
 
     with_parents = req.parents
@@ -161,47 +206,47 @@
 
     time_level = None
     time_restr = req.time_restriction
     if time_restr is not None:
         granularity = time_restr.level
         time_level = (
             cube.get_time_level(granularity.value)
-            if isinstance(granularity, RestrictionScale) else
-            cube.get_time_level(granularity)
+            if isinstance(granularity, RestrictionScale)
+            else cube.get_time_level(granularity)
         )
         involved_levels.add(time_level.name)
 
     # Ensure all levels involved in the request don't break
     # the 'single dimension, same hierarchy' rule
-    dimension_store: Mapping[DimensionTraverser, HierarchyTraverser] = {}
-    hierarchy_store: Mapping[HierarchyTraverser, List[LevelTraverser]] = defaultdict(list)
+    dim_store: Mapping[DimensionTraverser, HierarchyTraverser] = {}
+    hie_store: Mapping[HierarchyTraverser, List[LevelTraverser]] = defaultdict(list)
 
     for name in involved_levels:
         dimension, hierarchy, level = level_map[name]
-        if dimension_store.get(dimension, hierarchy) != hierarchy:
+        if dim_store.get(dimension, hierarchy) != hierarchy:
             raise ValueError(
                 "Multiple Hierarchies from the same Dimension are being requested. "
                 "Only a single Hierarchy can be used at a time for a query."
             )
-        dimension_store[dimension] = hierarchy
-        hierarchy_store[hierarchy].append(level)
+        dim_store[dimension] = hierarchy
+        hie_store[hierarchy].append(level)
 
     # Apply default members
     for dimension in cube.dimensions:
         # Get the relevant Hierarchy for each Dimension in the Cube
-        hierarchy = dimension_store.get(dimension, dimension.default_hierarchy)
+        hierarchy = dim_store.get(dimension, dimension.default_hierarchy)
 
         # The default_member logic will be applied only if the
         # (dimension, hierarchy) is not present in the user request
-        levels = hierarchy_store[hierarchy]
+        levels = hie_store[hierarchy]
         if len(levels) > 0:
             continue
 
         # Store the default hierarchy for the SQL subset filter
-        dimension_store[dimension] = hierarchy
+        dim_store[dimension] = hierarchy
 
         default_member = hierarchy.default_member
         if default_member is None:
             continue
 
         level, member = default_member
         levels.append(level)
@@ -209,35 +254,35 @@
 
     def _compose_field(level: "LevelTraverser", is_drilldown: bool) -> "LevelField":
         """Capsules the logic to fill a LevelField instance with data from both
         a Drilldown and a Cut.
         """
         kwargs = {
             "is_drilldown": is_drilldown,
-            "properties": frozenset(prop
-                                    for prop in level.properties
-                                    if prop.name in property_set),
-            "caption": next((capt
-                            for capt in level.properties
-                            if capt.name in caption_set), None),
+            "properties": frozenset(
+                prop for prop in level.properties if prop.name in property_set
+            ),
+            "caption": next(
+                (capt for capt in level.properties if capt.name in caption_set), None
+            ),
             "time_restriction": time_restr if time_level == level else None,
         }
 
         cut = cut_map.get(level.name)
         if cut is not None:
             kwargs["members_exclude"] = set(cut.exclude_members)
             kwargs["members_include"] = set(cut.include_members)
 
         return LevelField(level=level, **kwargs)
 
     def _resolve_fields(hierarchy: "HierarchyTraverser"):
         """Calculates the levels involved in the request, depending on the
         with_parent parameter.
         """
-        involved_levels = hierarchy_store[hierarchy]
+        involved_levels = hie_store[hierarchy]
         fields: List[LevelField] = []
 
         parent_flag = False
         # iterations will be done in reverse to use a flag for parents
         for level in reversed(tuple(hierarchy.levels)):
             # if includes_parents, and a deeper level is drilldown,
             # or if it's explicitly a drilldown
@@ -245,153 +290,78 @@
             # is_field means the level needs to be SELECTed
             # to be used as a foreign key for a drilldown or a cut
             is_field = is_drilldown or level in involved_levels
             if is_field:
                 fields.append(_compose_field(level, is_drilldown))
             # if level is marked in parents, raise flag
             # TODO: can be improved
-            parent_flag = parent_flag or (
-                is_drilldown and level.name in with_parents
-            )
+            parent_flag = parent_flag or (is_drilldown and level.name in with_parents)
 
         fields.reverse()
         return tuple(fields)
 
     return tuple(
         HierarchyField(dimension, hierarchy, levels)
         for dimension, hierarchy, levels in (
             (dimension, hierarchy, _resolve_fields(hierarchy))
             for dimension, hierarchy in (
-                sorted(dimension_store.items(), key=lambda item: item[0].name)
+                sorted(dim_store.items(), key=lambda item: item[0].name)
             )
         )
         if len(levels) > 0
     )
 
 
 def _get_data_measurefields(cube: "CubeTraverser", req: "DataRequest"):
-    """Regroups query parameters related to a Measure, to simplify contextual use.
-    """
-    measure_set = req.measures
+    """Regroups query parameters related to a Measure, to simplify contextual use."""
+    if isinstance(req.ranking, bool):
+        ranking_flags: Mapping[str, Literal["asc", "desc"]] = (
+            {item: "desc" for item in req.measures} if req.ranking else {}
+        )
 
-    ranking_flags = _resolve_ranking(req)
+    else:
+        ranking_flags = req.ranking
+        # All measures in the requested ranking must be in the requested measures
+        rank_diff = set(ranking_flags.keys()).difference(req.measures)
+        if len(rank_diff) > 0:
+            raise MissingMeasures("ranking", rank_diff)
 
-    measure_map = immu.Map(
-        (item.name, item)
-        for measure in cube.measure_map.values()
-        for item in _yield_all_measures(measure)
-    )
+    filter_constr = {item.field: item.condition for item in req.filters.values()}
 
-    try:
-        involved_measures = set(measure_map[name] for name in chain(
-            req.measures,
-            (item.field for item in req.filters.values()),
-        ))
-    except KeyError as exc:
-        raise InvalidEntityName("Measure", exc.args[0]) from None
-
-    involved_submeasures = set(
-        submeasure
-        for measure in involved_measures
-        for submeasure in measure.submeasures.values()
+    return tuple(
+        MeasureField(
+            measure=item,
+            with_ranking=ranking_flags.get(item.name),
+            constraint=filter_constr.get(item.name),
+        )
+        for measure in (
+            cube.get_measure(name)
+            for name in sorted(req.measures.union(filter_constr.keys()))
+        )
+        for item in measure.and_submeasures()
     )
-    involved_measures.update(involved_submeasures)
-
-    def _compose_field(measure: "AnyMeasure") -> "MeasureField":
-        kwargs = {
-            "is_measure": measure.name in measure_set,
-            "constraint1": None,
-            "with_ranking": None,
-        }
-
-        with_ranking = ranking_flags.get(measure.name)
-        # Ranking is available for top level measures only
-        if with_ranking and measure.name in cube.measure_map:
-            kwargs["with_ranking"] = with_ranking
-
-        fltr = req.filters.get(measure.name)
-        if fltr is None:
-            pass
-        elif len(fltr.condition) == 1: # is (NumConstr)
-            kwargs["constraint1"] = fltr.condition[0]
-        elif len(fltr.condition) == 3: # is (NumConstr, LogicOp, NumConstr)
-            kwargs["constraint1"] = fltr.condition[0]
-            kwargs["joint"] = LogicOperator.from_str(fltr.condition[1])
-            kwargs["constraint2"] = fltr.condition[2]
-
-        return MeasureField(measure, **kwargs)
-
-    return tuple(_compose_field(measure) for measure in involved_measures)
 
 
 def _get_members_hierarfield(cube: "CubeTraverser", req: "MembersRequest"):
     """Regroups query parameters related to a Level, to simplify later usage."""
     level_name = req.level
     with_parents = req.options.get("parents", False)
 
     try:
-        dimension, hierarchy, level = next((dimension, hierarchy, level)
-                                           for dimension in cube.dimensions
-                                           for hierarchy in dimension.hierarchies
-                                           for level in hierarchy.levels
-                                           if level.name == level_name)
+        dimension, hierarchy, level = next(
+            (dimension, hierarchy, level)
+            for dimension in cube.dimensions
+            for hierarchy in dimension.hierarchies
+            for level in hierarchy.levels
+            if level.name == level_name
+        )
     except StopIteration:
         raise InvalidEntityName("Level", level_name) from None
 
     if with_parents:
         levels = tuple(hierarchy.levels)
         last_index = levels.index(level) + 1
         fields = tuple(LevelField(level) for level in levels[0:last_index])
     else:
-        fields = LevelField(level),
+        fields = (LevelField(level),)
 
     return HierarchyField(dimension, hierarchy, levels=fields)
-
-
-def _yield_all_measures(measure: "AnyMeasure"):
-    """Yields a Measure and all its Submeasures, up to one level of depth."""
-    yield measure
-    for submeasure in measure.submeasures.values():
-        yield submeasure
-
-
-def _yield_column_entities(
-    hierarchies: Iterable["HierarchyField"],
-    measures: Iterable["MeasureField"],
-    locale: str,
-):
-    for hiefi in hierarchies:
-        for lvlfi in hiefi.levels:
-            if not lvlfi.is_drilldown:
-                continue
-
-            yield lvlfi.name, lvlfi.level
-
-            if lvlfi.level.get_name_column(locale) is not None:
-                yield f"{lvlfi.name} ID", lvlfi.level
-
-            for propty in lvlfi.properties:
-                yield propty.name, propty
-
-    for msrfi in measures:
-        if msrfi.is_measure:
-            yield msrfi.name, msrfi.measure
-
-
-def _resolve_ranking(req: "DataRequest") -> Mapping[str, Literal["asc", "desc"]]:
-    """Restructures the ranking parameter to be used in SQL building."""
-    measure_set = req.measures
-
-    # Resolve the hashmap of measures for the ranking request
-    ranking_flags: Mapping[str, Literal["asc", "desc"]] = {}
-    if req.ranking is True:
-        ranking_flags = {item: "desc" for item in measure_set}
-    elif isinstance(req.ranking, dict):
-        ranking_flags = req.ranking
-
-    # Check if the measures in the ranking request are in the requested measures
-    rank_diff = set(ranking_flags.keys())
-    rank_diff.difference_update(measure_set)
-    if len(rank_diff) > 0:
-        raise MissingMeasures("ranking", rank_diff)
-
-    return ranking_flags
```

### Comparing `tesseract_olap-0.9.1/tesseract_olap/query/requests.py` & `tesseract_olap-0.9.2/tesseract_olap/query/requests.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 Contains structs to build a :class:`DataRequest` instance: an object to describe
 the parameters needed for the query using only entity names and relationships.
 """
 
 import hashlib
 from dataclasses import dataclass, field
-from functools import cached_property
 from itertools import chain
 from typing import Mapping, Optional, Set, Tuple, Union
 
 from typing_extensions import Literal, Protocol, TypedDict
 
-from tesseract_olap.common import Array
+from tesseract_olap.common import Array, stringify
+from tesseract_olap.query import AnyOrder
 
 from .models import (
     CutIntent,
     DoubleFilterCondition,
     FilterIntent,
     PaginationIntent,
     SingleFilterCondition,
@@ -49,32 +49,32 @@
     cuts_exclude: Mapping[str, Array[str]]
     cuts_include: Mapping[str, Array[str]]
     filters: Mapping[str, Union[SingleFilterCondition, DoubleFilterCondition]]
     locale: str
     pagination: Union[str, Tuple[int, int]]
     parents: Union[bool, Array[str]]
     properties: Array[str]
-    ranking: Union[bool, Mapping[str, Literal["asc", "desc"]]]
+    ranking: Union[bool, Mapping[str, AnyOrder]]
     roles: Array[str]
-    sorting: Tuple[str, Literal["asc", "desc"]]
+    sorting: Union[str, Tuple[str, AnyOrder]]
     time: str
 
 
 class DataRequestParams(DataRequestOptionalParams, total=True):
     """DataRequestParams interface.
 
     Determines the expected params in a :class:`dict`, to use when creating a
     new :class:`DataRequest` object via the :func:`DataRequest.new` class method.
     """
 
     drilldowns: Array[str]
     measures: Array[str]
 
 
-@dataclass(eq=False, order=False)
+@dataclass(eq=False, order=False, repr=False)
 class DataRequest:
     """Represents the intent for a Data Query made by the user.
 
     All its properties are defined by strings of the names of the components
     from the schema.
     None of these parameters are verified during construction, so it's possible
     for the query to be invalid; a subclass of :class:`backend.exceptions.BackendError`
@@ -102,15 +102,34 @@
     sorting: Optional["SortingIntent"] = None
     time_restriction: Optional["TimeRestriction"] = None
 
     def __eq__(self, __value: object) -> bool:
         return isinstance(__value, DataRequest) and hash(self) == hash(__value)
 
     def __hash__(self):
-        return hash((*sorted(self.roles), self.request_id))
+        return hash((repr(self), *sorted(self.roles)))
+
+    def __repr__(self):
+        params = (
+            f"cube={repr(self.cube)}",
+            f"locale={repr(self.locale)}",
+            f"drilldowns={stringify(self.drilldowns)}",
+            f"captions={stringify(self.captions)}",
+            f"properties={stringify(self.properties)}",
+            f"cuts={stringify(list(self.cuts.values()))}",
+            f"time={repr(self.time_restriction)}",
+            f"measures={stringify(self.measures)}",
+            f"filters={stringify(list(self.filters.values()))}",
+            f"ranking={stringify(self.ranking)}",
+            f"options={stringify(self.options)}",
+            f"pagination={repr(self.pagination)}",
+            f"parents={stringify(self.parents)}",
+            f"sorting={repr(self.sorting)}",
+        )
+        return f"{type(self).__name__}({', '.join(params)})"
 
     @classmethod
     def new(cls, cube: str, request: DataRequestParams):
         """Creates a new :class:`DataRequest` instance from a set of parameters
         defined in a dict.
 
         This should be the preferred method by final users, as it doesn't
@@ -140,29 +159,29 @@
             "captions": set(request.get("captions", [])),
             "properties": set(request.get("properties", [])),
             "options": {},
             "ranking": request.get("ranking", False),
             "roles": set(roles) if isinstance(roles, (list, tuple)) else roles,
         }
 
-        item = request.get("pagination", (0, 0))
+        item = request.get("pagination") or (0, 0)
         if isinstance(item, str):
             kwargs["pagination"] = PaginationIntent.from_str(item)
         elif isinstance(item, (list, tuple)):
             kwargs["pagination"] = PaginationIntent(*item)
 
         item = request.get("parents", False)
         if isinstance(item, (set, bool)):
             kwargs["parents"] = item
         elif isinstance(item, (list, tuple)):
             kwargs["parents"] = set(item)
         elif isinstance(item, str):
-            kwargs["parents"] = {item}
+            kwargs["parents"] = set(item.split(","))
 
-        item = request.get("sorting")
+        item = request.get("sorting") or None
         if isinstance(item, str):
             kwargs["sorting"] = SortingIntent.from_str(item)
         elif isinstance(item, (list, tuple)):
             kwargs["sorting"] = SortingIntent.new(*item)
 
         item = request.get("time")
         if isinstance(item, str):
@@ -171,85 +190,23 @@
         return cls(
             cube=cube,
             drilldowns=set(request["drilldowns"]),
             measures=set(request["measures"]),
             **kwargs,
         )
 
-    @cached_property
-    def request_id(self):
+    def key(self):
         """Generates a hash to differentiate the parameters that influence the resulting data.
 
         This hash can be used to compare requests, and as cache key for the resulting data.
         It doesn't consider roles on purpose, as the roles define the access to the dataset
         instead of its contents. This also means a comparison operation between requests must
-        compare roles separetely.
+        compare roles separately.
         """
-        measures = (
-            stringify_filter(name, name in self.measures, self.filters.get(name))
-            for name in sorted(self.measures.union(self.filters.keys()))
-        )
-        drilldowns = (
-            stringify_cut(name, name in self.drilldowns, self.cuts.get(name))
-            for name in sorted(self.drilldowns.union(self.cuts.keys()))
-        )
-        parents = (
-            f"Parents({self.parents})"
-            if isinstance(self.parents, bool)
-            else f"Parents({str(sorted(self.parents))[1:-1]})"
-        )
-        ranking = (
-            ", ".join(sorted(f"{key}={value}" for key, value in self.ranking.items()))
-            if isinstance(self.ranking, Mapping)
-            else self.ranking
-        )
-        sorting = (
-            str(self.sorting).replace("Intent", "") if self.sorting else "Sorting(None)"
-        )
-        time = (
-            str(self.time_restriction).replace("Restriction", "")
-            if self.time_restriction
-            else "Time(None)"
-        )
-        params = [
-            f"Cube: {self.cube}",
-            *measures,
-            *drilldowns,
-            f"Captions: {sorted(self.captions)}",
-            f"Properties: {sorted(self.properties)}",
-            f"Locale: {self.locale}",
-            f"Pagination: {tuple(self.pagination)}",
-            parents,
-            f"Ranking({ranking})",
-            sorting,
-            time,
-            # *(f"{key.capitalize()}: {value}" for key, value in self.options.items()),
-        ]
-        return hashlib.md5("\n".join(params).encode("utf-8")).hexdigest()
-
-
-def stringify_cut(name: str, is_drilldown: bool, item: Optional[CutIntent]):
-    string = f"Level '{name}': {is_drilldown}"
-    if item is not None:
-        if len(item.include_members) > 0:
-            string += f"\n  with {sorted(item.include_members)}"
-        if len(item.exclude_members) > 0:
-            string += f"\n  without {sorted(item.include_members)}"
-    return string
-
-
-def stringify_filter(name: str, is_measure: bool, item: Optional[FilterIntent]):
-    string = f"Measure '{name}': {is_measure}"
-    if item is not None:
-        string += f"\n  where {item.condition[0][0]} {item.condition[0][1]}"
-        if len(item.condition) == 3:
-            string += "\n  {joint:>5} {cond[0]} {cond[1]}".format(
-                joint=item.condition[1], cond=item.condition[2]
-            )
-    return string
+        return hashlib.md5(repr(self).encode("utf-8")).hexdigest()
 
 
 class MembersRequestOptionalParams(TypedDict, total=False):
     """Defines the optional parameters in the MembersRequestParams interface.
 
     Is a separate class is due to the implementation of the
     [Totality](https://www.python.org/dev/peps/pep-0589/#totality) in the
@@ -257,15 +214,15 @@
 
     This will give a better hint to the type checker when the user makes use of
     this interface.
     """
 
     children: bool
     locale: str
-    pagination: Tuple[int, int]
+    pagination: Union[str, Tuple[int, int]]
     parents: bool
     roles: Array[str]
     search: str
 
 
 class MembersRequestParams(MembersRequestOptionalParams, total=True):
     """MembersRequestParams interface.
@@ -303,16 +260,19 @@
         defined in a dict.
 
         This should be the preferred method by final users, as it doesn't
         require the use of internal dataclasses and the setup of internal
         structures and unique conditions.
         """
 
-        item = request.get("pagination", (0, 0))
-        pagination = PaginationIntent(*item)
+        item = request.get("pagination") or (0, 0)
+        if isinstance(item, str):
+            pagination = PaginationIntent.from_str(item)
+        else:
+            pagination = PaginationIntent(*item)
 
         item = request.get("roles", [])
         roles = set(item) if isinstance(item, (list, tuple)) else item
 
         return cls(
             cube=cube,
             level=request["level"],
```

### Comparing `tesseract_olap-0.9.1/tesseract_olap/schema/__init__.py` & `tesseract_olap-0.9.2/tesseract_olap/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.1/tesseract_olap/schema/aggregators.py` & `tesseract_olap-0.9.2/tesseract_olap/schema/aggregators.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,51 @@
 """Schema Aggregators module.
 
 Contains the different types of aggregator that can be used in the definition of
 a Measure in the Schema.
 """
 
-import dataclasses
-from typing import Any, Dict, List, Set, Tuple, Union
+import dataclasses as dcls
+from typing import Any, Dict, List, Tuple, Union
 
 from .enums import AggregatorType
 
 
-def _get_fields(obj: object) -> Set[str]:
-    """Returns a set of strings, with the names of the fields in this class.
-    """
-    return set(f.name for f in dataclasses.fields(obj)) \
-           if dataclasses.is_dataclass(obj) else \
-           set()
+def _get_fields(obj: object) -> List[str]:
+    """Returns a set of strings, with the names of the fields in this class."""
+    return sorted(f.name for f in dcls.fields(obj)) if dcls.is_dataclass(obj) else []
 
 
 class Aggregator:
     """Base class for aggregator methods.
 
     The instances contain parameters to compose the associated SQL query.
     Backend packages should extend these according to support, and implement
     the methods needed for conversion to string.
     """
-    def __init__(self) -> None:
-        ...
 
-    def __repr__(self) -> str:
-        return "{0}({1})".format(type(self).__name__, ", ".join(
-            "{0}={1}".format(field, repr(getattr(self, field)))
-            for field in _get_fields(self)
-        ))
+    def __repr__(self):
+        params = ", ".join(
+            f"{field}={repr(getattr(self, field))}" for field in _get_fields(self)
+        )
+        return f"{type(self).__name__}({params})"
 
     def __str__(self) -> str:
         return type(self).__name__
 
     def __iter__(self):
         yield "type", type(self).__name__
-        yield from (
-            (field, getattr(self, field))
-            for field in _get_fields(self)
-        )
+        yield from ((field, getattr(self, field)) for field in _get_fields(self))
 
     def get_params(self) -> Dict[str, str]:
         """Returns a dict with the serialized params of the instance.
 
         Base class just returns an empty dict. More complex subclasses must
         override this method."""
-        return dict(
-            (field, getattr(self, field))
-            for field in _get_fields(self)
-        )
+        return dict((field, getattr(self, field)) for field in _get_fields(self))
 
     @classmethod
     def new(cls, kwargs: Dict[str, Any]) -> "Aggregator":
         field_names = _get_fields(cls)
         return cls(**{k: v for k, v in kwargs.items() if k in field_names})
 
     @staticmethod
@@ -71,15 +60,15 @@
             AggregatorType.SUM: Sum,
             AggregatorType.BASICGROUPEDMEDIAN: BasicGroupedMedian,
             AggregatorType.CALCULATEDMOE: CalculatedMoe,
             AggregatorType.QUANTILE: Quantile,
             AggregatorType.REPLICATEWEIGHTMOE: ReplicateWeightMoe,
             AggregatorType.WEIGHTEDAVERAGE: WeightedAverage,
             AggregatorType.WEIGHTEDAVERAGEMOE: WeightedAverageMoe,
-            AggregatorType.WEIGHTEDSUM: WeightedSum
+            AggregatorType.WEIGHTEDSUM: WeightedSum,
         }
         return agg_classes[enum]
 
 
 class Sum(Aggregator):
     pass
 
@@ -104,91 +93,97 @@
     pass
 
 
 class Median(Aggregator):
     pass
 
 
-@dataclasses.dataclass(frozen=True)
+@dcls.dataclass(frozen=True)
 class Quantile(Aggregator):
     """Quantile is calculated against the measure's value column.
 
     `quantile(quantile_level)(column)`
 
     where quantile_level = Quantile level between 0 and 1
     """
+
     quantile_level: Union[str, float]
 
 
-@dataclasses.dataclass(frozen=True)
+@dcls.dataclass(frozen=True)
 class BasicGroupedMedian(Aggregator):
     group_aggregator: str
     group_dimension: str
 
 
-@dataclasses.dataclass(frozen=True)
+@dcls.dataclass(frozen=True)
 class WeightedSum(Aggregator):
     """Weighted Sum is calculated against the measure's value column.
 
     `sum(column * weight_column)`
 
     First roll-up is sum(column * weight_column) as weighted_sum_first
     Second roll-up is sum(weighted_sum_first) as weighted_sum_final
     """
+
     weight_column: str
 
 
-@dataclasses.dataclass(frozen=True)
+@dcls.dataclass(frozen=True)
 class WeightedAverage(Aggregator):
     """Weighted Average is calculated against the measure's value column.
 
     `sum(column * weight_column) / sum(weight_column)`
     """
+
     weight_column: Union[str, Tuple[str, float]]
 
 
-@dataclasses.dataclass(frozen=True)
+@dcls.dataclass(frozen=True)
 class ReplicateWeightMoe(Aggregator):
     """Where the measure column is the primary value, and a list of secondary
     columns is provided to the MO aggregator:
 
     The general equation for Margin of Error is
 
     `cv * pow(df * (pow(sum(column) - sum(secondary_columns[0]), 2) + pow(sum(column) - sum(secondary_columns_[1]), 2) + ...), 0.5)`
 
     where cv = critical value, for 90% confidence interval it's 1.645
     where df = design factor / #samples
     """
+
     critical_value: float
     design_factor: float
     secondary_columns: List[str]
 
 
-@dataclasses.dataclass(frozen=True)
+@dcls.dataclass(frozen=True)
 class CalculatedMoe(Aggregator):
     """Where the moe is already calculated for each row, and this just
     aggregates them correctly.
 
     `sqrt(sum(power(moe / cv, 2))) * cv`
 
     where cv = critical value; for 90% confidence interval it's 1.645
     """
+
     critical_value: Union[str, float]
 
 
-@dataclasses.dataclass(frozen=True)
+@dcls.dataclass(frozen=True)
 class WeightedAverageMoe(Aggregator):
     """
     Where the measure column is the primary value,
     and a list of secondary weight columns is provided to the MO aggregator:
 
     The general equation for Margin of Error is
 
     `cv * pow(df * (pow(( sum(column * primary_weight)/sum(primary_weight) ) - ( sum(column * secondary_weight_columns[0])/sum(secondary_weight_columns[0]) ), 2) + pow(( sum(column * primary_weight)/sum(primary_weight) ) - ( sum(column * secondary_weight_columns[1]/sum(secondary_weight_columns[1]) ), 2) + ...), 0.5)`
 
     where cv = critical value, for 90% confidence interval it's 1.645
     where df = design factor / #samples
     """
+
     critical_value: float
     design_factor: float
     primary_weight: str
     secondary_weight_columns: List[str]
```

### Comparing `tesseract_olap-0.9.1/tesseract_olap/schema/csv.py` & `tesseract_olap-0.9.2/tesseract_olap/schema/csv.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 
 import immutables as immu
 
 from tesseract_olap.common import is_numeric, numerify
 
 from . import models
 
-DELIMITER_TRANSLATE = immu.Map({
-    "comma": ",",
-    "semicolon": ";",
-    "tab": "\t",
-    "space": " ",
-})
+DELIMITER_TRANSLATE = immu.Map(
+    comma=",",
+    semicolon=";",
+    tab="\t",
+    space=" ",
+)
 
 
 class ColumnTypeInferrer:
     def __init__(self, iterable: Iterable[str], csv_params: dict):
         self.csv_params = csv_params
         self.headers = ""
         self.iterator = iter(iterable)
@@ -27,16 +27,15 @@
         return self
 
     def __next__(self):
         row = next(self.iterator)
         if self.headers:
             row_items = next(csv.reader([row], **self.csv_params))
             self.types = [
-                itype and is_numeric(item)
-                for item, itype in zip(row_items, self.types)
+                itype and is_numeric(item) for item, itype in zip(row_items, self.types)
             ]
         else:
             self.headers = list(csv.reader(row))
             self.types = [True for item in self.headers]
         return row
 
     def cast(
@@ -97,24 +96,25 @@
     return list(content.cast(table))
 
 
 def parse_csv_schema(
     source: Union[str, Path, TextIO], table_name: str = ""
 ) -> "CSVSchema":
     if isinstance(source, Path):
-        table_name = source.name.replace(source.suffix, "")
-        with source.open("r") as io:
-            headers, *rows = parse_csv(line for line in io)
+        if not table_name:
+            table_name = source.name.replace(source.suffix, "")
+        with source.open("r", encoding="utf8") as io:
+            headers, *rows = parse_csv(io)
 
     elif isinstance(source, str):
         headers, *rows = parse_csv(source.splitlines())
 
-    else: # isinstance(a, TextIO) has runtime issues
+    else:  # isinstance(a, TextIO) has runtime issues
         try:
-            table_name = source.name
+            table_name = source.name if not table_name else table_name
         except AttributeError:
             pass
         headers, *rows = parse_csv(source.readlines())
         source.close()
 
     table = CSVInlineTable(
         name=table_name,
```

### Comparing `tesseract_olap-0.9.1/tesseract_olap/schema/enums.py` & `tesseract_olap-0.9.2/tesseract_olap/schema/enums.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from enum import Enum
-from typing import Any, Optional, Sequence
+from typing import Any, Dict, Optional, Sequence, Type
+
+import polars as pl
 
 
 class AggregatorType(Enum):
     """Lists the possible aggregation operations to perform on the data to
     return a measure."""
+
     SUM = "sum"
     COUNT = "count"
     AVERAGE = "avg"
     MAX = "max"
     MIN = "min"
     MODE = "mode"
     BASICGROUPEDMEDIAN = "basic_grouped_median"
@@ -27,29 +30,37 @@
             return next((item for item in cls if item.value == value))
         except StopIteration:
             raise ValueError(f"Invalid AggregatorType value: {value}")
 
 
 class DimensionType(Enum):
     """Lists the kinds of data a dimension is storing."""
+
     STANDARD = "standard"
     TIME = "time"
     GEO = "geo"
 
+    def __repr__(self):
+        return f"{type(self).__name__}.{self.name}"
+
+    def __str__(self):
+        return self.value
+
     @classmethod
     def from_str(cls, value: Optional[str]):
         if value is None:
             return cls.STANDARD
         value = value.lower()
         return next((item for item in cls if item.value == value), cls.STANDARD)
 
 
 class MemberType(Enum):
     """Lists the types of the data the user can expect to find in the associated
     column."""
+
     BOOLEAN = "bool"
     DATE = "date"
     TIME = "time"
     DATETIME = "dttm"
     TIMESTAMP = "stmp"
     FLOAT32 = "f32"
     FLOAT64 = "f64"
@@ -61,34 +72,46 @@
     UINT8 = "u8"
     UINT16 = "u16"
     UINT32 = "u32"
     UINT64 = "u64"
     UINT128 = "u128"
     STRING = "str"
 
+    def __repr__(self):
+        return f"{type(self).__name__}.{self.name}"
+
+    def __str__(self):
+        return self.value
+
     def get_caster(self):
-        if self in (
-            MemberType.INT8, MemberType.INT16, MemberType.INT32, MemberType.INT64, MemberType.INT128,
-            MemberType.UINT8, MemberType.UINT16, MemberType.UINT32, MemberType.UINT64, MemberType.UINT128,
-        ):
+        pldt = self.to_polars()
+        if pldt.is_integer():
             return int
-        if self in (MemberType.FLOAT32, MemberType.FLOAT64):
+        elif pldt.is_float():
             return float
-        if self == MemberType.BOOLEAN:
+        elif self is MemberType.BOOLEAN:
             return bool
         return str
 
+    def to_polars(self):
+        return _POLARS_DATATYPES[self]
+
     @classmethod
     def from_str(cls, value: Optional[str]):
         if value is None:
             return cls.INT64
         value = value.lower()
         return next((item for item in cls if item.value == value), cls.INT64)
 
     @classmethod
+    def from_polars(cls, value: Type[pl.DataType]):
+        name = _MEMBERTYPE_REVERSE[value]
+        return cls[name]
+
+    @classmethod
     def from_values(cls, values: Sequence[Any]):
         types = frozenset(type(value) for value in values)
 
         if len(types) == 1 and bool in types:
             return MemberType.BOOLEAN
 
         if float in types:
@@ -101,28 +124,52 @@
 
     @classmethod
     def from_int_values(cls, values: Sequence[int]):
         mini = min(values)
         maxi = max(values)
 
         if mini < 0:
-            if mini < -(2**63) or maxi > 2**63-1:
+            if mini < -(2**63) or maxi > 2**63 - 1:
                 return MemberType.INT128
-            elif mini < -(2**31) or maxi > 2**31-1:
+            elif mini < -(2**31) or maxi > 2**31 - 1:
                 return MemberType.INT64
-            elif mini < -(2**15) or maxi > 2**15-1:
+            elif mini < -(2**15) or maxi > 2**15 - 1:
                 return MemberType.INT32
             elif mini < -128 or maxi > 127:
                 return MemberType.INT16
             else:
                 return MemberType.INT8
         else:
-            if maxi > 2**64-1:
+            if maxi > 2**64 - 1:
                 return MemberType.UINT128
-            elif maxi > 2**32-1:
+            elif maxi > 2**32 - 1:
                 return MemberType.UINT64
             elif maxi > 65535:
                 return MemberType.UINT32
             elif maxi > 255:
                 return MemberType.UINT16
             else:
                 return MemberType.UINT8
+
+
+_POLARS_DATATYPES: Dict[MemberType, Type[pl.DataType]] = {
+    MemberType.BOOLEAN: pl.Boolean,
+    MemberType.DATE: pl.Date,
+    MemberType.TIME: pl.Time,
+    MemberType.DATETIME: pl.Datetime,
+    MemberType.TIMESTAMP: pl.UInt64,
+    MemberType.FLOAT32: pl.Float32,
+    MemberType.FLOAT64: pl.Float64,
+    MemberType.INT8: pl.Int8,
+    MemberType.INT16: pl.Int16,
+    MemberType.INT32: pl.Int32,
+    MemberType.INT64: pl.Int64,
+    MemberType.INT128: pl.Int64,
+    MemberType.UINT8: pl.UInt8,
+    MemberType.UINT16: pl.UInt16,
+    MemberType.UINT32: pl.UInt32,
+    MemberType.UINT64: pl.UInt64,
+    MemberType.UINT128: pl.UInt64,
+    MemberType.STRING: pl.String,
+}
+
+_MEMBERTYPE_REVERSE = {value: key.name for key, value in _POLARS_DATATYPES.items()}
```

### Comparing `tesseract_olap-0.9.1/tesseract_olap/schema/exceptions.py` & `tesseract_olap-0.9.2/tesseract_olap/exceptions/schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import Union
 
 from lxml import etree
 
-from tesseract_olap.common import BaseError
+from . import SchemaError
 
 
-class XMLParseError(BaseError):
+class XMLParseError(SchemaError):
     """An error happened while trying to parse a XML Schema."""
 
 
 class MalformedXML(XMLParseError):
     """An unexpected node was found."""
 
     def __init__(self, expected: str, actual: Union[str, etree._Element]) -> None:
-        message = (
-            "A node '{1}' was found while attempting to parse a '{0}'"
-        ).format(expected, actual)
+        message = ("A node '{1}' was found while attempting to parse a '{0}'").format(
+            expected, actual
+        )
         super().__init__(message)
 
 
 class InvalidXMLAttributeName(XMLParseError):
     """An invalid attribute was found in a node."""
 
     def __init__(self, node: str, node_name: str, attr: str) -> None:
@@ -40,54 +40,50 @@
         super().__init__(message)
 
 
 class MissingXMLNode(XMLParseError):
     """A required child node is missing."""
 
     def __init__(self, node: str, node_name: str, child_node: str) -> None:
-        message = (
-            "A '{2}' child node is missing in {0} '{1}'"
-        ).format(node, node_name, child_node)
+        message = ("A '{2}' child node is missing in {0} '{1}'").format(
+            node, node_name, child_node
+        )
         super().__init__(message)
 
 
 class MissingXMLAttribute(XMLParseError):
     """A required attribute is not present."""
 
     def __init__(self, node: str, attr: str) -> None:
-        message = (
-            "A required attribute '{1}' is missing in a '{0}' node"
-        ).format(node, attr)
+        message = ("A required attribute '{1}' is missing in a '{0}' node").format(
+            node, attr
+        )
         super().__init__(message)
 
 
-class JSONParseError(BaseError):
+class JSONParseError(SchemaError):
     """An error happened while trying to parse a JSON Schema."""
 
 
 class MalformedJSON(JSONParseError):
     """An unexpected object was found."""
 
     def __init__(self, expected: str) -> None:
         message = ""
         super().__init__(message)
 
 
-class SchemaError(BaseError):
-    """An error happened when validating the internal references in a schema."""
-
-
 class MissingPropertyError(SchemaError):
     """A mandatory property couldn't be retrieved from a Shared/Usage entity
     combination."""
 
     def __init__(self, entity: str, name: str, attr: str):
-        message = (
-            "There's a missing '{2}' attribute in {0} '{1}'."
-        ).format(entity, name, attr)
+        message = ("There's a missing '{2}' attribute in {0} '{1}'.").format(
+            entity, name, attr
+        )
         super().__init__(message)
 
 
 class InvalidNameError(SchemaError):
     """The name of an Entity contains invalid characters."""
 
     def __init__(self, cube: str, entity: str, name: str) -> None:
@@ -110,11 +106,11 @@
 
 
 class EntityUsageError(SchemaError):
     """There's a declared Usage reference pointing to a non-existent shared
     Entity."""
 
     def __init__(self, entity: str, source: str) -> None:
-        message = (
-            "An usage reference for '{}' {} cannot be found."
-        ).format(source, entity)
+        message = ("An usage reference for '{}' {} cannot be found.").format(
+            source, entity
+        )
         super().__init__(message)
```

### Comparing `tesseract_olap-0.9.1/tesseract_olap/schema/json.py` & `tesseract_olap-0.9.2/tesseract_olap/schema/json.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.1/tesseract_olap/schema/models.py` & `tesseract_olap-0.9.2/tesseract_olap/schema/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from dataclasses import dataclass, field
-from typing import Iterable, List, Mapping, Optional, Sequence, Tuple, Union
+from typing import Iterable, Mapping, Optional, Set, Tuple, Union
 
 import immutables as immu
 
 from tesseract_olap.common import get_localization
 
 from .aggregators import Aggregator, Count
 from .enums import DimensionType, MemberType
@@ -61,42 +61,47 @@
 
 
 @dataclass(eq=True, frozen=True, repr=False)
 class AccessControl:
     public: bool = True
     rules: Mapping[str, bool] = field(default_factory=immu.Map)
 
-    def __repr__(self) -> str:
-        return "Public" if self.public else f"Private({len(self.rules)})"
+    def __repr__(self):
+        return "Public" if self.public else f"Private(rules=<{len(self.rules)}>)"
 
     def is_authorized(self, roles: Iterable[str]) -> bool:
+        if self.public:
+            return True
         rules = self.rules
-        return self.public or any(rules.get(role, False) for role in roles)
+        roles = {roles} if isinstance(roles, str) else roles
+        if any(rules.get(role) is False for role in roles):  # restricted
+            return False
+        return any(rules.get(role, False) for role in roles)  # allowed
 
 
 @dataclass(eq=True, frozen=True, repr=False)
 class InlineTable:
     name: str
     headers: Tuple[str, ...]
     types: Tuple[MemberType, ...]
-    rows: List[Tuple[Union[str, float], ...]]
+    rows: Iterable[Tuple[Union[float, str], ...]]
 
-    def __repr__(self) -> str:
-        return "{0.__class__.__name__}(name='{0.name}')".format(self)
+    def __repr__(self):
+        return f"{type(self).__name__}(name={repr(self.name)})"
 
     @staticmethod
-    def infer_types(rows: Sequence[Tuple[Union[float, str], ...]]):
+    def infer_types(rows: Iterable[Tuple[Union[float, str], ...]]):
         return tuple(MemberType.from_values(column) for column in zip(*rows))
 
 
 class Entity:
     name: str
     annotations: Annotations
     captions: CaptionSet
-    acl: AccessControl = field(default_factory=AccessControl)
+    acl: AccessControl
 
     def get_annotation(self, name: str) -> Optional[str]:
         """Retrieves an annotation for the entity.
         If the annotation is not defined, raises a :class:`KeyError`.
         """
         return self.annotations[name]
 
@@ -105,23 +110,22 @@
         If the a caption hasn't been defined for said locale, will attempt to
         return the fallback caption, and if not defined either, will return the
         entity name.
         """
         caption = get_localization(self.captions, locale)
         return self.name if caption is None else caption
 
-    def get_locale_available(self) -> List[str]:
+    def get_locale_available(self) -> Set[str]:
         """Retrieves the list of locales for whose a caption has been defined in
         this entity.
         """
-        return sorted(self.captions.keys())
+        return set(self.captions.keys())
 
-    def is_authorized(self, role: Iterable[str]) -> bool:
-        role = {role} if isinstance(role, str) else role
-        return self.acl.is_authorized(role)
+    def is_authorized(self, roles: Iterable[str]) -> bool:
+        return self.acl.is_authorized(roles)
 
 
 @dataclass(eq=True, frozen=True)
 class Cube(Entity):
     name: str
     table: Union["InlineTable", "Table", str]
     acl: AccessControl = field(default_factory=AccessControl)
@@ -177,52 +181,60 @@
     name_column_map: Mapping[str, str] = field(default_factory=immu.Map)
     key_type: MemberType = MemberType.STRING
     property_map: Mapping[str, "Property"] = field(default_factory=immu.Map)
 
     def get_name_column(self, locale: str = "xx") -> Optional[str]:
         return get_localization(self.name_column_map, locale)
 
-    def get_locale_available(self) -> List[str]:
-        return sorted(set(self.captions.keys()).union(self.name_column_map.keys()))
+    def get_locale_available(self) -> Set[str]:
+        return set(self.captions.keys()).union(self.name_column_map.keys())
 
 
 @dataclass(eq=True, frozen=True)
 class Property(Entity):
     name: str
     annotations: Annotations = field(default_factory=immu.Map)
     captions: CaptionSet = field(default_factory=immu.Map)
     key_column_map: Mapping[str, str] = field(default_factory=immu.Map)
     key_type: MemberType = MemberType.STRING
 
     def get_key_column(self, locale: str = "xx") -> str:
         return get_localization(self.key_column_map, locale, force=True)
 
-    def get_locale_available(self) -> List[str]:
-        return sorted(set(self.captions.keys()).union(self.key_column_map.keys()))
+    def get_locale_available(self) -> Set[str]:
+        return set(self.captions.keys()).union(self.key_column_map.keys())
 
 
 @dataclass(eq=True, frozen=True)
 class Measure(Entity):
     name: str
     key_column: str
     aggregator: Aggregator = field(default_factory=Count)
     annotations: Annotations = field(default_factory=immu.Map)
     captions: CaptionSet = field(default_factory=immu.Map)
     submeasures: Mapping[str, "AnyMeasure"] = field(default_factory=immu.Map)
 
+    def and_submeasures(self):
+        yield self
+        yield from self.submeasures.values()
+
 
 @dataclass(eq=True, frozen=True)
 class CalculatedMeasure(Entity):
     name: str
     formula: AST
     aggregator: Aggregator = field(default_factory=Count)
     annotations: Annotations = field(default_factory=immu.Map)
     captions: CaptionSet = field(default_factory=immu.Map)
     submeasures: Mapping[str, "AnyMeasure"] = field(default_factory=immu.Map)
 
+    def and_submeasures(self):
+        yield self
+        yield from self.submeasures.values()
+
     @staticmethod
     def _parse_formula(formula: str) -> AST:
         return Parser(Lexer(formula)).parse()
 
 
 class Usage(Entity):
     """Defines a base class for Usage entities, so the type checker can enforce
```

### Comparing `tesseract_olap-0.9.1/tesseract_olap/schema/parser.py` & `tesseract_olap-0.9.2/tesseract_olap/schema/parser.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.1/tesseract_olap/schema/public.py` & `tesseract_olap-0.9.2/tesseract_olap/schema/public.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 from typing import List, Optional
 
 from . import traverse
 from .enums import DimensionType, MemberType
 from .models import Annotations
 
 
-@dataclass(eq=False, order=False)
+@dataclass(eq=False, frozen=True, order=False)
 class PublicSchema:
     name: str
+    locales: List[str]
     default_locale: str
     annotations: Annotations
     cubes: List["PublicCube"]
 
     @classmethod
     def from_entity(
         cls,
@@ -22,26 +23,26 @@
         locale: Optional[str] = None,
     ):
         """Generates a dataclass-schema object describing this entity."""
         default_locale = entity.schema.default_locale
         locale = default_locale if locale is None else locale
         return cls(
             name=entity.schema.name,
-            # "locales": self.get_locale_available(),
+            locales=sorted(entity.get_locale_available()),
             default_locale=default_locale,
             cubes=[
                 PublicCube.from_entity(item, locale)
                 for item in entity.cube_map.values()
                 if item.visible and item.is_authorized(roles)
             ],
             annotations=dict(entity.schema.annotations),
         )
 
 
-@dataclass(eq=False, order=False)
+@dataclass(eq=False, frozen=True, order=False)
 class PublicCube:
     name: str
     caption: str
     annotations: Annotations
     dimensions: List["PublicDimension"]
     measures: List["PublicMeasure"]
 
@@ -58,15 +59,15 @@
             measures=[
                 PublicMeasure.from_entity(item, locale) for item in entity.measures
             ],
             annotations=dict(entity.annotations),
         )
 
 
-@dataclass(eq=False, order=False)
+@dataclass(eq=False, frozen=True, order=False)
 class PublicMeasure:
     name: str
     caption: str
     aggregator: str
     annotations: Annotations
     attached: List["PublicMeasure"]
 
@@ -80,15 +81,15 @@
             annotations=dict(entity.annotations),
             attached=[
                 cls.from_entity(item, locale) for item in entity.submeasures.values()
             ],
         )
 
 
-@dataclass(eq=False, order=False)
+@dataclass(eq=False, frozen=True, order=False)
 class PublicDimension:
     name: str
     caption: str
     type: DimensionType
     annotations: Annotations
     hierarchies: List["PublicHierarchy"]
     default_hierarchy: str
@@ -104,15 +105,15 @@
             hierarchies=[
                 PublicHierarchy.from_entity(item, locale) for item in entity.hierarchies
             ],
             default_hierarchy=entity._entity.default_hierarchy,
         )
 
 
-@dataclass(eq=False, order=False)
+@dataclass(eq=False, frozen=True, order=False)
 class PublicHierarchy:
     name: str
     caption: str
     annotations: Annotations
     levels: List["PublicLevel"]
 
     @classmethod
@@ -122,15 +123,15 @@
             name=entity.name,
             caption=entity.get_caption(locale),
             annotations=dict(entity.annotations),
             levels=[PublicLevel.from_entity(item, locale) for item in entity.levels],
         )
 
 
-@dataclass(eq=False, order=False)
+@dataclass(eq=False, frozen=True, order=False)
 class PublicLevel:
     name: str
     caption: str
     depth: int
     annotations: Annotations
     properties: List["PublicProperty"]
 
@@ -144,15 +145,15 @@
             annotations=dict(entity.annotations),
             properties=[
                 PublicProperty.from_entity(item, locale) for item in entity.properties
             ],
         )
 
 
-@dataclass(eq=False, order=False)
+@dataclass(eq=False, frozen=True, order=False)
 class PublicProperty:
     name: str
     caption: str
     type: MemberType
     annotations: Annotations
 
     @classmethod
```

### Comparing `tesseract_olap-0.9.1/tesseract_olap/schema/schema.xsd` & `tesseract_olap-0.9.2/tesseract_olap/schema/schema.xsd`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.1/tesseract_olap/schema/traverse.py` & `tesseract_olap-0.9.2/tesseract_olap/schema/traverse.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,36 +4,38 @@
 from itertools import chain
 from typing import (
     TYPE_CHECKING,
     Dict,
     Generic,
     Iterable,
     Iterator,
-    List,
     Mapping,
     Optional,
     OrderedDict,
+    Set,
     TypeVar,
     Union,
 )
 
+import immutables as immu
+
 from tesseract_olap.common import T, get_localization
-from tesseract_olap.query.exceptions import (
+from tesseract_olap.exceptions.query import (
     InvalidEntityName,
     TimeDimensionUnavailable,
     TimeScaleUnavailable,
 )
-
-from .enums import DimensionType, MemberType
-from .exceptions import (
+from tesseract_olap.exceptions.schema import (
     DuplicatedNameError,
     EntityUsageError,
     InvalidNameError,
     MissingPropertyError,
 )
+
+from .enums import DimensionType, MemberType
 from .models import (
     Annotations,
     AnyMeasure,
     CalculatedMeasure,
     CaptionSet,
     Cube,
     Dimension,
@@ -67,17 +69,22 @@
     """Wrapper class for Schema model, to generate the relationships between the
     shared entities and their usages.
     """
 
     def __init__(self, schema: "Schema"):
         self.schema = schema
         self.cube_map = OrderedDict(
-            (name, CubeTraverser(cube,
-                                 dimension_map=schema.shared_dimension_map,
-                                 table_map=schema.shared_table_map))
+            (
+                name,
+                CubeTraverser(
+                    cube,
+                    dimension_map=schema.shared_dimension_map,
+                    table_map=schema.shared_table_map,
+                ),
+            )
             for name, cube in schema.cube_map.items()
         )
 
     def __len__(self) -> int:
         return len(self.cube_map)
 
     def __getitem__(self, key: str) -> "CubeTraverser":
@@ -92,37 +99,36 @@
 
     def get_cube(self, cube_name: str) -> "CubeTraverser":
         try:
             return self.cube_map[cube_name]
         except KeyError:
             raise InvalidEntityName("Cube", cube_name) from None
 
-    def get_locale_available(self) -> List[str]:
-        locales = set()
+    def get_locale_available(self) -> Set[str]:
+        locales = {self.schema.default_locale}
         for item in self.cube_map.values():
             locales.update(item.get_locale_available())
         # TODO: add from shared_dimension_map and shared_table_map
         locales.discard("xx")
-        locales.add(self.schema.default_locale)
-        return sorted(locales)
+        return locales
 
     def is_authorized(self, request: "RequestWithRoles") -> bool:
         """Validates a request has enough permissions to be executed."""
         return self.get_cube(request.cube).is_authorized(request.roles)
 
     def validate(self):
         """Performs some verifications on the resulting data structure, after
         parsing the schema file."""
 
         for cube in self.cube_map.values():
             cubename = cube.name
             nameset = {item.name: type(item).__name__ for item in cube.measures}
 
             for measure in cube.measures:
-                for item in measure.submeasures.values():
+                for item in measure.and_submeasures():
                     validate_entity_names(cubename, item, nameset)
 
             for level in cube.levels:
                 validate_entity_names(cubename, level, nameset)
                 for prop in level.properties:
                     validate_entity_names(cubename, prop, nameset)
 
@@ -137,15 +143,15 @@
 
             # Index fact tables
             tables[table.name].update(
                 [table.primary_key],
                 (
                     item.key_column
                     for measure in cube.measures
-                    for item in (measure, *measure.submeasures.values())
+                    for item in measure.and_submeasures()
                     if isinstance(item, Measure)
                 ),
                 (dimension.foreign_key for dimension in cube.dimensions),
             )
 
             for hierarchy in cube.hierarchies:
                 table = hierarchy.table
@@ -193,26 +199,36 @@
         cube: "Cube",
         *,
         dimension_map: Mapping[str, "Dimension"],
         table_map: Mapping[str, "InlineTable"],
     ) -> None:
         self._cube = cube
         self._dimension_map = OrderedDict(
-            (name, DimensionTraverser(item, table_map=table_map)
-                   if isinstance(item, Dimension) else
-                   DimensionTraverser(
-                       get_shared_entity(dimension_map, item.source), item,
-                       table_map=table_map))
+            (
+                name,
+                DimensionTraverser(item, table_map=table_map)
+                if isinstance(item, Dimension)
+                else DimensionTraverser(
+                    get_shared_entity(dimension_map, item.source),
+                    item,
+                    table_map=table_map,
+                ),
+            )
             for name, item in cube.dimension_map.items()
         )
-        self._table = table_map[cube.table] \
-                      if isinstance(cube.table, str) else \
-                      cube.table
+        self.measure_map = immu.Map(
+            (item.name, item)
+            for measure in self._cube.measure_map.values()
+            for item in measure.and_submeasures()
+        )
+        self._table = (
+            table_map[cube.table] if isinstance(cube.table, str) else cube.table
+        )
 
-    def __repr__(self) -> str:
+    def __repr__(self):
         return f"CubeTraverser(name='{self._cube.name}', table={self.table})"
 
     def __getattr__(self, _name: str):
         return getattr(self._cube, _name)
 
     @property
     def table(self) -> Union["Table", "InlineTable"]:
@@ -220,27 +236,27 @@
 
     @property
     def measures(self) -> Iterable["AnyMeasure"]:
         return self._cube.measure_map.values()
 
     @property
     def calculated_measures(self) -> Iterable["CalculatedMeasure"]:
-        return (item
-                for item in self._cube.measure_map.values()
-                if isinstance(item, CalculatedMeasure))
+        return (
+            item
+            for item in self._cube.measure_map.values()
+            if isinstance(item, CalculatedMeasure)
+        )
 
     @property
     def dimensions(self) -> Iterable["DimensionTraverser"]:
         return self._dimension_map.values()
 
     @property
     def time_dimensions(self) -> Iterable["DimensionTraverser"]:
-        return (item
-                for item in self.dimensions
-                if item.dim_type == DimensionType.TIME)
+        return (item for item in self.dimensions if item.dim_type == DimensionType.TIME)
 
     @property
     def hierarchies(self) -> Iterable["HierarchyTraverser"]:
         return chain(*(item.hierarchies for item in self.dimensions))
 
     @property
     def levels(self) -> Iterable["LevelTraverser"]:
@@ -259,31 +275,31 @@
 
     def get_annotation(self, name: str) -> Optional[str]:
         return self._cube.get_annotation(name)
 
     def get_caption(self, locale: str = "xx") -> str:
         return self._cube.get_caption(locale)
 
-    def get_locale_available(self) -> List[str]:
+    def get_locale_available(self) -> Set[str]:
         """Returns a list of strings containing the locale code keys available
         for captions in entities inside this :class:`Cube`."""
         locales = set(self.captions.keys())
         for item in self.dimensions:
             locales.update(item.get_locale_available())
         for item in self.measures:
             locales.update(item.get_locale_available())
-        return sorted(locales)
+        return locales
 
     def get_measure(self, name: str) -> "AnyMeasure":
         """Attempts to retrieve a Measure by its name.
 
         Raises :class:`InvalidEntityName` if the entity can't be found.
         """
         try:
-            return self._cube.measure_map[name]
+            return self.measure_map[name]
         except KeyError:
             raise InvalidEntityName("Measure", name) from None
 
     def get_dimension(self, name: str) -> "DimensionTraverser":
         """Attempts to retrieve a Dimension by its name.
 
         Raises :class:`InvalidEntityName` if the entity can't be found.
@@ -321,25 +337,27 @@
         Raises :class:`TimeDimensionUnavailable` if the :class:`Cube` doesn't
         contain a TIME-type :class:`Dimension`, and :class:`TimeScaleUnavailable`
         if the time scale requested is not available in the :class:`Dimension`.
         """
         dimension = None
 
         for dimension in self.time_dimensions:
-            exact_match = next((item for item in dimension.levels
-                               if item.name == scale), None)
+            exact_match = next(
+                (item for item in dimension.levels if item.name == scale), None
+            )
             if exact_match is not None:
                 return exact_match
 
         if dimension is None:
             raise TimeDimensionUnavailable(self._cube.name)
 
         for dimension in self.time_dimensions:
-            substr_match = next((item for item in dimension.levels
-                                if scale in item.name.lower()), None)
+            substr_match = next(
+                (item for item in dimension.levels if scale in item.name.lower()), None
+            )
             if substr_match is not None:
                 return substr_match
 
         raise TimeScaleUnavailable(self._cube.name, scale)
 
     def get_property(self, name: str) -> "PropertyTraverser":
         """Attempts to retrieve a Property by its name.
@@ -347,15 +365,15 @@
         Raises :class:`InvalidEntityName` if the entity can't be found.
         """
         try:
             return next(item for item in self.properties if item.name == name)
         except StopIteration:
             raise InvalidEntityName("Property", name) from None
 
-    def is_authorized(self, roles: Iterable[str]):
+    def is_authorized(self, roles: Iterable[str]) -> bool:
         return self._cube.is_authorized(roles)
 
 
 class EntityUsageTraverser(Generic[EntityType, UsageType]):
     """Wrapper class to unify an usage with its entity.
 
     Its properties are looked on the usage, then on the entity if not found.
@@ -375,16 +393,16 @@
 
     def __dir__(self) -> Iterable[str]:
         return sorted(set(dir(self._entity) + dir(self)))
 
     def __getattr__(self, name: str):
         return getattr(self._entity, name)
 
-    def __repr__(self) -> str:
-        return "{}(name='{}')".format(self.__class__.__name__, self.name)
+    def __repr__(self):
+        return f"{type(self).__name__}(name={repr(self.name)})"
 
     @property
     def name(self) -> str:
         """Returns the new name given by the usage reference, or the original
         name of the entity if not defined."""
         return self._entity.name if self._usage is None else self._usage.name
 
@@ -415,19 +433,19 @@
         If the a caption hasn't been defined for said locale, will attempt to
         return the fallback caption, and if not defined either, will return the
         entity name.
         """
         caption = get_localization(self.captions, locale)
         return self.name if caption is None else caption
 
-    def get_locale_available(self) -> List[str]:
+    def get_locale_available(self) -> Set[str]:
         """Retrieves the list of locales for whose a caption has been defined in
         this entity.
         """
-        return sorted(self.captions.keys())
+        return set(self.captions.keys())
 
 
 class DimensionTraverser(EntityUsageTraverser[Dimension, DimensionUsage]):
     """Allows seamless aliasing of values between a Dimension and a DimensionUsage."""
 
     hierarchy_map: Mapping[str, "HierarchyTraverser"]
     dim_type: DimensionType
@@ -444,29 +462,33 @@
         if usage is None or len(usage.hierarchy_map) == 0:
             self.hierarchy_map = OrderedDict(
                 (name, HierarchyTraverser(item, table_map=table_map))
                 for name, item in entity.hierarchy_map.items()
             )
         else:
             self.hierarchy_map = OrderedDict(
-                (name, HierarchyTraverser(
-                    entity.hierarchy_map[item.source], item, table_map=table_map
-                ))
+                (
+                    name,
+                    HierarchyTraverser(
+                        entity.hierarchy_map[item.source], item, table_map=table_map
+                    ),
+                )
                 for name, item in usage.hierarchy_map.items()
             )
 
     @property
     def foreign_key(self) -> str:
         """Returns the foreign key for this Dimension."""
         # A DimensionTraverser represents PrivateDimension or DimensionUsage,
         # and the foreign_key property must be present in both, final value
         # depends solely on self._usage presence.
         if self._usage is not None:
             return self._usage.foreign_key
-        if self._entity.foreign_key is None:  # should be unreachable, but checks types
+        if self._entity.foreign_key is None:
+            # should be unreachable, but checks types
             raise MissingPropertyError("Dimension", self.name, "foreign_key")
         return self._entity.foreign_key
 
     @property
     def default_hierarchy(self) -> "HierarchyTraverser":
         hie = self._entity.get_default_hierarchy()
         if self._usage is None:
```

### Comparing `tesseract_olap-0.9.1/tesseract_olap/schema/xml.py` & `tesseract_olap-0.9.2/tesseract_olap/schema/xml.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,20 +19,24 @@
     Union,
 )
 
 import immutables as immu
 from lxml import etree
 
 from tesseract_olap.common import is_numeric, numerify
+from tesseract_olap.exceptions.schema import (
+    InvalidXMLAttributeValue,
+    MissingXMLAttribute,
+    MissingXMLNode,
+)
 
 from . import models
 from .aggregators import Aggregator
 from .csv import parse_csv
 from .enums import AggregatorType, DimensionType, MemberType
-from .exceptions import InvalidXMLAttributeValue, MissingXMLAttribute, MissingXMLNode
 
 logger = logging.getLogger(__name__)
 
 XMLEntity = Union[
     "XMLSharedDimension",
     "XMLHierarchy",
     "XMLLevel",
```

### Comparing `tesseract_olap-0.9.1/tesseract_olap/server/exceptions.py` & `tesseract_olap-0.9.2/tesseract_olap/exceptions/server.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,21 @@
-from tesseract_olap.common import BaseError
-
-
-class ServerError(BaseError):
-    """Base class for exceptions in `tesseract_olap.server` module."""
+from . import ServerError
 
 
 class UnknownBackendError(ServerError):
     """This error occurs when the user attempts to initialize the Server with
     a connection string that doesn't match any known compatible Backend.
 
     The user must be informed to ensure they're using a compatible database.
     """
 
     def __init__(self, connection_str: str) -> None:
-        message = (
-            "Couldn't find a matching Backend for connection string: {}"
-        ).format(connection_str)
-        super().__init__(message)
+        super().__init__(
+            f"Couldn't find a matching Backend for connection string: {connection_str}"
+        )
 
 
 class UnknownSchemaError(ServerError):
     """This error occurs when the user attempts to point the location of the
     Schema to a file in an unknown format.
 
     The user must be informed that by default, only XML and JSON files are
```

### Comparing `tesseract_olap-0.9.1/tesseract_olap/server/schema.py` & `tesseract_olap-0.9.2/tesseract_olap/server/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import logging
 from itertools import chain
 from pathlib import Path
 from typing import TextIO, Union
 
 import httpx
 
+from tesseract_olap.exceptions.server import UnknownSchemaError
 from tesseract_olap.schema import (
     Schema,
     parse_csv_schema,
     parse_json_schema,
     parse_xml_schema,
 )
 
-from .exceptions import UnknownSchemaError
-
 logger = logging.getLogger("tesseract_olap.server")
 
 
 def setup_schema(source: Union[str, Path, TextIO]) -> "Schema":
     """Generates a new Schema instance from a string source.
 
     The source can be a path to a local file, an URL to an external schema file,
@@ -75,30 +74,35 @@
             % (source, response.status_code)
         )
 
     path = response.url.path
     ctype = response.headers["Content-Type"].lower()
     text = response.text.strip()
 
-    if path.endswith(".xml") \
-    or ctype == "text/xml" \
-    or text.startswith(("<Schema ", "<?xml ")):
+    if (
+        path.endswith(".xml")
+        or ctype == "text/xml"
+        or text.startswith(("<Schema ", "<?xml "))
+    ):
         logger.debug("Parsing XML schema from URL: %s", source)
         return parse_xml_schema(text)
 
-    if path.endswith(".json") \
-    or ctype == "application/json" \
-    or text.startswith(('{"', "[{")):
+    if (
+        path.endswith(".json")
+        or ctype == "application/json"
+        or text.startswith(('{"', "[{"))
+    ):
         logger.debug("Parsing JSON schema from URL: %s", source)
         return parse_json_schema(text)
 
-    if path.endswith(".csv") \
-    or ctype in ("text/csv", "application/vnd.ms-excel"):
+    if path.endswith(".csv") or ctype in ("text/csv", "application/vnd.ms-excel"):
         logger.debug("Parsing CSV table from URL: %s", source)
-        return parse_csv_schema(text)
+        _, _, table_name = path.rpartition("/")
+        table_name = table_name.replace(".csv", "")
+        return parse_csv_schema(text, table_name)
 
     raise UnknownSchemaError("Linked source couldn't be parsed: %s" % source)
 
 
 def _parse_source_raw_string(source: str) -> Union["Schema", None]:
     """Attempts to parse the contents of the provided string as a Schema."""
     # Check if argument is a raw XML string
```

### Comparing `tesseract_olap-0.9.1/tesseract_olap/server/server.py` & `tesseract_olap-0.9.2/tesseract_olap/server/server.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import logging
 from pathlib import Path
 from typing import Union
 
 from typing_extensions import deprecated
 
-from tesseract_olap.backend import Backend
+from tesseract_olap.backend import Backend, CacheProvider, DummyProvider
+from tesseract_olap.exceptions.query import InvalidQuery
+from tesseract_olap.exceptions.server import UnknownBackendError
 from tesseract_olap.query import (
     AnyRequest,
     DataQuery,
     DataRequest,
     MembersQuery,
     MembersRequest,
 )
-from tesseract_olap.query.exceptions import InvalidQuery
 from tesseract_olap.schema import Schema, SchemaTraverser
 
-from .exceptions import UnknownBackendError
 from .schema import setup_schema
 
 logger = logging.getLogger("tesseract_olap.server")
 
 
 class OlapServer:
     """Main server class.
@@ -27,22 +27,29 @@
     This object manages the connection with the backend database and the schema
     instance containing the database references, to enable make queries against
     them.
     """
 
     schema: "SchemaTraverser"
     backend: "Backend"
+    cache: "CacheProvider"
 
     def __init__(
-        self, backend: Union[str, "Backend"], schema: Union[str, "Path", "Schema"]
+        self,
+        *,
+        backend: Union[str, "Backend"],
+        schema: Union[str, "Path", "Schema"],
+        cache: Union[str, "CacheProvider"] = "",
     ):
         self.backend = (
             backend if isinstance(backend, Backend) else _setup_backend(backend)
         )
 
+        self.cache = cache if isinstance(cache, CacheProvider) else _setup_cache(cache)
+
         self.schema = SchemaTraverser(
             schema if isinstance(schema, Schema) else setup_schema(schema)
         )
 
     @property
     def raw_schema(self):
         """Retrieves the raw Schema instance used by this server."""
@@ -72,15 +79,15 @@
         """
         try:
             return self.backend.ping()
         except Exception:
             return False
 
     def session(self):
-        return self.backend.new_session()
+        return self.backend.new_session(cache=self.cache)
 
     def validate(self):
         """Verifies the information declared in the Schema matches the data
         structures in the Backend."""
         self.schema.validate()
         self.backend.validate_schema(self.schema)
 
@@ -91,7 +98,17 @@
     """
     if dsn.startswith("clickhouse:") or dsn.startswith("clickhouses:"):
         from tesseract_olap.backend.clickhouse import ClickhouseBackend
 
         return ClickhouseBackend(dsn)
 
     raise UnknownBackendError(dsn)
+
+
+def _setup_cache(dsn: str) -> CacheProvider:
+    """Generates a new instance of a CacheProvider bundled in this package."""
+    if dsn.startswith("redis:") or dsn.startswith("rediss:"):
+        from tesseract_olap.backend.redis import RedisProvider
+
+        return RedisProvider(dsn)
+
+    return DummyProvider()
```

### Comparing `tesseract_olap-0.9.1/PKG-INFO` & `tesseract_olap-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tesseract-olap
-Version: 0.9.1
+Version: 0.9.2
 Summary: A simple OLAP library.
 Home-page: https://github.com/Datawheel/tesseract-python
 License: MIT
 Author: Francisco Abarzua
 Author-email: francisco@datawheel.us
 Maintainer: Francisco Abarzua
 Maintainer-email: francisco@datawheel.us
@@ -13,22 +13,24 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: clickhouse
+Provides-Extra: redis
 Requires-Dist: PyPika (>=0.48.0,<1.0)
 Requires-Dist: clickhouse-cityhash (>=1.0.2.4,<2.0.0.0) ; extra == "clickhouse"
 Requires-Dist: clickhouse-driver[lz4] (>=0.2.0,<0.3.0) ; extra == "clickhouse"
 Requires-Dist: httpx (>=0.18.0,<1.0)
 Requires-Dist: immutables (>=0.16,<1.0)
 Requires-Dist: lxml (>=4.6.0,<5.0.0)
 Requires-Dist: orjson (>=3.9.15,<4.0.0)
 Requires-Dist: polars (>=0.20.0,<0.21.0)
+Requires-Dist: redis (>=5.0.0,<6.0.0) ; extra == "redis"
 Requires-Dist: typing-extensions (>=3.7.4)
 Requires-Dist: xlsxwriter (>=3.2.0,<4.0.0)
 Project-URL: Repository, https://github.com/Datawheel/tesseract-python
 Description-Content-Type: text/markdown
 
 <p>
 <a href="https://github.com/Datawheel/tesseract-python/releases"><img src="https://flat.badgen.net/github/release/Datawheel/tesseract-python" /></a>
```

