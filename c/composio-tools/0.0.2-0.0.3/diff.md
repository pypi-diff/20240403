# Comparing `tmp/composio-tools-0.0.2.tar.gz` & `tmp/composio-tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio-tools-0.0.2.tar", last modified: Sat Mar 23 10:54:30 2024, max compression
+gzip compressed data, was "composio-tools-0.0.3.tar", last modified: Wed Apr  3 10:28:10 2024, max compression
```

## Comparing `composio-tools-0.0.2.tar` & `composio-tools-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-03-23 10:54:30.071584 composio-tools-0.0.2/
--rw-r--r--   0 karanvaidya   (501) staff       (20)      472 2024-03-23 10:54:30.071257 composio-tools-0.0.2/PKG-INFO
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-03-23 10:54:30.054700 composio-tools-0.0.2/composio_tools/
--rw-r--r--   0 karanvaidya   (501) staff       (20)       84 2024-03-07 11:30:04.000000 composio-tools-0.0.2/composio_tools/__init__.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-03-23 10:54:30.070393 composio-tools-0.0.2/composio_tools/lib/
--rw-r--r--   0 karanvaidya   (501) staff       (20)       89 2024-03-07 11:30:04.000000 composio-tools-0.0.2/composio_tools/lib/__init__.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     1196 2024-03-22 20:33:28.000000 composio-tools-0.0.2/composio_tools/lib/action.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     1136 2024-03-07 11:30:04.000000 composio-tools-0.0.2/composio_tools/lib/headers.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     4691 2024-03-23 10:33:04.000000 composio-tools-0.0.2/composio_tools/lib/tool.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     1665 2024-03-23 07:45:20.000000 composio-tools-0.0.2/composio_tools/lib/trigger.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-03-23 10:54:30.070921 composio-tools-0.0.2/composio_tools.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)      472 2024-03-23 10:54:29.000000 composio-tools-0.0.2/composio_tools.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      386 2024-03-23 10:54:30.000000 composio-tools-0.0.2/composio_tools.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-03-23 10:54:30.000000 composio-tools-0.0.2/composio_tools.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       20 2024-03-23 10:54:30.000000 composio-tools-0.0.2/composio_tools.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       15 2024-03-23 10:54:30.000000 composio-tools-0.0.2/composio_tools.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      273 2024-03-23 10:53:48.000000 composio-tools-0.0.2/pyproject.toml
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-03-23 10:54:30.071648 composio-tools-0.0.2/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)      589 2024-03-23 10:53:27.000000 composio-tools-0.0.2/setup.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-03 10:28:10.849342 composio-tools-0.0.3/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      472 2024-04-03 10:28:10.849152 composio-tools-0.0.3/PKG-INFO
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-03 10:28:10.846962 composio-tools-0.0.3/composio_tools/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       84 2024-03-07 11:30:04.000000 composio-tools-0.0.3/composio_tools/__init__.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-03 10:28:10.848711 composio-tools-0.0.3/composio_tools/lib/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       89 2024-03-07 11:30:04.000000 composio-tools-0.0.3/composio_tools/lib/__init__.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     1187 2024-04-02 17:32:33.000000 composio-tools-0.0.3/composio_tools/lib/action.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     1136 2024-03-07 11:30:04.000000 composio-tools-0.0.3/composio_tools/lib/headers.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     5830 2024-04-02 17:32:33.000000 composio-tools-0.0.3/composio_tools/lib/tool.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     1801 2024-04-02 17:32:33.000000 composio-tools-0.0.3/composio_tools/lib/trigger.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-03 10:28:10.848966 composio-tools-0.0.3/composio_tools.egg-info/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      472 2024-04-03 10:28:10.000000 composio-tools-0.0.3/composio_tools.egg-info/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      386 2024-04-03 10:28:10.000000 composio-tools-0.0.3/composio_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-03 10:28:10.000000 composio-tools-0.0.3/composio_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       20 2024-04-03 10:28:10.000000 composio-tools-0.0.3/composio_tools.egg-info/requires.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       15 2024-04-03 10:28:10.000000 composio-tools-0.0.3/composio_tools.egg-info/top_level.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      273 2024-03-26 08:33:45.000000 composio-tools-0.0.3/pyproject.toml
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-03 10:28:10.849382 composio-tools-0.0.3/setup.cfg
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      589 2024-04-03 10:11:04.000000 composio-tools-0.0.3/setup.py
```

### Comparing `composio-tools-0.0.2/composio_tools/lib/action.py` & `composio-tools-0.0.3/composio_tools/lib/action.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pydantic import BaseModel
 from typing import List
 
-class Action(BaseModel):
+class Action():
     _display_name: str = ""  # Add an internal variable to hold the display name
     _request_schema: BaseModel = None  # Placeholder for request schema
     _response_schema: BaseModel = None  # Placeholder for response schema
 
     @property
     def display_name(self) -> str:
         return self._display_name
```

### Comparing `composio-tools-0.0.2/composio_tools/lib/headers.py` & `composio-tools-0.0.3/composio_tools/lib/headers.py`

 * *Files identical despite different names*

### Comparing `composio-tools-0.0.2/composio_tools/lib/tool.py` & `composio-tools-0.0.3/composio_tools/lib/tool.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import json
 import jsonref
 import inflection
-from pydantic import BaseModel
 from typing import List
 from .action import Action
-from .trigger import Trigger
+from .trigger import AlreadyExistsError, Trigger
     
 def add_tool_name(tool_name: str, action_name: str) -> str:
     return f"{tool_name.lower()}_{inflection.underscore(action_name)}"
 
-class Tool(BaseModel):
+class Tool():
     _custom_id: str = "default"  # Add an internal variable to hold the custom repo name
 
     @property
     def custom_id(self) -> str:
         return self._custom_id
     
     @custom_id.setter
     def custom_id(self, value: str):
         self._custom_id = value  # Set the internal variable
 
+    def identifier_name(self) -> str:
+        return f"{self.__class__.__name__.lower()}_{self.custom_id}"
+
     def actions(self) -> List[Action]:
         raise NotImplementedError("This method should be overridden by subclasses.")
     
     def triggers(self) -> List[Trigger]:
         raise NotImplementedError("This method should be overridden by subclasses.")
 
     def execute_action(self, action_name: str, request_data: dict, authorisation_data: dict) -> dict:
@@ -33,41 +35,55 @@
             if action_name_shared == action_name:
                 print(f"Executing {action.__name__} on Tool: {tool_name} with request data {request_data} and authorisation data {authorisation_data}")
                 try:
                     request_schema = action().request_schema
                     req = request_schema.model_validate_json(json_data=json.dumps(request_data))
                     return action().execute(req, authorisation_data)
                 except Exception as e:
+                    print(f"Error executing {action.__name__} on Tool: {tool_name}: {e}")
                     return {"status": "failure", "details": str(e)}
         return {"status": "failure", "details": "Action not found"}
     
-    def transform_trigger_payload(self, payload: dict) -> dict:
-        tool_name = self.__class__.__name__
-        for trigger in self.triggers():
-            try:
-                (match, converted_payload) = trigger().check_and_convert_to_identifier_payload_schema(payload)
-                if match:
-                    converted_payload["trigger_name"] = add_tool_name(tool_name, trigger.__name__)
-                    return converted_payload
-            except Exception as e:
-                print(f"Error transforming trigger payload for Tool: {tool_name} with payload {payload}: {str(e)}")
-        return {"status": "failure", "details": "Trigger not found"}
-    
     def set_webhook_url(self, trigger_name: str, authorisation_data: dict, trigger_config: dict) -> dict: 
         tool_name = self.__class__.__name__
         for trigger in self.triggers():
             trigger_name_shared = add_tool_name(tool_name, trigger.__name__)
             if trigger_name_shared == trigger_name:
                 print(f"Setting webhook URL for Trigger: {trigger_name} on Tool: {tool_name} with URL {trigger_config['webhook_url']} and authorisation data {authorisation_data}")
                 try:
-                    response = trigger().set_webhook_url(authorisation_data, trigger_config)
-                    return {"status": "success", "connection_data": response}
+                    webhook_url = trigger_config["webhook_url"]
+                    del trigger_config["webhook_url"]
+                    trigger_config_schema = trigger().trigger_config_schema
+                    tc = trigger_config_schema.model_validate_json(json_data=json.dumps(trigger_config))
+                    conn_data = trigger().set_webhook_url(authorisation_data, webhook_url, tc)
+                    return {"status": "success", "connection_data": conn_data}
+                except AlreadyExistsError as e:
+                    print(f"Webhook URL already exists for Trigger: {trigger_name} on Tool: {tool_name}: {e}")
+                    return {"status": "failure", "details": "Webhook URL already exists"}
                 except Exception as e:
+                    print(f"Error setting webhook URL for Trigger: {trigger_name} on Tool: {tool_name}: {e}")
                     return {"status": "failure", "details": str(e)}
         return {"status": "failure", "details": "Trigger not found"}
+    
+    def transform_trigger_payload(self, payload: dict) -> dict:
+        tool_name = self.__class__.__name__
+        for trigger in self.triggers():
+            try:
+                print(f"Transforming trigger payload for Tool: {tool_name}")
+                (match, connection_data, converted_payload) = trigger().check_and_convert_to_identifier_payload_schema(payload)
+                print(f"Match: {match}, Connection Data: {connection_data}, Converted Payload: {converted_payload}")
+                if match:
+                    return {
+                        "trigger_name": add_tool_name(tool_name, trigger.__name__),
+                        "connection_data": connection_data,
+                        "payload": converted_payload
+                    }
+            except Exception as e:
+                print(f"Error transforming trigger payload for Tool: {tool_name}: {str(e)}")
+        return {"status": "failure", "details": "Trigger not found"}
         
         
     def json_schema(self):
         tool_name = self.__class__.__name__
         return {
             "Name": tool_name,
             "Description": self.__doc__.strip() if self.__doc__ else None,
@@ -83,13 +99,14 @@
             ],
             "Triggers": [
                 {
                     "name": add_tool_name(tool_name, trigger.__name__),
                     "display_name": trigger().display_name,
                     "description": trigger.__doc__.strip() if trigger.__doc__ else None,
                     "payload": jsonref.loads(json.dumps(trigger().payload_schema.model_json_schema())),
-                    "config": jsonref.loads(json.dumps(trigger().trigger_config.model_json_schema())),
+                    "config": jsonref.loads(json.dumps(trigger().trigger_config_schema.model_json_schema())),
                     "instructions": trigger().trigger_instructions
                 } for trigger in self.triggers()
             ],
         }
 
+
```

### Comparing `composio-tools-0.0.2/composio_tools/lib/trigger.py` & `composio-tools-0.0.3/composio_tools/lib/trigger.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from pydantic import BaseModel
 
+class AlreadyExistsError(Exception):
+    pass
+
 class Trigger(BaseModel):
     _display_name: str = ""  # Add an internal variable to hold the display name
     _payload_schema: BaseModel = None  # Placeholder for payload schema
-    _trigger_config: BaseModel = None  # Placeholder for trigger config
+    _trigger_config_schema: BaseModel = None  # Placeholder for trigger config
     _trigger_instructions: str = ""  # Placeholder for trigger instructions
 
     @property
     def display_name(self) -> str:
         return self._display_name
 
     @display_name.setter
@@ -19,28 +22,28 @@
         return self._payload_schema
 
     @payload_schema.setter
     def payload_schema(self, value: BaseModel):
         self._payload_schema = value  # Set the internal variable
 
     @property
-    def trigger_config(self) -> BaseModel:
-        return self._trigger_config
+    def trigger_config_schema(self) -> BaseModel:
+        return self._trigger_config_schema
     
-    @trigger_config.setter
-    def trigger_config(self, value: BaseModel):
-        self._trigger_config = value  # Set the internal variable
+    @trigger_config_schema.setter
+    def trigger_config_schema(self, value: BaseModel):
+        self._trigger_config_schema = value  # Set the internal variable
 
     @property
     def trigger_instructions(self) -> str:
         return self._trigger_instructions
     
     @trigger_instructions.setter
     def trigger_instructions(self, value: str):
         self._trigger_instructions = value  # Set the internal variable
 
-    def check_and_convert_to_identifier_payload_schema(self, data: dict) -> (bool, dict):
+    def check_and_convert_to_identifier_payload_schema(self, data: dict) -> (bool, str, _payload_schema):
         raise NotImplementedError("This method should be overridden by subclasses.")
     
-    def set_webhook_url(self, authorisation_data: dict, req: _trigger_config) -> dict:
+    def set_webhook_url(self, authorisation_data: dict, webhook_url_to_set: str, req: _trigger_config_schema) -> str:
         raise NotImplementedError("This method should be overridden by subclasses.")
```

### Comparing `composio-tools-0.0.2/setup.py` & `composio-tools-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup 
 
 setup(
     name = 'composio-tools',
-    version = '0.0.2',
+    version = '0.0.3',
     author = 'Karan',
     author_email = 'karan@composio.dev',
     description = 'Add tools to Composio using this package',
     long_description = "",
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/SamparkAI/tools',
     classifiers = [
```

