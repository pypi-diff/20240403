# Comparing `tmp/dynamojo-0.2.2.tar.gz` & `tmp/dynamojo-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamojo-0.2.2.tar", max compression
+gzip compressed data, was "dynamojo-1.0.0.tar", max compression
```

## Comparing `dynamojo-0.2.2.tar` & `dynamojo-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     4181 2024-03-28 19:01:25.019286 dynamojo-0.2.2/README.md
--rw-r--r--   0        0        0      449 2024-03-28 19:01:25.019636 dynamojo-0.2.2/dynamojo/__init__.py
--rwxr-xr-x   0        0        0    19977 2024-04-01 20:21:05.180906 dynamojo-0.2.2/dynamojo/base.py
--rw-r--r--   0        0        0       89 2024-03-28 19:01:25.020045 dynamojo-0.2.2/dynamojo/boto.py
--rw-r--r--   0        0        0     2212 2024-03-28 19:01:25.020184 dynamojo-0.2.2/dynamojo/config.py
--rw-r--r--   0        0        0      445 2024-03-28 19:01:25.020304 dynamojo-0.2.2/dynamojo/exceptions.py
--rw-r--r--   0        0        0     4406 2024-03-28 19:01:25.020555 dynamojo-0.2.2/dynamojo/index.py
--rw-r--r--   0        0        0     1882 2024-03-28 19:01:25.020700 dynamojo-0.2.2/dynamojo/utils.py
--rw-r--r--   0        0        0      644 2024-04-03 20:18:30.948916 dynamojo-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4677 1970-01-01 00:00:00.000000 dynamojo-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     4181 2024-03-28 19:01:25.019286 dynamojo-1.0.0/README.md
+-rw-r--r--   0        0        0      449 2024-04-03 21:30:22.401274 dynamojo-1.0.0/dynamojo/__init__.py
+-rwxr-xr-x   0        0        0    20356 2024-04-03 21:31:37.755246 dynamojo-1.0.0/dynamojo/base.py
+-rw-r--r--   0        0        0       89 2024-04-03 20:38:31.250208 dynamojo-1.0.0/dynamojo/boto.py
+-rw-r--r--   0        0        0     2098 2024-04-03 21:30:22.427738 dynamojo-1.0.0/dynamojo/config.py
+-rw-r--r--   0        0        0      445 2024-04-03 20:38:31.251170 dynamojo-1.0.0/dynamojo/exceptions.py
+-rw-r--r--   0        0        0     4404 2024-04-03 21:30:22.449865 dynamojo-1.0.0/dynamojo/index.py
+-rw-r--r--   0        0        0     1991 2024-04-03 21:30:22.437078 dynamojo-1.0.0/dynamojo/utils.py
+-rw-r--r--   0        0        0      643 2024-04-03 21:30:19.509805 dynamojo-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4676 1970-01-01 00:00:00.000000 dynamojo-1.0.0/PKG-INFO
```

### Comparing `dynamojo-0.2.2/README.md` & `dynamojo-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `dynamojo-0.2.2/dynamojo/base.py` & `dynamojo-1.0.0/dynamojo/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,148 +6,151 @@
 from logging import getLogger
 from typing import Any, Dict, List, TypeVar, Union
 
 from boto3.dynamodb.conditions import (
     AttributeBase,
     ConditionBase,
     ConditionExpressionBuilder,
-    Attr,
-    Key
 )
 from pydantic import BaseModel, PrivateAttr
 
 from .boto import DYNAMOCLIENT
 from .index import Index, Lsi
 from .config import DynamojoConfig
 from .exceptions import StaticAttributeError, IndexNotFoundError
 from .utils import Delta, TYPE_SERIALIZER, TYPE_DESERIALIZER
 
 
 class DynamojoBase(BaseModel):
     """A class to use as a base for modeling objects to store in Dynamodb. This class
     is intended to be inherited by another class, which actually defines the model.
-    """    
+    """
 
     #: All subclasses should override with their own config of the type `:class:dynamojo.config.DynamojoConfig`
-    _config: DynamojoConfig = PrivateAttr()
+    __config__: DynamojoConfig
+
     #: Original object
-    _original: DynamojoBase = PrivateAttr()
+    __original__: DynamojoBase
 
-    def __new__(cls: DynamojoModel, *_: List[Any], **__: Dict[Any, Any]) -> DynamojoModel:
+    def __new__(
+        cls: DynamojoModel, *_: List[Any], **__: Dict[Any, Any]
+    ) -> DynamojoModel:
         if cls is DynamojoBase:
             raise TypeError(f"{cls} must be subclassed")
         return super().__new__(cls)
 
     def __init__(self: DynamojoModel, **kwargs: Dict[str, Any]) -> None:
-
-        """Initialize a new object with any required or optional attributes"""        
+        """Initialize a new object with any required or optional attributes"""
         super().__init__(**kwargs)
 
-        for attr in self._config.joined_attributes:
-            if attr.attribute in self.dict():
+        for attr in self.__config__.joined_attributes:
+            if attr.attribute in self.model_dump():
                 raise AttributeError(
                     f"Attribute '{attr}' cannot be declared as a member and a joined field"
                 )
-        for attr in self._config.__index_keys__:
-            if attr in self.dict():
+        for attr in self.__config__._index_keys:
+            if attr in self.model_dump():
                 raise AttributeError(
                     f"Attribute {attr} is part of an index and cannot be declared directly. Use IndexMap() and an alias instead"
                 )
 
         # TODO: Flush out these mutators.
         for k, v in kwargs.items():
-            if k in self._config.mutators:
+            if k in self.__config__.mutators:
                 kwargs[k] = self._mutate_attribute(k, v)
 
-        self._original = deepcopy(self)
+        self.__original__ = deepcopy(self)
 
     @property
     def _deepdiff(self):
-        return Delta(new=self, old=self._original, deep=True)
+        return Delta(new=self, old=self.__original__, deep=True)
 
     @property
     def _diff(self):
-        return Delta(new=self, old=self._original)
+        return Delta(new=self, old=self.__original__)
 
     def __getattribute__(self: DynamojoModel, name: str) -> Any:
-        if super().__getattribute__("_config").__joined_attributes__.get(name):
+        if super().__getattribute__("__config__").__joined_attributes__.get(name):
             return self._generate_joined_attribute(name)
 
         return super().__getattribute__(name)
 
     @property
     def _has_changed(self):
         return self._deepdiff.hasChanged
 
     def __setattr__(self: DynamojoModel, field: str, val: Any) -> None:
         # Mutations should happen first to allow for other dynamic fields to get their updated value
-        if field in self._config.mutators:
+        if field in self.__config__.mutators:
             val = self._mutate_attribute(field, val)
 
-        if field in self._config.__joined_attributes__:
+        if field in self.__config__.__joined_attributes__:
             raise AttributeError(
                 f"Attribute '{field}' is a joined field and cannot be set directly"
             )
 
-        if field in self._config.__index_keys__:
+        if field in self.__config__._index_keys:
             raise AttributeError(
                 f"Attribute '{field}' is an index key and cannot be set directly. Use IndexMap() to create an alias"
             )
 
         # Static fields can only be set once
         if (
-            field in self._config.static_attributes
+            field in self.__config__.static_attributes
             and hasattr(self, field)
             and self.__getattribute__(field) != val
         ):
             raise StaticAttributeError(f"Attribute '{field}' is immutable.")
 
         return super().__setattr__(field, val)
 
     def _db_item(self) -> Dict[str, Any]:
         """
-        Returns the item exactly as it is in the database. If self._config.store_aliases is False
+        Returns the item exactly as it is in the database. If self.__config__.store_aliases is False
         then those aliases will be omitted.
         """
-        item = {**self.dict(), **self.joined_attributes(), **self.index_attributes()}
-        if not self._config.store_aliases:
-            for attr in self._config.__index_aliases__.values():
+        item = {
+            **self.model_dump(),
+            **self.joined_attributes(),
+            **self.index_attributes(),
+        }
+        if not self.__config__.store_aliases:
+            for attr in self.__config__._index_aliases.values():
                 if attr in item:
                     del item[attr]
         return item
 
     def _generate_joined_attribute(self: DynamojoModel, name: str) -> str:
         """
-        Takes attribute names defined in self._config.joined_attributes and stores them with the values
+        Takes attribute names defined in self.__config__.joined_attributes and stores them with the values
         of the corresponding attributes concatenated by JoinedAttribute.separator.
         """
         item = super().__getattribute__("dict")()
-        joiner = super().__getattribute__("_config").__joined_attributes__[name]
+        joiner = super().__getattribute__("__config__").__joined_attributes__[name]
         sources = joiner.fields
         separator = joiner.separator
         new_val = [item.get(source, "") for source in sources]
         return separator.join(new_val)
 
     @classmethod
     def _get_index_from_attributes(
         cls, partitionkey: str = None, sortkey: str = None
     ) -> Index:
         """
         Returns an Index() object based on attributes being passed as arguments.
         If multiple indexes match then the table index, if matched is returned first. If
         not the table index then the first match in the list.
         """
-        for x in cls._config.index_maps:
+        for x in cls.__config__.index_maps:
             if x.index.name == "table":
                 table_index_map = x
                 break
         matches = {}
 
-        for mapping in cls._config.index_maps:
-
+        for mapping in cls.__config__.index_maps:
             if isinstance(mapping.index, Lsi):
                 pk = table_index_map.partitionkey
             else:
                 pk = mapping.partitionkey
 
             if hasattr(mapping, "sortkey"):
                 sk = mapping.sortkey
@@ -254,153 +257,156 @@
             opts[expression_type] = opts[expression_type].replace(key, new_key)
 
         for key, val in raw_exp.attribute_value_placeholders.items():
             new_key = key.replace(original_value_prefix, new_value_prefix)
             opts["ExpressionAttributeValues"][new_key] = val
             opts[expression_type] = opts[expression_type].replace(key, new_key)
 
-        opts["TableName"] = self._config.table
+        opts["TableName"] = self.__config__.table
         return opts
 
     @classmethod
     def _construct_from_db(cls, item: Dict) -> DynamojoModel:
         """
         Rehydrates an object from an item out of the DB.
         """
         item = cls._deserialize_dynamo(item)
         res = {}
 
         for attr, val in item.items():
             if not (
-                attr in cls._config.__index_keys__
-                or attr in cls._config.__joined_attributes__
+                attr in cls.__config__._index_keys
+                or attr in cls.__config__.__joined_attributes__
             ):
                 res[attr] = val
 
-        if not cls._config.store_aliases:
-            for index, alias in cls._config.__index_aliases__.items():
+        if not cls.__config__.store_aliases:
+            for index, alias in cls.__config__._index_aliases.items():
                 res[alias] = item[index]
 
         return cls.construct(**(res))
 
-    def delete(self) -> None:
+    async def delete(self) -> None:
         """
         Deletes an item from the table
         """
         key = {
-            self._config.indexes.table.partitionkey: self.index_attributes()[self._config.indexes.table.partitionkey]
+            self.__config__.indexes.table.partitionkey: self.index_attributes()[
+                self.__config__.indexes.table.partitionkey
+            ]
         }
 
-        if self._config.indexes.table.is_composite:
-            key[self._config.indexes.table.sortkey] = self.index_attributes()[self._config.indexes.table.sortkey]
+        if self.__config__.indexes.table.is_composite:
+            key[self.__config__.indexes.table.sortkey] = self.index_attributes()[
+                self.__config__.indexes.table.sortkey
+            ]
 
         serialized_key = {k: TYPE_SERIALIZER.serialize(v) for k, v in key.items()}
 
         res = DYNAMOCLIENT.delete_item(
-            Key=serialized_key,
-            TableName=self._config.table
+            Key=serialized_key, TableName=self.__config__.table
         )
 
         return res
 
     @staticmethod
     def _deserialize_dynamo(data: Dict[str, Any]) -> Dict[str, Any]:
         """
         Deserializes the results from a low-level boto3 Dynamodb client query/get_item
         into a standard dictionary.
         """
         return {k: TYPE_DESERIALIZER.deserialize(v) for k, v in data.items()}
 
     @classmethod
-    def fetch(cls, pk: str, sk: str = None, **kwargs: Dict[str, Any]) -> DynamojoModel:
+    async def fetch(
+        cls, pk: str, sk: str = None, **kwargs: Dict[str, Any]
+    ) -> DynamojoModel:
         """
         Returns a rehydrated object from the database
         """
 
-        key = {cls._config.indexes.table.partitionkey: pk}
+        key = {cls.__config__.indexes.table.partitionkey: pk}
 
-        if cls._config.indexes.table.sortkey:
-            key[cls._config.indexes.table.sortkey] = sk
+        if cls.__config__.indexes.table.sortkey:
+            key[cls.__config__.indexes.table.sortkey] = sk
 
         serialized_key = {k: TYPE_SERIALIZER.serialize(v) for k, v in key.items()}
 
-        opts = {"Key": serialized_key, "TableName": cls._config.table, **kwargs}
+        opts = {"Key": serialized_key, "TableName": cls.__config__.table, **kwargs}
 
         res = DYNAMOCLIENT.get_item(**opts)
 
         if item := res.get("Item"):
             return cls._construct_from_db(item)
 
     @classmethod
     def get_index_by_name(cls, name: str) -> Index:
         """
         Accepts a string as a name and returns an Index() object
         """
         try:
-            return cls._config.indexes[name]
+            return cls.__config__.indexes[name]
         except KeyError:
             raise IndexNotFoundError(f"Index {name} does not exist")
 
     def index_attributes(self) -> Dict[str, Any]:
         """
         Returns a dict containing index attributes as keys along with their set values
         """
         indexes = {}
-        for mapping in self._config.index_maps:
+        for mapping in self.__config__.index_maps:
             if hasattr(mapping, "partitionkey"):
                 indexes[mapping.index.partitionkey] = self.__getattribute__(
                     mapping.partitionkey
                 )
             if hasattr(mapping, "sortkey"):
                 indexes[mapping.index.sortkey] = self.__getattribute__(mapping.sortkey)
         return indexes
 
     def item(self) -> Dict[str, Any]:
         """
         Returns a dict that contains declared attributes and attributes dynamically generated
-        by self._config.joined_attributes
+        by self.__config__.joined_attributes
         """
-        return {**self.dict(), **self.joined_attributes()}
+        return {**self.model_dump(), **self.joined_attributes()}
 
     def joined_attributes(self) -> Dict[str, str]:
         """
-        Returns a dict of attributes created dynamically by self._config.joined_attributes
+        Returns a dict of attributes created dynamically by self.__config__.joined_attributes
         """
         return {
-            attr: self.__getattribute__(attr) for attr in self._config.__joined_attributes__
+            attr: self.__getattribute__(attr)
+            for attr in self.__config__.__joined_attributes__
         }
 
     @classmethod
     def _mutate_attribute(cls, field: str, val: Any) -> Any:
         """
-        Returns the mutated value using the callable specified in cls._config.mutators for
+        Returns the mutated value using the callable specified in cls.__config__.mutators for
         an attribute.
         """
         return super().__setattr__(
-            field, cls._config.mutators[field].callable(field, val, cls)
+            field, cls.__config__.mutators[field].callable(field, val, cls)
         )
 
     def _prepare_db_item(self):
         """
         Serializes self.item() for storage in the database using the low-level dynamodb client.
         """
-        item = {
-            k: TYPE_SERIALIZER.serialize(v)
-            for k, v in self._db_item().items()
-        }
+        item = {k: TYPE_SERIALIZER.serialize(v) for k, v in self._db_item().items()}
 
-        if not self._config.store_aliases:
-            for alias in self._config.__index_aliases__.values():
+        if not self.__config__.store_aliases:
+            for alias in self.__config__._index_aliases.values():
                 if alias in item:
                     del item[alias]
 
-        return  item
+        return item
 
     @classmethod
-    def query(
+    async def query(
         cls,
         KeyConditionExpression: ConditionBase,
         Index: Union[Index, str] = None,
         FilterExpression: AttributeBase = None,
         Limit: int = 1000,
         ExclusiveStartKey: dict = None,
         result_type: str = "standard",
@@ -408,15 +414,17 @@
     ) -> QueryResults:
         """
         Runs a Dynamodb query using a condition from db.Index. The kwargs argument can be any
         boto3.client("dynamodb").query() argument that is not explicitely defined in the signature.
         """
 
         if result_type not in ("standard", "deserialized", "raw"):
-            raise ValueError("Argument 'result_type' must be one of standard, raw, or deserialized")
+            raise ValueError(
+                "Argument 'result_type' must be one of standard, raw, or deserialized"
+            )
 
         opts = {**kwargs, "Limit": Limit}
 
         opts.update(
             cls._get_raw_condition_expression(exp=KeyConditionExpression, index=Index)
         )
 
@@ -440,105 +448,113 @@
             if opts.get("IndexName")
             else "Querying with table index"
         )
 
         getLogger().info(msg)
 
         res = DYNAMOCLIENT.query(**opts)
-        
+
         res["Items"] = [cls._construct_from_db(item) for item in res["Items"]]
         return QueryResults(**res)
 
-    def save(
-        self, ConditionExpression: ConditionBase = None, fail_on_exists: bool = True, **kwargs: Dict[str, Any]
+    async def save(
+        self,
+        ConditionExpression: ConditionBase = None,
+        fail_on_exists: bool = True,
+        **kwargs: Dict[str, Any],
     ) -> None:
         """
         Stores our item in Dynamodb
         """
 
-        table_pk = self._config.indexes.table.partitionkey
-        table_sk = self._config.indexes.table.sortkey
-
+        table_pk = self.__config__.indexes.table.partitionkey
+        table_sk = self.__config__.indexes.table.sortkey
 
         item = self._prepare_db_item()
 
-        opts = {"TableName": self._config.table, "Item": item, **kwargs}
+        opts = {"TableName": self.__config__.table, "Item": item, **kwargs}
 
         if ConditionExpression:
             exp = self._get_raw_condition_expression(
                 ConditionExpression, expression_type="ConditionExpression"
             )
             opts.update(exp)
 
         if fail_on_exists:
             sk_expression = f"attribute_not_exists({table_sk})"
             pk_expression = f"attribute_not_exists({table_pk})"
-            fail_expression = f"({pk_expression} AND {sk_expression}) " if table_sk is not None else pk_expression
+            fail_expression = (
+                f"({pk_expression} AND {sk_expression}) "
+                if table_sk is not None
+                else pk_expression
+            )
             if ConditionExpression:
-                opts["ConditionExpression"] = f"{fail_expression} AND {opts['ConditionExpression']}"
+                opts[
+                    "ConditionExpression"
+                ] = f"{fail_expression} AND {opts['ConditionExpression']}"
             else:
                 opts["ConditionExpression"] = fail_expression
 
         return DYNAMOCLIENT.put_item(**opts)
 
-    def update(self, **opts):
+    async def update(self, **opts):
         diff = self._deepdiff
 
         if not diff.hasChanged:
             return None
 
-        pk_name = self._config.indexes.table.partitionkey
-        sk_name = self._config.indexes.table.sortkey
-        if (
-            pk_name in diff.keys
-            or sk_name in diff.keys
-        ):
-            raise AttributeError("Cannot update table key attributes. Use `self.save()` instead.")
+        pk_name = self.__config__.indexes.table.partitionkey
+        sk_name = self.__config__.indexes.table.sortkey
+        if pk_name in diff.keys or sk_name in diff.keys:
+            raise AttributeError(
+                "Cannot update table key attributes. Use `self.save()` instead."
+            )
 
         attribute_names = {}
         attribute_values = {}
         set_statement_items = []
         del_statement_items = []
         set_items = {**diff.added, **diff.changed}
-        key = {
-            pk_name: TYPE_SERIALIZER.serialize(self._db_item()[pk_name])
-        }
+        key = {pk_name: TYPE_SERIALIZER.serialize(self._db_item()[pk_name])}
         if sk_name is not None:
             key[sk_name] = TYPE_SERIALIZER.serialize(self._db_item()[sk_name])
 
         for attr, val in self._db_item().items():
             if attr in diff.keys:
                 attribute_names[f"#{attr}"] = attr
                 attribute_values[f":{attr}"] = val
                 if attr in set_items.keys():
                     statement = f"#{attr} = :{attr}"
                     set_statement_items.append(statement)
                 else:
                     del_statement_items.append(statement)
 
-        set_statement = f"SET {', '.join(set_statement_items)}" if set_statement_items else ""
-        del_statement = f"REMOVE {', '.join(del_statement_items)}" if del_statement_items else ""
+        set_statement = (
+            f"SET {', '.join(set_statement_items)}" if set_statement_items else ""
+        )
+        del_statement = (
+            f"REMOVE {', '.join(del_statement_items)}" if del_statement_items else ""
+        )
 
-        opts["TableName"] = self._config.table
+        opts["TableName"] = self.__config__.table
         opts["Key"] = key
         opts["ExpressionAttributeNames"] = attribute_names
         opts["ExpressionAttributeValues"] = {
-            k: TYPE_SERIALIZER.serialize(v)
-            for k, v in attribute_values.items()
+            k: TYPE_SERIALIZER.serialize(v) for k, v in attribute_values.items()
         }
 
         opts["UpdateExpression"] = f"{set_statement} {del_statement}"
         DYNAMOCLIENT.update_item(**opts)
         return self
 
+
 @dataclass
 class QueryResults(UserDict):
     Items: List[DynamojoModel]
     Count: int
     ResponseMetadata: Dict[str, Any]
     ScannedCount: int
     LastEvaluatedKey: Dict[str, Dict[str, Any]] = None
     ConsumedCapacity: Dict[str, Any] = None
 
 
 DynamojoModel = TypeVar("DynamojoModel", bound=DynamojoBase)
-
```

### Comparing `dynamojo-0.2.2/dynamojo/config.py` & `dynamojo-1.0.0/dynamojo/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 from typing import Union, Callable, List, Dict
 
 from pydantic import BaseModel, PrivateAttr
 
 from .index import IndexList, IndexMap, Mutator
 
+
 class JoinedAttribute(BaseModel):
     attribute: str
     fields: List[str]
     separator: str = "~"
 
 
 class DynamojoConfig(BaseModel):
@@ -32,34 +33,31 @@
 
     mutators: List[Mutator] = []
 
     # If set to False then attributes that are aliases of indexes will be stripped
     # out before storing in the db
     store_aliases: bool = True
 
-    underscore_attrs_are_private: bool = True
-
     # Dict of `index key: alias name`
-    __index_aliases__: dict = PrivateAttr(default={})
+    _index_aliases: dict = PrivateAttr(default={})
 
-    __index_keys__: List[str] = PrivateAttr(default={})
+    _index_keys: List[str] = PrivateAttr(default={})
 
     class Config:
-        underscore_attrs_are_private: bool = True
         arbitrary_types_allowed = True
         extra = "allow"
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
         for attr in self.joined_attributes:
             self.__joined_attributes__[attr.attribute] = attr
 
         for index_map in self.index_maps:
             if sk_att := index_map.sortkey:
-                self.__index_aliases__[index_map.index.sortkey] = sk_att
+                self._index_aliases[index_map.index.sortkey] = sk_att
             if getattr(index_map, "partitionkey", None):
-                self.__index_aliases__[
+                self._index_aliases[
                     index_map.index.partitionkey
                 ] = index_map.partitionkey
 
-        self.__index_keys__ = list(set(self.__index_aliases__.keys()))
+        self._index_keys = list(set(self._index_aliases.keys()))
```

### Comparing `dynamojo-0.2.2/dynamojo/index.py` & `dynamojo-1.0.0/dynamojo/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     def __init__(
         self,
         *,
         name: str,
         sortkey: str,
         partitionkey: str = None,
     ) -> None:
-
         self.__partitionkey = partitionkey if partitionkey else None
         self.__sortkey = sortkey if sortkey else None
         self.__name = name
         self.is_composite = partitionkey and sortkey
 
     @property
     def partitionkey(self) -> str:
@@ -84,15 +83,14 @@
                 has_table = True
 
             super().__setattr__(index.name, index)
             self.data[index.name] = index
 
 
 def get_indexes(table_name: str) -> IndexList:
-
     desc = DYNAMOCLIENT.describe_table(TableName=table_name)["Table"]
     gsi_list = desc.get("GlobalSecondaryIndexes", [])
     lsi_list = desc.get("LocalSecondaryIndexes", [])
 
     table_list = [{"IndexName": "table", "KeySchema": desc["KeySchema"]}]
 
     def build_indexes(index_type, index_list):
```

### Comparing `dynamojo-0.2.2/dynamojo/utils.py` & `dynamojo-1.0.0/dynamojo/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,87 +1,81 @@
 #!/usr/bin/env python3
 from pydantic import BaseModel, PrivateAttr
-from typing import (
-  TYPE_CHECKING,
-  Any,
-  Dict,
-  NamedTuple
-)
+from typing import TYPE_CHECKING, Any, Dict, NamedTuple
 
 
 if TYPE_CHECKING:
-  from .base import DynamojoBase
+    from .base import DynamojoBase
 else:
-  DynamojoBase = object
+    DynamojoBase = object
 
 from boto3.dynamodb.types import TypeSerializer, TypeDeserializer
 
 
 TYPE_SERIALIZER = TypeSerializer()
 TYPE_DESERIALIZER = TypeDeserializer()
 
 Change = NamedTuple("Change", [("old", Any), ("new", Any)])
-Diff = NamedTuple("Diff", (("added", Dict[str, Any]), ("removed", Dict[str, Any]), ("changed", Dict[str, Any])))
+Diff = NamedTuple(
+    "Diff",
+    (
+        ("added", Dict[str, Any]),
+        ("removed", Dict[str, Any]),
+        ("changed", Dict[str, Any]),
+    ),
+)
 
 
 class Delta(BaseModel):
-  old: DynamojoBase = None
-  new: DynamojoBase = None
+    old: DynamojoBase = None
+    new: DynamojoBase = None
 
-  _deep: bool = PrivateAttr()
-  _old: Dict[str, Any] = PrivateAttr()
-  _new: Dict[str, Any] = PrivateAttr()  
-
-  def __init__(self, deep=True, **kwargs):
-    self._deep = deep
-    super().__init__(**kwargs)
-
-    if deep:
-      self._old = self.old._db_item()
-      self._new = self.new._db_item()
-    else:
-      self._old = self.old.item()
-      self._new = self.new.item()
-
-
-  @property
-  def delta(self) -> Diff:
-    diff = Diff({}, {}, {})
-
-    for key, val in self._old.items():
-        if key not in self._new:
-          diff.removed[key] = val
-        if key in self._new and val != self._new[key]:
-          diff.changed[key] = Change(
-            self._old[key],
-            self._new[key]
-          )
-
-    for key, val in self._new.items():
-        if key not in self._old:
-          diff.added[key] = val
-
-    return diff
-
-  @property
-  def added(self) -> Dict[str, Any]:
-    return self.delta.added
-  
-  @property
-  def changed(self) -> Change:
-    return self.delta.changed
-
-  @property
-  def removed(self) -> Dict[str, Any]:
-    return self.delta.removed 
-
-  @property
-  def hasChanged(self):
-      return not self._old == self._new
-
-  @property
-  def keys(self):
-    return {
-      **self.added,
-      **self.removed,
-      **self.changed
-    }.keys()
+    _deep: bool = PrivateAttr()
+    _old: Dict[str, Any] = PrivateAttr()
+    _new: Dict[str, Any] = PrivateAttr()
+
+    def __init__(self, deep=True, **kwargs):
+        self._deep = deep
+        super().__init__(**kwargs)
+
+        if deep:
+            self._old = self.old._db_item()
+            self._new = self.new._db_item()
+        else:
+            self._old = self.old.item()
+            self._new = self.new.item()
+
+    @property
+    def delta(self) -> Diff:
+        diff = Diff({}, {}, {})
+
+        for key, val in self._old.items():
+            if key not in self._new:
+                diff.removed[key] = val
+            if key in self._new and val != self._new[key]:
+                diff.changed[key] = Change(self._old[key], self._new[key])
+
+        for key, val in self._new.items():
+            if key not in self._old:
+                diff.added[key] = val
+
+        return diff
+
+    @property
+    def added(self) -> Dict[str, Any]:
+        return self.delta.added
+
+    @property
+    def changed(self) -> Change:
+        return self.delta.changed
+
+    @property
+    def removed(self) -> Dict[str, Any]:
+        return self.delta.removed
+
+    @property
+    def hasChanged(self):
+        return not self._old == self._new
+
+    @property
+    def keys(self):
+        return {**self.added, **self.removed, **self.changed}.keys()
```

### Comparing `dynamojo-0.2.2/pyproject.toml` & `dynamojo-1.0.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "Dynamojo"
-version = "0.2.2"
+version = "1.0.0"
 description = "ORM For dynamodb"
 authors = ["Mathew Moon <me@mathewmoon.net>"]
 homepage = "https://github.com/mathewmoon/dynamojo"
 repository = "https://github.com/mathewmoon/dynamojo"
 
 readme = "README.md"
 packages = [{include = "dynamojo", from = "."}]
 
 [tool.poetry.dependencies]
 python = "^3.12"
 boto3 = "^1.34.56"
-pydantic = "^1.10.0"
+pydantic = "^2.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "7.4.3"
 boto3-stubs = {extras = ["dynamodb"], version = "^1.34.58"}
 
 [tool.pytest.ini_options]
 xfail_strict = true
```

### Comparing `dynamojo-0.2.2/PKG-INFO` & `dynamojo-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: Dynamojo
-Version: 0.2.2
+Version: 1.0.0
 Summary: ORM For dynamodb
 Home-page: https://github.com/mathewmoon/dynamojo
 Author: Mathew Moon
 Author-email: me@mathewmoon.net
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3 (>=1.34.56,<2.0.0)
-Requires-Dist: pydantic (>=1.10.0,<2.0.0)
+Requires-Dist: pydantic (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/mathewmoon/dynamojo
 Description-Content-Type: text/markdown
 
 # Dynamojo
 ## Because one table is better than more
 
 Dynamojo takes the concept of Dynamodb Single Table design and creates a modeling framework for it. This library is opinionated in the following ways:
```

