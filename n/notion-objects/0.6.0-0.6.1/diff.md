# Comparing `tmp/notion-objects-0.6.0.tar.gz` & `tmp/notion-objects-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notion-objects-0.6.0.tar", last modified: Sun Mar 31 16:38:53 2024, max compression
+gzip compressed data, was "notion-objects-0.6.1.tar", last modified: Wed Apr  3 13:10:21 2024, max compression
```

## Comparing `notion-objects-0.6.0.tar` & `notion-objects-0.6.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-31 16:38:53.531095 notion-objects-0.6.0/
--rw-r--r--   0 thomas    (1000) thomas    (1000)    11357 2023-02-17 21:11:05.000000 notion-objects-0.6.0/LICENSE
--rw-r--r--   0 thomas    (1000) thomas    (1000)     5831 2024-03-31 16:38:53.531095 notion-objects-0.6.0/PKG-INFO
--rw-r--r--   0 thomas    (1000) thomas    (1000)     4666 2023-10-14 04:05:06.000000 notion-objects-0.6.0/README.md
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-31 16:38:53.531095 notion-objects-0.6.0/notion_objects/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      118 2024-03-31 16:38:33.000000 notion-objects-0.6.0/notion_objects/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     6960 2024-03-31 16:36:48.000000 notion-objects-0.6.0/notion_objects/database.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2064 2024-03-31 16:36:48.000000 notion-objects-0.6.0/notion_objects/encode.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     2833 2024-03-28 13:17:36.000000 notion-objects-0.6.0/notion_objects/objects.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    21206 2024-03-31 16:36:48.000000 notion-objects-0.6.0/notion_objects/properties.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5172 2024-03-31 16:36:48.000000 notion-objects-0.6.0/notion_objects/rich_text.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      630 2023-03-10 19:29:50.000000 notion-objects-0.6.0/notion_objects/values.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-31 16:38:53.531095 notion-objects-0.6.0/notion_objects.egg-info/
--rw-r--r--   0 thomas    (1000) thomas    (1000)     5831 2024-03-31 16:38:53.000000 notion-objects-0.6.0/notion_objects.egg-info/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      455 2024-03-31 16:38:53.000000 notion-objects-0.6.0/notion_objects.egg-info/SOURCES.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2024-03-31 16:38:53.000000 notion-objects-0.6.0/notion_objects.egg-info/dependency_links.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2024-03-31 16:38:51.000000 notion-objects-0.6.0/notion_objects.egg-info/not-zip-safe
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      132 2024-03-31 16:38:53.000000 notion-objects-0.6.0/notion_objects.egg-info/requires.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       15 2024-03-31 16:38:53.000000 notion-objects-0.6.0/notion_objects.egg-info/top_level.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)      503 2023-02-17 21:11:05.000000 notion-objects-0.6.0/pyproject.toml
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1100 2024-03-31 16:38:53.531095 notion-objects-0.6.0/setup.cfg
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-04-03 13:10:21.184106 notion-objects-0.6.1/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    11357 2023-02-17 21:11:05.000000 notion-objects-0.6.1/LICENSE
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     5831 2024-04-03 13:10:21.184106 notion-objects-0.6.1/PKG-INFO
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     4666 2023-10-14 04:05:06.000000 notion-objects-0.6.1/README.md
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-04-03 13:10:21.184106 notion-objects-0.6.1/notion_objects/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      118 2024-04-03 12:22:01.000000 notion-objects-0.6.1/notion_objects/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     6960 2024-03-31 16:36:48.000000 notion-objects-0.6.1/notion_objects/database.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2191 2024-04-03 12:28:24.000000 notion-objects-0.6.1/notion_objects/encode.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2833 2024-03-28 13:17:36.000000 notion-objects-0.6.1/notion_objects/objects.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    21579 2024-04-03 12:28:24.000000 notion-objects-0.6.1/notion_objects/properties.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5172 2024-03-31 16:36:48.000000 notion-objects-0.6.1/notion_objects/rich_text.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      766 2024-04-03 12:12:50.000000 notion-objects-0.6.1/notion_objects/values.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-04-03 13:10:21.184106 notion-objects-0.6.1/notion_objects.egg-info/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     5831 2024-04-03 13:10:21.000000 notion-objects-0.6.1/notion_objects.egg-info/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      455 2024-04-03 13:10:21.000000 notion-objects-0.6.1/notion_objects.egg-info/SOURCES.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2024-04-03 13:10:21.000000 notion-objects-0.6.1/notion_objects.egg-info/dependency_links.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2024-04-03 13:10:21.000000 notion-objects-0.6.1/notion_objects.egg-info/not-zip-safe
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      132 2024-04-03 13:10:21.000000 notion-objects-0.6.1/notion_objects.egg-info/requires.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       15 2024-04-03 13:10:21.000000 notion-objects-0.6.1/notion_objects.egg-info/top_level.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      503 2023-02-17 21:11:05.000000 notion-objects-0.6.1/pyproject.toml
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1100 2024-04-03 13:10:21.184106 notion-objects-0.6.1/setup.cfg
```

### Comparing `notion-objects-0.6.0/LICENSE` & `notion-objects-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `notion-objects-0.6.0/PKG-INFO` & `notion-objects-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notion-objects
-Version: 0.6.0
+Version: 0.6.1
 Summary: A python library to work with objects retrieved from the notion API
 Home-page: https://github.com/thrau/notion-objects
 Author: Thomas Rausch
 Author-email: thomas@thrau.at
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 4 - Beta
```

### Comparing `notion-objects-0.6.0/README.md` & `notion-objects-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `notion-objects-0.6.0/notion_objects/database.py` & `notion-objects-0.6.1/notion_objects/database.py`

 * *Files identical despite different names*

### Comparing `notion-objects-0.6.0/notion_objects/encode.py` & `notion-objects-0.6.1/notion_objects/encode.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import dataclasses
 import json
 from datetime import date, datetime
 from typing import Iterable
 
 from .properties import DateRange, DateTimeRange, Property, RichTextProperty
-from .values import DateValue, UserValue
+from .values import DateValue, UniqueIdValue, UserValue
 
 
 class JSONEncoder(json.JSONEncoder):
     def default(self, o):
         if isinstance(o, datetime):
             return o.isoformat()
         if isinstance(o, date):
@@ -25,15 +25,17 @@
             try:
                 value = getattr(self, prop.attr)
             except KeyError:
                 # TODO: handle more gracefully
                 continue
             key = prop.attr
 
-            if isinstance(value, DateValue):
+            if isinstance(value, UniqueIdValue):
+                result[key] = str(value)
+            elif isinstance(value, DateValue):
                 # TODO: timezone
                 if flat:
                     result[f"{key}_start"] = value.start
                     result[f"{key}_end"] = value.end
                 else:
                     result[key] = {"start": value.start, "end": value.end}
             elif isinstance(value, UserValue):
@@ -51,12 +53,12 @@
             elif isinstance(prop, RichTextProperty):
                 result[key] = "".join([text.plain_text for text in value])
             else:
                 result[key] = value
 
         return result
 
-    def to_json(self, flat: bool = False):
-        return json.dumps(self.to_dict(flat=flat), cls=JSONEncoder)
+    def to_json(self, flat: bool = False, **kwargs):
+        return json.dumps(self.to_dict(flat=flat), cls=JSONEncoder, **kwargs)
 
     def _get_properties(self) -> Iterable[Property]:
         raise NotImplementedError
```

### Comparing `notion-objects-0.6.0/notion_objects/objects.py` & `notion-objects-0.6.1/notion_objects/objects.py`

 * *Files identical despite different names*

### Comparing `notion-objects-0.6.0/notion_objects/properties.py` & `notion-objects-0.6.1/notion_objects/properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     TypeVar,
     Union,
 )
 
 import dateutil.parser
 
 from . import rich_text
-from .values import DateValue, UserValue
+from .values import DateValue, UniqueIdValue, UserValue
 
 property_types = [
     "title",
     "rich_text",
     "number",
     "select",
     "multi_select",
@@ -39,14 +39,15 @@
     "created_time",
     "created_by",  # TODO
     "last_edited_time",
     "last_edited_by",  # TODO
     "status",
     "emoji",  # TODO
     "external",  # TODO
+    "unique_id",
 ]
 
 PropertyType = Literal[
     "checkbox",
     "created_by",
     "created_time",
     "date",
@@ -61,14 +62,15 @@
     "phone_number",
     "relation",
     "rich_text",
     "rollup",
     "select",
     "status",
     "title",
+    "unique_id",
     "url",
 ]
 """The notion data type of a property, see https://developers.notion.com/reference/property-object."""
 
 _T = TypeVar("_T")
 _P = TypeVar("_P", bound="Property")
 
@@ -328,14 +330,24 @@
             if "." in value:
                 value = float(value)
             else:
                 value = int(value)
         obj[field] = {self.type: value}
 
 
+class UniqueId(Property[UniqueIdValue]):
+    type = "unique_id"
+
+    def get(self, field: str, obj: dict) -> UniqueIdValue:
+        return UniqueIdValue(**obj["properties"][field][self.type])
+
+    def set(self, field: str, value: _T, obj: dict):
+        raise NotImplementedError("setting unique IDs is not possible yet")
+
+
 class Integer(Property[Optional[int]]):
     type = "number"
 
     def get(self, field: str, obj: dict) -> Optional[int]:
         if value := obj["properties"][field][self.type]:
             return int(value)
```

### Comparing `notion-objects-0.6.0/notion_objects/rich_text.py` & `notion-objects-0.6.1/notion_objects/rich_text.py`

 * *Files identical despite different names*

### Comparing `notion-objects-0.6.0/notion_objects/values.py` & `notion-objects-0.6.1/notion_objects/values.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,7 +22,16 @@
     email: Optional[str] = None
 
     def __str__(self):
         if self.name is not None:
             return self.name
         else:
             return self.id
+
+
+@dataclass
+class UniqueIdValue:
+    prefix: str
+    number: int
+
+    def __str__(self):
+        return f"{self.prefix}-{self.number}"
```

### Comparing `notion-objects-0.6.0/notion_objects.egg-info/PKG-INFO` & `notion-objects-0.6.1/notion_objects.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notion-objects
-Version: 0.6.0
+Version: 0.6.1
 Summary: A python library to work with objects retrieved from the notion API
 Home-page: https://github.com/thrau/notion-objects
 Author: Thomas Rausch
 Author-email: thomas@thrau.at
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 4 - Beta
```

### Comparing `notion-objects-0.6.0/setup.cfg` & `notion-objects-0.6.1/setup.cfg`

 * *Files identical despite different names*

