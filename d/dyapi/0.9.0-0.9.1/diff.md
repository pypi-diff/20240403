# Comparing `tmp/dyapi-0.9.0.tar.gz` & `tmp/dyapi-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyapi-0.9.0.tar", max compression
+gzip compressed data, was "dyapi-0.9.1.tar", max compression
```

## Comparing `dyapi-0.9.0.tar` & `dyapi-0.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     3693 2024-03-31 19:41:39.711292 dyapi-0.9.0/README.md
--rw-r--r--   0        0        0      462 2024-04-02 06:08:42.117154 dyapi-0.9.0/dyapi/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 11:00:17.031695 dyapi-0.9.0/dyapi/entities/__init__.py
--rw-r--r--   0        0        0      556 2024-03-29 16:33:17.090998 dyapi-0.9.0/dyapi/entities/config.py
--rw-r--r--   0        0        0      308 2024-03-31 17:47:11.932909 dyapi-0.9.0/dyapi/entities/endpoint_settings.py
--rw-r--r--   0        0        0      235 2024-03-29 17:06:44.747416 dyapi-0.9.0/dyapi/entities/model_settings.py
--rw-r--r--   0        0        0      331 2024-03-29 11:50:46.579490 dyapi-0.9.0/dyapi/entities/pagination.py
--rw-r--r--   0        0        0        0 2024-03-29 08:54:12.822771 dyapi-0.9.0/dyapi/implementations/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 09:10:39.710706 dyapi-0.9.0/dyapi/implementations/builders/__init__.py
--rw-r--r--   0        0        0     2063 2024-03-31 19:30:12.023845 dyapi-0.9.0/dyapi/implementations/builders/api.py
--rw-r--r--   0        0        0     3666 2024-04-02 06:40:17.957670 dyapi-0.9.0/dyapi/implementations/builders/crud.py
--rw-r--r--   0        0        0     8076 2024-04-01 11:46:03.964862 dyapi-0.9.0/dyapi/implementations/builders/endpoint.py
--rw-r--r--   0        0        0     1419 2024-03-31 19:09:31.317882 dyapi-0.9.0/dyapi/implementations/builders/model.py
--rw-r--r--   0        0        0        0 2024-03-29 11:51:32.889326 dyapi-0.9.0/dyapi/implementations/storages/__init__.py
--rw-r--r--   0        0        0      141 2024-03-29 11:50:46.360544 dyapi-0.9.0/dyapi/implementations/storages/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-29 11:52:43.740255 dyapi-0.9.0/dyapi/implementations/storages/postgres/__init__.py
--rw-r--r--   0        0        0     6517 2024-04-01 11:42:18.110833 dyapi-0.9.0/dyapi/implementations/storages/postgres/base.py
--rw-r--r--   0        0        0     2349 2024-03-31 20:27:44.610185 dyapi-0.9.0/dyapi/implementations/storages/postgres/manager.py
--rw-r--r--   0        0        0        0 2024-03-29 09:09:32.173661 dyapi-0.9.0/dyapi/interfaces/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 08:49:20.167380 dyapi-0.9.0/dyapi/interfaces/builders/__init__.py
--rw-r--r--   0        0        0      775 2024-03-31 17:47:11.947727 dyapi-0.9.0/dyapi/interfaces/builders/api.py
--rw-r--r--   0        0        0      909 2024-03-31 17:47:11.948512 dyapi-0.9.0/dyapi/interfaces/builders/crud.py
--rw-r--r--   0        0        0     1319 2024-03-31 16:53:23.735626 dyapi-0.9.0/dyapi/interfaces/builders/endpoint.py
--rw-r--r--   0        0        0     1027 2024-03-31 17:47:11.949901 dyapi-0.9.0/dyapi/interfaces/builders/model.py
--rw-r--r--   0        0        0      118 2024-03-29 16:30:09.491190 dyapi-0.9.0/dyapi/interfaces/storages/__init__.py
--rw-r--r--   0        0        0      846 2024-03-31 20:27:44.610243 dyapi-0.9.0/dyapi/interfaces/storages/base.py
--rw-r--r--   0        0        0      235 2024-03-31 17:47:12.079538 dyapi-0.9.0/dyapi/interfaces/storages/manager.py
--rw-r--r--   0        0        0     2154 2024-04-02 08:11:41.795168 dyapi-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     4214 1970-01-01 00:00:00.000000 dyapi-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     3693 2024-03-31 19:41:39.711292 dyapi-0.9.1/README.md
+-rw-r--r--   0        0        0      463 2024-04-02 10:45:19.035467 dyapi-0.9.1/dyapi/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-29 11:00:17.031695 dyapi-0.9.1/dyapi/entities/__init__.py
+-rw-r--r--   0        0        0      556 2024-03-29 16:33:17.090998 dyapi-0.9.1/dyapi/entities/config.py
+-rw-r--r--   0        0        0      308 2024-03-31 17:47:11.932909 dyapi-0.9.1/dyapi/entities/endpoint_settings.py
+-rw-r--r--   0        0        0      235 2024-03-29 17:06:44.747416 dyapi-0.9.1/dyapi/entities/model_settings.py
+-rw-r--r--   0        0        0      331 2024-03-29 11:50:46.579490 dyapi-0.9.1/dyapi/entities/pagination.py
+-rw-r--r--   0        0        0        0 2024-03-29 08:54:12.822771 dyapi-0.9.1/dyapi/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-29 09:10:39.710706 dyapi-0.9.1/dyapi/implementations/builders/__init__.py
+-rw-r--r--   0        0        0     2063 2024-03-31 19:30:12.023845 dyapi-0.9.1/dyapi/implementations/builders/api.py
+-rw-r--r--   0        0        0     3643 2024-04-02 11:09:55.856179 dyapi-0.9.1/dyapi/implementations/builders/crud.py
+-rw-r--r--   0        0        0     8080 2024-04-02 11:09:55.741953 dyapi-0.9.1/dyapi/implementations/builders/endpoint.py
+-rw-r--r--   0        0        0     2986 2024-04-02 13:02:40.304147 dyapi-0.9.1/dyapi/implementations/builders/model.py
+-rw-r--r--   0        0        0        0 2024-03-29 11:51:32.889326 dyapi-0.9.1/dyapi/implementations/storages/__init__.py
+-rw-r--r--   0        0        0      141 2024-03-29 11:50:46.360544 dyapi-0.9.1/dyapi/implementations/storages/exceptions.py
+-rw-r--r--   0        0        0        0 2024-03-29 11:52:43.740255 dyapi-0.9.1/dyapi/implementations/storages/postgres/__init__.py
+-rw-r--r--   0        0        0     6517 2024-04-02 12:58:49.115195 dyapi-0.9.1/dyapi/implementations/storages/postgres/base.py
+-rw-r--r--   0        0        0     2311 2024-04-02 10:56:42.827026 dyapi-0.9.1/dyapi/implementations/storages/postgres/manager.py
+-rw-r--r--   0        0        0        0 2024-03-29 09:09:32.173661 dyapi-0.9.1/dyapi/interfaces/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-29 08:49:20.167380 dyapi-0.9.1/dyapi/interfaces/builders/__init__.py
+-rw-r--r--   0        0        0      775 2024-03-31 17:47:11.947727 dyapi-0.9.1/dyapi/interfaces/builders/api.py
+-rw-r--r--   0        0        0      909 2024-03-31 17:47:11.948512 dyapi-0.9.1/dyapi/interfaces/builders/crud.py
+-rw-r--r--   0        0        0     1319 2024-03-31 16:53:23.735626 dyapi-0.9.1/dyapi/interfaces/builders/endpoint.py
+-rw-r--r--   0        0        0     1027 2024-03-31 17:47:11.949901 dyapi-0.9.1/dyapi/interfaces/builders/model.py
+-rw-r--r--   0        0        0      118 2024-03-29 16:30:09.491190 dyapi-0.9.1/dyapi/interfaces/storages/__init__.py
+-rw-r--r--   0        0        0      846 2024-03-31 20:27:44.610243 dyapi-0.9.1/dyapi/interfaces/storages/base.py
+-rw-r--r--   0        0        0      235 2024-03-31 17:47:12.079538 dyapi-0.9.1/dyapi/interfaces/storages/manager.py
+-rw-r--r--   0        0        0     2154 2024-04-03 08:05:33.700515 dyapi-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     4214 1970-01-01 00:00:00.000000 dyapi-0.9.1/PKG-INFO
```

### Comparing `dyapi-0.9.0/README.md` & `dyapi-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `dyapi-0.9.0/dyapi/entities/config.py` & `dyapi-0.9.1/dyapi/entities/config.py`

 * *Files identical despite different names*

### Comparing `dyapi-0.9.0/dyapi/implementations/builders/api.py` & `dyapi-0.9.1/dyapi/implementations/builders/api.py`

 * *Files identical despite different names*

### Comparing `dyapi-0.9.0/dyapi/implementations/builders/crud.py` & `dyapi-0.9.1/dyapi/implementations/builders/crud.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from functools import cached_property
-from typing import AsyncContextManager, Type
-
-from fastapi import APIRouter
-from pydantic import BaseModel
-from sqlalchemy.ext.asyncio import AsyncSession
-from sqlalchemy.orm import DeclarativeBase
+from typing import Any, AsyncGenerator, Callable, Type
 
 from dyapi.entities.config import Config
 from dyapi.implementations.builders.endpoint import SQLAlchemyEndpointBuilder
 from dyapi.interfaces.builders.crud import ICRUDBuilder
 from dyapi.interfaces.builders.endpoint import IEndpointBuilder
 from dyapi.interfaces.builders.model import IModelBuilder
 from dyapi.interfaces.storages import IStorageManager
+from fastapi import APIRouter
+from pydantic import BaseModel
+from sqlalchemy.orm import DeclarativeBase
 
 
 class CRUDBuilder(ICRUDBuilder):
     def __init__(
         self,
         config: Config,
         storage_manager: IStorageManager,
@@ -65,21 +63,21 @@
         return router
 
 
 class SQLAlchemyCRUDBuilder:
     def __init__(
         self,
         db_model: Type[DeclarativeBase],
-        db_session: AsyncContextManager[AsyncSession],
+        db_session: Callable[[Any], AsyncGenerator[Any, None]],
         schema: Type[BaseModel],
         update_schema: Type[BaseModel],
         path_schema: Type[BaseModel],
         filter_schema: Type[BaseModel],
-        api_tags: list[str] = None,
-        api_prefix: str = '',
+        api_tags: list[str] | None = None,
+        api_prefix: str = "",
     ):
         """
 
         :param db_model:
         :param db_session:
         :param update_schema:
         """
```

### Comparing `dyapi-0.9.0/dyapi/implementations/builders/endpoint.py` & `dyapi-0.9.1/dyapi/implementations/builders/endpoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from functools import cached_property
-from typing import Any, AsyncContextManager, Callable, Type
+from typing import Any, AsyncGenerator, Callable, Type
 
 from dyapi.entities.pagination import PaginationContainer, PaginationEntity
 from dyapi.implementations.storages.exceptions import AlreadyExistsError, NotFoundError
 from dyapi.implementations.storages.postgres.base import SQLAlchemyStorage
 from dyapi.interfaces.builders.endpoint import IEndpointBuilder
 from dyapi.interfaces.builders.model import IModelBuilder
 from dyapi.interfaces.storages import IStorage
@@ -113,15 +113,15 @@
         return endpoint
 
 
 class SQLAlchemyEndpointBuilder:
     def __init__(
         self,
         db_model: Type[DeclarativeBase],
-        db_session: AsyncContextManager[AsyncSession],
+        db_session: Callable[[Any], AsyncGenerator[Any, None]],
         schema: Type[BaseModel],
         path_schema: Type[BaseModel],
         filter_schema: Type[BaseModel],
         update_schema: Type[BaseModel],
     ):
         self.db_model = db_model
         self.db_session = db_session
```

### Comparing `dyapi-0.9.0/dyapi/implementations/storages/postgres/base.py` & `dyapi-0.9.1/dyapi/implementations/storages/postgres/base.py`

 * *Files identical despite different names*

### Comparing `dyapi-0.9.0/dyapi/implementations/storages/postgres/manager.py` & `dyapi-0.9.1/dyapi/implementations/storages/postgres/manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import AsyncContextManager, Callable
-
-from sqlalchemy import Column, Float, Integer, MetaData, String, Table, UniqueConstraint
-from sqlalchemy.ext.asyncio import AsyncConnection, AsyncEngine, AsyncSession
+from typing import Callable
 
 from dyapi.entities.config import Config, ConfigField
 from dyapi.interfaces.storages import IStorage, IStorageManager
+from sqlalchemy import Column, Float, Integer, MetaData, String, Table, UniqueConstraint
+from sqlalchemy.ext.asyncio import AsyncEngine, AsyncSession
+
 from .base import PostgresEngineStorage, PostgresSessionStorage
 
 __all__ = ["PostgresEngineStorageManager"]
 
 
 class PostgresStorageManager:
     @staticmethod
```

### Comparing `dyapi-0.9.0/dyapi/interfaces/builders/api.py` & `dyapi-0.9.1/dyapi/interfaces/builders/api.py`

 * *Files identical despite different names*

### Comparing `dyapi-0.9.0/dyapi/interfaces/builders/crud.py` & `dyapi-0.9.1/dyapi/interfaces/builders/crud.py`

 * *Files identical despite different names*

### Comparing `dyapi-0.9.0/dyapi/interfaces/builders/endpoint.py` & `dyapi-0.9.1/dyapi/interfaces/builders/endpoint.py`

 * *Files identical despite different names*

### Comparing `dyapi-0.9.0/dyapi/interfaces/builders/model.py` & `dyapi-0.9.1/dyapi/interfaces/builders/model.py`

 * *Files identical despite different names*

### Comparing `dyapi-0.9.0/dyapi/interfaces/storages/base.py` & `dyapi-0.9.1/dyapi/interfaces/storages/base.py`

 * *Files identical despite different names*

### Comparing `dyapi-0.9.0/pyproject.toml` & `dyapi-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dyapi"
-version = "0.9.0"
+version = "0.9.1"
 description = ""
 authors = ["Artem Bogdanov <abogdaov@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "dyapi", from = "." }]
 
 
 [tool.poetry.dependencies]
```

### Comparing `dyapi-0.9.0/PKG-INFO` & `dyapi-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyapi
-Version: 0.9.0
+Version: 0.9.1
 Summary: 
 Author: Artem Bogdanov
 Author-email: abogdaov@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

