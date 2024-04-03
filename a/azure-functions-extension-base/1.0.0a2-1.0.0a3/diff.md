# Comparing `tmp/azure-functions-extension-base-1.0.0a2.tar.gz` & `tmp/azure-functions-extension-base-1.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-functions-extension-base-1.0.0a2.tar", last modified: Tue Mar 19 19:46:39 2024, max compression
+gzip compressed data, was "azure-functions-extension-base-1.0.0a3.tar", last modified: Wed Apr  3 21:22:45 2024, max compression
```

## Comparing `azure-functions-extension-base-1.0.0a2.tar` & `azure-functions-extension-base-1.0.0a3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 19:46:39.250435 azure-functions-extension-base-1.0.0a2/
--rw-rw-rw-   0        0        0     1093 2024-02-16 17:53:52.000000 azure-functions-extension-base-1.0.0a2/LICENSE
--rw-rw-rw-   0        0        0       91 2024-02-16 17:54:57.000000 azure-functions-extension-base-1.0.0a2/MANIFEST.in
--rw-rw-rw-   0        0        0      910 2024-03-19 19:46:39.250435 azure-functions-extension-base-1.0.0a2/PKG-INFO
--rw-rw-rw-   0        0        0      253 2024-03-19 15:28:23.000000 azure-functions-extension-base-1.0.0a2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-19 19:46:39.190305 azure-functions-extension-base-1.0.0a2/azure/
--rw-rw-rw-   0        0        0       66 2024-02-16 19:41:40.000000 azure-functions-extension-base-1.0.0a2/azure/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 19:46:39.192313 azure-functions-extension-base-1.0.0a2/azure/functions/
--rw-rw-rw-   0        0        0       66 2024-02-16 19:41:43.000000 azure-functions-extension-base-1.0.0a2/azure/functions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 19:46:39.193721 azure-functions-extension-base-1.0.0a2/azure/functions/extension/
--rw-rw-rw-   0        0        0       66 2024-02-16 19:41:46.000000 azure-functions-extension-base-1.0.0a2/azure/functions/extension/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 19:46:39.200230 azure-functions-extension-base-1.0.0a2/azure/functions/extension/base/
--rw-rw-rw-   0        0        0      838 2024-03-19 19:30:42.000000 azure-functions-extension-base-1.0.0a2/azure/functions/extension/base/__init__.py
--rw-rw-rw-   0        0        0     5959 2024-03-19 19:30:42.000000 azure-functions-extension-base-1.0.0a2/azure/functions/extension/base/meta.py
--rw-rw-rw-   0        0        0      294 2024-03-19 19:33:07.000000 azure-functions-extension-base-1.0.0a2/azure/functions/extension/base/sdkType.py
--rw-rw-rw-   0        0        0     8549 2024-02-16 19:41:52.000000 azure-functions-extension-base-1.0.0a2/azure/functions/extension/base/utils.py
--rw-rw-rw-   0        0        0     4129 2024-03-19 19:30:37.000000 azure-functions-extension-base-1.0.0a2/azure/functions/extension/base/web.py
-drwxrwxrwx   0        0        0        0 2024-03-19 19:46:39.240438 azure-functions-extension-base-1.0.0a2/azure_functions_extension_base.egg-info/
--rw-rw-rw-   0        0        0      910 2024-03-19 19:46:38.000000 azure-functions-extension-base-1.0.0a2/azure_functions_extension_base.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      695 2024-03-19 19:46:38.000000 azure-functions-extension-base-1.0.0a2/azure_functions_extension_base.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 19:46:38.000000 azure-functions-extension-base-1.0.0a2/azure_functions_extension_base.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      106 2024-03-19 19:46:38.000000 azure-functions-extension-base-1.0.0a2/azure_functions_extension_base.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-19 19:46:38.000000 azure-functions-extension-base-1.0.0a2/azure_functions_extension_base.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-19 19:46:39.250435 azure-functions-extension-base-1.0.0a2/setup.cfg
--rw-rw-rw-   0        0        0     1456 2024-03-19 19:31:23.000000 azure-functions-extension-base-1.0.0a2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-19 19:46:39.250435 azure-functions-extension-base-1.0.0a2/tests/
--rw-rw-rw-   0        0        0      529 2024-02-15 18:51:16.000000 azure-functions-extension-base-1.0.0a2/tests/__init__.py
--rw-rw-rw-   0        0        0     1065 2024-02-15 18:51:16.000000 azure-functions-extension-base-1.0.0a2/tests/test_code_quality.py
--rw-rw-rw-   0        0        0     4316 2024-02-15 18:51:16.000000 azure-functions-extension-base-1.0.0a2/tests/test_meta.py
--rw-rw-rw-   0        0        0     3451 2024-02-15 18:51:16.000000 azure-functions-extension-base-1.0.0a2/tests/test_utils.py
--rw-rw-rw-   0        0        0     9370 2024-03-19 15:28:23.000000 azure-functions-extension-base-1.0.0a2/tests/test_web.py
+drwxrwxrwx   0        0        0        0 2024-04-03 21:22:45.810519 azure-functions-extension-base-1.0.0a3/
+-rw-rw-rw-   0        0        0     1093 2024-02-28 16:15:11.000000 azure-functions-extension-base-1.0.0a3/LICENSE
+-rw-rw-rw-   0        0        0       91 2024-02-28 16:15:11.000000 azure-functions-extension-base-1.0.0a3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1497 2024-04-03 21:22:45.809978 azure-functions-extension-base-1.0.0a3/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2024-03-27 18:57:52.000000 azure-functions-extension-base-1.0.0a3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 21:22:45.730142 azure-functions-extension-base-1.0.0a3/azure/
+-rw-rw-rw-   0        0        0       66 2024-02-28 16:15:11.000000 azure-functions-extension-base-1.0.0a3/azure/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 21:22:45.733725 azure-functions-extension-base-1.0.0a3/azure/functions/
+-rw-rw-rw-   0        0        0       66 2024-02-28 16:15:11.000000 azure-functions-extension-base-1.0.0a3/azure/functions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 21:22:45.740087 azure-functions-extension-base-1.0.0a3/azure/functions/extension/
+-rw-rw-rw-   0        0        0       66 2024-02-28 16:15:11.000000 azure-functions-extension-base-1.0.0a3/azure/functions/extension/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 21:22:45.754522 azure-functions-extension-base-1.0.0a3/azure/functions/extension/base/
+-rw-rw-rw-   0        0        0      856 2024-04-03 21:21:27.000000 azure-functions-extension-base-1.0.0a3/azure/functions/extension/base/__init__.py
+-rw-rw-rw-   0        0        0     5773 2024-04-03 21:21:10.000000 azure-functions-extension-base-1.0.0a3/azure/functions/extension/base/meta.py
+-rw-rw-rw-   0        0        0      296 2024-03-27 18:57:52.000000 azure-functions-extension-base-1.0.0a3/azure/functions/extension/base/sdkType.py
+-rw-rw-rw-   0        0        0     8534 2024-04-03 21:21:10.000000 azure-functions-extension-base-1.0.0a3/azure/functions/extension/base/utils.py
+-rw-rw-rw-   0        0        0     5071 2024-04-03 21:21:10.000000 azure-functions-extension-base-1.0.0a3/azure/functions/extension/base/web.py
+drwxrwxrwx   0        0        0        0 2024-04-03 21:22:45.808060 azure-functions-extension-base-1.0.0a3/azure_functions_extension_base.egg-info/
+-rw-rw-rw-   0        0        0     1497 2024-04-03 21:22:45.000000 azure-functions-extension-base-1.0.0a3/azure_functions_extension_base.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2024-04-03 21:22:45.000000 azure-functions-extension-base-1.0.0a3/azure_functions_extension_base.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 21:22:45.000000 azure-functions-extension-base-1.0.0a3/azure_functions_extension_base.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-03 21:22:45.000000 azure-functions-extension-base-1.0.0a3/azure_functions_extension_base.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-03 21:22:45.000000 azure-functions-extension-base-1.0.0a3/azure_functions_extension_base.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1405 2024-03-27 14:46:39.000000 azure-functions-extension-base-1.0.0a3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 21:22:45.810519 azure-functions-extension-base-1.0.0a3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 21:22:45.804896 azure-functions-extension-base-1.0.0a3/tests/
+-rw-rw-rw-   0        0        0      519 2024-04-03 21:21:10.000000 azure-functions-extension-base-1.0.0a3/tests/__init__.py
+-rw-rw-rw-   0        0        0    11521 2024-04-03 21:21:10.000000 azure-functions-extension-base-1.0.0a3/tests/test_meta.py
+-rw-rw-rw-   0        0        0      656 2024-04-03 21:21:10.000000 azure-functions-extension-base-1.0.0a3/tests/test_sdk_type.py
+-rw-rw-rw-   0        0        0    11042 2024-04-03 21:21:10.000000 azure-functions-extension-base-1.0.0a3/tests/test_utils.py
+-rw-rw-rw-   0        0        0    15462 2024-04-03 21:21:10.000000 azure-functions-extension-base-1.0.0a3/tests/test_web.py
```

### Comparing `azure-functions-extension-base-1.0.0a2/LICENSE` & `azure-functions-extension-base-1.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-functions-extension-base-1.0.0a2/azure/functions/extension/base/meta.py` & `azure-functions-extension-base-1.0.0a3/azure/functions/extension/base/meta.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 
 import abc
 import inspect
 import json
+from typing import Any, Dict, List, Mapping, Optional, Tuple, Union
 
-from . import utils
-from . import sdkType
-
-from typing import Any, Dict, List, Optional, Mapping, Union, Tuple
+from . import sdkType, utils
 
 
 class Datum:
     def __init__(self, value: Any, type: Optional[str]):
         self.value: Any = value
         self.type: Optional[str] = type
 
     @property
     def python_value(self) -> Any:
         if self.value is None or self.type is None:
             return None
-        elif self.type in ('bytes', 'string', 'int', 'double'):
+        elif self.type in ("bytes", "string", "int", "double"):
             return self.value
-        elif self.type == 'json':
+        elif self.type == "json":
             return json.loads(self.value)
-        elif self.type == 'collection_string':
+        elif self.type == "collection_string":
             return [v for v in self.value.string]
-        elif self.type == 'collection_bytes':
+        elif self.type == "collection_bytes":
             return [v for v in self.value.bytes]
-        elif self.type == 'collection_double':
+        elif self.type == "collection_double":
             return [v for v in self.value.double]
-        elif self.type == 'collection_sint64':
+        elif self.type == "collection_sint64":
             return [v for v in self.value.sint64]
         else:
             return self.value
 
     @property
     def python_type(self) -> type:
         return type(self.python_value)
@@ -47,35 +45,36 @@
 
     def __hash__(self):
         return hash((type(self), (self.value, self.type)))
 
     def __repr__(self):
         val_repr = repr(self.value)
         if len(val_repr) > 10:
-            val_repr = val_repr[:10] + '...'
-        return '<Datum {} {}>'.format(self.type, val_repr)
+            val_repr = val_repr[:10] + "..."
+        return "<Datum {} {}>".format(self.type, val_repr)
 
 
 class _ConverterMeta(abc.ABCMeta):
 
     _bindings: Dict[str, type] = {}
 
-    def __new__(mcls, name, bases, dct, *,
-                binding: Optional[str],
-                trigger: Optional[str] = None):
+    def __new__(
+        mcls, name, bases, dct, *, binding: Optional[str], trigger: Optional[str] = None
+    ):
         cls = super().__new__(mcls, name, bases, dct)
         cls._trigger = trigger  # type: ignore
         if binding is None:
             return cls
 
         if binding in mcls._bindings:
             raise RuntimeError(
-                f'cannot register a converter for {binding!r} binding: '
-                f'another converter for this binding has already been '
-                f'registered')
+                f"cannot register a converter for {binding!r} binding: "
+                f"another converter for this binding has already been "
+                f"registered"
+            )
 
         mcls._bindings[binding] = cls
         if trigger is not None:
             mcls._bindings[trigger] = cls
 
         return cls
 
@@ -97,59 +96,67 @@
         return cls._trigger is not None  # type: ignore
 
 
 class _BaseConverter(metaclass=_ConverterMeta, binding=None):
 
     @classmethod
     def _decode_typed_data(
-            cls, data: Datum, *,
-            python_type: Union[type, Tuple[type, ...]],
-            context: str = 'data') -> Any:
+        cls,
+        data: Datum,
+        *,
+        python_type: Union[type, Tuple[type, ...]],
+        context: str = "data",
+    ) -> Any:
         if data is None:
             return None
 
         data_type = data.type
-        if data_type == 'model_binding_data':
+        if data_type == "model_binding_data":
             result = data.value
         elif data_type is None:
             return None
         else:
-            raise ValueError(
-                f'unsupported type of {context}: {data_type}')
+            raise ValueError(f"unsupported type of {context}: {data_type}")
 
         if not isinstance(result, python_type):
             if isinstance(python_type, (tuple, list, dict)):
                 raise ValueError(
-                    f'unexpected value type in {context}: '
-                    f'{type(result).__name__}, expected one of: '
-                    f'{", ".join(t.__name__ for t in python_type)}')
+                    f"unexpected value type in {context}: "
+                    f"{type(result).__name__}, expected one of: "
+                    f'{", ".join(t.__name__ for t in python_type)}'
+                )
             else:
                 try:
                     # Try coercing into the requested type
                     result = python_type(result)
                 except (TypeError, ValueError) as e:
                     raise ValueError(
-                        f'cannot convert value of {context} into '
-                        f'{python_type.__name__}: {e}') from None
+                        f"cannot convert value of {context} into "
+                        f"{python_type.__name__}: {e}"
+                    ) from None
 
         return result
 
     @classmethod
     def _decode_trigger_metadata_field(
-            cls, trigger_metadata: Mapping[str, Datum],
-            field: str, *,
-            python_type: Union[type, Tuple[type, ...]]) \
-            -> Any:
+        cls,
+        trigger_metadata: Mapping[str, Datum],
+        field: str,
+        *,
+        python_type: Union[type, Tuple[type, ...]],
+    ) -> Any:
         data = trigger_metadata.get(field)
         if data is None:
             return None
         else:
             return cls._decode_typed_data(
-                data, python_type=python_type,
-                context=f'field {field!r} in trigger metadata')
+                data,
+                python_type=python_type,
+                context=f"field {field!r} in trigger metadata",
+            )
 
 
 class InConverter(_BaseConverter, binding=None):
 
     @classmethod
     @abc.abstractmethod
     def check_input_type_annotation(cls, pytype: type) -> bool:
@@ -171,19 +178,13 @@
     @classmethod
     @abc.abstractmethod
     def check_output_type_annotation(cls, pytype: type) -> bool:
         pass
 
     @classmethod
     @abc.abstractmethod
-    def encode(cls, obj: Any, *,
-               expected_type: Optional[type]) -> Optional[Datum]:
+    def encode(cls, obj: Any, *, expected_type: Optional[type]) -> Optional[Datum]:
         raise NotImplementedError
 
 
 def get_binding_registry():
     return _ConverterMeta
-
-
-def check_deferred_bindings_enabled(cls, sdk_binding_registry: _ConverterMeta, pytype: type) -> bool:
-    return (sdk_binding_registry is not None
-            and _ConverterMeta.check_supported_type(pytype))
```

### Comparing `azure-functions-extension-base-1.0.0a2/azure/functions/extension/base/utils.py` & `azure-functions-extension-base-1.0.0a3/azure/functions/extension/base/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 
 import inspect
 import json
 import re
-
 from abc import ABC
 from enum import Enum
 from typing import Any, Callable, Dict, List, Optional
 
 from . import meta
 
-SNAKE_CASE_RE = re.compile(r'^([a-zA-Z]+\d*_|_+[a-zA-Z\d])\w*$')
-WORD_RE = re.compile(r'^([a-zA-Z]+\d*)$')
+SNAKE_CASE_RE = re.compile(r"^([a-zA-Z]+\d*_|_+[a-zA-Z\d])\w*$")
+WORD_RE = re.compile(r"^([a-zA-Z]+\d*)$")
 
 
 class StringifyEnum(Enum):
     """This class output name of enum object when printed as string."""
 
     def __str__(self):
         return str(self.name)
@@ -34,18 +33,16 @@
         every binding class to collect list of params to include in building
         json dictionary which corresponds to function.json in legacy app.
         It will also apply :meth:`skip_none` to :meth:`get_dict_repr` to
         enable json dictionary generated for every binding has non-empty
         value fields. It is needed for enabling binding param optionality.
         """
         cls = super().__new__(mcs, name, bases, dct)
-        setattr(cls, '__init__',
-                cls.add_to_dict(getattr(cls, '__init__')))
-        setattr(cls, 'get_dict_repr',
-                cls.skip_none(getattr(cls, 'get_dict_repr')))
+        setattr(cls, "__init__", cls.add_to_dict(getattr(cls, "__init__")))
+        setattr(cls, "get_dict_repr", cls.skip_none(getattr(cls, "get_dict_repr")))
         return cls
 
     @staticmethod
     def skip_none(func):
         def wrapper(*args, **kw):
             res = func(*args, **kw)
             return BuildDictMeta.clean_nones(res)
@@ -53,64 +50,66 @@
         return wrapper
 
     @staticmethod
     def add_to_dict(func: Callable[..., Any]):
         def wrapper(*args, **kwargs):
             if args is None or len(args) == 0:
                 raise ValueError(
-                    f'{func.__name__} has no args. Please ensure func is an '
-                    f'object method.')
+                    f"{func.__name__} has no args. Please ensure func is an "
+                    f"object method."
+                )
 
             func(*args, **kwargs)
 
             self = args[0]
 
             init_params = list(inspect.signature(func).parameters.keys())
             init_params.extend(list(kwargs.keys()))
             for key in kwargs.keys():
                 if not hasattr(self, key):
                     setattr(self, key, kwargs[key])
 
-            setattr(self, 'init_params', init_params)
+            setattr(self, "init_params", init_params)
 
         return wrapper
 
     @staticmethod
     def clean_nones(value):
         """
         Recursively remove all None values from dictionaries and lists,
         and returns
         the result as a new dictionary or list.
         """
         if isinstance(value, list):
-            return [BuildDictMeta.clean_nones(x) for x in value if
-                    x is not None]
+            return [BuildDictMeta.clean_nones(x) for x in value if x is not None]
         elif isinstance(value, dict):
             return {
                 key: BuildDictMeta.clean_nones(val)
                 for key, val in value.items()
                 if val is not None
             }
         else:
             return value
 
 
 # Enums
 class BindingDirection(StringifyEnum):
     """Direction of the binding used in function.json"""
+
     IN = 0
     """Input binding direction."""
     OUT = 1
     """Output binding direction."""
     INOUT = 2
     """Some bindings support a special binding direction. """
 
 
 class DataType(StringifyEnum):
     """Data type of the binding used in function.json"""
+
     """Parse binding argument as undefined."""
     UNDEFINED = 0
     """Parse binding argument as string."""
     STRING = 1
     """Parse binding argument as binary."""
     BINARY = 2
     """Parse binding argument as stream."""
@@ -119,38 +118,42 @@
 
 class Binding(ABC):
     """Abstract binding class which captures common attributes and
     functions. :meth:`get_dict_repr` can auto generate the function.json for
     every binding, the only restriction is ***ENSURE*** __init__ parameter
     names of any binding class are snake case form of corresponding
     attribute in function.json when new binding classes are created.
-    Ref: https://aka.ms/azure-function-binding-http """
+    Ref: https://aka.ms/azure-function-binding-http"""
 
-    EXCLUDED_INIT_PARAMS = {'self', 'kwargs', 'type', 'data_type', 'direction'}
+    EXCLUDED_INIT_PARAMS = {"self", "kwargs", "type", "data_type", "direction"}
 
     @staticmethod
     def get_binding_name() -> str:
         pass
 
-    def __init__(self, name: str,
-                 direction: BindingDirection,
-                 data_type: Optional[DataType] = None,
-                 type: Optional[str] = None):  # NoQa
+    def __init__(
+        self,
+        name: str,
+        direction: BindingDirection,
+        data_type: Optional[DataType] = None,
+        type: Optional[str] = None,
+    ):  # NoQa
         # For natively supported bindings, get_binding_name is always
         # implemented, and for generic bindings, type is a required argument
         # in decorator functions.
-        self.type = self.get_binding_name() \
-            if self.get_binding_name() is not None else type
+        self.type = (
+            self.get_binding_name() if self.get_binding_name() is not None else type
+        )
         self.name = name
         self._direction = direction
         self._data_type = data_type
         self._dict = {
             "direction": self._direction,
             "dataType": self._data_type,
-            "type": self.type
+            "type": self.type,
         }
 
     @property
     def data_type(self) -> Optional[int]:
         return self._data_type.value if self._data_type else None
 
     @property
@@ -162,46 +165,49 @@
         cased binding field names defined in `init_params` list and
         :class:`Binding` class. \n
         This method is invoked in function :meth:`get_raw_bindings` of class
         :class:`Function` to generate json dict for each binding.
 
         :return: Dictionary representation of the binding.
         """
-        params = list(dict.fromkeys(getattr(binding, 'init_params', [])))
+        params = list(dict.fromkeys(getattr(binding, "init_params", [])))
         for p in params:
             if p not in Binding.EXCLUDED_INIT_PARAMS:
                 binding._dict[to_camel_case(p)] = getattr(binding, p, None)
 
         # Adding flag to signal to the host to send MBD object
         # 1. check if the binding is a supported type (blob, blobTrigger)
         # 2. check if the binding is an input binding
         # 3. check if the defined type is an SdkType
-        if (binding.type in meta._ConverterMeta._bindings
-                and binding.direction == 0
-                and meta._ConverterMeta.check_supported_type(
-                    input_types.get(binding.name).pytype)):
+        if (
+            binding.type in meta._ConverterMeta._bindings
+            and binding.direction == 0
+            and meta._ConverterMeta.check_supported_type(
+                input_types.get(binding.name).pytype
+            )
+        ):
             binding._dict["properties"] = {"SupportsDeferredBinding": True}
         # if it isn't, we set the flag to false
         else:
             binding._dict["properties"] = {"SupportsDeferredBinding": False}
 
         return binding._dict
 
 
 def to_camel_case(snake_case_str: str):
     if snake_case_str is None or len(snake_case_str) == 0:
-        raise ValueError(
-            f"Please ensure arg name {snake_case_str} is not empty!")
+        raise ValueError(f"Please ensure arg name {snake_case_str} is not empty!")
 
     if not is_snake_case(snake_case_str) and not is_word(snake_case_str):
         raise ValueError(
             f"Please ensure {snake_case_str} is a word or snake case "
-            f"string with underscore as separator.")
-    words = snake_case_str.split('_')
-    return words[0] + ''.join([ele.title() for ele in words[1:]])
+            f"string with underscore as separator."
+        )
+    words = snake_case_str.split("_")
+    return words[0] + "".join([ele.title() for ele in words[1:]])
 
 
 def is_snake_case(input_string: str) -> bool:
     """
     Checks if a string is formatted as "snake case".
     A string is considered snake case when:
     - it's composed only by lowercase/uppercase letters and digits
@@ -229,10 +235,11 @@
     :param input_string: String to test.
     :return: True for one word string, false otherwise.
     """
     return WORD_RE.match(input_string) is not None
 
 
 def get_raw_bindings(indexed_function, input_types) -> List[str]:
-    return [json.dumps(Binding.get_dict_repr(b, input_types),
-                       cls=StringifyEnumJsonEncoder)
-            for b in indexed_function._bindings]
+    return [
+        json.dumps(Binding.get_dict_repr(b, input_types), cls=StringifyEnumJsonEncoder)
+        for b in indexed_function._bindings
+    ]
```

### Comparing `azure-functions-extension-base-1.0.0a2/azure/functions/extension/base/web.py` & `azure-functions-extension-base-1.0.0a3/azure/functions/extension/base/web.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,84 +1,111 @@
+import abc
+import inspect
 from abc import abstractmethod
 from enum import Enum
-import inspect
 from typing import Callable
 
 base_extension_module = __name__
 
 
 # Base extension pkg
 class ModuleTrackerMeta(type):
     _module = None
 
     def __new__(cls, name, bases, dct, **kwargs):
         new_class = super().__new__(cls, name, bases, dct)
-        new_module = dct.get('__module__')
+        new_module = dct.get("__module__")
         if new_module != base_extension_module:
             if cls._module is None:
                 cls._module = new_module
             elif cls._module != new_module:
-                raise Exception(f'Only one web extension package shall be imported, '
-                                f'{cls._module} and {new_module} are imported')
+                raise Exception(
+                    f"Only one web extension package shall be imported, "
+                    f"{cls._module} and {new_module} are imported"
+                )
         return new_class
 
     @classmethod
     def get_module(cls):
         return cls._module
 
     @classmethod
     def module_imported(cls):
         return cls._module is not None
 
 
 class RequestTrackerMeta(type):
     _request_type = None
+    _synchronizer: None
 
     def __new__(cls, name, bases, dct, **kwargs):
         new_class = super().__new__(cls, name, bases, dct)
 
-        request_type = dct.get('request_type')
+        request_type = dct.get("request_type")
 
         if request_type is None:
-            raise Exception(f'Request type not provided for class {name}')
+            raise TypeError(f"Request type not provided for class {name}")
 
         if cls._request_type is not None and cls._request_type != request_type:
-            raise Exception(f'Only one request type shall be recorded for class {name} '
-                            f'but found {cls._request_type} and {request_type}')
+            raise TypeError(
+                f"Only one request type shall be recorded for class {name} "
+                f"but found {cls._request_type} and {request_type}"
+            )
         cls._request_type = request_type
+        cls._synchronizer = dct.get("synchronizer")
+
+        if cls._synchronizer is None:
+            raise TypeError(f"Request synchronizer not provided for class {name}")
 
         return new_class
 
     @classmethod
     def get_request_type(cls):
         return cls._request_type
 
     @classmethod
+    def get_synchronizer(cls):
+        return cls._synchronizer
+
+    @classmethod
     def check_type(cls, pytype: type) -> bool:
         if pytype is not None and inspect.isclass(pytype):
-            return cls._request_type is not None and issubclass(pytype, cls._request_type)
+            return cls._request_type is not None and issubclass(
+                pytype, cls._request_type
+            )
         return False
 
 
+class RequestSynchronizer(abc.ABC):
+    @abstractmethod
+    def sync_route_params(self, request, path_params):
+        raise NotImplementedError()
+
+
 class ResponseTrackerMeta(type):
     _response_types = {}
 
     def __new__(cls, name, bases, dct, **kwargs):
         new_class = super().__new__(cls, name, bases, dct)
 
-        label = dct.get('label')
-        response_type = dct.get('response_type')
+        label = dct.get("label")
+        response_type = dct.get("response_type")
 
         if label is None:
-            raise Exception(f'Response label not provided for class {name}')
+            raise TypeError(f"Response label not provided for class {name}")
         if response_type is None:
-            raise Exception(f'Response type not provided for class {name}')
-        if cls._response_types.get(label) is not None and cls._response_types.get(label) != response_type:
-            raise Exception(f'Only one response type shall be recorded for class {name} '
-                            f'but found {cls._response_types.get(label)} and {response_type}')
+            raise TypeError(f"Response type not provided for class {name}")
+        if (
+            cls._response_types.get(label) is not None
+            and cls._response_types.get(label) != response_type
+        ):
+            raise TypeError(
+                f"Only one response type shall be recorded for class {name} "
+                f"but found {cls._response_types.get(label)} and {response_type}"
+            )
 
         cls._response_types[label] = response_type
 
         return new_class
 
     @classmethod
     def get_standard_response_type(cls):
@@ -87,46 +114,62 @@
     @classmethod
     def get_response_type(cls, label):
         return cls._response_types.get(label)
 
     @classmethod
     def check_type(cls, pytype: type) -> bool:
         if pytype is not None and inspect.isclass(pytype):
-            return cls._response_types is not None and any(issubclass(pytype, response_type)
-                                                            for response_type in cls._response_types.values())
+            return cls._response_types is not None and any(
+                issubclass(pytype, response_type)
+                for response_type in cls._response_types.values()
+            )
         return False
 
-class WebApp(metaclass=ModuleTrackerMeta):
+
+class ABCModuleTrackerMeta(abc.ABCMeta, ModuleTrackerMeta):
+    pass
+
+
+class WebApp(metaclass=ABCModuleTrackerMeta):
     @abstractmethod
     def route(self, func: Callable):
-        pass
+        raise NotImplementedError()
 
     @abstractmethod
     def get_app(self):
-        pass
+        raise NotImplementedError()
 
 
-class WebServer(metaclass=ModuleTrackerMeta):
+class WebServer(metaclass=ABCModuleTrackerMeta):
     def __init__(self, hostname, port, web_app: WebApp):
         self.hostname = hostname
         self.port = port
         self.web_app = web_app.get_app()
 
     @abstractmethod
     async def serve(self):
-        pass
+        raise NotImplementedError()  # pragma: no cover
 
 
-def http_v2_enabled() -> bool:
-    return ModuleTrackerMeta.module_imported()
+class HttpV2FeatureChecker:
+    @staticmethod
+    def http_v2_enabled():
+        return ModuleTrackerMeta.module_imported()
 
 
 class ResponseLabels(Enum):
-    STANDARD = 'standard'
-    STREAMING = 'streaming'
-    FILE = 'file'
-    HTML = 'html'
-    JSON = 'json'
-    ORJSON = 'orjson'
-    PLAIN_TEXT = 'plain_text'
-    REDIRECT = 'redirect'
-    UJSON = 'ujson'
+    STANDARD = "standard"
+    STREAMING = "streaming"
+    FILE = "file"
+    HTML = "html"
+    JSON = "json"
+    ORJSON = "orjson"
+    PLAIN_TEXT = "plain_text"
+    REDIRECT = "redirect"
+    UJSON = "ujson"
+    INT = "int"
+    FLOAT = "float"
+    STR = "str"
+    LIST = "list"
+    DICT = "dict"
+    BOOL = "bool"
+    PYDANTIC = "pydantic"
```

### Comparing `azure-functions-extension-base-1.0.0a2/azure_functions_extension_base.egg-info/SOURCES.txt` & `azure-functions-extension-base-1.0.0a3/azure_functions_extension_base.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 LICENSE
 MANIFEST.in
 README.md
-setup.py
+pyproject.toml
 azure/__init__.py
 azure/functions/__init__.py
 azure/functions/extension/__init__.py
 azure/functions/extension/base/__init__.py
 azure/functions/extension/base/meta.py
 azure/functions/extension/base/sdkType.py
 azure/functions/extension/base/utils.py
 azure/functions/extension/base/web.py
 azure_functions_extension_base.egg-info/PKG-INFO
 azure_functions_extension_base.egg-info/SOURCES.txt
 azure_functions_extension_base.egg-info/dependency_links.txt
 azure_functions_extension_base.egg-info/requires.txt
 azure_functions_extension_base.egg-info/top_level.txt
 tests/__init__.py
-tests/test_code_quality.py
 tests/test_meta.py
+tests/test_sdk_type.py
 tests/test_utils.py
 tests/test_web.py
```

### Comparing `azure-functions-extension-base-1.0.0a2/setup.py` & `azure-functions-extension-base-1.0.0a3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,91 +1,88 @@
-00000000: 2320 436f 7079 7269 6768 7420 2863 2920  # Copyright (c) 
-00000010: 4d69 6372 6f73 6f66 7420 436f 7270 6f72  Microsoft Corpor
-00000020: 6174 696f 6e2e 2041 6c6c 2072 6967 6874  ation. All right
-00000030: 7320 7265 7365 7276 6564 2e0d 0a23 204c  s reserved...# L
-00000040: 6963 656e 7365 6420 756e 6465 7220 7468  icensed under th
-00000050: 6520 4d49 5420 4c69 6365 6e73 652e 0d0a  e MIT License...
-00000060: 0d0a 6672 6f6d 2073 6574 7570 746f 6f6c  ..from setuptool
-00000070: 7320 696d 706f 7274 2073 6574 7570 2c20  s import setup, 
-00000080: 6669 6e64 5f70 6163 6b61 6765 730d 0a0d  find_packages...
-00000090: 0a45 5854 5241 5f52 4551 5549 5245 5320  .EXTRA_REQUIRES 
-000000a0: 3d20 7b0d 0a20 2020 2027 6465 7627 3a20  = {..    'dev': 
-000000b0: 5b0d 0a20 2020 2020 2020 2027 666c 616b  [..        'flak
-000000c0: 6538 7e3d 342e 302e 3127 2c0d 0a20 2020  e8~=4.0.1',..   
-000000d0: 2020 2020 2027 666c 616b 6538 2d6c 6f67       'flake8-log
-000000e0: 6769 6e67 2d66 6f72 6d61 7427 2c0d 0a20  ging-format',.. 
-000000f0: 2020 2020 2020 2027 6d79 7079 272c 0d0a         'mypy',..
-00000100: 2020 2020 2020 2020 2770 7974 6573 7427          'pytest'
-00000110: 2c0d 0a20 2020 2020 2020 2027 7079 7465  ,..        'pyte
-00000120: 7374 2d63 6f76 272c 0d0a 2020 2020 2020  st-cov',..      
-00000130: 2020 2772 6571 7565 7374 733d 3d32 2e2a    'requests==2.*
-00000140: 272c 0d0a 2020 2020 2020 2020 2763 6f76  ',..        'cov
-00000150: 6572 6167 6527 2c0d 0a20 2020 2020 2020  erage',..       
-00000160: 2022 7079 7465 7374 2d69 6e73 7461 6661   "pytest-instafa
-00000170: 696c 220d 0a20 2020 205d 0d0a 7d0d 0a0d  il"..    ]..}...
-00000180: 0a73 6574 7570 280d 0a20 2020 206e 616d  .setup(..    nam
-00000190: 653d 2761 7a75 7265 2d66 756e 6374 696f  e='azure-functio
-000001a0: 6e73 2d65 7874 656e 7369 6f6e 2d62 6173  ns-extension-bas
-000001b0: 6527 2c0d 0a20 2020 2076 6572 7369 6f6e  e',..    version
-000001c0: 3d27 312e 302e 3061 3227 2c0d 0a20 2020  ='1.0.0a2',..   
-000001d0: 2061 7574 686f 723d 2741 7a75 7265 2046   author='Azure F
-000001e0: 756e 6374 696f 6e73 2074 6561 6d20 6174  unctions team at
-000001f0: 204d 6963 726f 736f 6674 2043 6f72 702e   Microsoft Corp.
-00000200: 272c 0d0a 2020 2020 6175 7468 6f72 5f65  ',..    author_e
-00000210: 6d61 696c 3d27 617a 7572 6566 756e 6374  mail='azurefunct
-00000220: 696f 6e73 406d 6963 726f 736f 6674 2e63  ions@microsoft.c
-00000230: 6f6d 272c 0d0a 2020 2020 6465 7363 7269  om',..    descri
-00000240: 7074 696f 6e3d 2742 6173 6520 5079 7468  ption='Base Pyth
-00000250: 6f6e 2077 6f72 6b65 7220 6578 7465 6e73  on worker extens
-00000260: 696f 6e20 666f 7220 417a 7572 6520 4675  ion for Azure Fu
-00000270: 6e63 7469 6f6e 732e 272c 0d0a 2020 2020  nctions.',..    
-00000280: 7061 636b 6167 6573 3d66 696e 645f 7061  packages=find_pa
-00000290: 636b 6167 6573 2865 7863 6c75 6465 3d5b  ckages(exclude=[
-000002a0: 0d0a 2020 2020 2020 2020 2761 7a75 7265  ..        'azure
-000002b0: 2e66 756e 6374 696f 6e73 2e65 7874 656e  .functions.exten
-000002c0: 7369 6f6e 272c 2027 617a 7572 652e 6675  sion', 'azure.fu
-000002d0: 6e63 7469 6f6e 7327 2c20 2761 7a75 7265  nctions', 'azure
-000002e0: 272c 2027 7465 7374 7327 0d0a 2020 2020  ', 'tests'..    
-000002f0: 5d29 2c0d 0a20 2020 2063 6c61 7373 6966  ]),..    classif
-00000300: 6965 7273 3d5b 0d0a 2020 2020 2020 2020  iers=[..        
-00000310: 274c 6963 656e 7365 203a 3a20 4f53 4920  'License :: OSI 
-00000320: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
-00000330: 4c69 6365 6e73 6527 2c0d 0a20 2020 2020  License',..     
-00000340: 2020 2027 496e 7465 6e64 6564 2041 7564     'Intended Aud
-00000350: 6965 6e63 6520 3a3a 2044 6576 656c 6f70  ience :: Develop
-00000360: 6572 7327 2c0d 0a20 2020 2020 2020 2027  ers',..        '
-00000370: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000380: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000390: 3a20 3327 2c0d 0a20 2020 2020 2020 2027  : 3',..        '
-000003a0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000003b0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000003c0: 3a20 332e 3827 2c0d 0a20 2020 2020 2020  : 3.8',..       
-000003d0: 2027 5072 6f67 7261 6d6d 696e 6720 4c61   'Programming La
-000003e0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000003f0: 203a 3a20 332e 3927 2c0d 0a20 2020 2020   :: 3.9',..     
-00000400: 2020 2027 5072 6f67 7261 6d6d 696e 6720     'Programming 
-00000410: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000420: 6f6e 203a 3a20 332e 3130 272c 0d0a 2020  on :: 3.10',..  
-00000430: 2020 2020 2020 2750 726f 6772 616d 6d69        'Programmi
-00000440: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000450: 7974 686f 6e20 3a3a 2033 2e31 3127 2c0d  ython :: 3.11',.
-00000460: 0a20 2020 2020 2020 2027 4f70 6572 6174  .        'Operat
-00000470: 696e 6720 5379 7374 656d 203a 3a20 4d69  ing System :: Mi
-00000480: 6372 6f73 6f66 7420 3a3a 2057 696e 646f  crosoft :: Windo
-00000490: 7773 272c 0d0a 2020 2020 2020 2020 274f  ws',..        'O
-000004a0: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-000004b0: 3a3a 2050 4f53 4958 272c 0d0a 2020 2020  :: POSIX',..    
-000004c0: 2020 2020 274f 7065 7261 7469 6e67 2053      'Operating S
-000004d0: 7973 7465 6d20 3a3a 204d 6163 4f53 203a  ystem :: MacOS :
-000004e0: 3a20 4d61 634f 5320 5827 2c0d 0a20 2020  : MacOS X',..   
-000004f0: 2020 2020 2027 456e 7669 726f 6e6d 656e       'Environmen
-00000500: 7420 3a3a 2057 6562 2045 6e76 6972 6f6e  t :: Web Environ
-00000510: 6d65 6e74 272c 0d0a 2020 2020 2020 2020  ment',..        
-00000520: 2744 6576 656c 6f70 6d65 6e74 2053 7461  'Development Sta
-00000530: 7475 7320 3a3a 2035 202d 2050 726f 6475  tus :: 5 - Produ
-00000540: 6374 696f 6e2f 5374 6162 6c65 272c 0d0a  ction/Stable',..
-00000550: 2020 2020 5d2c 0d0a 2020 2020 6c69 6365      ],..    lice
-00000560: 6e73 653d 274d 4954 272c 0d0a 2020 2020  nse='MIT',..    
-00000570: 6578 7472 6173 5f72 6571 7569 7265 3d45  extras_require=E
-00000580: 5854 5241 5f52 4551 5549 5245 532c 0d0a  XTRA_REQUIRES,..
-00000590: 2020 2020 7079 7468 6f6e 5f72 6571 7569      python_requi
-000005a0: 7265 733d 273e 3d33 2e38 270d 0a29 0d0a  res='>=3.8'..)..
+00000000: 5b62 7569 6c64 2d73 7973 7465 6d5d 0d0a  [build-system]..
+00000010: 7265 7175 6972 6573 203d 205b 2273 6574  requires = ["set
+00000020: 7570 746f 6f6c 7320 3e3d 2036 312e 3022  uptools >= 61.0"
+00000030: 5d0d 0a62 7569 6c64 2d62 6163 6b65 6e64  ]..build-backend
+00000040: 203d 2022 7365 7475 7074 6f6f 6c73 2e62   = "setuptools.b
+00000050: 7569 6c64 5f6d 6574 6122 0d0a 0d0a 5b70  uild_meta"....[p
+00000060: 726f 6a65 6374 5d0d 0a6e 616d 6520 3d20  roject]..name = 
+00000070: 2261 7a75 7265 2d66 756e 6374 696f 6e73  "azure-functions
+00000080: 2d65 7874 656e 7369 6f6e 2d62 6173 6522  -extension-base"
+00000090: 0d0a 6479 6e61 6d69 6320 3d20 5b22 7665  ..dynamic = ["ve
+000000a0: 7273 696f 6e22 5d0d 0a72 6571 7569 7265  rsion"]..require
+000000b0: 732d 7079 7468 6f6e 203d 2022 3e3d 332e  s-python = ">=3.
+000000c0: 3822 0d0a 6175 7468 6f72 7320 3d20 5b7b  8"..authors = [{
+000000d0: 206e 616d 6520 3d20 2241 7a75 7265 2046   name = "Azure F
+000000e0: 756e 6374 696f 6e73 2074 6561 6d20 6174  unctions team at
+000000f0: 204d 6963 726f 736f 6674 2043 6f72 702e   Microsoft Corp.
+00000100: 222c 2065 6d61 696c 203d 2022 617a 7572  ", email = "azur
+00000110: 6566 756e 6374 696f 6e73 406d 6963 726f  efunctions@micro
+00000120: 736f 6674 2e63 6f6d 227d 5d0d 0a64 6573  soft.com"}]..des
+00000130: 6372 6970 7469 6f6e 203d 2022 4261 7365  cription = "Base
+00000140: 2050 7974 686f 6e20 776f 726b 6572 2065   Python worker e
+00000150: 7874 656e 7369 6f6e 2066 6f72 2041 7a75  xtension for Azu
+00000160: 7265 2046 756e 6374 696f 6e73 2e22 0d0a  re Functions."..
+00000170: 7265 6164 6d65 203d 2022 5245 4144 4d45  readme = "README
+00000180: 2e6d 6422 0d0a 6c69 6365 6e73 6520 3d20  .md"..license = 
+00000190: 7b74 6578 7420 3d20 224d 4954 204c 6963  {text = "MIT Lic
+000001a0: 656e 7365 227d 0d0a 636c 6173 7369 6669  ense"}..classifi
+000001b0: 6572 733d 205b 0d0a 2020 2020 2020 2020  ers= [..        
+000001c0: 274c 6963 656e 7365 203a 3a20 4f53 4920  'License :: OSI 
+000001d0: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
+000001e0: 4c69 6365 6e73 6527 2c0d 0a20 2020 2020  License',..     
+000001f0: 2020 2027 496e 7465 6e64 6564 2041 7564     'Intended Aud
+00000200: 6965 6e63 6520 3a3a 2044 6576 656c 6f70  ience :: Develop
+00000210: 6572 7327 2c0d 0a20 2020 2020 2020 2027  ers',..        '
+00000220: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000230: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000240: 3a20 3327 2c0d 0a20 2020 2020 2020 2027  : 3',..        '
+00000250: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000260: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000270: 3a20 332e 3827 2c0d 0a20 2020 2020 2020  : 3.8',..       
+00000280: 2027 5072 6f67 7261 6d6d 696e 6720 4c61   'Programming La
+00000290: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000002a0: 203a 3a20 332e 3927 2c0d 0a20 2020 2020   :: 3.9',..     
+000002b0: 2020 2027 5072 6f67 7261 6d6d 696e 6720     'Programming 
+000002c0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000002d0: 6f6e 203a 3a20 332e 3130 272c 0d0a 2020  on :: 3.10',..  
+000002e0: 2020 2020 2020 2750 726f 6772 616d 6d69        'Programmi
+000002f0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000300: 7974 686f 6e20 3a3a 2033 2e31 3127 2c0d  ython :: 3.11',.
+00000310: 0a20 2020 2020 2020 2027 4f70 6572 6174  .        'Operat
+00000320: 696e 6720 5379 7374 656d 203a 3a20 4d69  ing System :: Mi
+00000330: 6372 6f73 6f66 7420 3a3a 2057 696e 646f  crosoft :: Windo
+00000340: 7773 272c 0d0a 2020 2020 2020 2020 274f  ws',..        'O
+00000350: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+00000360: 3a3a 2050 4f53 4958 272c 0d0a 2020 2020  :: POSIX',..    
+00000370: 2020 2020 274f 7065 7261 7469 6e67 2053      'Operating S
+00000380: 7973 7465 6d20 3a3a 204d 6163 4f53 203a  ystem :: MacOS :
+00000390: 3a20 4d61 634f 5320 5827 2c0d 0a20 2020  : MacOS X',..   
+000003a0: 2020 2020 2027 456e 7669 726f 6e6d 656e       'Environmen
+000003b0: 7420 3a3a 2057 6562 2045 6e76 6972 6f6e  t :: Web Environ
+000003c0: 6d65 6e74 272c 0d0a 2020 2020 2020 2020  ment',..        
+000003d0: 2744 6576 656c 6f70 6d65 6e74 2053 7461  'Development Sta
+000003e0: 7475 7320 3a3a 2035 202d 2050 726f 6475  tus :: 5 - Produ
+000003f0: 6374 696f 6e2f 5374 6162 6c65 272c 0d0a  ction/Stable',..
+00000400: 2020 2020 5d0d 0a0d 0a5b 7072 6f6a 6563      ]....[projec
+00000410: 742e 6f70 7469 6f6e 616c 2d64 6570 656e  t.optional-depen
+00000420: 6465 6e63 6965 735d 0d0a 6465 7620 3d20  dencies]..dev = 
+00000430: 5b0d 0a20 2020 2020 2020 2027 7079 7465  [..        'pyte
+00000440: 7374 272c 0d0a 2020 2020 2020 2020 2770  st',..        'p
+00000450: 7974 6573 742d 636f 7627 2c0d 0a20 2020  ytest-cov',..   
+00000460: 2020 2020 2027 636f 7665 7261 6765 272c       'coverage',
+00000470: 0d0a 2020 2020 2020 2020 2770 7974 6573  ..        'pytes
+00000480: 742d 696e 7374 6166 6169 6c27 2c0d 0a20  t-instafail',.. 
+00000490: 2020 2020 2020 2027 7072 652d 636f 6d6d         'pre-comm
+000004a0: 6974 270d 0a20 2020 205d 0d0a 0d0a 5b74  it'..    ]....[t
+000004b0: 6f6f 6c2e 7365 7475 7074 6f6f 6c73 2e64  ool.setuptools.d
+000004c0: 796e 616d 6963 5d0d 0a76 6572 7369 6f6e  ynamic]..version
+000004d0: 203d 207b 6174 7472 203d 2022 617a 7572   = {attr = "azur
+000004e0: 652e 6675 6e63 7469 6f6e 732e 6578 7465  e.functions.exte
+000004f0: 6e73 696f 6e2e 6261 7365 2e5f 5f76 6572  nsion.base.__ver
+00000500: 7369 6f6e 5f5f 227d 0d0a 0d0a 5b74 6f6f  sion__"}....[too
+00000510: 6c2e 7365 7475 7074 6f6f 6c73 2e70 6163  l.setuptools.pac
+00000520: 6b61 6765 732e 6669 6e64 5d0d 0a65 7863  kages.find]..exc
+00000530: 6c75 6465 203d 205b 2761 7a75 7265 2e66  lude = ['azure.f
+00000540: 756e 6374 696f 6e73 2e65 7874 656e 7369  unctions.extensi
+00000550: 6f6e 272c 2027 617a 7572 652e 6675 6e63  on', 'azure.func
+00000560: 7469 6f6e 7327 2c20 2761 7a75 7265 272c  tions', 'azure',
+00000570: 2027 7465 7374 7327 5d0d 0a0d 0a          'tests']....
```

