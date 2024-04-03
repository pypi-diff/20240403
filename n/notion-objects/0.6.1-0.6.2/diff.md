# Comparing `tmp/notion-objects-0.6.1.tar.gz` & `tmp/notion-objects-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notion-objects-0.6.1.tar", last modified: Wed Apr  3 13:10:21 2024, max compression
+gzip compressed data, was "notion-objects-0.6.2.tar", last modified: Wed Apr  3 13:42:30 2024, max compression
```

## Comparing `notion-objects-0.6.1.tar` & `notion-objects-0.6.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-04-03 13:10:21.184106 notion-objects-0.6.1/
--rw-r--r--   0 thomas    (1000) thomas    (1000)    11357 2023-02-17 21:11:05.000000 notion-objects-0.6.1/LICENSE
--rw-r--r--   0 thomas    (1000) thomas    (1000)     5831 2024-04-03 13:10:21.184106 notion-objects-0.6.1/PKG-INFO
--rw-r--r--   0 thomas    (1000) thomas    (1000)     4666 2023-10-14 04:05:06.000000 notion-objects-0.6.1/README.md
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-04-03 13:10:21.184106 notion-objects-0.6.1/notion_objects/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      118 2024-04-03 12:22:01.000000 notion-objects-0.6.1/notion_objects/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     6960 2024-03-31 16:36:48.000000 notion-objects-0.6.1/notion_objects/database.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2191 2024-04-03 12:28:24.000000 notion-objects-0.6.1/notion_objects/encode.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     2833 2024-03-28 13:17:36.000000 notion-objects-0.6.1/notion_objects/objects.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    21579 2024-04-03 12:28:24.000000 notion-objects-0.6.1/notion_objects/properties.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5172 2024-03-31 16:36:48.000000 notion-objects-0.6.1/notion_objects/rich_text.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      766 2024-04-03 12:12:50.000000 notion-objects-0.6.1/notion_objects/values.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-04-03 13:10:21.184106 notion-objects-0.6.1/notion_objects.egg-info/
--rw-r--r--   0 thomas    (1000) thomas    (1000)     5831 2024-04-03 13:10:21.000000 notion-objects-0.6.1/notion_objects.egg-info/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      455 2024-04-03 13:10:21.000000 notion-objects-0.6.1/notion_objects.egg-info/SOURCES.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2024-04-03 13:10:21.000000 notion-objects-0.6.1/notion_objects.egg-info/dependency_links.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2024-04-03 13:10:21.000000 notion-objects-0.6.1/notion_objects.egg-info/not-zip-safe
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      132 2024-04-03 13:10:21.000000 notion-objects-0.6.1/notion_objects.egg-info/requires.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       15 2024-04-03 13:10:21.000000 notion-objects-0.6.1/notion_objects.egg-info/top_level.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)      503 2023-02-17 21:11:05.000000 notion-objects-0.6.1/pyproject.toml
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1100 2024-04-03 13:10:21.184106 notion-objects-0.6.1/setup.cfg
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-04-03 13:42:30.981337 notion-objects-0.6.2/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    11357 2023-02-17 21:11:05.000000 notion-objects-0.6.2/LICENSE
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     5831 2024-04-03 13:42:30.981337 notion-objects-0.6.2/PKG-INFO
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     4666 2023-10-14 04:05:06.000000 notion-objects-0.6.2/README.md
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-04-03 13:42:30.977337 notion-objects-0.6.2/notion_objects/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      118 2024-04-03 13:20:51.000000 notion-objects-0.6.2/notion_objects/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     6960 2024-03-31 16:36:48.000000 notion-objects-0.6.2/notion_objects/database.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2191 2024-04-03 12:28:24.000000 notion-objects-0.6.2/notion_objects/encode.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2833 2024-03-28 13:17:36.000000 notion-objects-0.6.2/notion_objects/objects.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    21574 2024-04-03 13:19:32.000000 notion-objects-0.6.2/notion_objects/properties.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5172 2024-03-31 16:36:48.000000 notion-objects-0.6.2/notion_objects/rich_text.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      766 2024-04-03 12:12:50.000000 notion-objects-0.6.2/notion_objects/values.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-04-03 13:42:30.977337 notion-objects-0.6.2/notion_objects.egg-info/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     5831 2024-04-03 13:42:30.000000 notion-objects-0.6.2/notion_objects.egg-info/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      455 2024-04-03 13:42:30.000000 notion-objects-0.6.2/notion_objects.egg-info/SOURCES.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2024-04-03 13:42:30.000000 notion-objects-0.6.2/notion_objects.egg-info/dependency_links.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2024-04-03 13:42:30.000000 notion-objects-0.6.2/notion_objects.egg-info/not-zip-safe
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      132 2024-04-03 13:42:30.000000 notion-objects-0.6.2/notion_objects.egg-info/requires.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       15 2024-04-03 13:42:30.000000 notion-objects-0.6.2/notion_objects.egg-info/top_level.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      503 2023-02-17 21:11:05.000000 notion-objects-0.6.2/pyproject.toml
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1100 2024-04-03 13:42:30.981337 notion-objects-0.6.2/setup.cfg
```

### Comparing `notion-objects-0.6.1/LICENSE` & `notion-objects-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `notion-objects-0.6.1/PKG-INFO` & `notion-objects-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notion-objects
-Version: 0.6.1
+Version: 0.6.2
 Summary: A python library to work with objects retrieved from the notion API
 Home-page: https://github.com/thrau/notion-objects
 Author: Thomas Rausch
 Author-email: thomas@thrau.at
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 4 - Beta
```

### Comparing `notion-objects-0.6.1/README.md` & `notion-objects-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `notion-objects-0.6.1/notion_objects/database.py` & `notion-objects-0.6.2/notion_objects/database.py`

 * *Files identical despite different names*

### Comparing `notion-objects-0.6.1/notion_objects/encode.py` & `notion-objects-0.6.2/notion_objects/encode.py`

 * *Files identical despite different names*

### Comparing `notion-objects-0.6.1/notion_objects/objects.py` & `notion-objects-0.6.2/notion_objects/objects.py`

 * *Files identical despite different names*

### Comparing `notion-objects-0.6.1/notion_objects/properties.py` & `notion-objects-0.6.2/notion_objects/properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,15 +213,15 @@
 
 class TitleText(Property[str]):
     type = "title"
 
     def get(self, field: str, obj: dict) -> str:
         items = obj["properties"][field]["title"]
         if items:
-            return "".join([item["text"]["content"] for item in items])
+            return "".join([item["plain_text"] for item in items])
         return ""
 
     def set(self, field: str, value: Optional[str], obj: dict):
         # TODO: allow rich-text
         obj[field] = {
             "title": [
                 {
```

### Comparing `notion-objects-0.6.1/notion_objects/rich_text.py` & `notion-objects-0.6.2/notion_objects/rich_text.py`

 * *Files identical despite different names*

### Comparing `notion-objects-0.6.1/notion_objects/values.py` & `notion-objects-0.6.2/notion_objects/values.py`

 * *Files identical despite different names*

### Comparing `notion-objects-0.6.1/notion_objects.egg-info/PKG-INFO` & `notion-objects-0.6.2/notion_objects.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notion-objects
-Version: 0.6.1
+Version: 0.6.2
 Summary: A python library to work with objects retrieved from the notion API
 Home-page: https://github.com/thrau/notion-objects
 Author: Thomas Rausch
 Author-email: thomas@thrau.at
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 4 - Beta
```

### Comparing `notion-objects-0.6.1/setup.cfg` & `notion-objects-0.6.2/setup.cfg`

 * *Files identical despite different names*

