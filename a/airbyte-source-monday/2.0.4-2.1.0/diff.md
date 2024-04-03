# Comparing `tmp/airbyte_source_monday-2.0.4.tar.gz` & `tmp/airbyte_source_monday-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_monday-2.0.4.tar", max compression
+gzip compressed data, was "airbyte_source_monday-2.1.0.tar", max compression
```

## Comparing `airbyte_source_monday-2.0.4.tar` & `airbyte_source_monday-2.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     4496 2024-02-28 11:30:26.000000 airbyte_source_monday-2.0.4/README.md
--rw-r--r--   0        0        0      745 2024-02-28 11:41:56.617318 airbyte_source_monday-2.0.4/pyproject.toml
--rw-r--r--   0        0        0      203 2024-02-28 11:30:26.000000 airbyte_source_monday-2.0.4/source_monday/__init__.py
--rw-r--r--   0        0        0    10081 2024-02-28 11:30:26.000000 airbyte_source_monday-2.0.4/source_monday/components.py
--rw-r--r--   0        0        0     4839 2024-02-28 11:30:26.000000 airbyte_source_monday-2.0.4/source_monday/extractor.py
--rw-r--r--   0        0        0    11056 2024-02-28 11:30:26.000000 airbyte_source_monday-2.0.4/source_monday/graphql_requester.py
--rw-r--r--   0        0        0     4401 2024-02-28 11:30:26.000000 airbyte_source_monday-2.0.4/source_monday/item_pagination_strategy.py
--rw-r--r--   0        0        0     6699 2024-02-28 11:30:26.000000 airbyte_source_monday-2.0.4/source_monday/manifest.yaml
--rw-r--r--   0        0        0      230 2024-02-28 11:30:26.000000 airbyte_source_monday-2.0.4/source_monday/run.py
--rw-r--r--   0        0        0      481 2024-02-28 11:30:26.000000 airbyte_source_monday-2.0.4/source_monday/schemas/activity_logs.json
--rw-r--r--   0        0        0     3633 2024-02-28 11:30:26.000000 airbyte_source_monday-2.0.4/source_monday/schemas/boards.json
--rw-r--r--   0        0        0     2694 2024-02-28 11:30:26.000000 airbyte_source_monday-2.0.4/source_monday/schemas/items.json
--rw-r--r--   0        0        0      232 2024-02-28 11:30:26.000000 airbyte_source_monday-2.0.4/source_monday/schemas/tags.json
--rw-r--r--   0        0        0      474 2024-02-28 11:30:26.000000 airbyte_source_monday-2.0.4/source_monday/schemas/teams.json
--rw-r--r--   0        0        0     1916 2024-02-28 11:30:26.000000 airbyte_source_monday-2.0.4/source_monday/schemas/updates.json
--rw-r--r--   0        0        0     1408 2024-02-28 11:30:26.000000 airbyte_source_monday-2.0.4/source_monday/schemas/users.json
--rw-r--r--   0        0        0     1982 2024-02-28 11:30:26.000000 airbyte_source_monday-2.0.4/source_monday/schemas/workspaces.json
--rw-r--r--   0        0        0      474 2024-02-28 11:30:26.000000 airbyte_source_monday-2.0.4/source_monday/source.py
--rw-r--r--   0        0        0     3989 2024-02-28 11:30:26.000000 airbyte_source_monday-2.0.4/source_monday/spec.json
--rw-r--r--   0        0        0     5200 1970-01-01 00:00:00.000000 airbyte_source_monday-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0     4496 2024-04-03 10:39:23.000000 airbyte_source_monday-2.1.0/README.md
+-rw-r--r--   0        0        0      739 2024-04-03 10:52:21.842249 airbyte_source_monday-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      203 2024-04-03 10:39:23.000000 airbyte_source_monday-2.1.0/source_monday/__init__.py
+-rw-r--r--   0        0        0    10241 2024-04-03 10:39:23.000000 airbyte_source_monday-2.1.0/source_monday/components.py
+-rw-r--r--   0        0        0     4839 2024-04-03 10:39:23.000000 airbyte_source_monday-2.1.0/source_monday/extractor.py
+-rw-r--r--   0        0        0    11056 2024-04-03 10:39:23.000000 airbyte_source_monday-2.1.0/source_monday/graphql_requester.py
+-rw-r--r--   0        0        0     4401 2024-04-03 10:39:23.000000 airbyte_source_monday-2.1.0/source_monday/item_pagination_strategy.py
+-rw-r--r--   0        0        0     6699 2024-04-03 10:39:23.000000 airbyte_source_monday-2.1.0/source_monday/manifest.yaml
+-rw-r--r--   0        0        0      230 2024-04-03 10:39:23.000000 airbyte_source_monday-2.1.0/source_monday/run.py
+-rw-r--r--   0        0        0      481 2024-04-03 10:39:23.000000 airbyte_source_monday-2.1.0/source_monday/schemas/activity_logs.json
+-rw-r--r--   0        0        0     3633 2024-04-03 10:39:23.000000 airbyte_source_monday-2.1.0/source_monday/schemas/boards.json
+-rw-r--r--   0        0        0     2694 2024-04-03 10:39:23.000000 airbyte_source_monday-2.1.0/source_monday/schemas/items.json
+-rw-r--r--   0        0        0      232 2024-04-03 10:39:23.000000 airbyte_source_monday-2.1.0/source_monday/schemas/tags.json
+-rw-r--r--   0        0        0      474 2024-04-03 10:39:23.000000 airbyte_source_monday-2.1.0/source_monday/schemas/teams.json
+-rw-r--r--   0        0        0     1916 2024-04-03 10:39:23.000000 airbyte_source_monday-2.1.0/source_monday/schemas/updates.json
+-rw-r--r--   0        0        0     1408 2024-04-03 10:39:23.000000 airbyte_source_monday-2.1.0/source_monday/schemas/users.json
+-rw-r--r--   0        0        0     1982 2024-04-03 10:39:23.000000 airbyte_source_monday-2.1.0/source_monday/schemas/workspaces.json
+-rw-r--r--   0        0        0      474 2024-04-03 10:39:23.000000 airbyte_source_monday-2.1.0/source_monday/source.py
+-rw-r--r--   0        0        0     3989 2024-04-03 10:39:23.000000 airbyte_source_monday-2.1.0/source_monday/spec.json
+-rw-r--r--   0        0        0     5198 1970-01-01 00:00:00.000000 airbyte_source_monday-2.1.0/PKG-INFO
```

### Comparing `airbyte_source_monday-2.0.4/README.md` & `airbyte_source_monday-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_monday-2.0.4/pyproject.toml` & `airbyte_source_monday-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.0.4"
+version = "2.1.0"
 name = "airbyte-source-monday"
 description = "Source implementation for Monday."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -18,15 +18,15 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_monday" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "==0.62.0"
+airbyte-cdk = "^0"
 
 [tool.poetry.scripts]
 source-monday = "source_monday.run:run"
 
 [tool.poetry.group.dev.dependencies]
 requests-mock = "^1.9.3"
 pytest-mock = "^3.6.1"
```

### Comparing `airbyte_source_monday-2.0.4/source_monday/components.py` & `airbyte_source_monday-2.1.0/source_monday/components.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         latest_record = self._state if self.is_greater_than_or_equal(self._state, most_recent_record) else most_recent_record
 
         if not latest_record:
             return
         self._state[self.cursor_field.eval(self.config)] = latest_record[self.cursor_field.eval(self.config)]
 
     def stream_slices(self) -> Iterable[Mapping[str, Any]]:
-        yield {}
+        yield StreamSlice(partition={}, cursor_slice={})
 
     def should_be_synced(self, record: Record) -> bool:
         """
         As of 2023-06-28, the expectation is that this method will only be used for semi-incremental and data feed and therefore the
         implementation is irrelevant for greenhouse
         """
         return True
@@ -166,15 +166,15 @@
         self, sync_mode: SyncMode, cursor_field: Optional[str], stream_state: Mapping[str, Any]
     ) -> Iterable[Mapping[str, Any]]:
         self.parent_stream.state = stream_state
 
         # check if state is empty ->
         if not stream_state.get(self.parent_cursor_field):
             # yield empty slice for complete fetch of items stream
-            yield {}
+            yield StreamSlice(partition={}, cursor_slice={})
             return
 
         all_ids = set()
         slice_ids = list()
         empty_parent_slice = True
 
         for parent_slice in self.parent_stream.stream_slices(sync_mode=sync_mode, cursor_field=cursor_field, stream_state=stream_state):
@@ -196,19 +196,19 @@
                     # check if record with this id was already processed
                     if substream_slice not in all_ids:
                         all_ids.add(substream_slice)
                         slice_ids.append(substream_slice)
 
                         # yield slice with desired number of ids
                         if self.nested_items_per_page == len(slice_ids):
-                            yield {self.substream_slice_field: slice_ids}
+                            yield StreamSlice(partition={self.substream_slice_field: slice_ids}, cursor_slice={})
                             slice_ids = list()
         # yield leftover ids if any left
         if slice_ids:
-            yield {self.substream_slice_field: slice_ids}
+            yield StreamSlice(partition={self.substream_slice_field: slice_ids}, cursor_slice={})
 
         # If the parent slice contains no records
         if empty_parent_slice:
             yield from []
 
     def stream_slices(self) -> Iterable[Mapping[str, Any]]:
         parent_state = (self._state or {}).get(self.parent_stream_name, {})
```

### Comparing `airbyte_source_monday-2.0.4/source_monday/extractor.py` & `airbyte_source_monday-2.1.0/source_monday/extractor.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_monday-2.0.4/source_monday/graphql_requester.py` & `airbyte_source_monday-2.1.0/source_monday/graphql_requester.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_monday-2.0.4/source_monday/item_pagination_strategy.py` & `airbyte_source_monday-2.1.0/source_monday/item_pagination_strategy.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_monday-2.0.4/source_monday/manifest.yaml` & `airbyte_source_monday-2.1.0/source_monday/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_monday-2.0.4/source_monday/schemas/boards.json` & `airbyte_source_monday-2.1.0/source_monday/schemas/boards.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_monday-2.0.4/source_monday/schemas/items.json` & `airbyte_source_monday-2.1.0/source_monday/schemas/items.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_monday-2.0.4/source_monday/schemas/updates.json` & `airbyte_source_monday-2.1.0/source_monday/schemas/updates.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_monday-2.0.4/source_monday/schemas/users.json` & `airbyte_source_monday-2.1.0/source_monday/schemas/users.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_monday-2.0.4/source_monday/schemas/workspaces.json` & `airbyte_source_monday-2.1.0/source_monday/schemas/workspaces.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_monday-2.0.4/source_monday/spec.json` & `airbyte_source_monday-2.1.0/source_monday/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_monday-2.0.4/PKG-INFO` & `airbyte_source_monday-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-monday
-Version: 2.0.4
+Version: 2.1.0
 Summary: Source implementation for Monday.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: airbyte-cdk (==0.62.0)
+Requires-Dist: airbyte-cdk (>=0,<1)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/monday
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Monday source connector
```

