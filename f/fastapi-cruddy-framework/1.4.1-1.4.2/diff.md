# Comparing `tmp/fastapi_cruddy_framework-1.4.1.tar.gz` & `tmp/fastapi_cruddy_framework-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_cruddy_framework-1.4.1.tar", max compression
+gzip compressed data, was "fastapi_cruddy_framework-1.4.2.tar", max compression
```

## Comparing `fastapi_cruddy_framework-1.4.1.tar` & `fastapi_cruddy_framework-1.4.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1074 2023-03-03 18:31:12.339513 fastapi_cruddy_framework-1.4.1/LICENSE
--rw-r--r--   0        0        0    54883 2024-03-20 18:15:08.572389 fastapi_cruddy_framework-1.4.1/README.md
--rw-r--r--   0        0        0     2483 2024-03-20 18:15:08.576001 fastapi_cruddy_framework-1.4.1/fastapi_cruddy_framework/__init__.py
--rw-r--r--   0        0        0     6747 2024-01-06 16:48:05.591411 fastapi_cruddy_framework-1.4.1/fastapi_cruddy_framework/adapters.py
--rw-r--r--   0        0        0    41158 2024-03-20 18:15:08.576318 fastapi_cruddy_framework-1.4.1/fastapi_cruddy_framework/controller.py
--rw-r--r--   0        0        0    15489 2024-03-20 18:15:08.576677 fastapi_cruddy_framework-1.4.1/fastapi_cruddy_framework/graphql.py
--rw-r--r--   0        0        0       46 2023-03-03 18:31:12.343965 fastapi_cruddy_framework-1.4.1/fastapi_cruddy_framework/inflector.py
--rw-r--r--   0        0        0     3575 2024-01-06 19:00:34.485202 fastapi_cruddy_framework-1.4.1/fastapi_cruddy_framework/pubsub.py
--rw-r--r--   0        0        0    36195 2024-03-29 16:59:37.552395 fastapi_cruddy_framework-1.4.1/fastapi_cruddy_framework/repository.py
--rw-r--r--   0        0        0    28115 2024-03-15 14:58:27.880363 fastapi_cruddy_framework-1.4.1/fastapi_cruddy_framework/resource.py
--rw-r--r--   0        0        0     2375 2023-10-24 11:53:06.377545 fastapi_cruddy_framework-1.4.1/fastapi_cruddy_framework/router.py
--rw-r--r--   0        0        0     5591 2024-03-20 18:15:08.577043 fastapi_cruddy_framework-1.4.1/fastapi_cruddy_framework/schemas.py
--rw-r--r--   0        0        0    11050 2023-12-12 17:22:31.207802 fastapi_cruddy_framework-1.4.1/fastapi_cruddy_framework/test_helpers.py
--rw-r--r--   0        0        0     6287 2024-03-20 18:15:08.577324 fastapi_cruddy_framework-1.4.1/fastapi_cruddy_framework/util.py
--rw-r--r--   0        0        0    16184 2024-01-30 17:02:35.391956 fastapi_cruddy_framework-1.4.1/fastapi_cruddy_framework/websocket_manager.py
--rw-r--r--   0        0        0     2279 2024-03-29 17:01:18.255965 fastapi_cruddy_framework-1.4.1/pyproject.toml
--rw-r--r--   0        0        0    56460 1970-01-01 00:00:00.000000 fastapi_cruddy_framework-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-03-03 18:31:12.339513 fastapi_cruddy_framework-1.4.2/LICENSE
+-rw-r--r--   0        0        0    54838 2024-04-03 17:29:13.060260 fastapi_cruddy_framework-1.4.2/README.md
+-rw-r--r--   0        0        0     2483 2024-03-20 18:15:08.576001 fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/__init__.py
+-rw-r--r--   0        0        0     6747 2024-01-06 16:48:05.591411 fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/adapters.py
+-rw-r--r--   0        0        0    41158 2024-03-20 18:15:08.576318 fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/controller.py
+-rw-r--r--   0        0        0    15489 2024-03-20 18:15:08.576677 fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/graphql.py
+-rw-r--r--   0        0        0       46 2023-03-03 18:31:12.343965 fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/inflector.py
+-rw-r--r--   0        0        0     3575 2024-01-06 19:00:34.485202 fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/pubsub.py
+-rw-r--r--   0        0        0    36269 2024-03-29 20:29:49.898024 fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/repository.py
+-rw-r--r--   0        0        0    28384 2024-04-03 17:54:33.618921 fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/resource.py
+-rw-r--r--   0        0        0     2375 2023-10-24 11:53:06.377545 fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/router.py
+-rw-r--r--   0        0        0     5687 2024-04-03 17:41:13.269559 fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/schemas.py
+-rw-r--r--   0        0        0    11050 2023-12-12 17:22:31.207802 fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/test_helpers.py
+-rw-r--r--   0        0        0     6287 2024-03-20 18:15:08.577324 fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/util.py
+-rw-r--r--   0        0        0    16184 2024-01-30 17:02:35.391956 fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/websocket_manager.py
+-rw-r--r--   0        0        0     2252 2024-04-03 18:22:26.256931 fastapi_cruddy_framework-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0    56415 1970-01-01 00:00:00.000000 fastapi_cruddy_framework-1.4.2/PKG-INFO
```

### Comparing `fastapi_cruddy_framework-1.4.1/LICENSE` & `fastapi_cruddy_framework-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.1/README.md` & `fastapi_cruddy_framework-1.4.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -884,51 +884,51 @@
 def event_loop():
     loop = get_event_loop_policy().new_event_loop()
     yield loop
     loop.close()
 
 
 @fixture(scope="session", autouse=True)
-@mark.asyncio
+
 async def app():
     # Don't move this import!
     from your_app.main import app
 
     yield app
 
 
 @fixture(scope="session", autouse=True)
-@mark.asyncio
+
 async def client(app: FastAPI):
     # By using "with" the FastAPI app launch hook is run, connecting the application router
     async with TestClient(app, use_cookies=False) as client:
         while (await client.get("/health")).json() != True:
             await sleep(0.5)
         yield client
 
 
 @fixture(scope="session", autouse=True)
-@mark.asyncio
+
 async def unauthenticated_client(client: TestClient):
     blank_client = BrowserTestClient(client=client, cookies=None, headers=None)
     yield blank_client
 
 
 @fixture(scope="session", autouse=True)
-@mark.asyncio
+
 async def authenticated_client(client: TestClient):
     sessioned_client = BrowserTestClient(
         client=client, cookies=None, headers=FAKE_AUTH_HEADERS
     )
     await sessioned_client.get(f"/users/authorization{FAKE_AUTH_QP}")
     yield sessioned_client
 
 
 @fixture(scope="function")
-@mark.asyncio
+
 async def authenticated_websocket(authenticated_client: BrowserTestClient):
     async with authenticated_client.websocket_connect("/ws") as websocket:
         # For example: data = await websocket.receive_json()
         # Or await websocket.send_json(data)
         # If your server sends any kind of "welcome" messages, make
         # sure you purge them here BEFORE yielding the socket back
         # to whatever function needs to run tests
@@ -979,21 +979,21 @@
 from sqlalchemy.dialects.postgresql import JSONB, UUID as psqlUUID
 from fastapi_cruddy_framework import  CruddyModel, CruddyCreatedUpdatedMixin, UUID, uuid7
 
 
 class ExampleUpdate(CruddyModel):
     data: Any = Field(
         schema_extra={
-            "examples": [
-                {
+            "json_schema_extra": {
+                "example": {
                     "some": {
                         "key": "value"
                     }
                 }
-            ]
+            }
         }
     )
 
 
 class ExampleCreate(ExampleUpdate):
     pass
```

#### html2text {}

```diff
@@ -614,27 +614,26 @@
 get_event_loop_policy, sleep from pytest import fixture, mark from fastapi
 import FastAPI from fastapi_cruddy_framework import TestClient,
 BrowserTestClient logger = getLogger(__name__) FAKE_AUTH_TOKEN =
 "somefaketokenvalue" FAKE_AUTH_QP = f"?auth_token={FAKE_AUTH_TOKEN}"
 FAKE_AUTH_HEADERS = {"Authorization": f"Bearer {FAKE_AUTH_TOKEN}"} @fixture
 (scope="session", autouse=True) def event_loop(): loop = get_event_loop_policy
 ().new_event_loop() yield loop loop.close() @fixture(scope="session",
-autouse=True) @mark.asyncio async def app(): # Don't move this import! from
-your_app.main import app yield app @fixture(scope="session", autouse=True)
-@mark.asyncio async def client(app: FastAPI): # By using "with" the FastAPI app
-launch hook is run, connecting the application router async with TestClient
-(app, use_cookies=False) as client: while (await client.get("/health")).json()
-!= True: await sleep(0.5) yield client @fixture(scope="session", autouse=True)
-@mark.asyncio async def unauthenticated_client(client: TestClient):
-blank_client = BrowserTestClient(client=client, cookies=None, headers=None)
-yield blank_client @fixture(scope="session", autouse=True) @mark.asyncio async
-def authenticated_client(client: TestClient): sessioned_client =
-BrowserTestClient( client=client, cookies=None, headers=FAKE_AUTH_HEADERS )
-await sessioned_client.get(f"/users/authorization{FAKE_AUTH_QP}") yield
-sessioned_client @fixture(scope="function") @mark.asyncio async def
+autouse=True) async def app(): # Don't move this import! from your_app.main
+import app yield app @fixture(scope="session", autouse=True) async def client
+(app: FastAPI): # By using "with" the FastAPI app launch hook is run,
+connecting the application router async with TestClient(app, use_cookies=False)
+as client: while (await client.get("/health")).json() != True: await sleep(0.5)
+yield client @fixture(scope="session", autouse=True) async def
+unauthenticated_client(client: TestClient): blank_client = BrowserTestClient
+(client=client, cookies=None, headers=None) yield blank_client @fixture
+(scope="session", autouse=True) async def authenticated_client(client:
+TestClient): sessioned_client = BrowserTestClient( client=client, cookies=None,
+headers=FAKE_AUTH_HEADERS ) await sessioned_client.get(f"/users/authorization
+{FAKE_AUTH_QP}") yield sessioned_client @fixture(scope="function") async def
 authenticated_websocket(authenticated_client: BrowserTestClient): async with
 authenticated_client.websocket_connect("/ws") as websocket: # For example: data
 = await websocket.receive_json() # Or await websocket.send_json(data) # If your
 server sends any kind of "welcome" messages, make # sure you purge them here
 BEFORE yielding the socket back # to whatever function needs to run tests yield
 websocket ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
@@ -652,18 +651,18 @@
 sqlalchemy docs regarding functionality. To add a `tsvector` field to your
 cruddy data model, complete with proper indexing for performance, add the
 following to your table model class: ```python # models/example.py from typing
 import Any from sqlmodel import Field, cast, func, Text from sqlalchemy import
 Column, Index, literal_column from sqlalchemy.dialects.postgresql import JSONB,
 UUID as psqlUUID from fastapi_cruddy_framework import CruddyModel,
 CruddyCreatedUpdatedMixin, UUID, uuid7 class ExampleUpdate(CruddyModel): data:
-Any = Field( schema_extra={ "examples": [ { "some": { "key": "value" } } ] } )
-class ExampleCreate(ExampleUpdate): pass class Example
-(CruddyCreatedUpdatedMixin(), ExampleCreate, table=True): # type: ignore id:
-UUID = Field( sa_column=Column( psqlUUID(as_uuid=True), primary_key=True,
+Any = Field( schema_extra={ "json_schema_extra": { "example": { "some":
+{ "key": "value" } } } } ) class ExampleCreate(ExampleUpdate): pass class
+Example(CruddyCreatedUpdatedMixin(), ExampleCreate, table=True): # type: ignore
+id: UUID = Field( sa_column=Column( psqlUUID(as_uuid=True), primary_key=True,
 index=True, nullable=False, default=uuid7, ) ) data: Any = Field( default=None,
 sa_column=Column(JSONB, nullable=True, default=None), ) __table_args__ =
 ( Index("ix_Example_data_gin", "data", postgresql_using="gin"), Index
 ('ix_Example_data_tsvector', func.to_tsvector(literal_column("'english'"), cast
 (data.sa_column, Text)), postgresql_using="gin"), ) ``` A `Text` (or any other)
 cast: ```python where = {"a_json_column_name:Text": {"*icontains": "some
 substring"}} ``` The query stage's casting key name should match the format `:
```

### Comparing `fastapi_cruddy_framework-1.4.1/fastapi_cruddy_framework/__init__.py` & `fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.1/fastapi_cruddy_framework/adapters.py` & `fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/adapters.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.1/fastapi_cruddy_framework/controller.py` & `fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/controller.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.1/fastapi_cruddy_framework/graphql.py` & `fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/graphql.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.1/fastapi_cruddy_framework/pubsub.py` & `fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/pubsub.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.1/fastapi_cruddy_framework/repository.py` & `fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,15 +398,18 @@
         offset_page = query_conf["page"] - 1
         # pagination
         query = query.offset(offset_page * query_conf["limit"]).limit(
             query_conf["limit"]
         )
         # total record
 
-        async with self.adapter.getSession() as session1, self.adapter.getSession() as session2:
+        async with (
+            self.adapter.getSession() as session1,
+            self.adapter.getSession() as session2,
+        ):
             async with TaskGroup() as tg:
                 task1 = tg.create_task(session1.execute(count_query))
                 task2 = tg.create_task(session2.execute(query))
             count: Result = task1.result()
             records: Result = task2.result()
             total_record = count.scalar() or 0
             result = records.fetchall()
@@ -498,15 +501,18 @@
         offset_page = query_conf["page"] - 1
         # pagination
         query = query.offset(offset_page * query_conf["limit"]).limit(
             query_conf["limit"]
         )
         # total record
 
-        async with self.adapter.getSession() as session1, self.adapter.getSession() as session2:
+        async with (
+            self.adapter.getSession() as session1,
+            self.adapter.getSession() as session2,
+        ):
             async with TaskGroup() as tg:
                 task1 = tg.create_task(session1.execute(count_query))
                 task2 = tg.create_task(session2.execute(query))
             count: Result = task1.result()
             records: Result = task2.result()
             total_record = count.scalar() or 0
             result = records.fetchall()
```

### Comparing `fastapi_cruddy_framework-1.4.1/fastapi_cruddy_framework/resource.py` & `fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,19 +70,17 @@
     schemas: SchemaDict
     controller_lifecycles: dict[str, lifecycle_types]
 
     def __init__(
         self,
         # Only id_type, adapter, resource_create_model, resource_update_model, resource_model, and response_schema are required
         id_type: Type[int] | Type[UUID] | Type[str] = int,
-        adapter: BaseAdapter
-        | SqliteAdapter
-        | MysqlAdapter
-        | PostgresqlAdapter
-        | None = None,
+        adapter: (
+            BaseAdapter | SqliteAdapter | MysqlAdapter | PostgresqlAdapter | None
+        ) = None,
         resource_create_model: Type[CruddyModel] = ExampleCreate,
         resource_update_model: Type[CruddyModel] = ExampleUpdate,
         resource_model: Type[CruddyModel] = Example,
         response_schema: Type[CruddyModel] = ExampleView,
         # None of the following arguments are required. But they allow you to do powerful things!
         response_meta_schema: Type[CruddyModel] | Type[CruddyGenericModel] = MetaObject,
         # the adapter type only has two options because sqlite will take priority if its options are set
@@ -266,17 +264,19 @@
         if self.repository.id_type == str:
             example_id = str(example_id)
         possible_id = response_schema.model_fields.get("id", None)
         if possible_id is not None and issubclass(
             self.repository.id_type, possible_id.annotation  # type: ignore
         ):
             example_dict = {
-                "example": int(str(example_id))
-                if self.repository.id_type == int
-                else str(example_id)
+                "example": (
+                    int(str(example_id))
+                    if self.repository.id_type == int
+                    else str(example_id)
+                )
             }
             if possible_id.json_schema_extra is not None:
                 possible_id_example = possible_id.json_schema_extra.get("example", None)
                 if possible_id_example is not None:
                     example_id = possible_id_example
                 possible_id.json_schema_extra.update(example_dict)
             else:
@@ -293,17 +293,19 @@
             self._protected_relationships + self._protected_update_relationships
         )
         for k, v in self._relations.items():
             link_object[k] = (
                 str,
                 Field(
                     schema_extra={
-                        "examples": [
-                            self._single_link(id=str(example_id), relationship=k)
-                        ]
+                        "json_schema_extra": {
+                            "example": self._single_link(
+                                id=str(example_id), relationship=k
+                            )
+                        }
                     }
                 ),
             )
             rel_def = self._derive_shadow_relationship(
                 v.orm_relationship.direction, v.foreign_resource._id_type
             )
             if k not in create_protected_relationships:
@@ -311,17 +313,19 @@
             if k not in update_protected_relationships:
                 false_update_attrs[k] = rel_def
         for item in self._artificial_relationship_paths:
             link_object[item] = (
                 str,
                 Field(
                     schema_extra={
-                        "examples": [
-                            self._single_link(id=str(example_id), relationship=item)
-                        ]
+                        "json_schema_extra": {
+                            "example": self._single_link(
+                                id=str(example_id), relationship=item
+                            )
+                        }
                     }
                 ),
             )
         link_object["__base__"] = CruddyModel
 
         LinkModel = create_model(f"{resource_model_name}Links", **link_object)
         # End shared link model
@@ -353,25 +357,25 @@
             },  # type: ignore
         )
         # End update record envelope schema
 
         # Single record schema with embedded links
         SingleSchemaLinked = create_model(
             f"{resource_response_name}Linked",
-            links=(LinkModel | None, None),
+            links=(LinkModel, None),
             __base__=response_schema,
         )
         # End single record schema with embedded links
 
         # Single record return payload (for get/{id})
         SingleSchemaEnvelope = create_model(
             f"{resource_response_name}Envelope",
             __base__=CruddyGenericModel,
             **{
-                resource_model_name: (SingleSchemaLinked | None, None),
+                resource_model_name: (SingleSchemaLinked, ...),
                 "meta": (dict[str, Any] | None, None),
             },  # type: ignore
         )
 
         handle_data_or_none = self._create_schema_arg_handler(
             single_schema_linked=SingleSchemaLinked,
             resource_model_name=resource_model_name,
@@ -389,37 +393,39 @@
         # End single record return payload
 
         # Many records return payload (for get/ and queries with "where")
         ManySchemaEnvelope = create_model(
             f"{resource_response_name}List",
             __base__=CruddyGenericModel,
             **{
-                resource_model_plural: (list[SingleSchemaLinked] | None, None),
+                resource_model_plural: (list[SingleSchemaLinked], ...),
             },  # type: ignore
             meta=(response_meta_schema, ...),
         )
 
         old_many_init = ManySchemaEnvelope.__init__
 
         def new_many_init(self, *args, **kwargs):
             old_many_init(
                 self,
                 *args,
                 **{
-                    resource_model_plural: [
-                        SingleSchemaLinked(
-                            **x._mapping,
-                            links=local_resource._link_builder(  # type: ignore
-                                id=x._mapping[local_resource.repository.primary_key]
-                            ),
-                        )
-                        for x in kwargs["data"]
-                    ]
-                    if resource_model_plural not in kwargs
-                    else kwargs[resource_model_plural],
+                    resource_model_plural: (
+                        [
+                            SingleSchemaLinked(
+                                **x._mapping,
+                                links=local_resource._link_builder(  # type: ignore
+                                    id=x._mapping[local_resource.repository.primary_key]
+                                ),
+                            )
+                            for x in kwargs["data"]
+                        ]
+                        if resource_model_plural not in kwargs
+                        else kwargs[resource_model_plural]
+                    ),
                     "data": kwargs["data"] if "data" in kwargs else [],
                     "meta": kwargs["meta"],
                 },
             )
 
         ManySchemaEnvelope.__init__ = new_many_init
         # End many records return payload
```

### Comparing `fastapi_cruddy_framework-1.4.1/fastapi_cruddy_framework/router.py` & `fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/router.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.1/fastapi_cruddy_framework/schemas.py` & `fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/schemas.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,15 +86,17 @@
     data: Sequence[Row]
 
     class Config:
         arbitrary_types_allowed = True
 
 
 class SocketMessage(CruddyGenericModel):
-    route: str = BROADCAST_EVENT  # How to route this between the pubsub/connection_manager module (default to a broadcast)
+    route: str = (
+        BROADCAST_EVENT  # How to route this between the pubsub/connection_manager module (default to a broadcast)
+    )
     target: str | None = None  # A target for the message (if route is "room" or "user")
     type: str | None = None  # Message type
     sender: str | None = None  # Sender (if any)
     data: dict | None = None  # Message payload
 
 
 class SocketRoomConfiguration(CruddyGenericModel):
@@ -109,18 +111,18 @@
 class CruddyModel(SQLModel):
     @declared_attr.directive
     def __tablename__(cls) -> str:
         return cls.__name__
 
 
 class MetaObject(CruddyModel):
-    page: int = Field(schema_extra={"examples": [1]})
-    limit: int = Field(schema_extra={"examples": [10]})
-    pages: int = Field(schema_extra={"examples": [1]})
-    records: int = Field(schema_extra={"examples": [1]})
+    page: int = Field(schema_extra={"json_schema_extra": {"example": 1}})
+    limit: int = Field(schema_extra={"json_schema_extra": {"example": 10}})
+    pages: int = Field(schema_extra={"json_schema_extra": {"example": 1}})
+    records: int = Field(schema_extra={"json_schema_extra": {"example": 1}})
 
 
 class PageResponse(CruddyGenericModel):
     # The response for a pagination query.
     meta: Type[CruddyModel] | Type[CruddyGenericModel]
     data: list[Any]
```

### Comparing `fastapi_cruddy_framework-1.4.1/fastapi_cruddy_framework/test_helpers.py` & `fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/test_helpers.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.1/fastapi_cruddy_framework/util.py` & `fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/util.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.1/fastapi_cruddy_framework/websocket_manager.py` & `fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.1/pyproject.toml` & `fastapi_cruddy_framework-1.4.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-cruddy-framework"
-version = "1.4.1"
+version = "1.4.2"
 description = "A holistic CRUD/MVC framework for FastAPI, with endpoint policies and relationships"
 authors = ["mdconaway <mdconaway@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "fastapi_cruddy_framework"}]
 homepage = "https://github.com/mdconaway/fastapi-cruddy-framework"
 repository = "https://github.com/mdconaway/fastapi-cruddy-framework"
 keywords = ["fastapi", "crud", "mvc", "orm", "ember", "sails", "json"]
@@ -42,30 +42,29 @@
 SQLAlchemy = { extras = ["asyncio"], version = ">=2.0.0" }
 sqlmodel = "^0.0.16"
 inflect = "^7.0.0"
 async-asgi-testclient = "^1.4.11"
 validator-collection = "^1.5.0"
 uuid7 = "^0.1.0"
 redis = ">=5.0.1,<6.0.0"
-fakeredis = ">=2.20.1"
+fakeredis = ">=2.21.3"
 async-timeout = ">=4.0.0,<5.0.0"
 pymitter = ">=0.5.0"
-strawberry-graphql = {extras = ["fastapi"], version = ">=0.220.0"}
+strawberry-graphql = {extras = ["fastapi"], version = ">=0.223.0"}
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.12.0"
+black = "^24.3.0"
 uvicorn = "^0.24.0"
 starlette-session = "^0.4.3"
-aiosqlite = "^0.19.0"
+aiosqlite = "^0.20.0"
 bcrypt = "^4.1.2"
-pytest = "^7.4.3"
-pylint = "^3.0.3"
-pytest-asyncio = "0.21.1"
-pytest-dependency = "^0.5.1"
-coverage = "^7.3.3"
+pylint = "^3.1.0"
+pytest = "^8.1.1"
+pytest-dependency = "^0.6.0"
+coverage = "^7.4.4"
 
 [tool.poetry.scripts]
 start_sqlite = "examples.fastapi_cruddy_sqlite.bootloader:start"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fastapi_cruddy_framework-1.4.1/PKG-INFO` & `fastapi_cruddy_framework-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-cruddy-framework
-Version: 1.4.1
+Version: 1.4.2
 Summary: A holistic CRUD/MVC framework for FastAPI, with endpoint policies and relationships
 Home-page: https://github.com/mdconaway/fastapi-cruddy-framework
 Keywords: fastapi,crud,mvc,orm,ember,sails,json
 Author: mdconaway
 Author-email: mdconaway@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -17,21 +17,21 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: SQLAlchemy-Utils (>=0.41.1,<0.42.0)
 Requires-Dist: SQLAlchemy[asyncio] (>=2.0.0)
 Requires-Dist: async-asgi-testclient (>=1.4.11,<2.0.0)
 Requires-Dist: async-timeout (>=4.0.0,<5.0.0)
-Requires-Dist: fakeredis (>=2.20.1)
+Requires-Dist: fakeredis (>=2.21.3)
 Requires-Dist: fastapi[all] (>=0.100.0)
 Requires-Dist: inflect (>=7.0.0,<8.0.0)
 Requires-Dist: pymitter (>=0.5.0)
 Requires-Dist: redis (>=5.0.1,<6.0.0)
 Requires-Dist: sqlmodel (>=0.0.16,<0.0.17)
-Requires-Dist: strawberry-graphql[fastapi] (>=0.220.0)
+Requires-Dist: strawberry-graphql[fastapi] (>=0.223.0)
 Requires-Dist: uuid7 (>=0.1.0,<0.2.0)
 Requires-Dist: validator-collection (>=1.5.0,<2.0.0)
 Project-URL: Repository, https://github.com/mdconaway/fastapi-cruddy-framework
 Description-Content-Type: text/markdown
 
 <a name="readme-top"></a>
 
@@ -919,51 +919,51 @@
 def event_loop():
     loop = get_event_loop_policy().new_event_loop()
     yield loop
     loop.close()
 
 
 @fixture(scope="session", autouse=True)
-@mark.asyncio
+
 async def app():
     # Don't move this import!
     from your_app.main import app
 
     yield app
 
 
 @fixture(scope="session", autouse=True)
-@mark.asyncio
+
 async def client(app: FastAPI):
     # By using "with" the FastAPI app launch hook is run, connecting the application router
     async with TestClient(app, use_cookies=False) as client:
         while (await client.get("/health")).json() != True:
             await sleep(0.5)
         yield client
 
 
 @fixture(scope="session", autouse=True)
-@mark.asyncio
+
 async def unauthenticated_client(client: TestClient):
     blank_client = BrowserTestClient(client=client, cookies=None, headers=None)
     yield blank_client
 
 
 @fixture(scope="session", autouse=True)
-@mark.asyncio
+
 async def authenticated_client(client: TestClient):
     sessioned_client = BrowserTestClient(
         client=client, cookies=None, headers=FAKE_AUTH_HEADERS
     )
     await sessioned_client.get(f"/users/authorization{FAKE_AUTH_QP}")
     yield sessioned_client
 
 
 @fixture(scope="function")
-@mark.asyncio
+
 async def authenticated_websocket(authenticated_client: BrowserTestClient):
     async with authenticated_client.websocket_connect("/ws") as websocket:
         # For example: data = await websocket.receive_json()
         # Or await websocket.send_json(data)
         # If your server sends any kind of "welcome" messages, make
         # sure you purge them here BEFORE yielding the socket back
         # to whatever function needs to run tests
@@ -1014,21 +1014,21 @@
 from sqlalchemy.dialects.postgresql import JSONB, UUID as psqlUUID
 from fastapi_cruddy_framework import  CruddyModel, CruddyCreatedUpdatedMixin, UUID, uuid7
 
 
 class ExampleUpdate(CruddyModel):
     data: Any = Field(
         schema_extra={
-            "examples": [
-                {
+            "json_schema_extra": {
+                "example": {
                     "some": {
                         "key": "value"
                     }
                 }
-            ]
+            }
         }
     )
 
 
 class ExampleCreate(ExampleUpdate):
     pass
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: fastapi-cruddy-framework Version: 1.4.1 Summary: A
+Metadata-Version: 2.1 Name: fastapi-cruddy-framework Version: 1.4.2 Summary: A
 holistic CRUD/MVC framework for FastAPI, with endpoint policies and
 relationships Home-page: https://github.com/mdconaway/fastapi-cruddy-framework
 Keywords: fastapi,crud,mvc,orm,ember,sails,json Author: mdconaway Author-email:
 mdconaway@users.noreply.github.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Web Environment
 Classifier: Framework :: FastAPI Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development Classifier: Topic :: Software
 Development :: Libraries :: Application Frameworks Classifier: Topic ::
 Software Development :: Libraries :: Python Modules Requires-Dist: SQLAlchemy-
 Utils (>=0.41.1,<0.42.0) Requires-Dist: SQLAlchemy[asyncio] (>=2.0.0) Requires-
 Dist: async-asgi-testclient (>=1.4.11,<2.0.0) Requires-Dist: async-timeout
-(>=4.0.0,<5.0.0) Requires-Dist: fakeredis (>=2.20.1) Requires-Dist: fastapi
+(>=4.0.0,<5.0.0) Requires-Dist: fakeredis (>=2.21.3) Requires-Dist: fastapi
 [all] (>=0.100.0) Requires-Dist: inflect (>=7.0.0,<8.0.0) Requires-Dist:
 pymitter (>=0.5.0) Requires-Dist: redis (>=5.0.1,<6.0.0) Requires-Dist:
 sqlmodel (>=0.0.16,<0.0.17) Requires-Dist: strawberry-graphql[fastapi]
-(>=0.220.0) Requires-Dist: uuid7 (>=0.1.0,<0.2.0) Requires-Dist: validator-
+(>=0.223.0) Requires-Dist: uuid7 (>=0.1.0,<0.2.0) Requires-Dist: validator-
 collection (>=1.5.0,<2.0.0) Project-URL: Repository, https://github.com/
 mdconaway/fastapi-cruddy-framework Description-Content-Type: text/markdown
                     ********** FFaassttAAPPII -- CCrruuddddyy FFrraammeewwoorrkk **********
                                     _[_L_o_g_o_]
 ## About Cruddy Framework [![Product Name Screen Shot][product-screenshot]]
 (https://github.com/mdconaway/fastapi-cruddy-framework) CCrruuddddyy FFrraammeewwoorrkk nnooww
 ssuuppppoorrttss GGrraapphhQQLL!! FFoorr eexxaammpplleess,, sseeee tthhee [[eexxaammppllee sseerrvveerr]]((eexxaammpplleess//
@@ -635,27 +635,26 @@
 get_event_loop_policy, sleep from pytest import fixture, mark from fastapi
 import FastAPI from fastapi_cruddy_framework import TestClient,
 BrowserTestClient logger = getLogger(__name__) FAKE_AUTH_TOKEN =
 "somefaketokenvalue" FAKE_AUTH_QP = f"?auth_token={FAKE_AUTH_TOKEN}"
 FAKE_AUTH_HEADERS = {"Authorization": f"Bearer {FAKE_AUTH_TOKEN}"} @fixture
 (scope="session", autouse=True) def event_loop(): loop = get_event_loop_policy
 ().new_event_loop() yield loop loop.close() @fixture(scope="session",
-autouse=True) @mark.asyncio async def app(): # Don't move this import! from
-your_app.main import app yield app @fixture(scope="session", autouse=True)
-@mark.asyncio async def client(app: FastAPI): # By using "with" the FastAPI app
-launch hook is run, connecting the application router async with TestClient
-(app, use_cookies=False) as client: while (await client.get("/health")).json()
-!= True: await sleep(0.5) yield client @fixture(scope="session", autouse=True)
-@mark.asyncio async def unauthenticated_client(client: TestClient):
-blank_client = BrowserTestClient(client=client, cookies=None, headers=None)
-yield blank_client @fixture(scope="session", autouse=True) @mark.asyncio async
-def authenticated_client(client: TestClient): sessioned_client =
-BrowserTestClient( client=client, cookies=None, headers=FAKE_AUTH_HEADERS )
-await sessioned_client.get(f"/users/authorization{FAKE_AUTH_QP}") yield
-sessioned_client @fixture(scope="function") @mark.asyncio async def
+autouse=True) async def app(): # Don't move this import! from your_app.main
+import app yield app @fixture(scope="session", autouse=True) async def client
+(app: FastAPI): # By using "with" the FastAPI app launch hook is run,
+connecting the application router async with TestClient(app, use_cookies=False)
+as client: while (await client.get("/health")).json() != True: await sleep(0.5)
+yield client @fixture(scope="session", autouse=True) async def
+unauthenticated_client(client: TestClient): blank_client = BrowserTestClient
+(client=client, cookies=None, headers=None) yield blank_client @fixture
+(scope="session", autouse=True) async def authenticated_client(client:
+TestClient): sessioned_client = BrowserTestClient( client=client, cookies=None,
+headers=FAKE_AUTH_HEADERS ) await sessioned_client.get(f"/users/authorization
+{FAKE_AUTH_QP}") yield sessioned_client @fixture(scope="function") async def
 authenticated_websocket(authenticated_client: BrowserTestClient): async with
 authenticated_client.websocket_connect("/ws") as websocket: # For example: data
 = await websocket.receive_json() # Or await websocket.send_json(data) # If your
 server sends any kind of "welcome" messages, make # sure you purge them here
 BEFORE yielding the socket back # to whatever function needs to run tests yield
 websocket ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
@@ -673,18 +672,18 @@
 sqlalchemy docs regarding functionality. To add a `tsvector` field to your
 cruddy data model, complete with proper indexing for performance, add the
 following to your table model class: ```python # models/example.py from typing
 import Any from sqlmodel import Field, cast, func, Text from sqlalchemy import
 Column, Index, literal_column from sqlalchemy.dialects.postgresql import JSONB,
 UUID as psqlUUID from fastapi_cruddy_framework import CruddyModel,
 CruddyCreatedUpdatedMixin, UUID, uuid7 class ExampleUpdate(CruddyModel): data:
-Any = Field( schema_extra={ "examples": [ { "some": { "key": "value" } } ] } )
-class ExampleCreate(ExampleUpdate): pass class Example
-(CruddyCreatedUpdatedMixin(), ExampleCreate, table=True): # type: ignore id:
-UUID = Field( sa_column=Column( psqlUUID(as_uuid=True), primary_key=True,
+Any = Field( schema_extra={ "json_schema_extra": { "example": { "some":
+{ "key": "value" } } } } ) class ExampleCreate(ExampleUpdate): pass class
+Example(CruddyCreatedUpdatedMixin(), ExampleCreate, table=True): # type: ignore
+id: UUID = Field( sa_column=Column( psqlUUID(as_uuid=True), primary_key=True,
 index=True, nullable=False, default=uuid7, ) ) data: Any = Field( default=None,
 sa_column=Column(JSONB, nullable=True, default=None), ) __table_args__ =
 ( Index("ix_Example_data_gin", "data", postgresql_using="gin"), Index
 ('ix_Example_data_tsvector', func.to_tsvector(literal_column("'english'"), cast
 (data.sa_column, Text)), postgresql_using="gin"), ) ``` A `Text` (or any other)
 cast: ```python where = {"a_json_column_name:Text": {"*icontains": "some
 substring"}} ``` The query stage's casting key name should match the format `:
```

