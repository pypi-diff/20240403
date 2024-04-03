# Comparing `tmp/graphene_django_query_optimizer-0.4.2.tar.gz` & `tmp/graphene_django_query_optimizer-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphene_django_query_optimizer-0.4.2.tar", max compression
+gzip compressed data, was "graphene_django_query_optimizer-0.5.0.tar", max compression
```

## Comparing `graphene_django_query_optimizer-0.4.2.tar` & `graphene_django_query_optimizer-0.5.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1064 2024-03-26 21:02:47.592792 graphene_django_query_optimizer-0.4.2/LICENSE
--rw-r--r--   0        0        0     3151 2024-03-26 21:02:47.592792 graphene_django_query_optimizer-0.4.2/README.md
--rw-r--r--   0        0        0     6905 2024-03-26 21:02:47.592792 graphene_django_query_optimizer-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      496 2024-03-26 21:02:47.592792 graphene_django_query_optimizer-0.4.2/query_optimizer/__init__.py
--rw-r--r--   0        0        0    11596 2024-03-26 21:02:47.592792 graphene_django_query_optimizer-0.4.2/query_optimizer/ast.py
--rw-r--r--   0        0        0     4629 2024-03-26 21:02:47.592792 graphene_django_query_optimizer-0.4.2/query_optimizer/cache.py
--rw-r--r--   0        0        0     8342 2024-03-26 21:02:47.592792 graphene_django_query_optimizer-0.4.2/query_optimizer/compiler.py
--rw-r--r--   0        0        0     2938 2024-03-26 21:02:47.592792 graphene_django_query_optimizer-0.4.2/query_optimizer/converters.py
--rw-r--r--   0        0        0      177 2024-03-26 21:02:47.592792 graphene_django_query_optimizer-0.4.2/query_optimizer/errors.py
--rw-r--r--   0        0        0    15955 2024-03-26 21:02:47.592792 graphene_django_query_optimizer-0.4.2/query_optimizer/fields.py
--rw-r--r--   0        0        0     1686 2024-03-26 21:02:47.592792 graphene_django_query_optimizer-0.4.2/query_optimizer/filter.py
--rw-r--r--   0        0        0     5238 2024-03-26 21:02:47.592792 graphene_django_query_optimizer-0.4.2/query_optimizer/filter_info.py
--rw-r--r--   0        0        0    11343 2024-03-26 21:02:47.592792 graphene_django_query_optimizer-0.4.2/query_optimizer/optimizer.py
--rw-r--r--   0        0        0     3887 2024-03-26 21:02:47.592792 graphene_django_query_optimizer-0.4.2/query_optimizer/prefetch_hack.py
--rw-r--r--   0        0        0        0 2024-03-26 21:02:47.592792 graphene_django_query_optimizer-0.4.2/query_optimizer/py.typed
--rw-r--r--   0        0        0     2627 2024-03-26 21:02:47.592792 graphene_django_query_optimizer-0.4.2/query_optimizer/settings.py
--rw-r--r--   0        0        0     2719 2024-03-26 21:02:47.592792 graphene_django_query_optimizer-0.4.2/query_optimizer/types.py
--rw-r--r--   0        0        0     4174 2024-03-26 21:02:47.592792 graphene_django_query_optimizer-0.4.2/query_optimizer/typing.py
--rw-r--r--   0        0        0     6141 2024-03-26 21:02:47.592792 graphene_django_query_optimizer-0.4.2/query_optimizer/utils.py
--rw-r--r--   0        0        0     3840 2024-03-26 21:02:47.592792 graphene_django_query_optimizer-0.4.2/query_optimizer/validators.py
--rw-r--r--   0        0        0     4694 1970-01-01 00:00:00.000000 graphene_django_query_optimizer-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-03 16:39:48.753631 graphene_django_query_optimizer-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3151 2024-04-03 16:39:48.753631 graphene_django_query_optimizer-0.5.0/README.md
+-rw-r--r--   0        0        0     6905 2024-04-03 16:39:48.753631 graphene_django_query_optimizer-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      496 2024-04-03 16:39:48.753631 graphene_django_query_optimizer-0.5.0/query_optimizer/__init__.py
+-rw-r--r--   0        0        0    11596 2024-04-03 16:39:48.753631 graphene_django_query_optimizer-0.5.0/query_optimizer/ast.py
+-rw-r--r--   0        0        0     8039 2024-04-03 16:39:48.757631 graphene_django_query_optimizer-0.5.0/query_optimizer/compiler.py
+-rw-r--r--   0        0        0     2847 2024-04-03 16:39:48.757631 graphene_django_query_optimizer-0.5.0/query_optimizer/converters.py
+-rw-r--r--   0        0        0      177 2024-04-03 16:39:48.757631 graphene_django_query_optimizer-0.5.0/query_optimizer/errors.py
+-rw-r--r--   0        0        0    15513 2024-04-03 16:39:48.757631 graphene_django_query_optimizer-0.5.0/query_optimizer/fields.py
+-rw-r--r--   0        0        0     1686 2024-04-03 16:39:48.757631 graphene_django_query_optimizer-0.5.0/query_optimizer/filter.py
+-rw-r--r--   0        0        0     5238 2024-04-03 16:39:48.757631 graphene_django_query_optimizer-0.5.0/query_optimizer/filter_info.py
+-rw-r--r--   0        0        0    11297 2024-04-03 16:39:48.757631 graphene_django_query_optimizer-0.5.0/query_optimizer/optimizer.py
+-rw-r--r--   0        0        0     4130 2024-04-03 16:39:48.757631 graphene_django_query_optimizer-0.5.0/query_optimizer/prefetch_hack.py
+-rw-r--r--   0        0        0        0 2024-04-03 16:39:48.757631 graphene_django_query_optimizer-0.5.0/query_optimizer/py.typed
+-rw-r--r--   0        0        0     2627 2024-04-03 16:39:48.757631 graphene_django_query_optimizer-0.5.0/query_optimizer/settings.py
+-rw-r--r--   0        0        0     2996 2024-04-03 16:39:48.757631 graphene_django_query_optimizer-0.5.0/query_optimizer/types.py
+-rw-r--r--   0        0        0     3639 2024-04-03 16:39:48.757631 graphene_django_query_optimizer-0.5.0/query_optimizer/typing.py
+-rw-r--r--   0        0        0     6141 2024-04-03 16:39:48.757631 graphene_django_query_optimizer-0.5.0/query_optimizer/utils.py
+-rw-r--r--   0        0        0     3840 2024-04-03 16:39:48.757631 graphene_django_query_optimizer-0.5.0/query_optimizer/validators.py
+-rw-r--r--   0        0        0     4694 1970-01-01 00:00:00.000000 graphene_django_query_optimizer-0.5.0/PKG-INFO
```

### Comparing `graphene_django_query_optimizer-0.4.2/LICENSE` & `graphene_django_query_optimizer-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.4.2/README.md` & `graphene_django_query_optimizer-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.4.2/pyproject.toml` & `graphene_django_query_optimizer-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "graphene-django-query-optimizer"
-version = "0.4.2"
+version = "0.5.0"
 description = "Automatically optimize SQL queries in Graphene-Django schemas."
 authors = [
     "Matti Lamppu <lamppu.matti.akseli@gmail.com>",
 ]
 packages = [
     { include = "query_optimizer" },
 ]
@@ -62,15 +62,15 @@
 [tool.poetry.group.test.dependencies]
 pytest = "8.1.1"
 coverage = "7.4.4"
 pytest-django = "4.8.0"
 pre-commit = "3.7.0"
 tox = "4.14.2"
 tox-gh-actions = "3.2.0"
-faker = "24.3.0"
+faker = "24.4.0"
 factory-boy = "3.3.0"
 sqlparse = "0.4.4"
 django-graphiql-debug-toolbar = "0.2.0"
 py-spy = "0.3.14"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "1.5.3"
```

### Comparing `graphene_django_query_optimizer-0.4.2/query_optimizer/ast.py` & `graphene_django_query_optimizer-0.5.0/query_optimizer/ast.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.4.2/query_optimizer/compiler.py` & `graphene_django_query_optimizer-0.5.0/query_optimizer/compiler.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,29 +4,27 @@
 from typing import TYPE_CHECKING, Optional, Union
 
 from django.db.models import ForeignKey, Manager, ManyToOneRel, Model, QuerySet
 from graphene.utils.str_converters import to_snake_case
 from graphene_django.utils import maybe_queryset
 
 from .ast import GraphQLASTWalker
-from .cache import get_from_query_cache, store_in_query_cache
 from .errors import OptimizerError
 from .optimizer import QueryOptimizer
+from .prefetch_hack import fetch_in_context
 from .settings import optimizer_settings
 from .utils import is_optimized, optimizer_logger
 
 if TYPE_CHECKING:
     import graphene
     from django.db import models
     from graphene.types.definitions import GrapheneObjectType
     from graphql import FieldNode
 
-    from .typing import PK, GQLInfo, ToManyField, ToOneField, TypeVar
-
-    TModel = TypeVar("TModel", bound=Model)
+    from .typing import PK, GQLInfo, TModel, ToManyField, ToOneField
 
 
 __all__ = [
     "optimize",
     "optimize_single",
     "OptimizationCompiler",
 ]
@@ -38,44 +36,38 @@
     *,
     max_complexity: Optional[int] = None,
 ) -> QuerySet[TModel]:
     """Optimize the given queryset according to the field selections received in the GraphQLResolveInfo."""
     optimizer = OptimizationCompiler(info, max_complexity=max_complexity).compile(queryset)
     if optimizer is not None:
         queryset = optimizer.optimize_queryset(queryset)
-        store_in_query_cache(queryset, optimizer, info)
+        fetch_in_context(queryset)
 
     return queryset
 
 
 def optimize_single(
     queryset: QuerySet[TModel],
     info: GQLInfo,
     *,
     pk: PK,
     max_complexity: Optional[int] = None,
 ) -> Optional[TModel]:
     """Optimize the given queryset for a single model instance by its primary key."""
-    queryset = queryset.filter(pk=pk)
-
     optimizer = OptimizationCompiler(info, max_complexity=max_complexity).compile(queryset)
     if optimizer is None:  # pragma: no cover
-        return queryset.first()
-
-    cached_item = get_from_query_cache(queryset.model, pk, optimizer, info)
-    if cached_item is not None:
-        return cached_item
+        return queryset.filter(pk=pk).first()
 
-    optimized_queryset = optimizer.optimize_queryset(queryset)
-    store_in_query_cache(optimized_queryset, optimizer, info)
+    queryset = optimizer.optimize_queryset(queryset.filter(pk=pk))
+    fetch_in_context(queryset)
 
     # Shouldn't use .first(), as it can apply additional ordering, which would cancel the optimization.
     # The queryset should have the right model instance, since we started by filtering by its pk,
     # so we can just pick that out of the result cache (if it hasn't been filtered out).
-    return next(iter(optimized_queryset._result_cache or []), None)
+    return next(iter(queryset), None)
 
 
 class OptimizationCompiler(GraphQLASTWalker):
     """Class for compiling SQL optimizations based on the given query."""
 
     def __init__(self, info: GQLInfo, max_complexity: Optional[int] = None) -> None:
         """
```

### Comparing `graphene_django_query_optimizer-0.4.2/query_optimizer/converters.py` & `graphene_django_query_optimizer-0.5.0/query_optimizer/converters.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,21 +32,19 @@
         type_: Optional[type[DjangoObjectType]] = registry.get_type_for_model(field.related_model)
         if type_ is None:  # pragma: no cover
             return None
 
         actual_field = field.field if isinstance(field, models.OneToOneRel) else field
         description: str = get_django_field_description(actual_field)
         required: bool = False if isinstance(field, models.OneToOneRel) else not field.null
-        reverse: bool = isinstance(field, models.OneToOneRel)
 
         from query_optimizer.fields import RelatedField
 
         return RelatedField(
             type_,
-            reverse=reverse,
             description=description,
             required=required,
         )
 
     return graphene.Dynamic(dynamic_type)
```

### Comparing `graphene_django_query_optimizer-0.4.2/query_optimizer/fields.py` & `graphene_django_query_optimizer-0.5.0/query_optimizer/fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,54 @@
 # ruff: noqa: UP006
 from __future__ import annotations
 
+import warnings
 from functools import cached_property, partial
 from typing import TYPE_CHECKING
 
 import graphene
 from graphene.relay.connection import connection_adapter, page_info_adapter
 from graphene.types.argument import to_arguments
 from graphene.utils.str_converters import to_camel_case, to_snake_case
 from graphene_django.settings import graphene_settings
 from graphene_django.utils.utils import DJANGO_FILTER_INSTALLED, maybe_queryset
 from graphql_relay.connection.array_connection import offset_to_cursor
 
 from .ast import get_underlying_type
-from .cache import store_in_query_cache
 from .compiler import OptimizationCompiler, optimize
+from .prefetch_hack import fetch_in_context
 from .settings import optimizer_settings
 from .utils import calculate_queryset_slice, is_optimized
 from .validators import validate_pagination_args
 
 if TYPE_CHECKING:
     from django.db import models
     from django.db.models import Model
     from django.db.models.manager import Manager
     from graphene.relay.connection import Connection
-    from graphene_django import DjangoObjectType
     from graphql_relay import EdgeType
     from graphql_relay.connection.connection import ConnectionType
 
+    from .types import DjangoObjectType
     from .typing import (
         Any,
         Callable,
         ConnectionResolver,
         ExpressionKind,
         GQLInfo,
         Iterable,
         ModelResolver,
         ObjectTypeInput,
         Optional,
         QuerySetResolver,
         Type,
-        TypeVar,
         Union,
         UnmountedTypeInput,
     )
 
-    TModel = TypeVar("TModel", bound=models.Model)
-
 __all__ = [
     "DjangoConnectionField",
     "DjangoListField",
     "RelatedField",
     "AnnotatedField",
     "MultiField",
 ]
@@ -60,57 +58,52 @@
     """Field for `to-one` related models with default resolvers."""
 
     def __init__(
         self,
         type_: ObjectTypeInput,
         /,
         *,
-        reverse: bool = False,
         field_name: Optional[str] = None,
         **kwargs: Any,
     ) -> None:
         """
         Initialize a related field for the given type.
 
         :param type_: DjangoObjectType the related field is for.
                       This can also be a dot import path to the object type,
                       or a callable that returns the object type.
-        :param reverse: Is the relation direction forward or reverse?
         :param field_name: The name of the model field or related accessor this related field is for.
                            Only needed if the field name on the ObjectType this field is
                            defined on is different from the field name on the model.
         :param kwargs: Extra arguments passed to `graphene.types.field.Field`.
         """
-        self.reverse = reverse
+        if kwargs.pop("reverse", None) is not None:  # pragma: no cover
+            msg = (
+                "The `reverse` argument is no longer required, and should be removed. "
+                "This will become an error in the future."
+            )
+            warnings.warn(msg, category=DeprecationWarning, stacklevel=1)
+
         self.field_name = field_name
         super().__init__(type_, **kwargs)
 
     def wrap_resolve(self, parent_resolver: ModelResolver) -> ModelResolver:
         # Allow user defined resolvers to override the default behavior.
         if not isinstance(parent_resolver, partial):
             return parent_resolver
-        if self.reverse:
-            return self.reverse_resolver
-        return self.forward_resolver
+        return self.related_resolver
 
-    def forward_resolver(self, root: models.Model, info: GQLInfo) -> Optional[models.Model]:
+    def related_resolver(self, root: models.Model, info: GQLInfo) -> Optional[models.Model]:
         field_name = self.field_name or to_snake_case(info.field_name)
-        db_field_key: str = root.__class__._meta.get_field(field_name).attname
-        object_pk = getattr(root, db_field_key, None)
-        if object_pk is None:  # pragma: no cover
+        # Related object should be optimized to the root model.
+        related_instance: Optional[models.Model] = getattr(root, field_name, None)
+        if related_instance is None:
             return None
-        return self.underlying_type.get_node(info, object_pk)
-
-    def reverse_resolver(self, root: models.Model, info: GQLInfo) -> Optional[models.Model]:
-        field_name = self.field_name or to_snake_case(info.field_name)
-        # Reverse object should be optimized to the root model.
-        reverse_object: Optional[models.Model] = getattr(root, field_name, None)
-        if reverse_object is None:
-            return None
-        return self.underlying_type.get_node(info, reverse_object.pk)
+        self.underlying_type.run_instance_checks(related_instance, info)
+        return related_instance
 
     @cached_property
     def underlying_type(self) -> type[DjangoObjectType]:
         return get_underlying_type(self.type)
 
 
 class FilteringMixin:
@@ -288,23 +281,20 @@
         )
         cut = calculate_queryset_slice(**pagination_args)
 
         # Prefetch queryset has already been sliced.
         if not already_optimized:
             queryset = queryset[cut]
 
-        # Store data in cache after pagination
-        if optimizer is not None:
-            store_in_query_cache(queryset, optimizer, info)
-
-        # Create a connection from the sliced queryset.
         edges: list[EdgeType] = [
+            # Create a connection from the sliced queryset.
             self.connection_type.Edge(node=value, cursor=offset_to_cursor(cut.start + index))
-            for index, value in enumerate(queryset)
+            for index, value in enumerate(fetch_in_context(queryset))
         ]
+
         connection = connection_adapter(
             cls=self.connection_type,
             edges=edges,
             pageInfo=page_info_adapter(
                 startCursor=edges[0].cursor if edges else None,
                 endCursor=edges[-1].cursor if edges else None,
                 hasPreviousPage=cut.start > 0,
```

### Comparing `graphene_django_query_optimizer-0.4.2/query_optimizer/filter.py` & `graphene_django_query_optimizer-0.5.0/query_optimizer/filter.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.4.2/query_optimizer/filter_info.py` & `graphene_django_query_optimizer-0.5.0/query_optimizer/filter_info.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.4.2/query_optimizer/optimizer.py` & `graphene_django_query_optimizer-0.5.0/query_optimizer/optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,15 @@
     mark_optimized,
     optimizer_logger,
 )
 from .validators import validate_pagination_args
 
 if TYPE_CHECKING:
     from .types import DjangoObjectType
-    from .typing import Any, ExpressionKind, GQLInfo, GraphQLFilterInfo, Optional, ToManyField, TypeVar
-
-    TModel = TypeVar("TModel", bound=Model)
+    from .typing import Any, ExpressionKind, GQLInfo, GraphQLFilterInfo, Optional, TModel, ToManyField
 
 
 __all__ = [
     "QueryOptimizer",
 ]
```

### Comparing `graphene_django_query_optimizer-0.4.2/query_optimizer/prefetch_hack.py` & `graphene_django_query_optimizer-0.5.0/query_optimizer/prefetch_hack.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from unittest.mock import patch
 from weakref import WeakKeyDictionary
 
 from django.db import models
 from django.db.models.fields.related_descriptors import _filter_prefetch_queryset
 from graphql import OperationDefinitionNode
 
-from .typing import ContextManager, GQLInfo, ToManyField, TypeAlias
+from .typing import ContextManager, GQLInfo, TModel, ToManyField, TypeAlias
 
 __all__ = [
     "_register_for_prefetch_hack",
     "fetch_context",
 ]
 
 
@@ -78,7 +78,13 @@
 def fetch_context() -> ContextManager:
     """Patches the prefetch mechanism if required."""
     try:
         with _HACK_CONTEXT if _PREFETCH_HACK_CACHE else nullcontext():
             yield
     finally:
         _PREFETCH_HACK_CACHE.clear()
+
+
+def fetch_in_context(queryset: models.QuerySet[TModel]) -> list[TModel]:
+    """Evaluates the queryset with the prefetch hack applied."""
+    with fetch_context():
+        return list(queryset)  # the database query is executed here
```

### Comparing `graphene_django_query_optimizer-0.4.2/query_optimizer/settings.py` & `graphene_django_query_optimizer-0.5.0/query_optimizer/settings.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.4.2/query_optimizer/types.py` & `graphene_django_query_optimizer-0.5.0/query_optimizer/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 from .compiler import optimize_single
 from .settings import optimizer_settings
 from .typing import PK, OptimizedDjangoOptions
 
 if TYPE_CHECKING:
     from django.db.models import Model, QuerySet
 
-    from .typing import Any, GQLInfo, Literal, Optional, TypeVar, Union
-
-    TModel = TypeVar("TModel", bound=Model)
+    from .typing import Any, GQLInfo, Literal, Optional, TModel, Union
 
 
 __all__ = [
     "DjangoObjectType",
 ]
 
 
@@ -71,8 +69,15 @@
     @classmethod
     def get_queryset(cls, queryset: QuerySet[TModel], info: GQLInfo) -> QuerySet[TModel]:
         return queryset
 
     @classmethod
     def get_node(cls, info: GQLInfo, pk: PK) -> Optional[TModel]:
         queryset = cls._meta.model._default_manager.all()
-        return optimize_single(queryset, info, pk=pk, max_complexity=cls._meta.max_complexity)
+        maybe_instance = optimize_single(queryset, info, pk=pk, max_complexity=cls._meta.max_complexity)
+        if maybe_instance is not None:  # pragma: no cover
+            cls.run_instance_checks(maybe_instance, info)
+        return maybe_instance
+
+    @classmethod
+    def run_instance_checks(cls, instance: TModel, info: GQLInfo) -> None:
+        """A hook for running checks after getting a single instance."""
```

### Comparing `graphene_django_query_optimizer-0.4.2/query_optimizer/typing.py` & `graphene_django_query_optimizer-0.5.0/query_optimizer/typing.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     TypeVar,
     Union,
     cast,
     overload,
 )
 
 from django.db import models
-from graphene.relay.connection import ConnectionOptions
 from graphene.types.unmountedtype import UnmountedType
 from graphene_django import DjangoObjectType
 from graphene_django.types import DjangoObjectTypeOptions
 from graphql_relay import ConnectionType
 
 # New in version 3.10
 try:
@@ -46,15 +45,15 @@
     ManyToManyField,
     ManyToManyRel,
     ManyToOneRel,
     Model,
     OneToOneField,
     QuerySet,
 )
-from graphql import FieldNode, GraphQLResolveInfo, SelectionNode
+from graphql import GraphQLResolveInfo
 
 if TYPE_CHECKING:
     from django.contrib.auth.models import AnonymousUser, User
     from django.contrib.contenttypes.fields import GenericForeignKey, GenericRelation
     from django.db.models.sql import Query
     from django_filters import FilterSet
 
@@ -62,65 +61,53 @@
     "Any",
     "Callable",
     "Collection",
     "ConnectionResolver",
     "ContextManager",
     "Expr",
     "ExpressionKind",
-    "FieldNodes",
-    "FilterFields",
     "GQLInfo",
     "GRAPHQL_BUILTIN",
     "Generator",
     "Generic",
     "GraphQLFilterInfo",
     "Hashable",
     "Iterable",
     "Literal",
     "ModelField",
     "ModelResolver",
     "NamedTuple",
     "ObjectTypeInput",
     "OptimizedDjangoOptions",
-    "OptimizerKey",
     "Optional",
     "PK",
     "ParamSpec",
-    "QueryCache",
     "QuerySetResolver",
-    "TableName",
     "ToManyField",
     "ToOneField",
     "Type",
     "TypeGuard",
-    "TypeOptions",
     "TypeVar",
     "TypedDict",
     "Union",
     "UnmountedTypeInput",
     "cast",
     "overload",
 ]
 
 
 TModel = TypeVar("TModel", bound=Model)
-TableName: TypeAlias = str
-OptimizerKey: TypeAlias = str
 PK: TypeAlias = Any
-QueryCache: TypeAlias = dict[TableName, dict[OptimizerKey, dict[PK, TModel]]]
 ModelField: TypeAlias = Union[Field, ForeignObjectRel, "GenericForeignKey"]
 ToManyField: TypeAlias = Union["GenericRelation", ManyToManyField, ManyToOneRel, ManyToManyRel]
 ToOneField: TypeAlias = Union["GenericRelation", ForeignObject, ForeignKey, OneToOneField]
-TypeOptions: TypeAlias = Union[DjangoObjectTypeOptions, ConnectionOptions]
 AnyUser: TypeAlias = Union["User", "AnonymousUser"]
-FilterFields: TypeAlias = Union[dict[str, list[str]], list[str]]
 QuerySetResolver: TypeAlias = Callable[..., Union[QuerySet, Manager, None]]
 ModelResolver: TypeAlias = Callable[..., Union[Model, None]]
 ConnectionResolver: TypeAlias = Callable[..., ConnectionType]
-FieldNodes: TypeAlias = Iterable[Union[FieldNode, SelectionNode]]
 ObjectTypeInput: TypeAlias = Union[type[DjangoObjectType], str, Callable[[], type[DjangoObjectType]]]
 UnmountedTypeInput: TypeAlias = Union[type[UnmountedType], str, Callable[[], type[UnmountedType]]]
 Expr: TypeAlias = Union[models.Expression, models.F, models.Q]
 
 
 GRAPHQL_BUILTIN = (
     "__typename",
```

### Comparing `graphene_django_query_optimizer-0.4.2/query_optimizer/utils.py` & `graphene_django_query_optimizer-0.5.0/query_optimizer/utils.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.4.2/query_optimizer/validators.py` & `graphene_django_query_optimizer-0.5.0/query_optimizer/validators.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.4.2/PKG-INFO` & `graphene_django_query_optimizer-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphene-django-query-optimizer
-Version: 0.4.2
+Version: 0.5.0
 Summary: Automatically optimize SQL queries in Graphene-Django schemas.
 Home-page: https://mrthearman.github.io/graphene-django-query-optimizer
 License: MIT
 Keywords: django,graphene,sql,graphql,python,query,optimizer,optimization
 Author: Matti Lamppu
 Author-email: lamppu.matti.akseli@gmail.com
 Requires-Python: >=3.9,<4
```

