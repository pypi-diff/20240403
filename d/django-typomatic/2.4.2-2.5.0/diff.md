# Comparing `tmp/django-typomatic-2.4.2.tar.gz` & `tmp/django-typomatic-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-typomatic-2.4.2.tar", last modified: Wed Sep 13 22:12:24 2023, max compression
+gzip compressed data, was "django-typomatic-2.5.0.tar", last modified: Tue Apr  2 22:44:54 2024, max compression
```

## Comparing `django-typomatic-2.4.2.tar` & `django-typomatic-2.5.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 22:12:24.392146 django-typomatic-2.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-09-13 22:12:06.000000 django-typomatic-2.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9838 2023-09-13 22:12:24.392146 django-typomatic-2.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9419 2023-09-13 22:12:06.000000 django-typomatic-2.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 22:12:24.392146 django-typomatic-2.4.2/django_typomatic/
--rw-r--r--   0 runner    (1001) docker     (127)    23300 2023-09-13 22:12:06.000000 django-typomatic-2.4.2/django_typomatic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 22:12:24.392146 django-typomatic-2.4.2/django_typomatic/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-13 22:12:06.000000 django-typomatic-2.4.2/django_typomatic/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2023-09-13 22:12:06.000000 django-typomatic-2.4.2/django_typomatic/management/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 22:12:24.392146 django-typomatic-2.4.2/django_typomatic/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-13 22:12:06.000000 django-typomatic-2.4.2/django_typomatic/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5362 2023-09-13 22:12:06.000000 django-typomatic-2.4.2/django_typomatic/management/commands/generate_ts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2023-09-13 22:12:06.000000 django-typomatic-2.4.2/django_typomatic/management/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 22:12:24.392146 django-typomatic-2.4.2/django_typomatic/management/settings/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2023-09-13 22:12:06.000000 django-typomatic-2.4.2/django_typomatic/management/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2023-09-13 22:12:06.000000 django-typomatic-2.4.2/django_typomatic/mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)    12097 2023-09-13 22:12:06.000000 django-typomatic-2.4.2/django_typomatic/test__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 22:12:24.392146 django-typomatic-2.4.2/django_typomatic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9838 2023-09-13 22:12:24.000000 django-typomatic-2.4.2/django_typomatic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      619 2023-09-13 22:12:24.000000 django-typomatic-2.4.2/django_typomatic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-13 22:12:24.000000 django-typomatic-2.4.2/django_typomatic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-13 22:12:24.000000 django-typomatic-2.4.2/django_typomatic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-09-13 22:12:24.000000 django-typomatic-2.4.2/django_typomatic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-09-13 22:12:24.000000 django-typomatic-2.4.2/django_typomatic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-13 22:12:24.392146 django-typomatic-2.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      789 2023-09-13 22:12:06.000000 django-typomatic-2.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:44:54.832271 django-typomatic-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-02 22:44:45.000000 django-typomatic-2.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9911 2024-04-02 22:44:54.832271 django-typomatic-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9435 2024-04-02 22:44:45.000000 django-typomatic-2.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:44:54.832271 django-typomatic-2.5.0/django_typomatic/
+-rw-r--r--   0 runner    (1001) docker     (127)    25266 2024-04-02 22:44:45.000000 django-typomatic-2.5.0/django_typomatic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-02 22:44:45.000000 django-typomatic-2.5.0/django_typomatic/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:44:54.832271 django-typomatic-2.5.0/django_typomatic/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 22:44:45.000000 django-typomatic-2.5.0/django_typomatic/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-02 22:44:45.000000 django-typomatic-2.5.0/django_typomatic/management/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:44:54.832271 django-typomatic-2.5.0/django_typomatic/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 22:44:45.000000 django-typomatic-2.5.0/django_typomatic/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-04-02 22:44:45.000000 django-typomatic-2.5.0/django_typomatic/management/commands/generate_ts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-02 22:44:45.000000 django-typomatic-2.5.0/django_typomatic/management/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:44:54.832271 django-typomatic-2.5.0/django_typomatic/management/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-02 22:44:45.000000 django-typomatic-2.5.0/django_typomatic/management/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-02 22:44:45.000000 django-typomatic-2.5.0/django_typomatic/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12097 2024-04-02 22:44:45.000000 django-typomatic-2.5.0/django_typomatic/test__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:44:54.832271 django-typomatic-2.5.0/django_typomatic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9911 2024-04-02 22:44:54.000000 django-typomatic-2.5.0/django_typomatic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-02 22:44:54.000000 django-typomatic-2.5.0/django_typomatic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 22:44:54.000000 django-typomatic-2.5.0/django_typomatic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 22:44:54.000000 django-typomatic-2.5.0/django_typomatic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 22:44:54.000000 django-typomatic-2.5.0/django_typomatic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-02 22:44:54.000000 django-typomatic-2.5.0/django_typomatic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 22:44:54.832271 django-typomatic-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-02 22:44:45.000000 django-typomatic-2.5.0/setup.py
```

### Comparing `django-typomatic-2.4.2/LICENSE` & `django-typomatic-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-typomatic-2.4.2/PKG-INFO` & `django-typomatic-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: django-typomatic
-Version: 2.4.2
+Version: 2.5.0
 Summary: A simple solution for generating Typescript interfaces from your Django Rest Framework Serializers.
 Home-page: https://github.com/adenh93/django-typomatic
 Author: Aden Herold
 Author-email: aden.herold1@gmail.com
 Keywords: Django,Django Rest Framework,DRF,Typescript,Python
 Platform: any
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: django
+Requires-Dist: djangorestframework
 
 # django-typomatic ![pypi badge](https://img.shields.io/pypi/v/django-typomatic)
 
 _A simple solution for generating Typescript interfaces from your [Django Rest Framework Serializers](https://www.django-rest-framework.org/api-guide/serializers/)._
 
 Since I now require a simple package to generate Typescript interfaces for Django Rest Framework serializers, I've decided to port over my [Typemallow](https://github.com/adenh93/typemallow/) package for use with DRF serializers!
 
@@ -322,22 +324,22 @@
 
 You can also generate modules separately, as an example, `-s user` will restrict generation to all serializers in the `user` application, and `-s user.UserSerializer` will restrict generation to just the `UserSerializer` serializer belonging to the `user` application.
 
 ### Examples
 
 _Generate TS for `user` app_
 
-`./manage.py generate_ts -s user`
+`./manage.py generate_ts --app_name user`
 
 _Generate TS for specific serializer from user app_
 
 `./manage.py generate_ts -s user.UserSerializer`
 
 _Generate TS for many apps or serializers_
 
 `./manage.py generate_ts -s user.UserSerializer group role.RoleSerializer role.RoleListSerializer`
 
 _Generate TS for user app with annotations, choices enums, trim serializer, camelize, enum values and custom output path_
 
-`./manage.py generate_ts -s user -a -ec -t -c -ev -o "./custom_folder/"`
+`./manage.py generate_ts --app_name user -a -ec -t -c -ev -o "./custom_folder/"`
```

### Comparing `django-typomatic-2.4.2/README.md` & `django-typomatic-2.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -310,22 +310,22 @@
 
 You can also generate modules separately, as an example, `-s user` will restrict generation to all serializers in the `user` application, and `-s user.UserSerializer` will restrict generation to just the `UserSerializer` serializer belonging to the `user` application.
 
 ### Examples
 
 _Generate TS for `user` app_
 
-`./manage.py generate_ts -s user`
+`./manage.py generate_ts --app_name user`
 
 _Generate TS for specific serializer from user app_
 
 `./manage.py generate_ts -s user.UserSerializer`
 
 _Generate TS for many apps or serializers_
 
 `./manage.py generate_ts -s user.UserSerializer group role.RoleSerializer role.RoleListSerializer`
 
 _Generate TS for user app with annotations, choices enums, trim serializer, camelize, enum values and custom output path_
 
-`./manage.py generate_ts -s user -a -ec -t -c -ev -o "./custom_folder/"`
+`./manage.py generate_ts --app_name user -a -ec -t -c -ev -o "./custom_folder/"`
```

### Comparing `django-typomatic-2.4.2/django_typomatic/__init__.py` & `django-typomatic-2.5.0/django_typomatic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 from pathlib import Path
 
 from rest_framework import serializers
 from rest_framework.serializers import BaseSerializer
 from rest_framework.fields import empty
 
+from django.db.models import OneToOneField
 from django.db.models.enums import Choices
 import inspect
 
 from typing import get_type_hints, get_origin, get_args
 
 from .mappings import mappings, format_mappings, primitives_mapping
 
@@ -16,14 +17,16 @@
 
 # Serializers
 __serializers = dict()
 # Custom serializers.Field to TS Type mappings
 __field_mappings = dict()
 # Custom field_name to TS Type overrides
 __mapping_overrides = dict()
+# TS Type imports import
+__imports = dict()
 
 
 def ts_field(ts_type: str, context='default'):
     '''
     Any valid Django Rest Framework Serializer Field with this class decorator will
     be added to a list in a __field_mappings dictionary.
     Useful to define the type mapping of custom serializer Fields.
@@ -202,40 +205,63 @@
         else:
             choices_enum = choices_enum + f"    {str(value).upper().replace(' ', '_')} = {key},\n"
     choices_enum = choices_enum + "}\n"
 
     return choices_enum
 
 
+def __is_known_serializer_type(serializer_type, context):
+    for _context, serializers in __serializers.items():
+        if serializer_type in serializers:
+            imports = __imports.get(context, {})
+            type_imports = imports.get(_context, set())
+            type_imports.add(serializer_type)
+            imports[_context] = type_imports
+            __imports[context] = imports
+            return True
+    return False
+
+
 def __process_field(field_name, field, context, serializer, trim_serializer_output, camelize,
                     enum_choices, enum_values, enum_keys):
     '''
     Generates and returns a tuple representing the Typescript field name and Type.
     '''
-    if hasattr(field, 'child'):
+    # For PrimaryKeyRelatedField, set field_type to the type of the primary key
+    # on the related model
+    if isinstance(field, serializers.PrimaryKeyRelatedField) and field.queryset:
+        is_many = False
+
+        target_field = field.queryset.model._meta.pk
+        while isinstance(target_field, OneToOneField):
+            # Recurse into the parent model the field is inheriting from
+            target_field = target_field.model._meta.pk.target_field
+
+        field_type = type(target_field)
+    elif hasattr(field, 'child'):
         is_many = True
         field_type = type(field.child)
     elif hasattr(field, 'child_relation'):
         is_many = True
         field_type = type(field.child_relation)
     else:
         is_many = False
         field_type = type(field)
 
-    if field_type in __serializers[context]:
+    if field_type in __serializers[context] or __is_known_serializer_type(field_type, context):
         ts_type = __get_trimmed_name(
             field_type.__name__, trim_serializer_output)
     elif field_type in __field_mappings[context]:
         ts_type = __field_mappings[context].get(field_type, 'any')
     elif (context in __mapping_overrides) and (serializer in __mapping_overrides[context]) \
             and field_name in __mapping_overrides[context][serializer]:
         ts_type = __mapping_overrides[context][serializer].get(
             field_name, 'any')
     elif field_type == serializers.PrimaryKeyRelatedField:
-        ts_type = "number | string"
+        ts_type = "number"
     elif hasattr(field, 'choice_strings_to_values') and enum_choices:
         ts_type = f"{''.join(x.title() for x in field_name.split('_'))}ChoiceEnum"
     elif hasattr(field, 'choice_strings_to_values') and enum_choices and enum_values \
             and not enum_keys:
         ts_type = f"{''.join(x.title() for x in field_name.split('_'))}ChoiceEnumValues"
     elif hasattr(field, 'choice_strings_to_values') and enum_keys:
         ts_type = f"{''.join(x.title() for x in field_name.split('_'))}ChoiceEnumKeys"
@@ -257,15 +283,18 @@
 
     return field_name, ts_type
 
 
 def __get_nested_serializer_field(context, enum_choices, enum_values, enum_keys, field, field_name,
                                   is_many, serializer, trim_serializer_output):
     types = []
-    field_function = getattr(serializer, f'get_{field_name}')
+    if field.method_name:
+        field_function = getattr(serializer, field.method_name)
+    else:
+        field_function = getattr(serializer, f'get_{field_name}')
     return_type = get_type_hints(field_function).get('return')
     is_generic_type = hasattr(return_type, '__origin__')
     is_serializer_type = False
     many = False
     # TODO type pass recursively to represent something like a list from a list e.g. List[List[int]]
     if is_generic_type:
         return_type, many = __process_generic_type(return_type)
@@ -295,19 +324,20 @@
 
         if issubclass(return_type, BaseSerializer):
             is_external_serializer = return_type.__module__.replace('.serializers',
                                                                     '') != context
             is_serializer_type = True
 
             if is_external_serializer and return_type not in __serializers.get(context, []):
-                # TODO import external interface, not duplicate
-                # Include external Interface
-                ts_interface(context=context)(return_type)
-                # For duplicate interface, set not exported
-                setattr(return_type, '__exported__', False)
+                # Import the serializer if it was previously generated
+                if not __is_known_serializer_type(return_type, context):
+                    # Include external Interface
+                    ts_interface(context=context)(return_type)
+                    # For duplicate interface, set not exported
+                    setattr(return_type, '__exported__', False)
 
         if is_serializer_type:
             ts_type = __get_trimmed_name(return_type.__name__, trim_serializer_output)
             is_many = many
 
         types.append(ts_type)
     else:
@@ -388,15 +418,15 @@
     through the serializer fields of the DRF Serializer class
     passed in as a parameter, and mapping them to the appropriate Typescript
     data type.
     '''
     name = __get_trimmed_name(serializer.__name__, trim_serializer_output)
     _LOG.debug(f"Creating interface for {name}")
     fields = []
-    if hasattr(serializer, 'get_fields'):
+    if hasattr(serializer, 'get_fields') and hasattr(serializer, 'Meta') and hasattr(serializer.Meta, 'model'):
         instance = serializer()
         fields = instance.get_fields().items()
     else:
         fields = serializer._declared_fields.items()
     ts_fields = []
     for key, value in fields:
         ts_property, ts_type = __process_field(key, value, context, serializer,
@@ -416,14 +446,30 @@
 
         ts_fields.append(f"    {ts_property}: {ts_type};")
     collapsed_fields = '\n'.join(ts_fields)
     exported = getattr(serializer, '__exported__', True)
     return f'{"export " if exported else ""}interface {name} {{\n{collapsed_fields}\n}}\n\n'
 
 
+def __generate_imports(context, trim_serializer_output):
+    imports_str = ''
+    if context in __imports:
+        for package, serializers in __imports[context].items():
+            names = []
+            for serializer in serializers:
+                name = __get_trimmed_name(
+                    serializer.__name__, trim_serializer_output)
+                names.append(name)
+
+            imports_str += "import type { %s } from '../%s';\n" % (
+                ', '.join(names), package)
+        imports_str += '\n'
+    return imports_str
+
+
 def __generate_interfaces(context, trim_serializer_output, camelize, enum_choices, enum_values,
                           enum_keys, annotations):
     if context not in __serializers:
         return []
     return [__get_ts_interface(serializer, context, trim_serializer_output, camelize,
                                enum_choices, enum_values, enum_keys, annotations) for serializer in
             __serializers[context]]
@@ -551,15 +597,16 @@
     with open(output_path, 'w') as output_file:
         interfaces = __generate_interfaces(context, trim_serializer_output, camelize, enum_choices,
                                            enum_values, enum_keys, annotations)
         enums = []
         if enum_choices or enum_values or enum_keys:
             enums = __generate_enums(context, enum_choices, enum_values, enum_keys)
         enums_string = __remove_duplicate_enums(enums)
-        output_file.write(enums_string + ''.join(interfaces))
+        imports = __generate_imports(context, trim_serializer_output)
+        output_file.write(imports + enums_string + ''.join(interfaces))
 
 
 def get_ts(context='default', trim_serializer_output=False, camelize=False, enum_choices=False,
            enum_values=False, enum_keys=False, annotations=False):
     '''
     Similar to generate_ts. But rather than outputting the generated
     interfaces to the specified file, will return the generated interfaces
```

### Comparing `django-typomatic-2.4.2/django_typomatic/management/commands/generate_ts.py` & `django-typomatic-2.5.0/django_typomatic/management/commands/generate_ts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import inspect
+from importlib import import_module
 from pathlib import Path
 
 from django.apps import apps
 from django.conf import settings
 from django.core.management.base import BaseCommand, CommandError
 import sys
 
@@ -20,21 +21,29 @@
     def log(self, msg):
         self.log_output.write(msg)
 
     def add_arguments(self, parser):
         parser.add_argument(
             '--serializers',
             '-s',
-            help='Serializers enumeration '
-                 'formats: module_name.SerializerName | module_name',
+            help='Serializers enumeration'
+                 'formats: module_name.SerializerName',
             nargs="*",
             type=str,
             default=[]
         )
         parser.add_argument(
+            '--app_name',
+            help='Application to generate TS for'
+                 'formats: app_name',
+            nargs=1,
+            type=str,
+            default=[]
+        )
+        parser.add_argument(
             '--all',
             help='Generate TS types for all project serializers',
             default=False,
             action='store_true'
         )
         parser.add_argument(
             '--trim',
@@ -84,78 +93,72 @@
             help='Output folder for save TS files, by default save as ./types folder',
             default='./types'
         )
 
     @staticmethod
     def _get_app_serializers(app_name):
         serializers = []
-        module = sys.modules.get(f'{app_name}.serializers', None)
-        possibly_serializers = filter(lambda name: not name.startswith('_'), dir(module))
+        modules = import_module(app_name)
+        possibly_modules = filter(lambda name: not name.startswith('_'), dir(modules))
 
-        for serializer_class_name in possibly_serializers:
-            serializer_class = getattr(module, serializer_class_name)
+        for module_name in possibly_modules:
+            module = import_module(f'{app_name}.{module_name}')
+            possibly_serializers = filter(lambda name: not name.startswith('_'), dir(module))
 
-            if not inspect.isclass(serializer_class):
-                continue
+            for serializer_class_name in possibly_serializers:
+                serializer_class = getattr(module, serializer_class_name)
 
-            # Skip imported serializer classes
-            if app_name not in serializer_class.__module__:
-                continue
+                if not inspect.isclass(serializer_class):
+                    continue
 
-            if issubclass(serializer_class, BaseSerializer):
-                serializers.append(f'{app_name}.{serializer_class.__name__}')
+                # Skip imported serializer classes
+                if app_name not in serializer_class.__module__:
+                    continue
+
+                if issubclass(serializer_class, BaseSerializer):
+                    serializers.append(f'{app_name}.{module_name}.{serializer_class.__name__}')
 
         return serializers
 
-    def _generate_ts(self, app_name, serializer_name, output, **options):
-        module = sys.modules.get(f'{app_name}.serializers', None)
+    def _generate_ts(self, module_name, serializer_name, output, **options):
+        module = import_module(module_name)
 
         if not module:
-            self.stdout.write(f'In app #{app_name} not found serializers file, skip', self.style.WARNING)
+            self.stdout.write(f'Module {module_name} not found, skip', self.style.WARNING)
             return
 
         serializer_class = getattr(module, serializer_name)
-        ts_interface(context=app_name)(serializer_class)
+        ts_interface(context=module_name)(serializer_class)
 
-        output_path = Path(output) / app_name / 'index.ts'
+        output_path = Path(output) / module_name / 'index.ts'
 
         generate_ts(
             output_path,
-            context=app_name,
+            context=module_name,
             enum_choices=options['enum_choices'],
             enum_values=options['enum_values'],
             enum_keys=options['enum_keys'],
             camelize=options['camelize'],
             trim_serializer_output=options['trim'],
             annotations=options['annotations']
         )
-        self.stdout.write(f'[+] {app_name}.{serializer_name}')
+        self.stdout.write(f'[+] {module_name}.{serializer_name}')
 
-    def handle(self, *args, serializers, output, all, **options):
-        if all and serializers:
-            raise CommandError('Only --all or --serializers must be specified, not together')
+    def handle(self, *args, serializers, app_name, output, all, **options):
+        if sum([bool(serializers), bool(app_name), bool(all)]) != 1:
+            raise CommandError('Only one of --all, --app_name or --serializers must be specified')
 
         if all:
             for app in apps.get_app_configs():
-                # Filter external modules
-                if str(settings.BASE_DIR.parent) not in app.path or '.venv' in app.path:
+                # Include only modules defined within this django project's
+                # directory
+                if Path(settings.BASE_DIR) not in Path(app.path).parents:
                     continue
 
                 serializers += self._get_app_serializers(app.name)
 
-        for serializer in serializers:
-            user_input = serializer.split('.')
+        if app_name:
+                serializers = self._get_app_serializers(app_name[0])
 
-            # Only app name
-            if len(user_input) == 1:
-                app_name = user_input[0]
-                serializers_list = self._get_app_serializers(app_name)
-
-                for s in serializers_list:
-                    _, serializer_name = s.split('.')
-                    self._generate_ts(app_name, serializer_name, output, **options)
-            # App name with serializer e.g. user.UserSerializer
-            elif len(user_input) == 2:
-                app_name, serializer_name = user_input
-                self._generate_ts(app_name, serializer_name, output, **options)
-            else:
-                self.stdout.write(f'Wrong format ({serializer})', self.style.ERROR)
+        for serializer in serializers:
+            module_name, serializer_name = serializer.rsplit('.', 1)
+            self._generate_ts(module_name, serializer_name, output, **options)
```

### Comparing `django-typomatic-2.4.2/django_typomatic/management/models.py` & `django-typomatic-2.5.0/django_typomatic/management/models.py`

 * *Files identical despite different names*

### Comparing `django-typomatic-2.4.2/django_typomatic/test__init__.py` & `django-typomatic-2.5.0/django_typomatic/test__init__.py`

 * *Files identical despite different names*

### Comparing `django-typomatic-2.4.2/django_typomatic.egg-info/PKG-INFO` & `django-typomatic-2.5.0/django_typomatic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: django-typomatic
-Version: 2.4.2
+Version: 2.5.0
 Summary: A simple solution for generating Typescript interfaces from your Django Rest Framework Serializers.
 Home-page: https://github.com/adenh93/django-typomatic
 Author: Aden Herold
 Author-email: aden.herold1@gmail.com
 Keywords: Django,Django Rest Framework,DRF,Typescript,Python
 Platform: any
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: django
+Requires-Dist: djangorestframework
 
 # django-typomatic ![pypi badge](https://img.shields.io/pypi/v/django-typomatic)
 
 _A simple solution for generating Typescript interfaces from your [Django Rest Framework Serializers](https://www.django-rest-framework.org/api-guide/serializers/)._
 
 Since I now require a simple package to generate Typescript interfaces for Django Rest Framework serializers, I've decided to port over my [Typemallow](https://github.com/adenh93/typemallow/) package for use with DRF serializers!
 
@@ -322,22 +324,22 @@
 
 You can also generate modules separately, as an example, `-s user` will restrict generation to all serializers in the `user` application, and `-s user.UserSerializer` will restrict generation to just the `UserSerializer` serializer belonging to the `user` application.
 
 ### Examples
 
 _Generate TS for `user` app_
 
-`./manage.py generate_ts -s user`
+`./manage.py generate_ts --app_name user`
 
 _Generate TS for specific serializer from user app_
 
 `./manage.py generate_ts -s user.UserSerializer`
 
 _Generate TS for many apps or serializers_
 
 `./manage.py generate_ts -s user.UserSerializer group role.RoleSerializer role.RoleListSerializer`
 
 _Generate TS for user app with annotations, choices enums, trim serializer, camelize, enum values and custom output path_
 
-`./manage.py generate_ts -s user -a -ec -t -c -ev -o "./custom_folder/"`
+`./manage.py generate_ts --app_name user -a -ec -t -c -ev -o "./custom_folder/"`
```

### Comparing `django-typomatic-2.4.2/django_typomatic.egg-info/SOURCES.txt` & `django-typomatic-2.5.0/django_typomatic.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 django_typomatic/__init__.py
+django_typomatic/__init__.pyi
 django_typomatic/mappings.py
 django_typomatic/test__init__.py
 django_typomatic.egg-info/PKG-INFO
 django_typomatic.egg-info/SOURCES.txt
 django_typomatic.egg-info/dependency_links.txt
 django_typomatic.egg-info/not-zip-safe
 django_typomatic.egg-info/requires.txt
```

### Comparing `django-typomatic-2.4.2/setup.py` & `django-typomatic-2.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open('README.md') as file:
     long_description = file.read()
 
 setuptools.setup(
     name="django-typomatic",
-    version="2.4.2",
+    version="2.5.0",
     url="https://github.com/adenh93/django-typomatic",
 
     author="Aden Herold",
     author_email="aden.herold1@gmail.com",
 
     description="A simple solution for generating Typescript interfaces from your Django Rest Framework Serializers.",
     long_description=long_description,
```

