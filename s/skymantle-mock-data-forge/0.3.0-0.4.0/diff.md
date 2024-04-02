# Comparing `tmp/skymantle_mock_data_forge-0.3.0.tar.gz` & `tmp/skymantle_mock_data_forge-0.4.0.tar.gz`

## Comparing `skymantle_mock_data_forge-0.3.0.tar` & `skymantle_mock_data_forge-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.3.0/src/skymantle_mock_data_forge/__init__.py
--rw-r--r--   0        0        0     6848 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.3.0/src/skymantle_mock_data_forge/base_forge.py
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.3.0/src/skymantle_mock_data_forge/dynamodb_forge.py
--rw-r--r--   0        0        0     5044 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.3.0/src/skymantle_mock_data_forge/forge_factory.py
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.3.0/src/skymantle_mock_data_forge/models.py
--rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.3.0/src/skymantle_mock_data_forge/s3_forge.py
--rw-r--r--   0        0        0     9804 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.3.0/tests/test_dynamodb_forge.py
--rw-r--r--   0        0        0    11821 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.3.0/tests/test_forge_factory.py
--rw-r--r--   0        0        0     9309 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.3.0/tests/test_overrides.py
--rw-r--r--   0        0        0    18845 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.3.0/tests/test_s3_forge.py
--rw-r--r--   0        0        0    28203 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.3.0/tests/data/amazon_webservices_logo.png
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.3.0/tests/data/forge_config.json
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.3.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.3.0/LICENSE
--rw-r--r--   0        0        0    16499 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.3.0/README.md
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    30247 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.4.0/src/skymantle_mock_data_forge/__init__.py
+-rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.4.0/src/skymantle_mock_data_forge/base_forge.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.4.0/src/skymantle_mock_data_forge/dynamodb_forge.py
+-rw-r--r--   0        0        0     6229 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.4.0/src/skymantle_mock_data_forge/forge_factory.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.4.0/src/skymantle_mock_data_forge/models.py
+-rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.4.0/src/skymantle_mock_data_forge/s3_forge.py
+-rw-r--r--   0        0        0    10940 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.4.0/tests/test_dynamodb_forge.py
+-rw-r--r--   0        0        0    12915 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.4.0/tests/test_forge_factory.py
+-rw-r--r--   0        0        0     9327 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.4.0/tests/test_overrides.py
+-rw-r--r--   0        0        0    20128 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.4.0/tests/test_s3_forge.py
+-rw-r--r--   0        0        0    28203 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.4.0/tests/data/amazon_web_services_logo.png
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.4.0/tests/data/forge_config.json
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.4.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.4.0/LICENSE
+-rw-r--r--   0        0        0    16766 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.4.0/README.md
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    30514 2020-02-02 00:00:00.000000 skymantle_mock_data_forge-0.4.0/PKG-INFO
```

### Comparing `skymantle_mock_data_forge-0.3.0/src/skymantle_mock_data_forge/base_forge.py` & `skymantle_mock_data_forge-0.4.0/src/skymantle_mock_data_forge/base_forge.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,43 +5,43 @@
 
 from boto3 import Session
 from skymantle_boto_buddy import cloudformation, ssm
 
 from skymantle_mock_data_forge.models import (
     DataForgeConfigOverride,
     ForgeQuery,
-    OverideType,
+    OverrideType,
 )
 
 
 class BaseForge:
     _operators: Final[dict[str, Callable]] = {
         "StringEquals": lambda value, condition_value: value == condition_value,
         "StringLike": lambda value, condition_value: condition_value in value,
     }
 
     def __init__(
         self, forge_id: str, overrides: list[DataForgeConfigOverride] | None = None, session: Session = None
     ) -> None:
-        self.forge_id: str = forge_id
-        self.aws_session = session
-        self.config_overrides = overrides
+        self._forge_id: str = forge_id
+        self._aws_session = session
+        self._overrides = overrides
 
     def _get_destination_identifier(self, resource_config):
         if resource_config.get("name"):
             value = resource_config["name"]
 
         elif resource_config.get("ssm"):
-            value = ssm.get_parameter(resource_config["ssm"], session=self.aws_session)
+            value = ssm.get_parameter(resource_config["ssm"], session=self._aws_session)
 
         else:
             stack_name = resource_config["stack"]["name"]
             output = resource_config["stack"]["output"]
 
-            outputs = cloudformation.get_stack_outputs(stack_name, session=self.aws_session)
+            outputs = cloudformation.get_stack_outputs(stack_name, session=self._aws_session)
             output_value = outputs.get(output)
 
             if output_value:
                 value = output_value
             else:
                 raise Exception(f"Unable to find a resource for stack: {stack_name} and output: {output}")
 
@@ -88,26 +88,24 @@
                 raise Exception("Tag values can only be strings or list of strings.")
 
         return matches
 
     def _override_data(self, items: list[dict]) -> list[dict]:
         data: list[dict] = [copy.deepcopy(item) for item in items]
 
-        if not self.config_overrides:
+        if not self._overrides:
             return data
 
-        if not (
-            isinstance(self.config_overrides, list) and all(isinstance(item, dict) for item in self.config_overrides)
-        ):
+        if not (isinstance(self._overrides, list) and all(isinstance(item, dict) for item in self._overrides)):
             raise Exception("Overrides must be a list[DataForgeConfigOverride]")
 
         if not (isinstance(data, list) and all(isinstance(item, dict) for item in data)):
             raise Exception("The provided data must be a list of dictionaries")
 
-        for config_override in self.config_overrides:
+        for config_override in self._overrides:
             key_paths = config_override.get("key_paths")
 
             if isinstance(key_paths, str):
                 key_paths = [key_paths]
 
             elif not (isinstance(key_paths, list) and all(isinstance(item, str) for item in key_paths)):
                 raise Exception("key_paths must be a str or list[str]")
@@ -117,15 +115,15 @@
 
             for key_path in key_paths:
                 for item in data:
                     self._update_item(item, key_path, override_type, override)
 
         return data
 
-    def _update_item(self, item: dict, key_path: str, override_type: OverideType, override: any):
+    def _update_item(self, item: dict, key_path: str, override_type: OverrideType, override: any):
         try:
             result = self._travel_key_path(item, key_path, override_type, override)
 
             if result is None:
                 return
 
             key = result[0]
@@ -139,32 +137,32 @@
 
             if suppress_key_path_errors in ["0", "false", "no", "off"]:
                 raise e
 
             return
 
         match override_type:
-            case OverideType.REPLACE_VALUE:
+            case OverrideType.REPLACE_VALUE:
                 item_to_update[key] = override
 
-            case OverideType.FORMAT_VALUE:
+            case OverrideType.FORMAT_VALUE:
                 value = item_to_update[key]
 
                 if not isinstance(value, str):
                     raise Exception(f"The value for key:{key} must be str for FORMAT_VALUE.")
 
                 item_to_update[key] = value.format(*override)
 
-            case OverideType.CALL_FUNCTION:
+            case OverrideType.CALL_FUNCTION:
                 item_to_update[key] = override(key, item_to_update[key], copy.deepcopy(item))
 
             case _:
                 raise Exception(f"Unsupported override type - {override_type}")
 
-    def _travel_key_path(self, item: dict, key_path: str, override_type: OverideType, override: any) -> dict:
+    def _travel_key_path(self, item: dict, key_path: str, override_type: OverrideType, override: any) -> dict:
         keys = key_path.split(".")
 
         prefix = ""
         temp_item = item
 
         for key in keys[:-1]:
             prefix += f"{key}."
```

### Comparing `skymantle_mock_data_forge-0.3.0/src/skymantle_mock_data_forge/dynamodb_forge.py` & `skymantle_mock_data_forge-0.4.0/src/skymantle_mock_data_forge/dynamodb_forge.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,42 +18,47 @@
         forge_id: str,
         config: DynamoDbForgeConfig,
         session: Session = None,
         overrides: list[DataForgeConfigOverride] | None = None,
     ) -> None:
         super().__init__(forge_id, overrides, session)
 
-        resource_config = config["table"]
-        self.table_name: str = self._get_destination_identifier(resource_config)
-
-        self.primary_key_names: list[str] = config["primary_key_names"].copy()
-        self.items: list[DynamoDbItemConfig] = self._override_data(config["items"])
+        self._config = config
+        self._primary_key_names: list[str] = config["primary_key_names"].copy()
+        self._items: list[DynamoDbItemConfig] = self._override_data(config["items"])
 
         # Populate the keys list with the keys from all the items.
         # TODO: Validate key conforms to primary_key_names
-        self.keys: list[dict[str, str]] = []
-        for item in self.items:
+        self._keys: list[dict[str, str]] = []
+        for item in self._items:
             key = {}
-            for primary_key_name in self.primary_key_names:
+            for primary_key_name in self._primary_key_names:
                 key[primary_key_name] = item["data"][primary_key_name]
 
-            self.keys.append(key)
+            self._keys.append(key)
+
+    def _get_table_name(self):
+        resource_config = self._config["table"]
+        return self._get_destination_identifier(resource_config)
+
+    def get_data(self, *, query: ForgeQuery, return_source: bool):
+        data = [copy.deepcopy(item) for item in self._items]
 
-    def get_data(self, query: ForgeQuery = None):
-        data = [copy.deepcopy(item) for item in self.items]
+        if query is not None:
+            data = self._get_data_query(query, data)
 
-        if query is None:
-            return data
+        if not return_source:
+            data = [item["data"] for item in data]
 
-        return self._get_data_query(query, data)
+        return data
 
     def add_key(self, key: dict[str, str]) -> None:
         # TODO: Validate key conforms to primary_key_names
-        self.keys.append(key)
+        self._keys.append(key)
 
     def load_data(self) -> None:
-        for item in self.items:
-            dynamodb.put_item_simplified(self.table_name, item["data"], session=self.aws_session)
+        for item in self._items:
+            dynamodb.put_item_simplified(self._get_table_name(), item["data"], session=self._aws_session)
 
     def cleanup_data(self) -> None:
-        for key in self.keys:
-            dynamodb.delete_item(self.table_name, key, session=self.aws_session)
+        for key in self._keys:
+            dynamodb.delete_item(self._get_table_name(), key, session=self._aws_session)
```

### Comparing `skymantle_mock_data_forge-0.3.0/src/skymantle_mock_data_forge/forge_factory.py` & `skymantle_mock_data_forge-0.4.0/src/skymantle_mock_data_forge/forge_factory.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+from typing import Any
 
 from boto3 import Session
 
 from skymantle_mock_data_forge.dynamodb_forge import DynamoDbForge
 from skymantle_mock_data_forge.models import (
     DataForgeConfig,
     DataForgeConfigOverride,
@@ -67,42 +68,67 @@
         data_manager = self.data_managers.get(forge_id)
 
         if data_manager:
             data_manager.add_key(key)
         else:
             raise Exception(f"{forge_id} not initialized ({','.join(self.data_managers.keys())}).")
 
-    def get_data(self, forge_id: str | None = None, query: ForgeQuery = None) -> list[dict]:
+    def get_data_first_item(
+        self, forge_id: str | None = None, query: ForgeQuery = None, *, default: Any = None, return_source: bool = False
+    ) -> list[dict]:
+        """Gets the first item from the data loaded into forge destination.
+        Does not return data created outside of the forge.
+
+        Args:
+            forge_id (str | None, optional): The forge to add the key too. Defaults to None.
+            query (ForgeQuery, optional): Query forge data tags to limit returned data. Defaults to None.
+            default (Any, optional): Default value if no items returned. Defaults to None.
+            return_source (bool, optional): Include all data from the config file. Defaults to False.
+
+        Raises:
+            Exception: Provided forge ID is not valid.
+
+        Returns:
+            dict: The first or default item
+        """
+        data = self.get_data(forge_id, query, return_source=return_source)
+
+        return next(iter(data), default)
+
+    def get_data(
+        self, forge_id: str | None = None, query: ForgeQuery = None, *, return_source: bool = False
+    ) -> list[dict]:
         """Gets a copy of the data loaded into forge destination. Does not return data created outside of the forge.
 
         Args:
             forge_id (str | None, optional): When provided will only get data for the specific forge. Defaults to None.
             query (ForgeQuery, optional): Query forge data tags to limit returned data. Defaults to None.
+            return_source (bool, optional): Include all data from the config file. Defaults to False.
 
         Raises:
             Exception: Provided forge ID is not valid.
 
         Returns:
             list[dict]: A list of stored data
         """
         forge_ids = self._get_forge_ids(forge_id)
 
         data = []
         for forge_id in forge_ids:
             data_manager = self.data_managers.get(forge_id)
 
             if data_manager:
-                data.extend(data_manager.get_data(query))
+                data.extend(data_manager.get_data(query=query, return_source=return_source))
             else:
                 raise Exception(f"{forge_id} not initialized ({','.join(self.data_managers.keys())}).")
 
         return data
 
     def load_data(self, forge_id: str | None = None) -> None:
-        """Loads all data into forge detinations
+        """Loads all data into forge destinations
 
         Args:
             forge_id (str | None, optional): When provided will only load data for the specific forge. Defaults to None.
 
         Raises:
             Exception: Provided forge ID is not valid.
         """
@@ -117,15 +143,15 @@
             else:
                 raise Exception(f"{forge_id} not initialized ({','.join(self.data_managers.keys())}).")
 
     def cleanup_data(self, forge_id: str | None = None) -> None:
         """Deletes all data from forge destinations
 
         Args:
-            forge_id (str | None, optional): When provided will only cleaup the specific forge. Defaults to None.
+            forge_id (str | None, optional): When provided will only cleanup the specific forge. Defaults to None.
 
         Raises:
             Exception: Provided forge ID is not valid.
         """
         forge_ids = self._get_forge_ids(forge_id)
 
         for forge_id in forge_ids:
```

### Comparing `skymantle_mock_data_forge-0.3.0/src/skymantle_mock_data_forge/models.py` & `skymantle_mock_data_forge-0.4.0/src/skymantle_mock_data_forge/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import TypedDict
+from typing import Any, TypedDict
 
 
 class ForgeQuery(TypedDict):
     StringEquals: dict[str, str | list[str]]
     StringLike: dict[str, str | list[str]]
 
 
@@ -50,18 +50,18 @@
 
 class DataForgeConfig(TypedDict):
     forge_id: str
     dynamodb: DynamoDbForgeConfig
     s3: S3ForgeConfig
 
 
-class OverideType(Enum):
+class OverrideType(Enum):
     REPLACE_VALUE = 0
     FORMAT_VALUE = 1
     CALL_FUNCTION = 2
 
 
 class DataForgeConfigOverride(TypedDict):
     forge_id: str | None
     key_paths: str | list[str]
-    override_type: OverideType
-    override: any
+    override_type: OverrideType
+    override: Any
```

### Comparing `skymantle_mock_data_forge-0.3.0/src/skymantle_mock_data_forge/s3_forge.py` & `skymantle_mock_data_forge-0.4.0/src/skymantle_mock_data_forge/s3_forge.py`

 * *Files 21% similar despite different names*

```diff
@@ -22,30 +22,35 @@
         forge_id: str,
         config: S3ForgeConfig,
         session: Session = None,
         overrides: list[DataForgeConfigOverride] | None = None,
     ) -> None:
         super().__init__(forge_id, overrides, session)
 
-        resource_config = config["bucket"]
-        self.bucket_name: str = self._get_destination_identifier(resource_config)
+        self._config = config
+        self._s3_objects: list[S3ObjectConfig] = self._override_data(config["s3_objects"])
+        self._keys: list[str] = [s3_object["key"] for s3_object in self._s3_objects]
 
-        self.s3_objects: list[S3ObjectConfig] = self._override_data(config["s3_objects"])
-        self.keys: list[str] = [s3_object["key"] for s3_object in self.s3_objects]
+    def _get_bucket_name(self):
+        resource_config = self._config["bucket"]
+        return self._get_destination_identifier(resource_config)
 
-    def get_data(self, query: ForgeQuery = None):
-        data = [copy.deepcopy(s3_object) for s3_object in self.s3_objects]
+    def get_data(self, *, query: ForgeQuery, return_source: bool):
+        data = [copy.deepcopy(s3_object) for s3_object in self._s3_objects]
 
-        if query is None:
-            return data
+        if query is not None:
+            data = self._get_data_query(query, data)
+
+        if not return_source:
+            data = [{"key": item["key"], "data": item["data"]} for item in data]
 
-        return self._get_data_query(query, data)
+        return data
 
     def add_key(self, key: str) -> None:
-        self.keys.append(key)
+        self._keys.append(key)
 
     def load_data(self) -> None:
         def create_csv(data: list[list[str | int]]):
             with io.StringIO() as string_io:
                 csv.writer(string_io).writerows(data)
                 return string_io.getvalue()
 
@@ -59,21 +64,21 @@
             "text": (lambda data: data),
             "json": (lambda data: json.dumps(data)),
             "base64": (lambda data: base64.b64decode(data)),
             "csv": create_csv,
             "file": load_file,
         }
 
-        for s3_object in self.s3_objects:
+        for s3_object in self._s3_objects:
             data_types = list(set(data_type_map.keys()).intersection(set(s3_object["data"].keys())))
 
             if len(data_types) != 1:
                 raise Exception(f"Can only have one of the following per s3 config: {list(data_type_map.keys())}")
 
             data_type = data_types[0]
             data_func = data_type_map[data_type]
             data = data_func(s3_object["data"][data_type])
 
-            s3.put_object(self.bucket_name, s3_object["key"], data, session=self.aws_session)
+            s3.put_object(self._get_bucket_name(), s3_object["key"], data, session=self._aws_session)
 
     def cleanup_data(self) -> None:
-        s3.delete_objects_simplified(self.bucket_name, self.keys, session=self.aws_session)
+        s3.delete_objects_simplified(self._get_bucket_name(), self._keys, session=self._aws_session)
```

### Comparing `skymantle_mock_data_forge-0.3.0/tests/test_dynamodb_forge.py` & `skymantle_mock_data_forge-0.4.0/tests/test_dynamodb_forge.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import json
 import os
 import uuid
 
 import boto3
 import pytest
-from moto import mock_cloudformation, mock_dynamodb, mock_ssm
+from moto import mock_aws
 from pytest_mock import MockerFixture
 
 from skymantle_mock_data_forge.dynamodb_forge import DynamoDbForge
-from skymantle_mock_data_forge.models import OverideType
+from skymantle_mock_data_forge.models import OverrideType
 
 
 @pytest.fixture(autouse=True)
 def environment(mocker: MockerFixture):
     return mocker.patch.dict(
         os.environ,
         {"AWS_DEFAULT_REGION": "ca-central-1", "BOTO_BUDDY_DISABLE_CACHE": "true"},
     )
 
 
-@mock_ssm
-@mock_dynamodb
+@mock_aws
 def test_load_data_by_ssm():
     dynamodb_client = boto3.client("dynamodb")
 
     dynamodb_client.create_table(
         BillingMode="PAY_PER_REQUEST",
         TableName="some_table",
         AttributeDefinitions=[{"AttributeName": "PK", "AttributeType": "S"}],
@@ -43,16 +42,15 @@
     manager = DynamoDbForge("some-config", data_loader_config)
     manager.load_data()
 
     response = dynamodb_client.get_item(TableName="some_table", Key={"PK": {"S": "some_key_1"}})
     assert response["Item"] == {"PK": {"S": "some_key_1"}, "Description": {"S": "Some description 1"}}
 
 
-@mock_cloudformation
-@mock_dynamodb
+@mock_aws
 def test_load_data_by_cfn():
     dynamodb_client = boto3.client("dynamodb")
 
     dynamodb_client.create_table(
         BillingMode="PAY_PER_REQUEST",
         TableName="some_table",
         AttributeDefinitions=[{"AttributeName": "PK", "AttributeType": "S"}],
@@ -78,16 +76,15 @@
     manager = DynamoDbForge("some-config", data_loader_config)
     manager.load_data()
 
     response = dynamodb_client.get_item(TableName="some_table", Key={"PK": {"S": "some_key_1"}})
     assert response["Item"] == {"PK": {"S": "some_key_1"}, "Description": {"S": "Some description 1"}}
 
 
-@mock_cloudformation
-@mock_dynamodb
+@mock_aws
 def test_load_data_by_cfn_invalid_output():
     dynamodb_client = boto3.client("dynamodb")
 
     dynamodb_client.create_table(
         BillingMode="PAY_PER_REQUEST",
         TableName="some_table",
         AttributeDefinitions=[{"AttributeName": "PK", "AttributeType": "S"}],
@@ -106,21 +103,22 @@
 
     data_loader_config = {
         "table": {"stack": {"name": "some_stack", "output": "db_name"}},
         "primary_key_names": ["PK"],
         "items": [{"data": {"PK": "some_key_1", "Description": "Some description 1"}}],
     }
 
+    forge = DynamoDbForge("some-config", data_loader_config)
     with pytest.raises(Exception) as e:
-        DynamoDbForge("some-config", data_loader_config)
+        forge.load_data()
 
     assert str(e.value) == "Unable to find a resource for stack: some_stack and output: db_name"
 
 
-@mock_dynamodb
+@mock_aws
 def test_load_and_cleanup_data():
     dynamodb_client = boto3.client("dynamodb")
 
     dynamodb_client.create_table(
         BillingMode="PAY_PER_REQUEST",
         TableName="some_table",
         AttributeDefinitions=[{"AttributeName": "PK", "AttributeType": "S"}],
@@ -141,15 +139,15 @@
 
     manager.cleanup_data()
 
     response = dynamodb_client.get_item(TableName="some_table", Key={"PK": {"S": "some_key_1"}})
     assert response.get("Item") is None
 
 
-@mock_dynamodb
+@mock_aws
 def test_get_data():
     dynamodb_client = boto3.client("dynamodb")
 
     dynamodb_client.create_table(
         BillingMode="PAY_PER_REQUEST",
         TableName="some_table",
         AttributeDefinitions=[{"AttributeName": "PK", "AttributeType": "S"}],
@@ -159,20 +157,20 @@
     data_loader_config = {
         "table": {"name": "some_table"},
         "primary_key_names": ["PK"],
         "items": [{"data": {"PK": "some_key_1", "Description": "Some description 1"}}],
     }
 
     manager = DynamoDbForge("some-config", data_loader_config)
-    data = manager.get_data()
+    data = manager.get_data(query=None, return_source=True)
 
     assert data == [{"data": {"PK": "some_key_1", "Description": "Some description 1"}}]
 
 
-@mock_dynamodb
+@mock_aws
 def test_get_data_query_string_equals():
     dynamodb_client = boto3.client("dynamodb")
 
     dynamodb_client.create_table(
         BillingMode="PAY_PER_REQUEST",
         TableName="some_table",
         AttributeDefinitions=[{"AttributeName": "PK", "AttributeType": "S"}],
@@ -187,20 +185,20 @@
             {"tags": {"tests": "test_2"}, "data": {"PK": "some_key_2", "Description": "Some description 2"}},
         ],
     }
 
     query = {"StringEquals": {"tests": "test_1"}}
 
     manager = DynamoDbForge("some-config", data_loader_config)
-    data = manager.get_data(query)
+    data = manager.get_data(query=query, return_source=True)
 
     assert data == [{"tags": {"tests": "test_1"}, "data": {"PK": "some_key_1", "Description": "Some description 1"}}]
 
 
-@mock_dynamodb
+@mock_aws
 def test_get_data_query_string_like():
     dynamodb_client = boto3.client("dynamodb")
 
     dynamodb_client.create_table(
         BillingMode="PAY_PER_REQUEST",
         TableName="some_table",
         AttributeDefinitions=[{"AttributeName": "PK", "AttributeType": "S"}],
@@ -216,23 +214,55 @@
             {"data": {"PK": "some_key_3", "Description": "Some description 3"}},
         ],
     }
 
     query = {"StringLike": {"tests": "test"}}
 
     manager = DynamoDbForge("some-config", data_loader_config)
-    data = manager.get_data(query)
+    data = manager.get_data(query=query, return_source=True)
 
     assert data == [
         {"tags": {"tests": "test_1"}, "data": {"PK": "some_key_1", "Description": "Some description 1"}},
         {"tags": {"tests": "test_2"}, "data": {"PK": "some_key_2", "Description": "Some description 2"}},
     ]
 
 
-@mock_dynamodb
+@mock_aws
+def test_get_data_exclude_tags():
+    dynamodb_client = boto3.client("dynamodb")
+
+    dynamodb_client.create_table(
+        BillingMode="PAY_PER_REQUEST",
+        TableName="some_table",
+        AttributeDefinitions=[{"AttributeName": "PK", "AttributeType": "S"}],
+        KeySchema=[{"AttributeName": "PK", "KeyType": "HASH"}],
+    )
+
+    data_loader_config = {
+        "table": {"name": "some_table"},
+        "primary_key_names": ["PK"],
+        "items": [
+            {"tags": {"tests": "test_1"}, "data": {"PK": "some_key_1", "Description": "Some description 1"}},
+            {"tags": {"tests": "test_2"}, "data": {"PK": "some_key_2", "Description": "Some description 2"}},
+            {"data": {"PK": "some_key_3", "Description": "Some description 3"}},
+        ],
+    }
+
+    query = {"StringLike": {"tests": "test"}}
+
+    manager = DynamoDbForge("some-config", data_loader_config)
+    data = manager.get_data(query=query, return_source=False)
+
+    assert data == [
+        {"PK": "some_key_1", "Description": "Some description 1"},
+        {"PK": "some_key_2", "Description": "Some description 2"},
+    ]
+
+
+@mock_aws
 def test_add_key_and_cleanup_data():
     dynamodb_client = boto3.client("dynamodb")
 
     dynamodb_client.create_table(
         BillingMode="PAY_PER_REQUEST",
         TableName="some_table",
         AttributeDefinitions=[{"AttributeName": "PK", "AttributeType": "S"}],
@@ -254,15 +284,15 @@
     manager.add_key({"PK": "some_key_1"})
     manager.cleanup_data()
 
     response = dynamodb_client.get_item(TableName="some_table", Key={"PK": {"S": "some_key_1"}})
     assert response.get("Item") is None
 
 
-@mock_dynamodb
+@mock_aws
 def test_override():
     dynamodb_client = boto3.client("dynamodb")
 
     dynamodb_client.create_table(
         BillingMode="PAY_PER_REQUEST",
         TableName="some_table",
         AttributeDefinitions=[{"AttributeName": "PK", "AttributeType": "S"}],
@@ -275,20 +305,20 @@
         "items": [{"data": {"PK": "", "Description": "Some description 1"}}],
     }
 
     pk = str(uuid.uuid4())
     overrides = [
         {
             "key_paths": "data.PK",
-            "override_type": OverideType.REPLACE_VALUE,
+            "override_type": OverrideType.REPLACE_VALUE,
             "override": pk,
         },
     ]
 
     manager = DynamoDbForge("some-config", data_loader_config, overrides=overrides)
     manager.load_data()
 
     response = dynamodb_client.get_item(TableName="some_table", Key={"PK": {"S": pk}})
     assert response["Item"] == {"PK": {"S": pk}, "Description": {"S": "Some description 1"}}
 
-    data = manager.get_data()
+    data = manager.get_data(query=None, return_source=True)
     assert data == [{"data": {"PK": pk, "Description": "Some description 1"}}]
```

### Comparing `skymantle_mock_data_forge-0.3.0/tests/test_forge_factory.py` & `skymantle_mock_data_forge-0.4.0/tests/test_forge_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from unittest.mock import MagicMock
 
 import pytest
 from pytest_mock import MockerFixture
 
 from skymantle_mock_data_forge.forge_factory import ForgeFactory
-from skymantle_mock_data_forge.models import OverideType
+from skymantle_mock_data_forge.models import OverrideType
 
 
 @pytest.fixture()
 def mock_dynamodb_forge(mocker: MockerFixture) -> MagicMock:
     mock = mocker.patch("skymantle_mock_data_forge.forge_factory.DynamoDbForge")
     return mock
 
@@ -55,29 +55,29 @@
                 "s3_objects": [{"key": "some_key_1", "data": {"text": "Some Data"}}],
             },
         },
     ]
 
     for_all = {
         "key_paths": "data.PK",
-        "override_type": OverideType.REPLACE_VALUE,
+        "override_type": OverrideType.REPLACE_VALUE,
         "override": "some_other_key_1",
     }
 
     for_dynamodb = {
         "forge_id": "some_config_1",
         "key_paths": "data.PK",
-        "override_type": OverideType.REPLACE_VALUE,
+        "override_type": OverrideType.REPLACE_VALUE,
         "override": "some_other_key_1",
     }
 
     for_s3 = {
         "forge_id": "some_config_2",
         "key_paths": "data.text",
-        "override_type": OverideType.REPLACE_VALUE,
+        "override_type": OverrideType.REPLACE_VALUE,
         "override": "Some Other Data",
     }
 
     ForgeFactory(data_forge_config, overrides=[for_all, for_dynamodb, for_s3])
 
     forge_id = data_forge_config[0]["forge_id"]
     dynamodb = data_forge_config[0]["dynamodb"]
@@ -343,37 +343,67 @@
 
     with pytest.raises(Exception) as e:
         forge_factory.add_key("invalid_config", {"PK": "some_key_2"})
 
     assert str(e.value) == "invalid_config not initialized (some_config)."
 
 
-def test_get_key_data(mock_dynamodb_forge):
+def test_get_data(mock_dynamodb_forge):
     data_forge_config = [
         {
             "forge_id": "some_config",
             "dynamodb": {
                 "table": {"name": "some_table"},
                 "primary_key_names": ["PK"],
                 "items": [{"data": {"PK": "some_key_1", "Description": "Some description 1"}}],
             },
         }
     ]
-    mock_dynamodb_forge.return_value.get_data.return_value = [{"PK": "some_key_1", "Description": "Some description 1"}]
+    mock_dynamodb_forge.return_value.get_data.return_value = [
+        {"data": {"PK": "some_key_1", "Description": "Some description 1"}}
+    ]
 
     forge_factory = ForgeFactory(data_forge_config)
 
     data = forge_factory.get_data("some_config")
 
-    mock_dynamodb_forge.return_value.get_data.assert_called_once_with(None)
+    mock_dynamodb_forge.return_value.get_data.assert_called_once_with(query=None, return_source=False)
+
+    assert data == [{"data": {"PK": "some_key_1", "Description": "Some description 1"}}]
+
+
+def test_get_data_first_item(mock_dynamodb_forge):
+    data_forge_config = [
+        {
+            "forge_id": "some_config",
+            "dynamodb": {
+                "table": {"name": "some_table"},
+                "primary_key_names": ["PK"],
+                "items": [
+                    {"data": {"PK": "some_key_1", "Description": "Some description 1"}},
+                    {"data": {"PK": "some_key_2", "Description": "Some description 2"}},
+                ],
+            },
+        }
+    ]
+    mock_dynamodb_forge.return_value.get_data.return_value = [
+        {"data": {"PK": "some_key_1", "Description": "Some description 1"}},
+        {"data": {"PK": "some_key_2", "Description": "Some description 2"}},
+    ]
+
+    forge_factory = ForgeFactory(data_forge_config)
+
+    data = forge_factory.get_data_first_item("some_config")
+
+    mock_dynamodb_forge.return_value.get_data.assert_called_once_with(query=None, return_source=False)
 
-    assert data == [{"PK": "some_key_1", "Description": "Some description 1"}]
+    assert data == {"data": {"PK": "some_key_1", "Description": "Some description 1"}}
 
 
-def test_get_key_invalid_id(mock_dynamodb_forge):
+def test_get_data_invalid_id(mock_dynamodb_forge):
     data_forge_config = [
         {
             "forge_id": "some_config",
             "dynamodb": {
                 "table": {"name": "some_table"},
                 "primary_key_names": ["PK"],
                 "items": [{"data": {"PK": "some_key_1", "Description": "Some description 1"}}],
```

### Comparing `skymantle_mock_data_forge-0.3.0/tests/test_overrides.py` & `skymantle_mock_data_forge-0.4.0/tests/test_overrides.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import uuid
 from datetime import UTC, datetime
 
 import pytest
 from pytest_mock import MockerFixture
 
 from skymantle_mock_data_forge.base_forge import BaseForge
-from skymantle_mock_data_forge.models import OverideType
+from skymantle_mock_data_forge.models import OverrideType
 
 
 @pytest.fixture(autouse=True)
 def environment(mocker: MockerFixture):
     return mocker.patch.dict(
         os.environ,
         {"AWS_DEFAULT_REGION": "us-east-1", "BOTO_BUDDY_DISABLE_CACHE": "true"},
@@ -29,15 +29,15 @@
 def test_replace_value():
     data = [{"create_date": ""}, {"create_date": ""}]
 
     current_date = datetime.now(UTC).isoformat()
     overrides = [
         {
             "key_paths": "create_date",
-            "override_type": OverideType.REPLACE_VALUE,
+            "override_type": OverrideType.REPLACE_VALUE,
             "override": current_date,
         }
     ]
 
     forge = BaseForge("string", overrides)
     update_data = forge._override_data(data)
 
@@ -46,15 +46,15 @@
 
 def test_format_value():
     data = [{"key_1": "{} Assemble!"}]
 
     overrides = [
         {
             "key_paths": "key_1",
-            "override_type": OverideType.FORMAT_VALUE,
+            "override_type": OverrideType.FORMAT_VALUE,
             "override": ["Avengers"],
         }
     ]
 
     forge = BaseForge("string", overrides)
     update_data = forge._override_data(data)
 
@@ -84,15 +84,15 @@
         return new_id
 
     data = [{"id": "old1"}, {"id": "old2"}]
 
     overrides = [
         {
             "key_paths": "id",
-            "override_type": OverideType.CALL_FUNCTION,
+            "override_type": OverrideType.CALL_FUNCTION,
             "override": generate_id,
         }
     ]
 
     forge = BaseForge("string", overrides)
     update_data = forge._override_data(data)
 
@@ -107,15 +107,15 @@
 def test_key_path_list():
     data = [{"create_date": "", "update_date": ""}]
 
     current_date = datetime.now(UTC).isoformat()
     overrides = [
         {
             "key_paths": ["create_date", "update_date"],
-            "override_type": OverideType.REPLACE_VALUE,
+            "override_type": OverrideType.REPLACE_VALUE,
             "override": current_date,
         }
     ]
 
     forge = BaseForge("string", overrides)
     update_data = forge._override_data(data)
 
@@ -127,20 +127,20 @@
 
     current_date = datetime.now(UTC).isoformat()
     key = str(uuid.uuid4())
 
     overrides = [
         {
             "key_paths": "key",
-            "override_type": OverideType.REPLACE_VALUE,
+            "override_type": OverrideType.REPLACE_VALUE,
             "override": key,
         },
         {
             "key_paths": "audit.create_date",
-            "override_type": OverideType.REPLACE_VALUE,
+            "override_type": OverrideType.REPLACE_VALUE,
             "override": current_date,
         },
     ]
 
     forge = BaseForge("string", overrides)
     update_data = forge._override_data(data)
 
@@ -151,15 +151,15 @@
     data = [{"id": "", "items": [{"id": ""}, {"id": ""}, {"id": ""}]}]
 
     key = str(uuid.uuid4())
 
     overrides = [
         {
             "key_paths": ["id", "items.id"],
-            "override_type": OverideType.REPLACE_VALUE,
+            "override_type": OverrideType.REPLACE_VALUE,
             "override": key,
         },
     ]
 
     forge = BaseForge("string", overrides)
     update_data = forge._override_data(data)
 
@@ -170,15 +170,15 @@
     data = [{"id": "", "items": []}]
 
     key = str(uuid.uuid4())
 
     overrides = [
         {
             "key_paths": ["id", "items.id"],
-            "override_type": OverideType.REPLACE_VALUE,
+            "override_type": OverrideType.REPLACE_VALUE,
             "override": key,
         },
     ]
 
     forge = BaseForge("string", overrides)
     update_data = forge._override_data(data)
 
@@ -191,15 +191,15 @@
     data = [{"id": "", "items": ["id", "id", "id"]}]
 
     key = str(uuid.uuid4())
 
     overrides = [
         {
             "key_paths": ["id", "items.id"],
-            "override_type": OverideType.REPLACE_VALUE,
+            "override_type": OverrideType.REPLACE_VALUE,
             "override": key,
         },
     ]
 
     forge = BaseForge("string", overrides)
 
     with pytest.raises(Exception) as e:
@@ -223,15 +223,15 @@
 
 def test_invalid_data():
     data = [""]
 
     overrides = [
         {
             "key_paths": "id",
-            "override_type": OverideType.REPLACE_VALUE,
+            "override_type": OverrideType.REPLACE_VALUE,
             "override": "a string",
         },
     ]
 
     forge = BaseForge("string", overrides)
 
     with pytest.raises(Exception) as e:
@@ -244,15 +244,15 @@
     os.environ["DATA_FORGE_SUPPRESS_KEY_PATH_ERRORS"] = "false"
 
     data = [{"create_date": "", "update_date": ""}]
 
     overrides = [
         {
             "key_paths": "id",
-            "override_type": OverideType.REPLACE_VALUE,
+            "override_type": OverrideType.REPLACE_VALUE,
             "override": "a string",
         },
     ]
 
     forge = BaseForge("string", overrides)
 
     with pytest.raises(Exception) as e:
@@ -262,15 +262,15 @@
 
 
 def test_invalid_key_path():
     data = [{"create_date": "", "update_date": ""}]
     overrides = [
         {
             "key_paths": 1,
-            "override_type": OverideType.REPLACE_VALUE,
+            "override_type": OverrideType.REPLACE_VALUE,
             "override": "a string",
         },
     ]
 
     forge = BaseForge("string", overrides)
 
     with pytest.raises(Exception) as e:
@@ -281,15 +281,15 @@
 
 def test_invalid_key_path_list():
     data = [{"create_date": "", "update_date": ""}]
 
     overrides = [
         {
             "key_paths": [1],
-            "override_type": OverideType.REPLACE_VALUE,
+            "override_type": OverrideType.REPLACE_VALUE,
             "override": "a string",
         },
     ]
 
     forge = BaseForge("string", overrides)
 
     with pytest.raises(Exception) as e:
@@ -303,15 +303,15 @@
 
     data = [{"audit": ""}]
 
     current_date = datetime.now(UTC).isoformat()
     overrides = [
         {
             "key_paths": "audit.create_date",
-            "override_type": OverideType.REPLACE_VALUE,
+            "override_type": OverrideType.REPLACE_VALUE,
             "override": current_date,
         },
     ]
 
     forge = BaseForge("string", overrides)
 
     with pytest.raises(Exception) as e:
@@ -323,20 +323,20 @@
 def test_base_key_exists_but_not_dict_suppress():
     data = [{"current_date": "", "audit": ""}]
 
     current_date = datetime.now(UTC).isoformat()
     overrides = [
         {
             "key_paths": "current_date",
-            "override_type": OverideType.REPLACE_VALUE,
+            "override_type": OverrideType.REPLACE_VALUE,
             "override": current_date,
         },
         {
             "key_paths": "audit.create_date",
-            "override_type": OverideType.REPLACE_VALUE,
+            "override_type": OverrideType.REPLACE_VALUE,
             "override": current_date,
         },
     ]
 
     forge = BaseForge("string", overrides)
     update_data = forge._override_data(data)
 
@@ -345,15 +345,15 @@
 
 def test_invalid_format_value():
     data = [{"key_1": 1234}]
 
     overrides = [
         {
             "key_paths": "key_1",
-            "override_type": OverideType.FORMAT_VALUE,
+            "override_type": OverrideType.FORMAT_VALUE,
             "override": ["Avengers"],
         }
     ]
 
     forge = BaseForge("string", overrides)
 
     with pytest.raises(Exception) as e:
```

### Comparing `skymantle_mock_data_forge-0.3.0/tests/test_s3_forge.py` & `skymantle_mock_data_forge-0.4.0/tests/test_s3_forge.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import json
 import os
 
 import boto3
 import pytest
-from moto import mock_cloudformation, mock_s3, mock_ssm
+from moto import mock_aws
 from pytest_mock import MockerFixture
 
-from skymantle_mock_data_forge.models import OverideType
+from skymantle_mock_data_forge.models import OverrideType
 from skymantle_mock_data_forge.s3_forge import S3Forge
 
 
 @pytest.fixture(autouse=True)
 def environment(mocker: MockerFixture):
     return mocker.patch.dict(
         os.environ,
         {"AWS_DEFAULT_REGION": "us-east-1", "BOTO_BUDDY_DISABLE_CACHE": "true"},
     )
 
 
-@mock_s3
-@mock_ssm
+@mock_aws
 def test_load_data_by_ssm():
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
 
     ssm_client = boto3.client("ssm")
     ssm_client.put_parameter(Name="some_ssm_key", Type="String", Value="some_bucket")
 
@@ -35,16 +34,15 @@
     manager = S3Forge("some-config", s3_config)
     manager.load_data()
 
     response = s3_client.get_object(Bucket="some_bucket", Key="some_key")
     assert response["Body"].read() == b"Some Data"
 
 
-@mock_cloudformation
-@mock_s3
+@mock_aws
 def test_load_data_by_cfn():
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
 
     cfn_template = {
         "AWSTemplateFormatVersion": "2010-09-09",
         "Description": "sample template",
@@ -63,16 +61,15 @@
     manager = S3Forge("some-config", s3_config)
     manager.load_data()
 
     response = s3_client.get_object(Bucket="some_bucket", Key="some_key")
     assert response["Body"].read() == b"Some Data"
 
 
-@mock_cloudformation
-@mock_s3
+@mock_aws
 def test_load_data_by_cfn_invalid_output():
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
 
     cfn_template = {
         "AWSTemplateFormatVersion": "2010-09-09",
         "Description": "sample template",
@@ -84,21 +81,22 @@
     cfn_client.create_stack(StackName="some_stack", TemplateBody=json.dumps(cfn_template))
 
     s3_config = {
         "bucket": {"stack": {"name": "some_stack", "output": "bucket_name"}},
         "s3_objects": [{"key": "some_key", "data": {"text": "Some Data"}}],
     }
 
+    forge = S3Forge("some-config", s3_config)
     with pytest.raises(Exception) as e:
-        S3Forge("some-config", s3_config)
+        forge.load_data()
 
     assert str(e.value) == "Unable to find a resource for stack: some_stack and output: bucket_name"
 
 
-@mock_s3
+@mock_aws
 def test_load_text_and_cleanup_data():
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
 
     s3_config = {
         "bucket": {"name": "some_bucket"},
         "s3_objects": [{"key": "some_key", "data": {"text": "Some Data"}}],
@@ -114,15 +112,15 @@
 
     with pytest.raises(Exception) as e:
         s3_client.get_object(Bucket="some_bucket", Key="some_key")
 
     assert "An error occurred (NoSuchKey) when calling the GetObject operation" in str(e.value)
 
 
-@mock_s3
+@mock_aws
 def test_load_json_and_cleanup_data():
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
 
     s3_config = {
         "bucket": {"name": "some_bucket"},
         "s3_objects": [{"key": "some_key", "data": {"json": {"some_key": "some_value"}}}],
@@ -138,15 +136,15 @@
 
     with pytest.raises(Exception) as e:
         s3_client.get_object(Bucket="some_bucket", Key="some_key")
 
     assert "An error occurred (NoSuchKey) when calling the GetObject operation" in str(e.value)
 
 
-@mock_s3
+@mock_aws
 def test_load_base64_and_cleanup_data():
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
 
     s3_config = {
         "bucket": {"name": "some_bucket"},
         "s3_objects": [{"key": "some_key", "data": {"base64": "SGVsbG8gV29ybGQh"}}],
@@ -162,15 +160,15 @@
 
     with pytest.raises(Exception) as e:
         s3_client.get_object(Bucket="some_bucket", Key="some_key")
 
     assert "An error occurred (NoSuchKey) when calling the GetObject operation" in str(e.value)
 
 
-@mock_s3
+@mock_aws
 def test_load_csv_and_cleanup_data():
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
 
     s3_config = {
         "bucket": {"name": "some_bucket"},
         "s3_objects": [
@@ -198,47 +196,47 @@
 
     with pytest.raises(Exception) as e:
         s3_client.get_object(Bucket="some_bucket", Key="some_key")
 
     assert "An error occurred (NoSuchKey) when calling the GetObject operation" in str(e.value)
 
 
-@mock_s3
+@mock_aws
 def test_load_file_and_cleanup_data():
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
 
     s3_config = {
         "bucket": {"name": "some_bucket"},
         "s3_objects": [
             {
                 "key": "some_key",
-                "data": {"file": "tests/data/amazon_webservices_logo.png"},
+                "data": {"file": "tests/data/amazon_web_services_logo.png"},
             }
         ],
     }
 
     manager = S3Forge("some-config", s3_config)
     manager.load_data()
 
-    with open("tests/data/amazon_webservices_logo.png", "rb") as file:
+    with open("tests/data/amazon_web_services_logo.png", "rb") as file:
         data = file.read()
 
     response = s3_client.get_object(Bucket="some_bucket", Key="some_key")
     assert response["Body"].read() == data
 
     manager.cleanup_data()
 
     with pytest.raises(Exception) as e:
         s3_client.get_object(Bucket="some_bucket", Key="some_key")
 
     assert "An error occurred (NoSuchKey) when calling the GetObject operation" in str(e.value)
 
 
-@mock_s3
+@mock_aws
 def test_load_data_invalid_type():
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
 
     s3_config = {
         "bucket": {"name": "some_bucket"},
         "s3_objects": [{"key": "some_key", "data": {"invalid": ""}}],
@@ -248,15 +246,15 @@
 
     with pytest.raises(Exception) as e:
         manager.load_data()
 
     assert "Can only have one of the following per s3 config:" in str(e.value)
 
 
-@mock_s3
+@mock_aws
 def test_load_data_to_many_types():
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
 
     s3_config = {
         "bucket": {"name": "some_bucket"},
         "s3_objects": [
@@ -274,31 +272,31 @@
 
     with pytest.raises(Exception) as e:
         manager.load_data()
 
     assert "Can only have one of the following per s3 config:" in str(e.value)
 
 
-@mock_s3
+@mock_aws
 def test_get_data():
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
 
     s3_config = {
         "bucket": {"name": "some_bucket"},
         "s3_objects": [{"key": "some_key", "data": {"text": "Some Data"}}],
     }
 
     manager = S3Forge("some-config", s3_config)
-    data = manager.get_data()
+    data = manager.get_data(query=None, return_source=True)
 
     assert data == [{"key": "some_key", "data": {"text": "Some Data"}}]
 
 
-@mock_s3
+@mock_aws
 def test_get_data_query_string_equals():
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
 
     s3_config = {
         "bucket": {"name": "some_bucket"},
         "s3_objects": [
@@ -314,20 +312,20 @@
             },
         ],
     }
 
     query = {"StringEquals": {"type": "text"}}
 
     manager = S3Forge("some-config", s3_config)
-    data = manager.get_data(query=query)
+    data = manager.get_data(query=query, return_source=True)
 
     assert data == [{"key": "some_key_1", "tags": {"type": "text"}, "data": {"text": "Some Data"}}]
 
 
-@mock_s3
+@mock_aws
 def test_get_data_query_string_equals_list():
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
 
     s3_config = {
         "bucket": {"name": "some_bucket"},
         "s3_objects": [
@@ -342,22 +340,22 @@
                 "data": {"json": {"some_key": "some_value"}},
             },
         ],
     }
     query = {"StringEquals": {"tests": "test_1"}}
 
     manager = S3Forge("some-config", s3_config)
-    data = manager.get_data(query=query)
+    data = manager.get_data(query=query, return_source=True)
 
     assert data == [
         {"key": "some_key_1", "tags": {"type": "text", "tests": ["test_1", "test_2"]}, "data": {"text": "Some Data"}},
     ]
 
 
-@mock_s3
+@mock_aws
 def test_get_data_query_string_like():
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
 
     s3_config = {
         "bucket": {"name": "some_bucket"},
         "s3_objects": [
@@ -377,23 +375,23 @@
                 "data": {"json": {"key": "value"}},
             },
         ],
     }
     query = {"StringLike": {"tests": "test"}}
 
     manager = S3Forge("some-config", s3_config)
-    data = manager.get_data(query=query)
+    data = manager.get_data(query=query, return_source=True)
 
     assert data == [
         {"key": "some_key_1", "tags": {"type": "text", "tests": ["test_1", "test_2"]}, "data": {"text": "Some Data"}},
         {"key": "some_key_2", "tags": {"type": "json", "tests": "test_3"}, "data": {"json": {"key": "value"}}},
     ]
 
 
-@mock_s3
+@mock_aws
 def test_get_data_query_compound():
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
 
     s3_config = {
         "bucket": {"name": "some_bucket"},
         "s3_objects": [
@@ -416,22 +414,22 @@
     }
     query = {
         "StringLike": {"tests": "test"},
         "StringEquals": {"type": "text"},
     }
 
     manager = S3Forge("some-config", s3_config)
-    data = manager.get_data(query=query)
+    data = manager.get_data(query=query, return_source=True)
 
     assert data == [
         {"key": "some_key_1", "tags": {"type": "text", "tests": ["test_1", "test_2"]}, "data": {"text": "Some Data"}}
     ]
 
 
-@mock_s3
+@mock_aws
 def test_get_data_query_no_matches():
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
 
     s3_config = {
         "bucket": {"name": "some_bucket"},
         "s3_objects": [
@@ -439,20 +437,20 @@
         ],
     }
     query = {
         "StringEquals": {"type": "json"},
     }
 
     manager = S3Forge("some-config", s3_config)
-    data = manager.get_data(query=query)
+    data = manager.get_data(query=query, return_source=True)
 
     assert data == []
 
 
-@mock_s3
+@mock_aws
 def test_get_data_query_no_matches_list():
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
 
     s3_config = {
         "bucket": {"name": "some_bucket"},
         "s3_objects": [
@@ -464,80 +462,80 @@
         ],
     }
     query = {
         "StringEquals": {"tests": "test_3"},
     }
 
     manager = S3Forge("some-config", s3_config)
-    data = manager.get_data(query=query)
+    data = manager.get_data(query=query, return_source=True)
 
     assert data == []
 
 
-@mock_s3
+@mock_aws
 def test_get_data_query_invalid_operator():
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
 
     s3_config = {
         "bucket": {"name": "some_bucket"},
         "s3_objects": [{"key": "some_key_1", "tags": {"type": "text"}, "data": {"text": "Some Data"}}],
     }
 
     query = {"StringNotEquals": {"type": "text"}}
 
     manager = S3Forge("some-config", s3_config)
 
     with pytest.raises(Exception) as e:
-        manager.get_data(query=query)
+        manager.get_data(query=query, return_source=True)
 
     assert "Only the following query operators are supported:" in str(e.value)
 
 
-@mock_s3
-def test_get_data__empty_query():
+@mock_aws
+def test_get_data_empty_query():
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
 
     s3_config = {
         "bucket": {"name": "some_bucket"},
         "s3_objects": [{"key": "some_key_1", "tags": {"type": "text"}, "data": {"text": "Some Data"}}],
     }
 
     query = {}
 
     manager = S3Forge("some-config", s3_config)
 
     with pytest.raises(Exception) as e:
-        manager.get_data(query=query)
+        manager.get_data(query=query, return_source=True)
 
     assert str(e.value) == "Missing operator from query"
 
 
-@mock_s3
+@mock_aws
 def test_get_data_query_invalid_condition():
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
 
     s3_config = {
         "bucket": {"name": "some_bucket"},
         "s3_objects": [{"key": "some_key_1", "tags": {"type": "text"}, "data": {"text": "Some Data"}}],
     }
 
     query = {"StringEquals": "condition"}
 
     manager = S3Forge("some-config", s3_config)
 
     with pytest.raises(Exception) as e:
-        manager.get_data(query=query)
+        manager.get_data(query=query, return_source=True)
 
     assert str(e.value) == "The condition for an operator must be a dict."
 
 
-@mock_s3
+@mock_aws
 def test_get_data_query_multiple_condition():
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
 
     s3_config = {
         "bucket": {"name": "some_bucket"},
         "s3_objects": [
@@ -558,62 +556,96 @@
             },
         ],
     }
     query = {"StringEquals": {"type": "text", "tests": "test_1"}}
 
     manager = S3Forge("some-config", s3_config)
 
-    data = manager.get_data(query=query)
+    data = manager.get_data(query=query, return_source=True)
 
     assert data == [
         {"key": "some_key_1", "tags": {"type": "text", "tests": ["test_1", "test_2"]}, "data": {"text": "Some Data"}}
     ]
 
 
-@mock_s3
+@mock_aws
+def test_get_data_exclude_tags():
+    s3_client = boto3.client("s3")
+    s3_client.create_bucket(Bucket="some_bucket")
+
+    s3_config = {
+        "bucket": {"name": "some_bucket"},
+        "s3_objects": [
+            {
+                "key": "some_key_1",
+                "tags": {"type": "text", "tests": ["test_1", "test_2"]},
+                "data": {"text": "Some Data"},
+            },
+            {
+                "key": "some_key_2",
+                "tags": {"type": "json", "tests": "test_3"},
+                "data": {"json": {"key": "value"}},
+            },
+            {
+                "key": "some_key_3",
+                "tags": {"type": "text"},
+                "data": {"text": "Some Data"},
+            },
+        ],
+    }
+    query = {"StringEquals": {"type": "text", "tests": "test_1"}}
+
+    manager = S3Forge("some-config", s3_config)
+
+    data = manager.get_data(query=query, return_source=False)
+
+    assert data == [{"key": "some_key_1", "data": {"text": "Some Data"}}]
+
+
+@mock_aws
 def test_get_data_query_invalid_tag_int():
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
 
     s3_config = {
         "bucket": {"name": "some_bucket"},
         "s3_objects": [{"key": "some_key_1", "tags": {"type": 0}, "data": {"text": "Some Data"}}],
     }
 
     query = {"StringEquals": {"type": "text"}}
 
     manager = S3Forge("some-config", s3_config)
 
     with pytest.raises(Exception) as e:
-        manager.get_data(query=query)
+        manager.get_data(query=query, return_source=True)
 
     assert str(e.value) == "Tag values can only be strings or list of strings."
 
 
-@mock_s3
+@mock_aws
 def test_get_data_query_invalid_tag_list():
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
 
     s3_config = {
         "bucket": {"name": "some_bucket"},
         "s3_objects": [{"key": "some_key_1", "tags": {"type": [0]}, "data": {"text": "Some Data"}}],
     }
 
     query = {"StringEquals": {"type": "text"}}
 
     manager = S3Forge("some-config", s3_config)
 
     with pytest.raises(Exception) as e:
-        manager.get_data(query=query)
+        manager.get_data(query=query, return_source=True)
 
     assert str(e.value) == "Tag values can only be strings or list of strings."
 
 
-@mock_s3
+@mock_aws
 def test_add_key_and_cleanup_data():
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
 
     s3_config = {
         "bucket": {"name": "some_bucket"},
         "s3_objects": [],
@@ -628,15 +660,15 @@
 
     with pytest.raises(Exception) as e:
         s3_client.get_object(Bucket="some_bucket", Key="some_key")
 
     assert "An error occurred (NoSuchKey) when calling the GetObject operation" in str(e.value)
 
 
-@mock_s3
+@mock_aws
 def test_override():
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
 
     s3_config = {
         "bucket": {"name": "some_bucket"},
         "s3_objects": [
@@ -646,20 +678,20 @@
             }
         ],
     }
 
     overrides = [
         {
             "key_paths": "data.json.some_key",
-            "override_type": OverideType.REPLACE_VALUE,
+            "override_type": OverrideType.REPLACE_VALUE,
             "override": "some_other_value",
         },
     ]
 
     manager = S3Forge("some-config", s3_config, overrides=overrides)
     manager.load_data()
 
     response = s3_client.get_object(Bucket="some_bucket", Key="some_key")
     assert response["Body"].read() == b'{"some_key": "some_other_value"}'
 
-    data = manager.get_data()
+    data = manager.get_data(query=None, return_source=True)
     assert data == [{"key": "some_key", "data": {"json": {"some_key": "some_other_value"}}}]
```

### Comparing `skymantle_mock_data_forge-0.3.0/tests/data/amazon_webservices_logo.png` & `skymantle_mock_data_forge-0.4.0/tests/data/amazon_web_services_logo.png`

 * *Files identical despite different names*

### Comparing `skymantle_mock_data_forge-0.3.0/.gitignore` & `skymantle_mock_data_forge-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `skymantle_mock_data_forge-0.3.0/LICENSE` & `skymantle_mock_data_forge-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skymantle_mock_data_forge-0.3.0/README.md` & `skymantle_mock_data_forge-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 ## Usage
 
 Use the forge factory to manage data to multiple destinations (any combination of DynamoDB tables and S3 buckets). An id is used to specify each unique destination. The forge factor provides the following functions:
 
 - `load_data` - will load data across all destinations or the destination of the provided forge ID
 - `get_data` - will return data across all destinations or the data for the provided forge ID, will only return data created by the forge
+- `get_data_first_item` - will return first item of data across all destinations or the data for the provided forge ID, will only return data created by the forge
 - `add_key` - when new data is created through tests you can provide it's key so that it's included in the `cleanup_data` call
 - `cleanup_data` - will remove data across all destinations or the destination of the provided forge ID
 
 ### Examples
 
 - manage data in DynamoDB, assumes aws credentials environment variable are set, such as `AWS_PROFILE`
 
@@ -152,15 +153,15 @@
 ```
 
 - Override specific values at run time. Useful when config files are stored in static json files or handling dates
 
 ```python
 from datetime import UTC, datetime
 from skymantle_mock_data_forge.forge_factory import ForgeFactory
-from skymantle_mock_data_forge.models import OverideType
+from skymantle_mock_data_forge.models import OverrideType
 
 config = [
     {
         "forge_id": "some_config_id",
         "dynamodb": {
             "table": {"name": "some_table"},
             "primary_key_names": ["PK"],
@@ -168,15 +169,15 @@
         },
     }
 ]
 
 overrides = [
     {
         "key_paths": "CreateDate",
-        "override_type": OverideType.REPLACE_VALUE,
+        "override_type": OverrideType.REPLACE_VALUE,
         "override": datetime.now(UTC).isoformat(),
     }
 ]
 
 factory = ForgeFactory(config, overrides=overrides)
 factory.load_data("some_config_id")
 
@@ -199,15 +200,15 @@
         "table": {"name": "some_table"},
         "primary_key_names": ["PK"],
         "items": [{"data": {"PK": "some_key_1", "Description": "Some description 1"}}],
     }
 }
 ```
 
-- By SSM paramter
+- By SSM parameter
 
 ```json
 {
     "forge_id": "some_config_id_1",
     "dynamodb": {
         "table": {"ssm": "ssm_parameter_key"},
         "primary_key_names": ["PK"],
@@ -280,15 +281,15 @@
         ]
     }
 }
 ```
 
 ## Querying Data For Testing
 
-Custom tags can be added to data that is managed by the forges, this will make it possible to catagorize and group data for use during tests. Tags are completely optional, but requried for querying.
+Custom tags can be added to data that is managed by the forges, this will make it possible to categorize and group data for use during tests. Tags are completely optional, but required for querying.
 
 - DynamoDB tag example
 ```json
 [
     {
         "tags": {
             "tests": ["test_get_item", "test_update_item"]
@@ -316,18 +317,18 @@
         "data": {"json": {"key": "value"}},
     }
 ]
 ```
 
 A query is made up of an operator and 1 or more condition key/value pairs. Supported operators are:
 
- - StringEquals - the value for the tag must match exactly to one of the items in thes specified tag
+ - StringEquals - the value for the tag must match exactly to one of the items in the specified tag
  - StringLike - the value must be contained in on of the items in the specified tag
 
- It's also possible to use both operators in the query. When dealing with multiple contitions and/or operators, queries are limited to logical `AND` queries.
+ It's also possible to use both operators in the query. When dealing with multiple conditions and/or operators, queries are limited to logical `AND` queries.
 
  ### Examples
 
 For the data provided
  ``` json
 [
     {
@@ -434,26 +435,26 @@
 
 - Replace Value
     - Will replace the value with a new one
     - For example if create date is current "" it can be replaced with "2023-01-01"
 - Format Value
     - Will used pythons `str.format(*args)`
     - The original value must be a string, the replacement is index based.
-    - For example if ddescription is "{} Assemble{}" it back be formated to "Avengers Assemble!"
+    - For example if description is "{} Assemble{}" it back be formatted to "Avengers Assemble!"
 - Call Function
     - will call a custom function when processing each item.
-    - The signature of the funct is func(key: str, value: any, context: dict) -> any:
+    - The signature of the function is func(key: str, value: any, context: dict) -> any:
         - key - The current key (ie: CreateDate)
         - value - The current value for the given key
-        - conext - The current item being built
+        - context - The current item being built
         - return - the new value.
 
-In the case of nested dictionaries, key paths are supported which are "." seperated, key paths will also traverse sub lists. Currently it's not possible to specify an index, all items in the list will be updated. 
+In the case of nested dictionaries, key paths are supported which are "." separated, key paths will also traverse sub lists. Currently it's not possible to specify an index, all items in the list will be updated. 
 
-If the same overide is needed for multiple keys then a list of key paths can be used. Currently overrides only work with json structured data. 
+If the same override is needed for multiple keys then a list of key paths can be used. Currently overrides only work with json structured data. 
 
 The default behaviour for overrides is to ignore key path errors, however this behaviour can be altered by setting the `DATA_FORGE_SUPPRESS_KEY_PATH_ERRORS` environment variable. Supported values are `0`, `false`, `no` and `off`.
 
 ### Example
 
 ```python
 # Current config stored in full or in part in json files
@@ -496,28 +497,28 @@
 
 overrides = [
     {
         "key_paths": [
             "data.pk",
             "data.items.id",
         ],
-        "override_type": OverideType.CALL_FUNCTION,
+        "override_type": OverrideType.CALL_FUNCTION,
         "override": generate_id,
     },
     {
         "key_paths": [
             "data.audit.create_date",
             "data.audit.last_update_date",
         ],
-        "override_type": OverideType.REPLACE_VALUE,
+        "override_type": OverrideType.REPLACE_VALUE,
         "override": current_date,
     },
     {
         "key_paths": "data.description",
-        "override_type": OverideType.FORMAT_VALUE,
+        "override_type": OverrideType.FORMAT_VALUE,
         "override": [environment],
     }
 ]
 
 # The resulting data 
 
 {
@@ -549,33 +550,35 @@
 By default, the same list of overrides is distributed to all destinations, if an override needs to vary by destination a forge Id can be provided.
 
 ```python
 
 overrides = [
     { # Will go to all destinations
         "key_paths": "data.text",
-        "override_type": OverideType.REPLACE_VALUE,
+        "override_type": OverrideType.REPLACE_VALUE,
         "override": "Some Other Data",
     },
     { # Will go to some_config_1
         "forge_id": "some_config_1",
         "key_paths": "PK",
-        "override_type": OverideType.REPLACE_VALUE,
+        "override_type": OverrideType.REPLACE_VALUE,
         "override": "some_other_key_1",
     },
     { # Will go to some_config_2
         "forge_id": "some_config_2",
         "key_paths": "PK",
-        "override_type": OverideType.REPLACE_VALUE,
+        "override_type": OverrideType.REPLACE_VALUE,
         "override": "some_other_key_2",
     }
 ]
 
 ```
 
 ## Source Code Dev Notes
 
 The following project commands are supported:
-- `make setup` - Installs all dependencies ands creates virtual environment
-- `make unitTests` - runs unit tests
-- `make lintAndAnalysis` - Runs [ruff](https://github.com/astral-sh/ruff), [bandit](https://github.com/PyCQA/bandit) and [black](https://github.com/psf/black)
+- `make` - provides command line help
+- `make clean` - cleans out virtual env and distribution folder
+- `make install` - Installs virtual env and required packages
+- `make unit_tests` - runs unit tests
+- `make lint_and_analysis` - Runs [ruff](https://github.com/astral-sh/ruff), [bandit](https://github.com/PyCQA/bandit) and [black](https://github.com/psf/black)
 - `make build` - Creates distribution
```

### Comparing `skymantle_mock_data_forge-0.3.0/pyproject.toml` & `skymantle_mock_data_forge-0.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "skymantle_mock_data_forge"
-version = "0.3.0"
+version = "0.4.0"
 dependencies=[
   "skymantle_boto_buddy[boto]"
 ]
 requires-python = ">=3.11"
 authors = [{ name = "Artin Yong-Bannayan", email = "ayongbannayan@skymantle.com" }]
 description = "A library for deploying test data to aws resources when running integration and end-to-end tests."
 readme = "README.md"
@@ -26,45 +26,29 @@
 Issues = "https://github.com/skymantle-tech/skymantle-mock-data-forge/issues"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.envs.default]
 dependencies = [
-  "mypy",
   "pytest",
   "pytest-cov",
   "pytest-mock",
   "bandit",
   "black",
   "ruff",
   "moto[s3,dynamodb,ssm,cloudformation]",
 ]
 path = ".venv"
 
-[tool.hatch.envs.default.scripts]
-_bandit = "bandit -c pyproject.toml -r {args:.}"
-_ruff = "ruff {args:.}"
-_black = "black --check --diff {args:.}"
-_mypy = "mypy --install-types --non-interactive {args:.}"
-cov = "pytest -v --cov-config=pyproject.toml --cov {args:./src} "
-
-
-[tool.mypy]
-exclude = [
-    "dist",
-    ".venv",
-]
-
 [tool.black]
 line-length = 120
 exclude = '''
 /(
     \.git
-  | \.mypy_cache
   | \.tox
   | venv
   | \.venv
   | _build
   | buck-out
   | build
   | dist
@@ -74,15 +58,15 @@
 [tool.bandit]
 skips = ['B324']
 exclude_dirs = [".venv", "tests", "dist"]
 
 [tool.ruff]
 target-version = "py311"
 line-length = 120
-select = [
+lint.select = [
   "A",
   "B",
   "C",
   "DTZ",
   "E",
   "EM",
   "F",
@@ -101,33 +85,33 @@
   "SIM",
   "T",
   "TID",
   "UP",
   "W",
   "YTT",
 ]
-ignore = [
+lint.ignore = [
   # Ignore checks for use `datetime.UTC` alias
   "UP017",
   # Ignore exception must not use a string literal
   "EM101",
   # Ignore checks for f-string literal in exception message
   "EM102",
   # Ignore too many arguments in function definition
   "PLR0913"
 ]
-unfixable = []
+lint.unfixable = []
 
-[tool.ruff.flake8-quotes]
+[tool.ruff.lint.flake8-quotes]
 inline-quotes = "double"
 
-[tool.ruff.flake8-tidy-imports]
+[tool.ruff.lint.flake8-tidy-imports]
 ban-relative-imports = "all"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "I001"]
 
 [tool.coverage.run]
 branch = true
 parallel = true
 source = ["src"]
```

### Comparing `skymantle_mock_data_forge-0.3.0/PKG-INFO` & `skymantle_mock_data_forge-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: skymantle_mock_data_forge
-Version: 0.3.0
+Version: 0.4.0
 Summary: A library for deploying test data to aws resources when running integration and end-to-end tests.
 Project-URL: Home, https://github.com/skymantle-tech/skymantle-mock-data-forge
 Project-URL: Issues, https://github.com/skymantle-tech/skymantle-mock-data-forge/issues
 Author-email: Artin Yong-Bannayan <ayongbannayan@skymantle.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -231,14 +231,15 @@
 
 ## Usage
 
 Use the forge factory to manage data to multiple destinations (any combination of DynamoDB tables and S3 buckets). An id is used to specify each unique destination. The forge factor provides the following functions:
 
 - `load_data` - will load data across all destinations or the destination of the provided forge ID
 - `get_data` - will return data across all destinations or the data for the provided forge ID, will only return data created by the forge
+- `get_data_first_item` - will return first item of data across all destinations or the data for the provided forge ID, will only return data created by the forge
 - `add_key` - when new data is created through tests you can provide it's key so that it's included in the `cleanup_data` call
 - `cleanup_data` - will remove data across all destinations or the destination of the provided forge ID
 
 ### Examples
 
 - manage data in DynamoDB, assumes aws credentials environment variable are set, such as `AWS_PROFILE`
 
@@ -370,15 +371,15 @@
 ```
 
 - Override specific values at run time. Useful when config files are stored in static json files or handling dates
 
 ```python
 from datetime import UTC, datetime
 from skymantle_mock_data_forge.forge_factory import ForgeFactory
-from skymantle_mock_data_forge.models import OverideType
+from skymantle_mock_data_forge.models import OverrideType
 
 config = [
     {
         "forge_id": "some_config_id",
         "dynamodb": {
             "table": {"name": "some_table"},
             "primary_key_names": ["PK"],
@@ -386,15 +387,15 @@
         },
     }
 ]
 
 overrides = [
     {
         "key_paths": "CreateDate",
-        "override_type": OverideType.REPLACE_VALUE,
+        "override_type": OverrideType.REPLACE_VALUE,
         "override": datetime.now(UTC).isoformat(),
     }
 ]
 
 factory = ForgeFactory(config, overrides=overrides)
 factory.load_data("some_config_id")
 
@@ -417,15 +418,15 @@
         "table": {"name": "some_table"},
         "primary_key_names": ["PK"],
         "items": [{"data": {"PK": "some_key_1", "Description": "Some description 1"}}],
     }
 }
 ```
 
-- By SSM paramter
+- By SSM parameter
 
 ```json
 {
     "forge_id": "some_config_id_1",
     "dynamodb": {
         "table": {"ssm": "ssm_parameter_key"},
         "primary_key_names": ["PK"],
@@ -498,15 +499,15 @@
         ]
     }
 }
 ```
 
 ## Querying Data For Testing
 
-Custom tags can be added to data that is managed by the forges, this will make it possible to catagorize and group data for use during tests. Tags are completely optional, but requried for querying.
+Custom tags can be added to data that is managed by the forges, this will make it possible to categorize and group data for use during tests. Tags are completely optional, but required for querying.
 
 - DynamoDB tag example
 ```json
 [
     {
         "tags": {
             "tests": ["test_get_item", "test_update_item"]
@@ -534,18 +535,18 @@
         "data": {"json": {"key": "value"}},
     }
 ]
 ```
 
 A query is made up of an operator and 1 or more condition key/value pairs. Supported operators are:
 
- - StringEquals - the value for the tag must match exactly to one of the items in thes specified tag
+ - StringEquals - the value for the tag must match exactly to one of the items in the specified tag
  - StringLike - the value must be contained in on of the items in the specified tag
 
- It's also possible to use both operators in the query. When dealing with multiple contitions and/or operators, queries are limited to logical `AND` queries.
+ It's also possible to use both operators in the query. When dealing with multiple conditions and/or operators, queries are limited to logical `AND` queries.
 
  ### Examples
 
 For the data provided
  ``` json
 [
     {
@@ -652,26 +653,26 @@
 
 - Replace Value
     - Will replace the value with a new one
     - For example if create date is current "" it can be replaced with "2023-01-01"
 - Format Value
     - Will used pythons `str.format(*args)`
     - The original value must be a string, the replacement is index based.
-    - For example if ddescription is "{} Assemble{}" it back be formated to "Avengers Assemble!"
+    - For example if description is "{} Assemble{}" it back be formatted to "Avengers Assemble!"
 - Call Function
     - will call a custom function when processing each item.
-    - The signature of the funct is func(key: str, value: any, context: dict) -> any:
+    - The signature of the function is func(key: str, value: any, context: dict) -> any:
         - key - The current key (ie: CreateDate)
         - value - The current value for the given key
-        - conext - The current item being built
+        - context - The current item being built
         - return - the new value.
 
-In the case of nested dictionaries, key paths are supported which are "." seperated, key paths will also traverse sub lists. Currently it's not possible to specify an index, all items in the list will be updated. 
+In the case of nested dictionaries, key paths are supported which are "." separated, key paths will also traverse sub lists. Currently it's not possible to specify an index, all items in the list will be updated. 
 
-If the same overide is needed for multiple keys then a list of key paths can be used. Currently overrides only work with json structured data. 
+If the same override is needed for multiple keys then a list of key paths can be used. Currently overrides only work with json structured data. 
 
 The default behaviour for overrides is to ignore key path errors, however this behaviour can be altered by setting the `DATA_FORGE_SUPPRESS_KEY_PATH_ERRORS` environment variable. Supported values are `0`, `false`, `no` and `off`.
 
 ### Example
 
 ```python
 # Current config stored in full or in part in json files
@@ -714,28 +715,28 @@
 
 overrides = [
     {
         "key_paths": [
             "data.pk",
             "data.items.id",
         ],
-        "override_type": OverideType.CALL_FUNCTION,
+        "override_type": OverrideType.CALL_FUNCTION,
         "override": generate_id,
     },
     {
         "key_paths": [
             "data.audit.create_date",
             "data.audit.last_update_date",
         ],
-        "override_type": OverideType.REPLACE_VALUE,
+        "override_type": OverrideType.REPLACE_VALUE,
         "override": current_date,
     },
     {
         "key_paths": "data.description",
-        "override_type": OverideType.FORMAT_VALUE,
+        "override_type": OverrideType.FORMAT_VALUE,
         "override": [environment],
     }
 ]
 
 # The resulting data 
 
 {
@@ -767,33 +768,35 @@
 By default, the same list of overrides is distributed to all destinations, if an override needs to vary by destination a forge Id can be provided.
 
 ```python
 
 overrides = [
     { # Will go to all destinations
         "key_paths": "data.text",
-        "override_type": OverideType.REPLACE_VALUE,
+        "override_type": OverrideType.REPLACE_VALUE,
         "override": "Some Other Data",
     },
     { # Will go to some_config_1
         "forge_id": "some_config_1",
         "key_paths": "PK",
-        "override_type": OverideType.REPLACE_VALUE,
+        "override_type": OverrideType.REPLACE_VALUE,
         "override": "some_other_key_1",
     },
     { # Will go to some_config_2
         "forge_id": "some_config_2",
         "key_paths": "PK",
-        "override_type": OverideType.REPLACE_VALUE,
+        "override_type": OverrideType.REPLACE_VALUE,
         "override": "some_other_key_2",
     }
 ]
 
 ```
 
 ## Source Code Dev Notes
 
 The following project commands are supported:
-- `make setup` - Installs all dependencies ands creates virtual environment
-- `make unitTests` - runs unit tests
-- `make lintAndAnalysis` - Runs [ruff](https://github.com/astral-sh/ruff), [bandit](https://github.com/PyCQA/bandit) and [black](https://github.com/psf/black)
+- `make` - provides command line help
+- `make clean` - cleans out virtual env and distribution folder
+- `make install` - Installs virtual env and required packages
+- `make unit_tests` - runs unit tests
+- `make lint_and_analysis` - Runs [ruff](https://github.com/astral-sh/ruff), [bandit](https://github.com/PyCQA/bandit) and [black](https://github.com/psf/black)
 - `make build` - Creates distribution
```

