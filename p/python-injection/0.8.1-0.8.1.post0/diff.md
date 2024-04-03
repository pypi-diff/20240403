# Comparing `tmp/python_injection-0.8.1.tar.gz` & `tmp/python_injection-0.8.1.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_injection-0.8.1.tar", max compression
+gzip compressed data, was "python_injection-0.8.1.post0.tar", max compression
```

## Comparing `python_injection-0.8.1.tar` & `python_injection-0.8.1.post0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2809 2024-04-01 11:37:27.304823 python_injection-0.8.1/documentation/basic-usage.md
--rw-r--r--   0        0        0       20 2024-04-01 11:37:27.304823 python_injection-0.8.1/injection/__init__.py
--rw-r--r--   0        0        0      647 2024-04-01 11:37:27.304823 python_injection-0.8.1/injection/_pkg.py
--rw-r--r--   0        0        0     5327 2024-04-01 11:37:27.304823 python_injection-0.8.1/injection/_pkg.pyi
--rw-r--r--   0        0        0        0 2024-04-01 11:37:27.304823 python_injection-0.8.1/injection/common/__init__.py
--rw-r--r--   0        0        0     1316 2024-04-01 11:37:27.304823 python_injection-0.8.1/injection/common/event.py
--rw-r--r--   0        0        0      558 2024-04-01 11:37:27.304823 python_injection-0.8.1/injection/common/invertible.py
--rw-r--r--   0        0        0     1401 2024-04-01 11:37:27.304823 python_injection-0.8.1/injection/common/lazy.py
--rw-r--r--   0        0        0     1443 2024-04-01 11:37:27.304823 python_injection-0.8.1/injection/common/queue.py
--rw-r--r--   0        0        0        0 2024-04-01 11:37:27.304823 python_injection-0.8.1/injection/common/tools/__init__.py
--rw-r--r--   0        0        0      271 2024-04-01 11:37:27.308823 python_injection-0.8.1/injection/common/tools/threading.py
--rw-r--r--   0        0        0     1276 2024-04-01 11:37:27.308823 python_injection-0.8.1/injection/common/tools/type.py
--rw-r--r--   0        0        0       22 2024-04-01 11:37:27.308823 python_injection-0.8.1/injection/core/__init__.py
--rw-r--r--   0        0        0    19284 2024-04-01 11:37:27.308823 python_injection-0.8.1/injection/core/module.py
--rw-r--r--   0        0        0      653 2024-04-01 11:37:27.308823 python_injection-0.8.1/injection/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-01 11:37:27.308823 python_injection-0.8.1/injection/integrations/__init__.py
--rw-r--r--   0        0        0      723 2024-04-01 11:37:27.308823 python_injection-0.8.1/injection/integrations/blacksheep.py
--rw-r--r--   0        0        0      676 2024-04-01 11:37:27.308823 python_injection-0.8.1/injection/utils.py
--rw-r--r--   0        0        0     1173 2024-04-01 11:37:42.176814 python_injection-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     3433 1970-01-01 00:00:00.000000 python_injection-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     3049 2024-04-03 18:32:39.943349 python_injection-0.8.1.post0/documentation/basic-usage.md
+-rw-r--r--   0        0        0       20 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/__init__.py
+-rw-r--r--   0        0        0      647 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/_pkg.py
+-rw-r--r--   0        0        0     5327 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/_pkg.pyi
+-rw-r--r--   0        0        0        0 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/common/__init__.py
+-rw-r--r--   0        0        0     1316 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/common/event.py
+-rw-r--r--   0        0        0      558 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/common/invertible.py
+-rw-r--r--   0        0        0     1401 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/common/lazy.py
+-rw-r--r--   0        0        0     1443 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/common/queue.py
+-rw-r--r--   0        0        0        0 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/common/tools/__init__.py
+-rw-r--r--   0        0        0      271 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/common/tools/threading.py
+-rw-r--r--   0        0        0     1276 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/common/tools/type.py
+-rw-r--r--   0        0        0       22 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/core/__init__.py
+-rw-r--r--   0        0        0    18952 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/core/module.py
+-rw-r--r--   0        0        0      653 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/integrations/__init__.py
+-rw-r--r--   0        0        0      723 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/integrations/blacksheep.py
+-rw-r--r--   0        0        0      676 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/utils.py
+-rw-r--r--   0        0        0     1212 2024-04-03 18:33:44.384278 python_injection-0.8.1.post0/pyproject.toml
+-rw-r--r--   0        0        0     3679 1970-01-01 00:00:00.000000 python_injection-0.8.1.post0/PKG-INFO
```

### Comparing `python_injection-0.8.1/documentation/basic-usage.md` & `python_injection-0.8.1.post0/documentation/basic-usage.md`

 * *Files 24% similar despite different names*

```diff
@@ -6,47 +6,50 @@
 
 If you wish to inject a singleton, use `singleton` decorator.
 
 ```python
 from injection import singleton
 
 @singleton
-class Singleton:
+class ServiceA:
     """ class implementation """
 ```
 
 If you wish to inject a new instance each time, use `injectable` decorator.
 
 ```python
 from injection import injectable
 
 @injectable
-class Injectable:
+class ServiceB:
     """ class implementation """
 ```
 
 If you have a constant (such as a global variable) and wish to register it as an injectable, use `set_constant`
 function.
 
 ```python
 from injection import set_constant
 
-app = set_constant(Application())
+class ServiceC:
+    """ class implementation """
+
+service_c = set_constant(ServiceC())
 ```
 
 ## Inject an instance
 
 To inject one or several instances, use `inject` decorator.
 _Don't forget to annotate type of parameter to inject._
 
 ```python
 from injection import inject
 
 @inject
-def my_function(instance: Injectable):
+def some_function(service_a: ServiceA):
     """ function implementation """
 ```
 
 If `inject` decorates a class, it will be applied to the `__init__` method.
 _Especially useful for dataclasses:_
 
 > **Note**: Doesn't work with Pydantic `BaseModel` because the signature of the `__init__` method doesn't contain the
@@ -55,94 +58,90 @@
 ```python
 from dataclasses import dataclass
 
 from injection import inject
 
 @inject
 @dataclass
-class DataClass:
-    instance: Injectable = ...
+class SomeDataClass:
+    service_a: ServiceA = ...
 ```
 
 ## Get an instance
 
 _Example with `get_instance` function:_
 
 ```python
 from injection import get_instance
 
-instance = get_instance(Injectable)
+service_a = get_instance(ServiceA)
 ```
 
 _Example with `get_lazy_instance` function:_
 
 ```python
 from injection import get_lazy_instance
 
-lazy_instance = get_lazy_instance(Injectable)
+lazy_service_a = get_lazy_instance(ServiceA)
 # ...
-instance = ~lazy_instance
+service_a = ~lazy_service_a
 ```
 
 ## Inheritance
 
 In the case of inheritance, you can use the decorator parameter `on` to link the injection to one or several other
 classes.
 
 **Warning: if the child class is in another file, make sure that file is imported before injection.**
 [_See `load_package` function._](utils.md#load_package)
 
 _Example with one class:_
 
 ```python
-from injection import singleton
-
-class A:
+class AbstractService(ABC):
     ...
 
-@singleton(on=A)
-class B(A):
+@injectable(on=AbstractService)
+class ConcreteService(AbstractService):
     ...
 ```
 
 _Example with several classes:_
 
 ```python
-from injection import singleton
-
-class A:
+class AbstractService(ABC):
     ...
 
-class B(A):
+class ConcreteService(AbstractService):
     ...
 
-@singleton(on=(A, B))
-class C(B):
+@injectable(on=(AbstractService, ConcreteService))
+class ConcreteServiceOverload(ConcreteService):
     ...
 ```
 
 If a class is registered in a package and you want to override it, there is the `override` parameter:
 
 ```python
-@singleton
-class A:
+@injectable
+class InaccessibleService:
     ...
 
 # ...
 
-@singleton(on=A, override=True)
-class B(A):
+@injectable(on=InaccessibleService, override=True)
+class ServiceOverload(InaccessibleService):
     ...
 ```
 
 ## Recipes
 
 A recipe is a function that tells the injector how to construct the instance to be injected. It is important to specify 
 the return type annotation when defining the recipe.
 
 ```python
-from injection import singleton
+from injection import injectable
 
-@singleton
-def my_recipe() -> Singleton:
+@injectable
+def service_d_recipe() -> ServiceD:
     """ recipe implementation """
 ```
```

### Comparing `python_injection-0.8.1/injection/_pkg.py` & `python_injection-0.8.1.post0/injection/_pkg.py`

 * *Files identical despite different names*

### Comparing `python_injection-0.8.1/injection/_pkg.pyi` & `python_injection-0.8.1.post0/injection/_pkg.pyi`

 * *Files identical despite different names*

### Comparing `python_injection-0.8.1/injection/common/event.py` & `python_injection-0.8.1.post0/injection/common/event.py`

 * *Files identical despite different names*

### Comparing `python_injection-0.8.1/injection/common/invertible.py` & `python_injection-0.8.1.post0/injection/common/invertible.py`

 * *Files identical despite different names*

### Comparing `python_injection-0.8.1/injection/common/lazy.py` & `python_injection-0.8.1.post0/injection/common/lazy.py`

 * *Files identical despite different names*

### Comparing `python_injection-0.8.1/injection/common/queue.py` & `python_injection-0.8.1.post0/injection/common/queue.py`

 * *Files identical despite different names*

### Comparing `python_injection-0.8.1/injection/common/tools/type.py` & `python_injection-0.8.1.post0/injection/common/tools/type.py`

 * *Files identical despite different names*

### Comparing `python_injection-0.8.1/injection/core/module.py` & `python_injection-0.8.1.post0/injection/core/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,22 +12,17 @@
     Mapping,
     MutableMapping,
     Set,
 )
 from contextlib import ContextDecorator, contextmanager, suppress
 from dataclasses import dataclass, field
 from enum import Enum, auto
-from functools import (
-    partialmethod,
-    singledispatchmethod,
-    update_wrapper,
-    wraps,
-)
+from functools import partialmethod, singledispatchmethod, update_wrapper
 from inspect import Signature, isclass
-from types import UnionType
+from types import MethodType, UnionType
 from typing import (
     Any,
     ClassVar,
     ContextManager,
     NamedTuple,
     NoReturn,
     Protocol,
@@ -631,64 +626,57 @@
     kwargs: Mapping[str, Any]
 
 
 class InjectedFunction(EventListener):
     __slots__ = (
         "__dict__",
         "__signature__",
+        "__wrapped__",
         "__dependencies",
         "__owner",
         "__setup_queue",
-        "__wrapper",
     )
 
     def __init__(self, wrapped: Callable[..., Any], /):
         update_wrapper(self, wrapped)
-
-        @wraps(wrapped)
-        def wrapper(*args, **kwargs):
-            self.__consume_setup_queue()
-            args, kwargs = self.bind(args, kwargs)
-            return wrapped(*args, **kwargs)
-
-        self.__wrapper = wrapper
         self.__dependencies = Dependencies.empty()
         self.__owner = None
         self.__setup_queue = LimitedQueue[Callable[[], Any]]()
-        self.on_setup(
-            lambda: self.__set_signature(
-                inspect.signature(
-                    wrapped,
-                    eval_str=True,
-                )
-            )
-        )
+        self.on_setup(self.__set_signature)
 
     def __repr__(self) -> str:
-        return repr(self.__wrapper)
+        return repr(self.wrapped)
 
     def __str__(self) -> str:
-        return str(self.__wrapper)
+        return str(self.wrapped)
 
     def __call__(self, /, *args, **kwargs) -> Any:
-        return self.__wrapper(*args, **kwargs)
+        for function in self.__setup_queue:
+            function()
+
+        args, kwargs = self.bind(args, kwargs)
+        return self.wrapped(*args, **kwargs)
 
     def __get__(self, instance: object = None, owner: type = None):
         if instance is None:
             return self
 
-        return self.__wrapper.__get__(instance, owner)
+        return MethodType(self, instance)
 
     def __set_name__(self, owner: type, name: str):
         self.set_owner(owner)
 
     @property
     def signature(self) -> Signature:
         return self.__signature__
 
+    @property
+    def wrapped(self) -> Callable[..., Any]:
+        return self.__wrapped__
+
     def bind(
         self,
         args: Iterable[Any] = (),
         kwargs: Mapping[str, Any] = None,
     ) -> Arguments:
         if kwargs is None:
             kwargs = {}
@@ -732,16 +720,10 @@
 
     @on_event.register
     @contextmanager
     def _(self, event: ModuleEvent, /) -> ContextManager:
         yield
         self.update(event.on_module)
 
-    def __consume_setup_queue(self):
-        for function in self.__setup_queue:
-            function()
-
-        return self
-
-    def __set_signature(self, signature: Signature):
-        self.__signature__ = signature
+    def __set_signature(self):
+        self.__signature__ = inspect.signature(self.wrapped, eval_str=True)
         return self
```

### Comparing `python_injection-0.8.1/injection/exceptions.py` & `python_injection-0.8.1.post0/injection/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_injection-0.8.1/injection/integrations/blacksheep.py` & `python_injection-0.8.1.post0/injection/integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `python_injection-0.8.1/injection/utils.py` & `python_injection-0.8.1.post0/injection/utils.py`

 * *Files identical despite different names*

### Comparing `python_injection-0.8.1/pyproject.toml` & `python_injection-0.8.1.post0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [tool.poetry]
 name = "python-injection"
-version = "0.8.1"
+version = "0.8.1.post0"
 description = "Fast and easy dependency injection framework."
 authors = ["remimd"]
 keywords = ["dependencies", "inject", "injection"]
 license = "MIT"
 packages = [{ include = "injection" }]
 readme = "documentation/basic-usage.md"
 repository = "https://github.com/100nm/python-injection"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <4"
 
 [tool.poetry.group.dev.dependencies]
+argon2-cffi = "*"
 blacksheep = "*"
+faker = "*"
 pydantic = "*"
 pytest = "*"
 pytest-asyncio = "*"
 pytest-cov = "*"
 ruff = "*"
 
 [tool.coverage.report]
@@ -27,15 +29,15 @@
     "raise NotImplementedError",
 ]
 
 [tool.pytest.ini_options]
 python_files = "test_*.py"
 addopts = "-p no:warnings --tb=short"
 asyncio_mode = "auto"
-testpaths = "tests/"
+testpaths = "**/tests/"
 
 [tool.ruff]
 line-length = 88
 indent-width = 4
 
 [tool.ruff.format]
 quote-style = "double"
```

### Comparing `python_injection-0.8.1/PKG-INFO` & `python_injection-0.8.1.post0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-injection
-Version: 0.8.1
+Version: 0.8.1.post0
 Summary: Fast and easy dependency injection framework.
 Home-page: https://github.com/100nm/python-injection
 License: MIT
 Keywords: dependencies,inject,injection
 Author: remimd
 Requires-Python: >=3.10,<4
 Classifier: License :: OSI Approved :: MIT License
@@ -23,47 +23,50 @@
 
 If you wish to inject a singleton, use `singleton` decorator.
 
 ```python
 from injection import singleton
 
 @singleton
-class Singleton:
+class ServiceA:
     """ class implementation """
 ```
 
 If you wish to inject a new instance each time, use `injectable` decorator.
 
 ```python
 from injection import injectable
 
 @injectable
-class Injectable:
+class ServiceB:
     """ class implementation """
 ```
 
 If you have a constant (such as a global variable) and wish to register it as an injectable, use `set_constant`
 function.
 
 ```python
 from injection import set_constant
 
-app = set_constant(Application())
+class ServiceC:
+    """ class implementation """
+
+service_c = set_constant(ServiceC())
 ```
 
 ## Inject an instance
 
 To inject one or several instances, use `inject` decorator.
 _Don't forget to annotate type of parameter to inject._
 
 ```python
 from injection import inject
 
 @inject
-def my_function(instance: Injectable):
+def some_function(service_a: ServiceA):
     """ function implementation """
 ```
 
 If `inject` decorates a class, it will be applied to the `__init__` method.
 _Especially useful for dataclasses:_
 
 > **Note**: Doesn't work with Pydantic `BaseModel` because the signature of the `__init__` method doesn't contain the
@@ -72,95 +75,91 @@
 ```python
 from dataclasses import dataclass
 
 from injection import inject
 
 @inject
 @dataclass
-class DataClass:
-    instance: Injectable = ...
+class SomeDataClass:
+    service_a: ServiceA = ...
 ```
 
 ## Get an instance
 
 _Example with `get_instance` function:_
 
 ```python
 from injection import get_instance
 
-instance = get_instance(Injectable)
+service_a = get_instance(ServiceA)
 ```
 
 _Example with `get_lazy_instance` function:_
 
 ```python
 from injection import get_lazy_instance
 
-lazy_instance = get_lazy_instance(Injectable)
+lazy_service_a = get_lazy_instance(ServiceA)
 # ...
-instance = ~lazy_instance
+service_a = ~lazy_service_a
 ```
 
 ## Inheritance
 
 In the case of inheritance, you can use the decorator parameter `on` to link the injection to one or several other
 classes.
 
 **Warning: if the child class is in another file, make sure that file is imported before injection.**
 [_See `load_package` function._](utils.md#load_package)
 
 _Example with one class:_
 
 ```python
-from injection import singleton
-
-class A:
+class AbstractService(ABC):
     ...
 
-@singleton(on=A)
-class B(A):
+@injectable(on=AbstractService)
+class ConcreteService(AbstractService):
     ...
 ```
 
 _Example with several classes:_
 
 ```python
-from injection import singleton
-
-class A:
+class AbstractService(ABC):
     ...
 
-class B(A):
+class ConcreteService(AbstractService):
     ...
 
-@singleton(on=(A, B))
-class C(B):
+@injectable(on=(AbstractService, ConcreteService))
+class ConcreteServiceOverload(ConcreteService):
     ...
 ```
 
 If a class is registered in a package and you want to override it, there is the `override` parameter:
 
 ```python
-@singleton
-class A:
+@injectable
+class InaccessibleService:
     ...
 
 # ...
 
-@singleton(on=A, override=True)
-class B(A):
+@injectable(on=InaccessibleService, override=True)
+class ServiceOverload(InaccessibleService):
     ...
 ```
 
 ## Recipes
 
 A recipe is a function that tells the injector how to construct the instance to be injected. It is important to specify 
 the return type annotation when defining the recipe.
 
 ```python
-from injection import singleton
+from injection import injectable
 
-@singleton
-def my_recipe() -> Singleton:
+@injectable
+def service_d_recipe() -> ServiceD:
     """ recipe implementation """
 ```
```

