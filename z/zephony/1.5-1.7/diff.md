# Comparing `tmp/zephony-1.5.tar.gz` & `tmp/zephony-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zephony-1.5.tar", last modified: Wed Apr  3 13:39:26 2024, max compression
+gzip compressed data, was "zephony-1.7.tar", last modified: Wed Apr  3 20:33:54 2024, max compression
```

## Comparing `zephony-1.5.tar` & `zephony-1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:39:26.550413 zephony-1.5/
--rw-r--r--   0 root         (0) root         (0)      274 2024-04-03 13:39:26.550413 zephony-1.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      290 2024-04-03 13:39:08.000000 zephony-1.5/README.md
--rw-r--r--   0 root         (0) root         (0)       79 2024-04-03 13:39:26.550413 zephony-1.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      406 2024-04-03 13:39:08.000000 zephony-1.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:39:26.550413 zephony-1.5/zephony/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 13:39:08.000000 zephony-1.5/zephony/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3323 2024-04-03 13:39:08.000000 zephony-1.5/zephony/decorators.py
--rw-r--r--   0 root         (0) root         (0)     4145 2024-04-03 13:39:08.000000 zephony-1.5/zephony/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    18046 2024-04-03 13:39:08.000000 zephony-1.5/zephony/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:39:26.550413 zephony-1.5/zephony/models/
--rw-r--r--   0 root         (0) root         (0)    41513 2024-04-03 13:39:08.000000 zephony-1.5/zephony/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7377 2024-04-03 13:39:08.000000 zephony-1.5/zephony/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:39:26.550413 zephony-1.5/zephony.egg-info/
--rw-r--r--   0 root         (0) root         (0)      274 2024-04-03 13:39:26.000000 zephony-1.5/zephony.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      314 2024-04-03 13:39:26.000000 zephony-1.5/zephony.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 13:39:26.000000 zephony-1.5/zephony.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-04-03 13:39:26.000000 zephony-1.5/zephony.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-03 13:39:26.000000 zephony-1.5/zephony.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:33:54.755849 zephony-1.7/
+-rw-r--r--   0 root         (0) root         (0)      274 2024-04-03 20:33:54.755849 zephony-1.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      290 2024-04-03 20:33:36.000000 zephony-1.7/README.md
+-rw-r--r--   0 root         (0) root         (0)       79 2024-04-03 20:33:54.755849 zephony-1.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      406 2024-04-03 20:33:36.000000 zephony-1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:33:54.751849 zephony-1.7/zephony/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 20:33:36.000000 zephony-1.7/zephony/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3323 2024-04-03 20:33:36.000000 zephony-1.7/zephony/decorators.py
+-rw-r--r--   0 root         (0) root         (0)     4145 2024-04-03 20:33:36.000000 zephony-1.7/zephony/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    18046 2024-04-03 20:33:36.000000 zephony-1.7/zephony/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:33:54.755849 zephony-1.7/zephony/models/
+-rw-r--r--   0 root         (0) root         (0)    45030 2024-04-03 20:33:36.000000 zephony-1.7/zephony/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7377 2024-04-03 20:33:36.000000 zephony-1.7/zephony/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:33:54.755849 zephony-1.7/zephony.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      274 2024-04-03 20:33:54.000000 zephony-1.7/zephony.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      314 2024-04-03 20:33:54.000000 zephony-1.7/zephony.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 20:33:54.000000 zephony-1.7/zephony.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-03 20:33:54.000000 zephony-1.7/zephony.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-03 20:33:54.000000 zephony-1.7/zephony.egg-info/top_level.txt
```

### Comparing `zephony-1.5/zephony/decorators.py` & `zephony-1.7/zephony/decorators.py`

 * *Files identical despite different names*

### Comparing `zephony-1.5/zephony/exceptions.py` & `zephony-1.7/zephony/exceptions.py`

 * *Files identical despite different names*

### Comparing `zephony-1.5/zephony/helpers.py` & `zephony-1.7/zephony/helpers.py`

 * *Files identical despite different names*

### Comparing `zephony-1.5/zephony/models/__init__.py` & `zephony-1.7/zephony/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import math
+import json
 import datetime
 import logging
 
 from ..helpers import responsify
 from flask import request
 from flask_sqlalchemy import SQLAlchemy
 from sqlalchemy import desc, or_, and_, cast, func
@@ -936,14 +937,38 @@
         if request and request.user and request.user.id_:
             self.id_deleted_user = request.user.id_
 
         db.session.flush()
 
         return self
 
+    @staticmethod
+    def convert_filters_to_ands_and_ors(join, model_string_alias_map):
+        # Returns something like this:
+        #
+        # and_(
+        #     or_(a==b, c==d),
+        #     or_(e==f, g==h),
+        # )
+
+        ors_list = []
+        for key in join['filters'].keys():
+            model_string, property_string = key.split('.')
+            Model = model_string_alias_map[model_string]
+
+            ands_list = []
+            for allowed_value in join['filters'][key]:
+                ands_list.append(getattr(Model, property_string)==allowed_value)
+
+            ors_list.append(
+                or_(*ands_list)
+            )
+        return and_(*ors_list)
+
+
     @classmethod
     def filter(
         cls,
         filters={},
         joins=[],
         bridge_joins=[],
         list_joins=[],
@@ -1009,34 +1034,82 @@
             q = (
                 q.outerjoin(aliased_model, getattr(cls, join[1])==aliased_model.id_)
                 .add_entity(aliased_model)
             )
 
         # NXN joins - aka. Bridge joins
         # Join bridge first and then the secondary table
-        for join in bridge_joins:
+        #
+        # Enumerating because the index is used as part of the alias name below
+        # to avoid collision
+        for i, join in enumerate(bridge_joins):
+            secondary_model_aliased = aliased(
+                join['secondary_model'],
+                name=(
+                    f'{join["secondary_model"].__name__}'
+                    # f'_{join["bridge_primary_id"]}'
+                    f'_{i}'
+                ),
+            )
+            bridge_model_aliased = aliased(
+                join['bridge_model'],
+                name=(
+                    f'{join["bridge_model"].__name__}'
+                    # f'_{join["bridge_primary_id"]}'
+                    f'_{i}'
+                ),
+            )
             q = (
                 q.outerjoin(
-                    join['bridge_model'],
+                    # join['bridge_model'],
+                    bridge_model_aliased,
                     and_(
-                        cls.id_==getattr(join['bridge_model'], join['bridge_primary_id']),
+                        # cls.id_==getattr(join['bridge_model'], join['bridge_primary_id']),
+                        cls.id_==getattr(bridge_model_aliased, join['bridge_primary_id']),
                         or_(
-                            join['bridge_model'].is_deleted==False,
-                            join['bridge_model'].is_deleted==None,
-                        )
+                            # join['bridge_model'].is_deleted==False,
+                            # join['bridge_model'].is_deleted==None,
+                            bridge_model_aliased.is_deleted==False,
+                            bridge_model_aliased.is_deleted==None,
+                        ),
+                        
+                        # Custom join conditions. Need to do the same for
+                        # joins and list joins
+                        cls.convert_filters_to_ands_and_ors(
+                            join=join,
+                            # Passing the aliased model, because that's
+                            # what should be used instead of the actual
+                            # model names
+                            model_string_alias_map={
+                                'bridge_model': bridge_model_aliased,
+                                'secondary_model': secondary_model_aliased,
+                            },
+                        ),
+                        
+                        # or_(
+                        #     MetadataObjectTypeRelationship.type_=='1xn',
+                        # ),
                     )
                 )
                 .outerjoin(
-                    join['secondary_model'],
-                    getattr(join['bridge_model'], join['bridge_secondary_id'])==join['secondary_model'].id_,
+                    # join['secondary_model'],
+                    secondary_model_aliased,
+                    getattr(
+                        bridge_model_aliased,
+                        join['bridge_secondary_id']
+                    # )==join['secondary_model'].id_,
+                    )==secondary_model_aliased.id_,
                 )
-                .add_entity(join['bridge_model'])
-                .add_entity(join['secondary_model'])
+                .add_entity(bridge_model_aliased)
+                # .add_entity(join['secondary_model'])
+                .add_entity(secondary_model_aliased)
             )
 
+        # TODO: alias is not implemented here like it is in normal joins
+        # and bridge joins
         # 1XN joins (aka. list joins)
         for join in list_joins:
             q = (
                 q.outerjoin(
                     join['secondary_model'],
                     and_(
                         cls.id_==getattr(join['secondary_model'], join['back_reference']),
@@ -1075,32 +1148,46 @@
                 primary_object = result
 
             if primary_object.id_ not in primary_objects_map:
                 primary_objects_map[primary_object.id_] = primary_object.get_details()
                 details = primary_objects_map[primary_object.id_]   # Helper variable
 
             for bridge_join_index, bridge_join in enumerate(bridge_joins):
+                bridge_object_alias_name = (
+                    f'{bridge_join["bridge_model"].__name__}'
+                    # f'_{bridge_join["bridge_primary_id"]}'
+                    f'_{bridge_join_index}'
+                )
                 bridge_object = getattr(
                     result,
-                    bridge_join['bridge_model'].__name__,
+                    # bridge_join['bridge_model'].__name__,
+                    bridge_object_alias_name,
                 )
 
                 if bridge_object is not None:
                     # Check if bridge object was already added
                     if bridge_object.id_ in bridge_objects_maps[bridge_join_index]:
                         continue
                     else:
                         bridge_objects_maps[bridge_join_index].append(bridge_object.id_)
 
                 if bridge_join['details_list_key'] not in details:
                     details[bridge_join['details_list_key']] = []
 
+                # Secondary object was aliased in-case we were bridging
+                # between the same table
+                secondary_object_alias_name = (
+                    f'{bridge_join["secondary_model"].__name__}'
+                    # f'_{bridge_join["bridge_primary_id"]}'
+                    f'_{bridge_join_index}'
+                )
                 secondary_object = getattr(
                     result,
-                    bridge_join['secondary_model'].__name__,
+                    # bridge_join['secondary_model'].__name__,
+                    secondary_object_alias_name,
                 )
 
                 # Skip if there's no bridge entry
                 if secondary_object is not None:
                     secondary_object_details = secondary_object.get_details()
 
                     # If bridge table row details are requested
```

### Comparing `zephony-1.5/zephony/validators.py` & `zephony-1.7/zephony/validators.py`

 * *Files identical despite different names*

