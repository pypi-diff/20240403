# Comparing `tmp/graphene_django_extensions-0.4.1.tar.gz` & `tmp/graphene_django_extensions-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphene_django_extensions-0.4.1.tar", max compression
+gzip compressed data, was "graphene_django_extensions-0.4.2.tar", max compression
```

## Comparing `graphene_django_extensions-0.4.1.tar` & `graphene_django_extensions-0.4.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1064 2024-03-21 06:40:19.663620 graphene_django_extensions-0.4.1/LICENSE
--rw-r--r--   0        0        0     4375 2024-03-21 06:40:19.663620 graphene_django_extensions-0.4.1/README.md
--rw-r--r--   0        0        0        0 2024-03-21 06:40:19.663620 graphene_django_extensions-0.4.1/gdx_pytest/__init__.py
--rw-r--r--   0        0        0      632 2024-03-21 06:40:19.663620 graphene_django_extensions-0.4.1/gdx_pytest/fixtures.py
--rw-r--r--   0        0        0      383 2024-03-21 06:40:19.663620 graphene_django_extensions-0.4.1/graphene_django_extensions/__init__.py
--rw-r--r--   0        0        0    31230 2024-03-21 06:40:19.667620 graphene_django_extensions-0.4.1/graphene_django_extensions/bases.py
--rw-r--r--   0        0        0      524 2024-03-21 06:40:19.667620 graphene_django_extensions-0.4.1/graphene_django_extensions/connections.py
--rw-r--r--   0        0        0      635 2024-03-21 06:40:19.667620 graphene_django_extensions-0.4.1/graphene_django_extensions/constants.py
--rw-r--r--   0        0        0    10013 2024-03-21 06:40:19.667620 graphene_django_extensions-0.4.1/graphene_django_extensions/converters.py
--rw-r--r--   0        0        0     7219 2024-03-21 06:40:19.667620 graphene_django_extensions-0.4.1/graphene_django_extensions/errors.py
--rw-r--r--   0        0        0      923 2024-03-21 06:40:19.667620 graphene_django_extensions-0.4.1/graphene_django_extensions/fields/__init__.py
--rw-r--r--   0        0        0     2765 2024-03-21 06:40:19.667620 graphene_django_extensions-0.4.1/graphene_django_extensions/fields/form.py
--rw-r--r--   0        0        0     6997 2024-03-21 06:40:19.667620 graphene_django_extensions-0.4.1/graphene_django_extensions/fields/graphql.py
--rw-r--r--   0        0        0     2760 2024-03-21 06:40:19.667620 graphene_django_extensions-0.4.1/graphene_django_extensions/fields/model.py
--rw-r--r--   0        0        0     3343 2024-03-21 06:40:19.667620 graphene_django_extensions-0.4.1/graphene_django_extensions/fields/serializer.py
--rw-r--r--   0        0        0     3882 2024-03-21 06:40:19.667620 graphene_django_extensions-0.4.1/graphene_django_extensions/files.py
--rw-r--r--   0        0        0    13174 2024-03-21 06:40:19.667620 graphene_django_extensions-0.4.1/graphene_django_extensions/filters.py
--rw-r--r--   0        0        0     3356 2024-03-21 06:40:19.667620 graphene_django_extensions-0.4.1/graphene_django_extensions/model_operations.py
--rw-r--r--   0        0        0     2012 2024-03-21 06:40:19.667620 graphene_django_extensions-0.4.1/graphene_django_extensions/options.py
--rw-r--r--   0        0        0     3694 2024-03-21 06:40:19.667620 graphene_django_extensions-0.4.1/graphene_django_extensions/permissions.py
--rw-r--r--   0        0        0        0 2024-03-21 06:40:19.667620 graphene_django_extensions-0.4.1/graphene_django_extensions/py.typed
--rw-r--r--   0        0        0    11264 2024-03-21 06:40:19.667620 graphene_django_extensions-0.4.1/graphene_django_extensions/serializers.py
--rw-r--r--   0        0        0     2662 2024-03-21 06:40:19.667620 graphene_django_extensions-0.4.1/graphene_django_extensions/settings.py
--rw-r--r--   0        0        0      367 2024-03-21 06:40:19.667620 graphene_django_extensions-0.4.1/graphene_django_extensions/testing/__init__.py
--rw-r--r--   0        0        0     8466 2024-03-21 06:40:19.667620 graphene_django_extensions-0.4.1/graphene_django_extensions/testing/builders.py
--rw-r--r--   0        0        0    13230 2024-03-21 06:40:19.667620 graphene_django_extensions-0.4.1/graphene_django_extensions/testing/client.py
--rw-r--r--   0        0        0     7286 2024-03-21 06:40:19.667620 graphene_django_extensions-0.4.1/graphene_django_extensions/testing/utils.py
--rw-r--r--   0        0        0     4660 2024-03-21 06:40:19.667620 graphene_django_extensions-0.4.1/graphene_django_extensions/typing.py
--rw-r--r--   0        0        0     5845 2024-03-21 06:40:19.667620 graphene_django_extensions-0.4.1/graphene_django_extensions/utils.py
--rw-r--r--   0        0        0     2924 2024-03-21 06:40:19.667620 graphene_django_extensions-0.4.1/graphene_django_extensions/views.py
--rw-r--r--   0        0        0     6817 2024-03-21 06:40:19.667620 graphene_django_extensions-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     6112 1970-01-01 00:00:00.000000 graphene_django_extensions-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/LICENSE
+-rw-r--r--   0        0        0     4375 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/gdx_pytest/__init__.py
+-rw-r--r--   0        0        0      632 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/gdx_pytest/fixtures.py
+-rw-r--r--   0        0        0      383 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/graphene_django_extensions/__init__.py
+-rw-r--r--   0        0        0    32115 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/graphene_django_extensions/bases.py
+-rw-r--r--   0        0        0      524 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/graphene_django_extensions/connections.py
+-rw-r--r--   0        0        0      635 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/graphene_django_extensions/constants.py
+-rw-r--r--   0        0        0    10013 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/graphene_django_extensions/converters.py
+-rw-r--r--   0        0        0     7331 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/graphene_django_extensions/errors.py
+-rw-r--r--   0        0        0      923 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/graphene_django_extensions/fields/__init__.py
+-rw-r--r--   0        0        0     2765 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/graphene_django_extensions/fields/form.py
+-rw-r--r--   0        0        0     6997 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/graphene_django_extensions/fields/graphql.py
+-rw-r--r--   0        0        0     2760 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/graphene_django_extensions/fields/model.py
+-rw-r--r--   0        0        0     3343 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/graphene_django_extensions/fields/serializer.py
+-rw-r--r--   0        0        0     3882 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/graphene_django_extensions/files.py
+-rw-r--r--   0        0        0    13174 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/graphene_django_extensions/filters.py
+-rw-r--r--   0        0        0     3356 2024-04-03 17:09:02.646790 graphene_django_extensions-0.4.2/graphene_django_extensions/model_operations.py
+-rw-r--r--   0        0        0     1745 2024-04-03 17:09:02.646790 graphene_django_extensions-0.4.2/graphene_django_extensions/options.py
+-rw-r--r--   0        0        0     3694 2024-04-03 17:09:02.646790 graphene_django_extensions-0.4.2/graphene_django_extensions/permissions.py
+-rw-r--r--   0        0        0        0 2024-04-03 17:09:02.646790 graphene_django_extensions-0.4.2/graphene_django_extensions/py.typed
+-rw-r--r--   0        0        0    11264 2024-04-03 17:09:02.646790 graphene_django_extensions-0.4.2/graphene_django_extensions/serializers.py
+-rw-r--r--   0        0        0     2722 2024-04-03 17:09:02.646790 graphene_django_extensions-0.4.2/graphene_django_extensions/settings.py
+-rw-r--r--   0        0        0      367 2024-04-03 17:09:02.646790 graphene_django_extensions-0.4.2/graphene_django_extensions/testing/__init__.py
+-rw-r--r--   0        0        0     8466 2024-04-03 17:09:02.646790 graphene_django_extensions-0.4.2/graphene_django_extensions/testing/builders.py
+-rw-r--r--   0        0        0    14361 2024-04-03 17:09:02.646790 graphene_django_extensions-0.4.2/graphene_django_extensions/testing/client.py
+-rw-r--r--   0        0        0     7286 2024-04-03 17:09:02.646790 graphene_django_extensions-0.4.2/graphene_django_extensions/testing/utils.py
+-rw-r--r--   0        0        0     4660 2024-04-03 17:09:02.646790 graphene_django_extensions-0.4.2/graphene_django_extensions/typing.py
+-rw-r--r--   0        0        0     5845 2024-04-03 17:09:02.646790 graphene_django_extensions-0.4.2/graphene_django_extensions/utils.py
+-rw-r--r--   0        0        0     2924 2024-04-03 17:09:02.646790 graphene_django_extensions-0.4.2/graphene_django_extensions/views.py
+-rw-r--r--   0        0        0     6817 2024-04-03 17:09:02.646790 graphene_django_extensions-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     6112 1970-01-01 00:00:00.000000 graphene_django_extensions-0.4.2/PKG-INFO
```

### Comparing `graphene_django_extensions-0.4.1/LICENSE` & `graphene_django_extensions-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.1/README.md` & `graphene_django_extensions-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.1/gdx_pytest/fixtures.py` & `graphene_django_extensions-0.4.2/gdx_pytest/fixtures.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.1/graphene_django_extensions/bases.py` & `graphene_django_extensions-0.4.2/graphene_django_extensions/bases.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 from __future__ import annotations
 
+import warnings
 from enum import Enum
 from functools import partial
 from typing import TYPE_CHECKING
 
 import graphene
 from django.forms import Form, ModelForm
 from graphene import Field, InputField, InputObjectType, Mutation
 from graphene.types.resolver import attr_resolver
 from graphene.types.utils import yank_fields_from_attrs
-from graphene_django import DjangoObjectType
 from graphene_django.converter import convert_django_field
 from graphene_django.forms.mutation import fields_for_form
 from graphene_django.registry import get_global_registry
 from graphene_django.rest_framework.mutation import fields_for_serializer
 from graphene_django.types import ALL_FIELDS
 from graphene_django.utils import is_valid_django_model
 from graphql_relay import to_global_id
-from query_optimizer import DjangoConnectionField, DjangoListField, optimize_single
-from query_optimizer.settings import optimizer_settings
+from query_optimizer import DjangoConnectionField, DjangoListField, DjangoObjectType
 from rest_framework.exceptions import ValidationError as SerializerValidationError
 from rest_framework.fields import SerializerMethodField, get_attribute
 from rest_framework.serializers import ListSerializer, ModelSerializer, Serializer
 
 from .connections import Connection
 from .converters import convert_form_fields_to_not_required, convert_serializer_fields_to_not_required
-from .errors import GQLPermissionDeniedError, validation_errors_to_graphql_errors
+from .errors import GDXWarning, GQLPermissionDeniedError, validation_errors_to_graphql_errors
 from .fields import RelatedField
 from .model_operations import get_model_lookup_field, get_object_or_404
 from .options import DjangoMutationOptions, DjangoNodeOptions
 from .permissions import AllowAny, BasePermission, restricted_field
 from .settings import gdx_settings
 from .typing import Fields, GQLFields, Sequence
 from .utils import add_translatable_fields, get_filter_info
@@ -113,21 +112,21 @@
 
     @classmethod
     def filter_queryset(cls, queryset: models.QuerySet, info: GQLInfo) -> models.QuerySet:
         """Implement this method filter to the available rows from the model on this node."""
         return queryset
 
     @classmethod
-    def __init_subclass_with_meta__(  # noqa: PLR0913
+    def __init_subclass_with_meta__(
         cls,
+        _meta: DjangoNodeOptions | None = None,
         model: type[models.Model] | None = None,
         fields: Fields | None = None,
         permission_classes: Sequence[type[BasePermission]] = (AllowAny,),
         restricted_fields: dict[FieldNameStr, PermCheck] | None = None,
-        max_complexity: int | None = None,
         **options: Any,
     ) -> None:
         if model is None:  # pragma: no cover
             msg = "`Meta.model` is required."
             raise ValueError(msg)
 
         if not is_valid_django_model(model):  # pragma: no cover
@@ -141,44 +140,31 @@
         if not (fields == ALL_FIELDS or isinstance(fields, Sequence)):  # pragma: no cover
             msg = f"`Meta.fields` is should be a Sequence of field names or `{ALL_FIELDS}`, received: `{fields}`."
             raise TypeError(msg)
 
         if fields != ALL_FIELDS:
             fields = add_translatable_fields(model, fields)
 
-        if not hasattr(cls, "pk") and (fields == ALL_FIELDS or "pk" in fields):
-            cls._add_pk_field(model)
-
         if restricted_fields is not None:
             cls._add_field_restrictions(fields, restricted_fields)
 
-        _meta = DjangoNodeOptions(
-            class_type=cls,
-            max_complexity=max_complexity or optimizer_settings.MAX_COMPLEXITY,
-            permission_classes=permission_classes,
-        )
-        options.setdefault("connection_class", Connection)
-        options.setdefault("interfaces", (graphene.relay.Node,))
+        if _meta is None:
+            _meta = DjangoNodeOptions(cls)
 
-        filterset_class = options.get("filterset_class", None)
-        filter_fields: dict[str, list[str]] | None = options.pop("filter_fields", None)
+        _meta.permission_classes = permission_classes
 
-        if filterset_class is None and filter_fields is not None:  # pragma: no cover
-            from query_optimizer.filter import create_filterset
+        options.setdefault("connection_class", Connection)
+        options.setdefault("interfaces", (graphene.relay.Node,))
 
-            options["filterset_class"] = create_filterset(model, filter_fields)
+        if not options.get("skip_registry", False):
+            _check_if_model_already_registered(cls, model)
 
         super().__init_subclass_with_meta__(_meta=_meta, model=model, fields=fields, **options)
 
     @classmethod
-    def _add_pk_field(cls, model: type[models.Model]) -> None:
-        cls.pk = graphene.Int() if model._meta.pk.name == "id" else graphene.ID()
-        cls.resolve_pk = cls.resolve_id
-
-    @classmethod
     def _add_field_restrictions(cls, fields: Fields, restricted_fields: dict[FieldNameStr, PermCheck]) -> None:
         for field_name, check in restricted_fields.items():
             if fields != ALL_FIELDS and field_name not in fields:  # pragma: no cover
                 msg = f"Field `{field_name}` not in `Meta.fields`."
                 raise ValueError(msg)
 
             resolver = getattr(cls, f"resolve_{field_name}", None)
@@ -194,24 +180,20 @@
             raise GQLPermissionDeniedError(
                 message=gdx_settings.FILTER_PERMISSION_ERROR_MESSAGE,
                 code=gdx_settings.FILTER_PERMISSION_ERROR_CODE,
             )
         return queryset
 
     @classmethod
-    def get_node(cls, info: GQLInfo, pk: Any) -> models.Model | None:
-        """Override `filter_queryset` instead of this method to add filtering of possible rows."""
-        queryset = cls._meta.model._default_manager.all()
-        instance = optimize_single(queryset, info, pk=pk, max_complexity=cls._meta.max_complexity)
-        if instance is not None and not cls.has_node_permissions(info, instance):
+    def run_instance_checks(cls, instance: models.Model, info: GQLInfo) -> None:
+        if not cls.has_node_permissions(info, instance):
             raise GQLPermissionDeniedError(
                 message=gdx_settings.QUERY_PERMISSION_ERROR_MESSAGE,
                 code=gdx_settings.QUERY_PERMISSION_ERROR_CODE,
             )
-        return instance
 
     @classmethod
     def has_node_permissions(cls, info: GQLInfo, instance: models.Model) -> bool:
         """Check which permissions are required to access single items of this type."""
         filters = get_filter_info(info)
         return all(
             perm.has_node_permission(
@@ -773,7 +755,39 @@
                 f"Make sure that the ObjectType for this model is registered before the "
                 f"`{mutation_class.__name__}` mutation class is crated. This can be achieved by "
                 f"importing the ObjectType before the mutation class is created."
             )
             raise LookupError(msg)
 
         _check_serializer_field_models_in_registry(mutation_class, field)
+
+
+def _check_if_model_already_registered(object_type: type[DjangoObjectType], model: type[models.Model]) -> None:
+    # This function is only used to check if an object type for a django model already exists in the registry.
+    # In this case, the former object type is replaced with the new one, which can lead to
+    # unexpected behavior if the object types are not identical.
+    global_registry = get_global_registry()
+    existing = global_registry.get_type_for_model(model)
+    if existing is not None:  # pragma: no cover
+        model_path = f"{model.__module__}.{model.__name__}"
+        exising_path = f"{existing.__module__}.{existing.__name__}"
+        new_path = f"{object_type.__module__}.{object_type.__name__}"
+        msg = (
+            f"An object type `{exising_path}` for model `{model_path}` is already registered. "
+            f"This will be replaced with the new object type: `{new_path}`. "
+            f"This means that the latter will be used when automatically determining object types for "
+            f"related model fields in other object types. "
+        )
+        if gdx_settings.ALLOW_MODEL_OBJECT_TYPE_REGISTRY_OVERRIDES:
+            msg += (
+                "The former object type can still be used, but it needs to be defined "
+                "on the other object type explicitly. This warning exists to notify of possible "
+                "unexpected behavior, but if you know what you are doing, you can ignore it. "
+                "You might consider using proxy-models, since they won't cause this issue."
+            )
+            warnings.warn(message=msg, category=GDXWarning, stacklevel=5)  # point to the object type definition
+        else:
+            msg += (
+                "Since this can lead to unexpected behavior, you should either use the existing object type "
+                "or use proxy models to avoid this issue."
+            )
+            raise LookupError(msg)
```

### Comparing `graphene_django_extensions-0.4.1/graphene_django_extensions/connections.py` & `graphene_django_extensions-0.4.2/graphene_django_extensions/connections.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.1/graphene_django_extensions/constants.py` & `graphene_django_extensions-0.4.2/graphene_django_extensions/constants.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.1/graphene_django_extensions/converters.py` & `graphene_django_extensions-0.4.2/graphene_django_extensions/converters.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.1/graphene_django_extensions/errors.py` & `graphene_django_extensions-0.4.2/graphene_django_extensions/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     from .typing import Callable, ParamSpec, SerializerErrorData, TypeVar, ValidationErrorType
 
     T = TypeVar("T")
     P = ParamSpec("P")
 
 
 __all__ = [
+    "GDXWarning",
     "get_constraint_message",
     "GQLNotFoundError",
     "GQLPermissionDeniedError",
     "GQLValidationError",
 ]
 
 
@@ -58,14 +59,18 @@
         errors = to_field_errors(detail)
         super().__init__(
             gdx_settings.MUTATION_VALIDATION_ERROR_MESSAGE,
             extensions={"code": gdx_settings.MUTATION_VALIDATION_ERROR_CODE, "errors": errors},
         )
 
 
+class GDXWarning(UserWarning):
+    """Base warning class for graphene-django-extensions."""
+
+
 def validation_errors_to_graphql_errors(func: Callable[P, T]) -> Callable[P, T]:
     @wraps(func)
     def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
         try:
             return func(*args, **kwargs)
         except (DjangoValidationError, SerializerValidationError) as error:
             raise GQLValidationError(error) from error
```

### Comparing `graphene_django_extensions-0.4.1/graphene_django_extensions/fields/__init__.py` & `graphene_django_extensions-0.4.2/graphene_django_extensions/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.1/graphene_django_extensions/fields/form.py` & `graphene_django_extensions-0.4.2/graphene_django_extensions/fields/form.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.1/graphene_django_extensions/fields/graphql.py` & `graphene_django_extensions-0.4.2/graphene_django_extensions/fields/graphql.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.1/graphene_django_extensions/fields/model.py` & `graphene_django_extensions-0.4.2/graphene_django_extensions/fields/model.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.1/graphene_django_extensions/fields/serializer.py` & `graphene_django_extensions-0.4.2/graphene_django_extensions/fields/serializer.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.1/graphene_django_extensions/files.py` & `graphene_django_extensions-0.4.2/graphene_django_extensions/files.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.1/graphene_django_extensions/filters.py` & `graphene_django_extensions-0.4.2/graphene_django_extensions/filters.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.1/graphene_django_extensions/model_operations.py` & `graphene_django_extensions-0.4.2/graphene_django_extensions/model_operations.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.1/graphene_django_extensions/options.py` & `graphene_django_extensions-0.4.2/graphene_django_extensions/options.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,33 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from graphene.types.mutation import MutationOptions
-from graphene_django.types import DjangoObjectTypeOptions
+from query_optimizer.typing import OptimizedDjangoOptions
 
 if TYPE_CHECKING:
     from django.db import models
     from django.forms import Form, ModelForm
     from rest_framework.serializers import ModelSerializer, Serializer
 
     from graphene_django_extensions.permissions import BasePermission
 
-    from .bases import DjangoMutation, DjangoNode
+    from .bases import DjangoMutation
     from .typing import FieldNameStr, Literal, Sequence
 
 
 __all__ = [
     "DjangoNodeOptions",
     "DjangoMutationOptions",
 ]
 
 
-class DjangoNodeOptions(DjangoObjectTypeOptions):
-    def __init__(
-        self,
-        class_type: type[DjangoNode],
-        max_complexity: int,
-        permission_classes: Sequence[type[BasePermission]] = (),
-    ) -> None:
-        self.max_complexity = max_complexity
-        self.permission_classes = permission_classes
-        super().__init__(class_type)
+class DjangoNodeOptions(OptimizedDjangoOptions):
+    permission_classes: Sequence[type[BasePermission]] = ()
 
 
 class DjangoMutationOptions(MutationOptions):
     def __init__(  # noqa: PLR0913
         self,
         class_type: type[DjangoMutation],
         lookup_field: FieldNameStr | None,
```

### Comparing `graphene_django_extensions-0.4.1/graphene_django_extensions/permissions.py` & `graphene_django_extensions-0.4.2/graphene_django_extensions/permissions.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.1/graphene_django_extensions/serializers.py` & `graphene_django_extensions-0.4.2/graphene_django_extensions/serializers.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.1/graphene_django_extensions/settings.py` & `graphene_django_extensions-0.4.2/graphene_django_extensions/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     DELETE_PERMISSION_ERROR_MESSAGE: str = "No permission to delete."
     DELETE_PERMISSION_ERROR_CODE: str = "DELETE_PERMISSION_DENIED"
     MUTATION_VALIDATION_ERROR_MESSAGE: str = "Mutation was unsuccessful."
     MUTATION_VALIDATION_ERROR_CODE: str = "MUTATION_VALIDATION_ERROR"
     NOT_FOUND_ERROR_CODE: str = "NOT_FOUND"
     ORDERING_FILTER_NAME: str = "order_by"
     EXTEND_USER_DEFINED_FILTER_OPERATIONS: list[str] | None = None
+    ALLOW_MODEL_OBJECT_TYPE_REGISTRY_OVERRIDES: bool = True
 
 
 DEFAULTS: dict[str, Any] = DefaultSettings()._asdict()
 
 IMPORT_STRINGS: set[Union[bytes, str]] = set()
 REMOVED_SETTINGS: set[str] = {
     "PERMISSION_DENIED_MESSAGE",
```

### Comparing `graphene_django_extensions-0.4.1/graphene_django_extensions/testing/builders.py` & `graphene_django_extensions-0.4.2/graphene_django_extensions/testing/builders.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.1/graphene_django_extensions/testing/client.py` & `graphene_django_extensions-0.4.2/graphene_django_extensions/testing/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,44 @@
 from __future__ import annotations
 
 import json
+import re
 from typing import TYPE_CHECKING
 
 import pytest
 from django.contrib.auth import get_user_model
 from django.test.client import MULTIPART_CONTENT, Client
 from graphene_django.settings import graphene_settings
 
 from ..files import extract_files
 from .utils import QueryData, capture_database_queries
 
 if TYPE_CHECKING:
-    from django.contrib.auth.models import User
     from django.core.files import File
     from django.http import HttpResponse
 
     from ..typing import Any, ClassVar, FieldError, Self
 
+
+User = get_user_model()
+
+
 __all__ = [
     "GraphQLClient",
 ]
 
 
+SCHEMA_ERRORS: list[re.Pattern] = [
+    # These do not cover all schema errors, only the most common ones.
+    re.compile(r"^Argument '\w+' .*"),
+    re.compile(r"^Variable '\$\w+' .*"),
+    re.compile(r"^\w+ cannot represent .*"),
+]
+
+
 class GQLResponse:
     def __init__(self, response: HttpResponse, query_data: QueryData) -> None:
         # 'django.test.client.Client.request' sets json attribute on the response.
         self.json: dict[str, Any] = response.json()  # type: ignore[attr-defined]
         self.query_data = query_data
 
     def __str__(self) -> str:
@@ -295,14 +307,29 @@
                     codes.append(error["code"])
                 except (KeyError, TypeError):
                     msg = f"Error code for field {field!r} not found in error: {error}"
                     pytest.fail(msg, pytrace=False)
 
         return codes
 
+    @property
+    def has_schema_errors(self) -> bool:
+        """
+        Return True if there are any known GraphQL schema validation errors in the response.
+
+        >>> self.json = {"errors": [{"message": "bar", ...}]}
+        >>> self.has_schema_errors
+        False
+
+        >>> self.json = {"errors": [{"message": f"Variable '$input' got invalid value...", ...}]}
+        >>> self.has_schema_errors
+        True
+        """
+        return any(any(e.match(error["message"]) is not None for e in SCHEMA_ERRORS) for error in self.errors)
+
     def assert_query_count(self, count: int) -> None:  # pragma: no cover
         if len(self.queries) != count:
             msg = f"Expected {count} queries, got {len(self.queries)}.\n{self.query_log}"
             pytest.fail(msg, pytrace=False)
 
 
 class GraphQLClient(Client):
@@ -357,16 +384,28 @@
                 data=data,
                 content_type=MULTIPART_CONTENT if files else "application/json",
                 headers=headers,
             )
 
         return self.response_class(response, results)
 
-    def login_with_superuser(self) -> User:
-        user = get_user_model().objects.create_superuser(username="superuser", email="superuser@django.com")
+    def login_with_superuser(self, username: str = "admin", **kwargs: Any) -> User:
+        defaults = {
+            "is_staff": True,
+            "is_superuser": True,
+            "email": "superuser@django.com",
+            **kwargs,
+        }
+        user, _ = User.objects.get_or_create(username=username, defaults=defaults)
         self.force_login(user)
         return user
 
-    def login_with_regular_user(self) -> User:
-        user = get_user_model().objects.create_user(username="user", email="user@django.com")
+    def login_with_regular_user(self, username: str = "user", **kwargs: Any) -> User:
+        defaults = {
+            "is_staff": False,
+            "is_superuser": False,
+            "email": "user@django.com",
+            **kwargs,
+        }
+        user, _ = User.objects.get_or_create(username=username, defaults=defaults)
         self.force_login(user)
         return user
```

### Comparing `graphene_django_extensions-0.4.1/graphene_django_extensions/testing/utils.py` & `graphene_django_extensions-0.4.2/graphene_django_extensions/testing/utils.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.1/graphene_django_extensions/typing.py` & `graphene_django_extensions-0.4.2/graphene_django_extensions/typing.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.1/graphene_django_extensions/utils.py` & `graphene_django_extensions-0.4.2/graphene_django_extensions/utils.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.1/graphene_django_extensions/views.py` & `graphene_django_extensions-0.4.2/graphene_django_extensions/views.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.1/pyproject.toml` & `graphene_django_extensions-0.4.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "graphene-django-extensions"
-version = "0.4.1"
+version = "0.4.2"
 description = "Extensions for graphene-django"
 authors = [
     "Matti Lamppu <lamppu.matti.akseli@gmail.com>",
 ]
 packages = [
     { include = "graphene_django_extensions" },
     { include = "gdx_pytest" },
@@ -54,27 +54,27 @@
 graphene_django_extensions = "gdx_pytest.fixtures"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4"
 Django = ">=4.2"
 djangorestframework = ">=3.14.0"
 graphene-django = ">=3.0.0"
-graphene-django-query-optimizer = ">=0.4.0"
+graphene-django-query-optimizer = ">=0.5.0"
 django-settings-holder = ">=0.1.2"
 django-filter = ">=23.5"
 typing-extensions = { version = ">=4.4.0", python = "<3.11" }
 django-modeltranslation = { version = ">=0.18.11", optional = true }
 pillow = { version = ">=10.2.0", optional = true }
 
 [tool.poetry.group.test.dependencies]
 pytest = "8.1.1"
 coverage = "7.4.4"
 pytest-django = "4.8.0"
-pre-commit = "3.6.2"
-tox = "4.14.1"
+pre-commit = "3.7.0"
+tox = "4.14.2"
 tox-gh-actions = "3.2.0"
 factory-boy = "3.3.0"
 django-graphiql-debug-toolbar = "0.2.0"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "1.5.3"
 pymdown-extensions = "10.7.1"
```

### Comparing `graphene_django_extensions-0.4.1/PKG-INFO` & `graphene_django_extensions-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphene-django-extensions
-Version: 0.4.1
+Version: 0.4.2
 Summary: Extensions for graphene-django
 Home-page: https://mrthearman.github.io/graphene-django-extensions
 License: MIT
 Keywords: django,graphene,extensions,graphql,graphene-django,mutations,queries,object_types,fields
 Author: Matti Lamppu
 Author-email: lamppu.matti.akseli@gmail.com
 Requires-Python: >=3.10,<4
@@ -26,15 +26,15 @@
 Provides-Extra: translation
 Requires-Dist: Django (>=4.2)
 Requires-Dist: django-filter (>=23.5)
 Requires-Dist: django-modeltranslation (>=0.18.11) ; extra == "translation"
 Requires-Dist: django-settings-holder (>=0.1.2)
 Requires-Dist: djangorestframework (>=3.14.0)
 Requires-Dist: graphene-django (>=3.0.0)
-Requires-Dist: graphene-django-query-optimizer (>=0.4.0)
+Requires-Dist: graphene-django-query-optimizer (>=0.5.0)
 Requires-Dist: pillow (>=10.2.0) ; extra == "files"
 Requires-Dist: typing-extensions (>=4.4.0) ; python_version < "3.11"
 Project-URL: Bug Tracker, https://github.com/MrThearMan/graphene-django-extensions/issues
 Project-URL: Repository, https://github.com/MrThearMan/graphene-django-extensions
 Description-Content-Type: text/markdown
 
 # Graphene Django Extensions
```

