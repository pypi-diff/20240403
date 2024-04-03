# Comparing `tmp/fab-react-toolkit-0.2.8.tar.gz` & `tmp/fab-react-toolkit-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fab-react-toolkit-0.2.8.tar", last modified: Fri Feb  2 10:41:09 2024, max compression
+gzip compressed data, was "fab-react-toolkit-0.2.9.tar", last modified: Fri Feb  2 15:46:16 2024, max compression
```

## Comparing `fab-react-toolkit-0.2.8.tar` & `fab-react-toolkit-0.2.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 10:41:09.907287 fab-react-toolkit-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-02 10:40:55.000000 fab-react-toolkit-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-02-02 10:41:09.907287 fab-react-toolkit-0.2.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 10:41:09.907287 fab-react-toolkit-0.2.8/example/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 10:41:09.907287 fab-react-toolkit-0.2.8/example/app/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-02-02 10:40:55.000000 fab-react-toolkit-0.2.8/example/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-02-02 10:40:55.000000 fab-react-toolkit-0.2.8/example/app/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-02-02 10:40:55.000000 fab-react-toolkit-0.2.8/example/app/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-02-02 10:40:55.000000 fab-react-toolkit-0.2.8/example/app/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-02-02 10:40:55.000000 fab-react-toolkit-0.2.8/example/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-02 10:40:55.000000 fab-react-toolkit-0.2.8/example/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-02-02 10:40:55.000000 fab-react-toolkit-0.2.8/example/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 10:41:09.907287 fab-react-toolkit-0.2.8/fab_react_toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-02-02 10:40:55.000000 fab-react-toolkit-0.2.8/fab_react_toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 10:41:09.907287 fab-react-toolkit-0.2.8/fab_react_toolkit/api/
--rw-r--r--   0 runner    (1001) docker     (127)    14170 2024-02-02 10:40:55.000000 fab-react-toolkit-0.2.8/fab_react_toolkit/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-02-02 10:40:55.000000 fab-react-toolkit-0.2.8/fab_react_toolkit/api/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-02-02 10:40:55.000000 fab-react-toolkit-0.2.8/fab_react_toolkit/api/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    26896 2024-02-02 10:40:55.000000 fab-react-toolkit-0.2.8/fab_react_toolkit/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)    12522 2024-02-02 10:40:55.000000 fab-react-toolkit-0.2.8/fab_react_toolkit/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-02-02 10:40:55.000000 fab-react-toolkit-0.2.8/fab_react_toolkit/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-02-02 10:40:55.000000 fab-react-toolkit-0.2.8/fab_react_toolkit/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 10:41:09.907287 fab-react-toolkit-0.2.8/fab_react_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-02-02 10:41:09.000000 fab-react-toolkit-0.2.8/fab_react_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-02-02 10:41:09.000000 fab-react-toolkit-0.2.8/fab_react_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 10:41:09.000000 fab-react-toolkit-0.2.8/fab_react_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-02 10:41:09.000000 fab-react-toolkit-0.2.8/fab_react_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-02-02 10:40:55.000000 fab-react-toolkit-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-02-02 10:40:55.000000 fab-react-toolkit-0.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-02-02 10:41:09.907287 fab-react-toolkit-0.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:46:16.358754 fab-react-toolkit-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-02-02 15:46:16.358754 fab-react-toolkit-0.2.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:46:16.354754 fab-react-toolkit-0.2.9/example/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:46:16.354754 fab-react-toolkit-0.2.9/example/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/example/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/example/app/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/example/app/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/example/app/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/example/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/example/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/example/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:46:16.354754 fab-react-toolkit-0.2.9/fab_react_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/fab_react_toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:46:16.358754 fab-react-toolkit-0.2.9/fab_react_toolkit/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    20840 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/fab_react_toolkit/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/fab_react_toolkit/api/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/fab_react_toolkit/api/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26896 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/fab_react_toolkit/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12522 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/fab_react_toolkit/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/fab_react_toolkit/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/fab_react_toolkit/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:46:16.358754 fab-react-toolkit-0.2.9/fab_react_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-02-02 15:46:16.000000 fab-react-toolkit-0.2.9/fab_react_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-02-02 15:46:16.000000 fab-react-toolkit-0.2.9/fab_react_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 15:46:16.000000 fab-react-toolkit-0.2.9/fab_react_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-02 15:46:16.000000 fab-react-toolkit-0.2.9/fab_react_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-02-02 15:46:16.358754 fab-react-toolkit-0.2.9/setup.cfg
```

### Comparing `fab-react-toolkit-0.2.8/LICENSE` & `fab-react-toolkit-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.2.8/PKG-INFO` & `fab-react-toolkit-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fab-react-toolkit
-Version: 0.2.8
+Version: 0.2.9
 Summary: A small example package
 Home-page: https://github.com/dttctcs/fab-react-toolkit
 Author: Datatactics GmbH
 Author-email: Matthias Leinweber <m.leinweber@datatactics.de>
 Project-URL: Homepage, https://github.com/dttctcs/fab-react-toolkit
 Project-URL: Issues, https://github.com/dttctcs/fab-react-toolkit/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fab-react-toolkit-0.2.8/example/app/__init__.py` & `fab-react-toolkit-0.2.9/example/app/__init__.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.2.8/example/app/apis.py` & `fab-react-toolkit-0.2.9/example/app/apis.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from app.models import Asset, Unit, Application
+from app.models import *
 from fab_react_toolkit import ModelRestApi, SQLAInterface
 from flask import request, Response
 from flask_appbuilder.api import expose, protect, safe, permission_name
 from app import appbuilder, db
 from typing import Any
 
 class AssetApi(ModelRestApi):
@@ -66,10 +66,25 @@
             "label": "Unit Name",
             "column": "name",
             "type": "multiselect",
             "options": [{"value": f"unit_{i}", "label": f"unit_{i}"} for i in range(10)]
         }
     ]
 
+class StringPkApi(ModelRestApi):
+    resource_name = "stringpk"
+
+    datamodel = SQLAInterface(StringPk)
+
+
+    def pre_add(self, item) -> None:
+        """
+        If criticality != green then close green status    
+        """
+        print(item.name)
+        item.id = item.name
+        pass
+
 appbuilder.add_api(AssetApi)
 appbuilder.add_api(ApplicationApi)
 appbuilder.add_api(UnitApi)
+appbuilder.add_api(StringPkApi)
```

### Comparing `fab-react-toolkit-0.2.8/example/app/config.py` & `fab-react-toolkit-0.2.9/example/app/config.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.2.8/example/app/models.py` & `fab-react-toolkit-0.2.9/example/app/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -41,7 +41,15 @@
     id = Column(Integer, primary_key=True, autoincrement=True)
     name = Column(String(512), nullable=False)
 
     def __repr__(self):
         return self.name
 
 
+
+
+class StringPk(Model):
+    id = Column(String, primary_key=True)
+    name = Column(String(512), nullable=False)
+
+    def __repr__(self):
+        return self.name
```

### Comparing `fab-react-toolkit-0.2.8/example/run.py` & `fab-react-toolkit-0.2.9/example/run.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.2.8/fab_react_toolkit/__init__.py` & `fab-react-toolkit-0.2.9/fab_react_toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.2.8/fab_react_toolkit/api/__init__.py` & `fab-react-toolkit-0.2.9/fab_react_toolkit/api/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,79 @@
 import functools
 import json
 import urllib
 from typing import Any, Callable, Optional, Dict
 import jsonschema
 import prison as prison
-from flask_appbuilder.api import BaseApi, ModelRestApi as FABModelRestApi, merge_response_func, expose, safe, rison, get_info_schema
+from flask_appbuilder.api import BaseApi, ModelRestApi as FABModelRestApi, merge_response_func, expose, safe, rison, get_info_schema, get_item_schema
 from flask_appbuilder._compat import as_unicode
 
+from flask_appbuilder.const import (
+    API_ADD_COLUMNS_RES_KEY,
+    API_ADD_COLUMNS_RIS_KEY,
+    API_ADD_TITLE_RES_KEY,
+    API_ADD_TITLE_RIS_KEY,
+    API_DESCRIPTION_COLUMNS_RES_KEY,
+    API_DESCRIPTION_COLUMNS_RIS_KEY,
+    API_EDIT_COLUMNS_RES_KEY,
+    API_EDIT_COLUMNS_RIS_KEY,
+    API_EDIT_TITLE_RES_KEY,
+    API_EDIT_TITLE_RIS_KEY,
+    API_FILTERS_RES_KEY,
+    API_FILTERS_RIS_KEY,
+    API_LABEL_COLUMNS_RES_KEY,
+    API_LABEL_COLUMNS_RIS_KEY,
+    API_LIST_COLUMNS_RES_KEY,
+    API_LIST_COLUMNS_RIS_KEY,
+    API_LIST_TITLE_RES_KEY,
+    API_LIST_TITLE_RIS_KEY,
+    API_ORDER_COLUMN_RIS_KEY,
+    API_ORDER_COLUMNS_RES_KEY,
+    API_ORDER_COLUMNS_RIS_KEY,
+    API_ORDER_DIRECTION_RIS_KEY,
+    API_PAGE_INDEX_RIS_KEY,
+    API_PAGE_SIZE_RIS_KEY,
+    API_PERMISSIONS_RES_KEY,
+    API_PERMISSIONS_RIS_KEY,
+    API_RESULT_RES_KEY,
+    API_SELECT_COLUMNS_RIS_KEY,
+    API_SHOW_COLUMNS_RES_KEY,
+    API_SHOW_COLUMNS_RIS_KEY,
+    API_SHOW_TITLE_RES_KEY,
+    API_SHOW_TITLE_RIS_KEY,
+    API_URI_RIS_KEY,
+    PERMISSION_PREFIX,
+)
+
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Set,
+    Tuple,
+    Type,
+    TYPE_CHECKING,
+    Union,
+)
+
 from flask_appbuilder.security.decorators import permission_name, protect
 from flask import  Response, request
 from flask_appbuilder.const import API_ADD_COLUMNS_RIS_KEY, API_ADD_TITLE_RIS_KEY, API_PERMISSIONS_RIS_KEY, \
     API_EDIT_COLUMNS_RIS_KEY, API_FILTERS_RIS_KEY, API_EDIT_TITLE_RIS_KEY, API_FILTERS_RES_KEY, \
     API_ORDER_COLUMNS_RIS_KEY, API_LABEL_COLUMNS_RIS_KEY, API_DESCRIPTION_COLUMNS_RIS_KEY, API_LIST_COLUMNS_RIS_KEY, \
     API_LIST_TITLE_RIS_KEY, API_URI_RIS_KEY
 from flask_appbuilder.api.schemas import get_list_schema
 from .convert import Model2SchemaConverter
 
 from copy import deepcopy
+
+ModelKeyType = Union[str, int]
+
 def better_rison(
         schema: Optional[Dict[str, Any]] = None
 ) -> Callable[[Callable[..., Any]], Callable[..., Any]]:
     """
     Use this decorator to parse URI *Rison* arguments to
     a python data structure, your method gets the data
     structure on kwargs['rison']. Response is HTTP 400
@@ -359,7 +412,172 @@
             Returns:
                 The response from the bulk operation.
 
             """
             id_list = request.get_json()
             bulk_func = getattr(self, f"bulk_{handler}")
             return bulk_func(id_list)
+
+
+    @expose("/<pk>", methods=["GET"])
+    @protect()
+    @safe
+    @permission_name("get")
+    @rison(get_item_schema)
+    @merge_response_func(FABModelRestApi.merge_show_label_columns, API_LABEL_COLUMNS_RIS_KEY)
+    @merge_response_func(FABModelRestApi.merge_show_columns, API_SHOW_COLUMNS_RIS_KEY)
+    @merge_response_func(FABModelRestApi.merge_description_columns, API_DESCRIPTION_COLUMNS_RIS_KEY)
+    @merge_response_func(FABModelRestApi.merge_show_title, API_SHOW_TITLE_RIS_KEY)
+    def get(self, pk: ModelKeyType, **kwargs: Any) -> Response:
+        """Get item from Model
+        ---
+        get:
+          description: >-
+            Get an item model
+          parameters:
+          - in: path
+            schema:              
+              oneOf:
+              - type: string
+              - type: integer
+            name: pk
+          - in: query
+            name: q
+            content:
+              application/json:
+                schema:
+                  $ref: '#/components/schemas/get_item_schema'
+          responses:
+            200:
+              description: Item from Model
+              content:
+                application/json:
+                  schema:
+                    type: object
+                    properties:
+                      label_columns:
+                        type: object
+                        properties:
+                          column_name:
+                            description: >-
+                              The label for the column name.
+                              Will be translated by babel
+                            example: A Nice label for the column
+                            type: string
+                      show_columns:
+                        description: >-
+                          A list of columns
+                        type: array
+                        items:
+                          type: string
+                      description_columns:
+                        type: object
+                        properties:
+                          column_name:
+                            description: >-
+                              The description for the column name.
+                              Will be translated by babel
+                            example: A Nice description for the column
+                            type: string
+                      show_title:
+                        description: >-
+                          A title to render.
+                          Will be translated by babel
+                        example: Show Item Details
+                        type: string
+                      id:
+                        description: The item id
+                        type: string
+                      result:
+                        $ref: '#/components/schemas/{{self.__class__.__name__}}.get'
+            400:
+              $ref: '#/components/responses/400'
+            401:
+              $ref: '#/components/responses/401'
+            404:
+              $ref: '#/components/responses/404'
+            422:
+              $ref: '#/components/responses/422'
+            500:
+              $ref: '#/components/responses/500'
+        """
+        return self.get_headless(pk, **kwargs)
+
+    @expose("/<pk>", methods=["PUT"])
+    @protect()
+    @safe
+    @permission_name("put")
+    def put(self, pk: ModelKeyType) -> Response:
+        """PUT item to Model
+        ---
+        put:
+          parameters:
+          - in: path
+            schema:
+              oneOf:
+              - type: string
+              - type: integer
+            name: pk
+          requestBody:
+            description: Model schema
+            required: true
+            content:
+              application/json:
+                schema:
+                  $ref: '#/components/schemas/{{self.__class__.__name__}}.put'
+          responses:
+            200:
+              description: Item changed
+              content:
+                application/json:
+                  schema:
+                    type: object
+                    properties:
+                      result:
+                        $ref: '#/components/schemas/{{self.__class__.__name__}}.put'
+            400:
+              $ref: '#/components/responses/400'
+            401:
+              $ref: '#/components/responses/401'
+            404:
+              $ref: '#/components/responses/404'
+            422:
+              $ref: '#/components/responses/422'
+            500:
+              $ref: '#/components/responses/500'
+        """
+        return self.put_headless(pk)    
+
+
+    @expose("/<pk>", methods=["DELETE"])
+    @protect()
+    @safe
+    @permission_name("delete")
+    def delete(self, pk: ModelKeyType) -> Response:
+        """Delete item from Model
+        ---
+        delete:
+          parameters:
+          - in: path
+            schema:
+              oneOf:
+              - type: string
+              - type: integer
+            name: pk
+          responses:
+            200:
+              description: Item deleted
+              content:
+                application/json:
+                  schema:
+                    type: object
+                    properties:
+                      message:
+                        type: string
+            404:
+              $ref: '#/components/responses/404'
+            422:
+              $ref: '#/components/responses/422'
+            500:
+              $ref: '#/components/responses/500'
+        """
+        return self.delete_headless(pk)
```

### Comparing `fab-react-toolkit-0.2.8/fab_react_toolkit/api/convert.py` & `fab-react-toolkit-0.2.9/fab_react_toolkit/api/convert.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.2.8/fab_react_toolkit/apis.py` & `fab-react-toolkit-0.2.9/fab_react_toolkit/apis.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.2.8/fab_react_toolkit/filters.py` & `fab-react-toolkit-0.2.9/fab_react_toolkit/filters.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.2.8/fab_react_toolkit/views.py` & `fab-react-toolkit-0.2.9/fab_react_toolkit/views.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.2.8/fab_react_toolkit.egg-info/PKG-INFO` & `fab-react-toolkit-0.2.9/fab_react_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fab-react-toolkit
-Version: 0.2.8
+Version: 0.2.9
 Summary: A small example package
 Home-page: https://github.com/dttctcs/fab-react-toolkit
 Author: Datatactics GmbH
 Author-email: Matthias Leinweber <m.leinweber@datatactics.de>
 Project-URL: Homepage, https://github.com/dttctcs/fab-react-toolkit
 Project-URL: Issues, https://github.com/dttctcs/fab-react-toolkit/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fab-react-toolkit-0.2.8/fab_react_toolkit.egg-info/SOURCES.txt` & `fab-react-toolkit-0.2.9/fab_react_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.2.8/pyproject.toml` & `fab-react-toolkit-0.2.9/pyproject.toml`

 * *Files identical despite different names*

