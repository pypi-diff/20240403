# Comparing `tmp/galaxy-schema-23.2.1.tar.gz` & `tmp/galaxy-schema-24.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/schema/dist/.tmp-p26hm_85/galaxy-schema-23.2.1.tar", last modified: Thu Feb 22 03:53:06 2024, max compression
+gzip compressed data, was "galaxy-schema-24.0.0.tar", last modified: Wed Apr  3 02:44:52 2024, max compression
```

## Comparing `galaxy-schema-23.2.1.tar` & `galaxy-schema-24.0.0.tar`

### file list

```diff
@@ -1,59 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:06.000000 galaxy-schema-23.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-02-22 03:53:06.000000 galaxy-schema-23.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:06.000000 galaxy-schema-23.2.1/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:06.000000 galaxy-schema-23.2.1/galaxy/schema/
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:06.000000 galaxy-schema-23.2.1/galaxy/schema/bco/
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/bco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/bco/description_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/bco/error_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/bco/execution_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/bco/io_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/bco/parametric_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/bco/provenance_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/bco/usability_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/bco/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:06.000000 galaxy-schema-23.2.1/galaxy/schema/drs/
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/drs/AccessMethod.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/drs/AccessURL.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/drs/Checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/drs/ContentsObject.py
--rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/drs/DrsObject.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/drs/DrsService.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/drs/Error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/drs/Service.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/drs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6946 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/fetch_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/help.py
--rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/invocation.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/item_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17175 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/remote_files.py
--rw-r--r--   0 runner    (1001) docker     (127)   115397 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/storage_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:06.000000 galaxy-schema-23.2.1/galaxy/schema/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/galaxy/schema/workflow/comments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:06.000000 galaxy-schema-23.2.1/galaxy_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-02-22 03:53:06.000000 galaxy-schema-23.2.1/galaxy_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-02-22 03:53:06.000000 galaxy-schema-23.2.1/galaxy_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 03:53:06.000000 galaxy-schema-23.2.1/galaxy_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-22 03:53:06.000000 galaxy-schema-23.2.1/galaxy_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-22 03:53:06.000000 galaxy-schema-23.2.1/galaxy_schema.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-02-22 03:53:06.000000 galaxy-schema-23.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-22 03:50:43.000000 galaxy-schema-23.2.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:52.922922 galaxy-schema-24.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-04-03 02:44:52.922922 galaxy-schema-24.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:52.914922 galaxy-schema-24.0.0/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:52.918922 galaxy-schema-24.0.0/galaxy/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:52.918922 galaxy-schema-24.0.0/galaxy/schema/bco/
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/bco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/bco/description_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/bco/error_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/bco/execution_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/bco/io_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/bco/parametric_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/bco/provenance_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/bco/usability_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/bco/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:52.918922 galaxy-schema-24.0.0/galaxy/schema/drs/
+-rw-r--r--   0 runner    (1001) docker     (127)    13396 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/drs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/fetch_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25194 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/invocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/item_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9118 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17423 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/remote_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)   117967 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/storage_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:52.918922 galaxy-schema-24.0.0/galaxy/schema/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/workflow/comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:52.922922 galaxy-schema-24.0.0/galaxy_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-04-03 02:44:52.000000 galaxy-schema-24.0.0/galaxy_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-03 02:44:52.000000 galaxy-schema-24.0.0/galaxy_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:44:52.000000 galaxy-schema-24.0.0/galaxy_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 02:44:52.000000 galaxy-schema-24.0.0/galaxy_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:44:52.000000 galaxy-schema-24.0.0/galaxy_schema.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-03 02:44:52.922922 galaxy-schema-24.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `galaxy-schema-23.2.1/LICENSE` & `galaxy-schema-24.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-schema-23.2.1/galaxy/schema/__init__.py` & `galaxy-schema-24.0.0/galaxy/schema/tasks.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,115 +1,121 @@
-from datetime import datetime
-from enum import Enum
 from typing import (
-    Dict,
     List,
     Optional,
-    Union,
 )
+from uuid import UUID
 
-from pydantic import (
-    BaseModel,
-    Field,
-    Required,
+from pydantic import Field
+
+from galaxy.util.hash_util import HashFunctionNameEnum
+from . import PdfDocumentType
+from .schema import (
+    BcoGenerationParametersMixin,
+    DatasetSourceType,
+    HistoryContentType,
+    Model,
+    ModelStoreFormat,
+    ShortTermStoreExportPayload,
+    WriteStoreToPayload,
 )
 
 
-class BootstrapAdminUser(BaseModel):
-    id = 0
-    email: Optional[str] = None
-    preferences: Dict[str, str] = {}
-    bootstrap_admin_user = True
-
-    def all_roles(*args) -> list:
-        return []
-
-
-class ValueFilterQueryParams(BaseModel):
-    """Allows filtering/querying elements by value like `q=<property>-<operator>&qv=<value>`
-
-    Multiple `q/qv` queries can be concatenated.
-    """
-
-    q: Optional[Union[List[str], str]] = Field(
-        default=None,
-        title="Filter Query",
-        description="Generally a property name to filter by followed by an (often optional) hyphen and operator string.",
-        example="create_time-gt",
-    )
-    qv: Optional[Union[List[str], str]] = Field(
-        default=None,
-        title="Filter Value",
-        description="The value to filter by.",
-        example="2015-01-29",
-    )
+class SetupHistoryExportJob(Model):
+    history_id: int
+    job_id: int
+    store_directory: str
+    include_files: bool
+    include_hidden: bool
+    include_deleted: bool
 
 
-class PaginationQueryParams(BaseModel):
-    """Used to paginate a the request results by limiting and offsetting."""
+class PrepareDatasetCollectionDownload(Model):
+    short_term_storage_request_id: UUID
+    history_dataset_collection_association_id: int
 
-    offset: Optional[int] = Field(
-        default=0,
-        ge=0,
-        title="Offset",
-        description="Starts at the beginning skip the first ( offset - 1 ) items and begin returning at the Nth item",
-    )
-    limit: Optional[int] = Field(
-        default=None,
-        ge=1,
-        title="Limit",
-        description="The maximum number of items to return.",
-    )
 
+class GeneratePdfDownload(Model):
+    short_term_storage_request_id: UUID
+    # basic markdown - Galaxy directives need to be processed before handing off to this task
+    basic_markdown: str
+    document_type: PdfDocumentType
 
-class FilterQueryParams(ValueFilterQueryParams, PaginationQueryParams):
-    """Contains full filtering options to query elements, paginate and order them."""
 
-    order: Optional[str] = Field(
-        default=None,
-        title="Order",
-        description=(
-            "String containing one of the valid ordering attributes followed (optionally) "
-            "by '-asc' or '-dsc' for ascending and descending order respectively. "
-            "Orders can be stacked as a comma-separated list of values."
-        ),
-        example="name-dsc,create_time",
-    )
+# serialize user info for tasks
+class RequestUser(Model):
+    user_id: int
+    # TODO: allow make the above optional and allow a session_id for anonymous users...
+    # session_id: Optional[str]
 
 
-class SerializationParams(BaseModel):
-    """Contains common parameters for customizing model serialization."""
+class GenerateHistoryDownload(ShortTermStoreExportPayload):
+    history_id: int
+    user: RequestUser
+    export_association_id: Optional[int] = None
 
-    view: Optional[str] = Field(
-        default=None,
-        title="View",
-        description=(
-            "The name of the view used to serialize this item. "
-            "This will return a predefined set of attributes of the item."
-        ),
-        example="summary",
+
+class GenerateHistoryContentDownload(ShortTermStoreExportPayload):
+    content_type: HistoryContentType
+    content_id: int
+    user: RequestUser
+
+
+class BcoGenerationTaskParametersMixin(BcoGenerationParametersMixin):
+    galaxy_url: str
+
+
+class GenerateInvocationDownload(ShortTermStoreExportPayload, BcoGenerationTaskParametersMixin):
+    invocation_id: int
+    user: RequestUser
+
+
+class WriteInvocationTo(WriteStoreToPayload, BcoGenerationTaskParametersMixin):
+    invocation_id: int
+    user: RequestUser
+
+
+class WriteHistoryContentTo(WriteStoreToPayload):
+    content_type: HistoryContentType
+    content_id: int
+    user: RequestUser
+
+
+class WriteHistoryTo(WriteStoreToPayload):
+    history_id: int
+    user: RequestUser
+    export_association_id: Optional[int] = None
+
+
+class ImportModelStoreTaskRequest(Model):
+    user: RequestUser
+    history_id: Optional[int] = None
+    source_uri: str
+    for_library: bool
+    model_store_format: Optional[ModelStoreFormat] = None
+
+
+class MaterializeDatasetInstanceTaskRequest(Model):
+    history_id: int
+    user: RequestUser
+    source: DatasetSourceType = Field(
+        title="Source",
+        description="The source of the content. Can be other history element to be copied or library elements.",
     )
-    keys: Optional[List[str]] = Field(
-        default=None,
-        title="Keys",
+    content: int = Field(
+        title="Content",
         description=(
-            "List of keys (name of the attributes) that will be returned in addition "
-            "to the ones included in the `view`."
+            "Depending on the `source` it can be:\n"
+            "- The encoded id of the source library dataset\n"
+            "- The encoded id of the HDA\n"
         ),
     )
-    default_view: Optional[str] = Field(
-        default=None,
-        title="Default View",
-        description="The item view that will be used in case none was specified.",
-    )
 
 
-class PdfDocumentType(str, Enum):
-    invocation_report = "invocation_report"
-    page = "page"
+class ComputeDatasetHashTaskRequest(Model):
+    dataset_id: int
+    extra_files_path: Optional[str] = None
+    hash_function: HashFunctionNameEnum
+    user: Optional[RequestUser] = None  # access checks should be done pre-celery so this is optional
 
 
-class APIKeyModel(BaseModel):
-    key: str = Field(Required, title="Key", description="API key to interact with the Galaxy API")
-    create_time: datetime = Field(
-        Required, title="Create Time", description="The time and date this API key was created."
-    )
+class PurgeDatasetsTaskRequest(Model):
+    dataset_ids: List[int]
```

### Comparing `galaxy-schema-23.2.1/galaxy/schema/bco/__init__.py` & `galaxy-schema-24.0.0/galaxy/schema/bco/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,17 +39,15 @@
 
 class GalaxyExtension(BaseModel):
     galaxy_url: str
     galaxy_version: str
 
 
 class GalaxyExtensionDomain(BaseModel):
-    extension_schema: Literal[
-        "https://raw.githubusercontent.com/biocompute-objects/extension_domain/1.2.0/galaxy/galaxy_extension.json"
-    ] = "https://raw.githubusercontent.com/biocompute-objects/extension_domain/1.2.0/galaxy/galaxy_extension.json"
+    extension_schema: Literal["galaxy_extension.json"] = "galaxy_extension.json"
     galaxy_extension: GalaxyExtension
 
 
 class BioComputeObjectCore(BaseModel):
     """BioComputeObject pre-hash, used to generate etag."""
 
     description_domain: DescriptionDomain
```

### Comparing `galaxy-schema-23.2.1/galaxy/schema/bco/description_domain.py` & `galaxy-schema-24.0.0/galaxy/schema/bco/description_domain.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,43 +10,43 @@
     List,
     Optional,
 )
 
 from pydantic import (
     AnyUrl,
     BaseModel,
+    ConfigDict,
     EmailStr,
-    Extra,
     Field,
+    RootModel,
 )
 
 
 class XrefItem(BaseModel):
-    namespace: str = Field(..., description="External resource vendor prefix", example=["pubchem.compound"])
-    name: str = Field(..., description="Name of external reference", example=["PubChem-compound"])
+    namespace: str = Field(..., description="External resource vendor prefix", examples=["pubchem.compound"])
+    name: str = Field(..., description="Name of external reference", examples=["PubChem-compound"])
     ids: List[str] = Field(..., description="List of reference identifiers")
     access_time: datetime = Field(..., description="Date and time the external reference was accessed")
 
 
 class Uri(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     filename: Optional[str] = None
     uri: AnyUrl
     access_time: Optional[datetime] = Field(
         None, description="Time stamp of when the request for this data was submitted"
     )
     sha1_checksum: Optional[str] = Field(
-        None, description="output of hash function that produces a message digest", regex="[A-Za-z0-9]+"
+        None, description="output of hash function that produces a message digest", pattern="[A-Za-z0-9]+"
     )
 
 
-class ObjectId(BaseModel):
-    __root__: str = Field(
+class ObjectId(RootModel):
+    root: str = Field(
         ...,
         description="A unique identifier that should be applied to each IEEE-2791 Object instance, generated and assigned by a IEEE-2791 database engine. IDs should never be reused",
     )
 
 
 class ContributionEnum(Enum):
     authoredBy = "authoredBy"
@@ -61,59 +61,57 @@
     providedBy = "providedBy"
     retrievedBy = "retrievedBy"
     retrievedFrom = "retrievedFrom"
     sourceAccessedBy = "sourceAccessedBy"
 
 
 class Contributor(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
-    name: str = Field(..., description="Name of contributor", example=["Charles Darwin"])
+    name: str = Field(..., description="Name of contributor", examples=["Charles Darwin"])
     affiliation: Optional[str] = Field(
-        None, description="Organization the particular contributor is affiliated with", example=["HMS Beagle"]
+        None, description="Organization the particular contributor is affiliated with", examples=["HMS Beagle"]
     )
     email: Optional[EmailStr] = Field(
         None,
         description="electronic means for identification and communication purposes",
-        example=["name@example.edu"],
+        examples=["name@example.edu"],
     )
     contribution: List[ContributionEnum] = Field(
         ..., description="type of contribution determined according to PAV ontology"
     )
     orcid: Optional[AnyUrl] = Field(
         None,
         description="Field to record author information. ORCID identifiers allow for the author to curate their information after submission. ORCID identifiers must be valid and must have the prefix ‘https://orcid.org/’",
-        example=["http://orcid.org/0000-0002-1825-0097"],
+        examples=["http://orcid.org/0000-0002-1825-0097"],
     )
 
 
 class PrerequisiteItem(BaseModel):
     name: str = Field(
-        ..., description="Public searchable name for reference or prereq.", example=["Hepatitis C virus genotype 1"]
+        ..., description="Public searchable name for reference or prereq.", examples=["Hepatitis C virus genotype 1"]
     )
     uri: Uri
 
 
 class PipelineStep(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     step_number: int = Field(
         ...,
         description="Non-negative integer value representing the position of the tool in a one-dimensional representation of the pipeline.",
     )
-    name: str = Field(..., description="This is a recognized name of the software tool", example=["HIVE-hexagon"])
+    name: str = Field(..., description="This is a recognized name of the software tool", examples=["HIVE-hexagon"])
     description: str = Field(
-        ..., description="Specific purpose of the tool.", example=["Alignment of reads to a set of references"]
+        ..., description="Specific purpose of the tool.", examples=["Alignment of reads to a set of references"]
     )
     version: Optional[str] = Field(
         None,
         description="Version assigned to the instance of the tool used corresponding to the upstream release.",
-        example=["1.3"],
+        examples=["1.3"],
     )
     prerequisite: Optional[List[PrerequisiteItem]] = Field(None, description="Reference or required prereqs")
     input_list: List[Uri] = Field(..., description="URIs (expressed as a URN or URL) of the input files for each tool.")
     output_list: List[Uri] = Field(
         ..., description="URIs (expressed as a URN or URL) of the output files for each tool."
     )
```

### Comparing `galaxy-schema-23.2.1/galaxy/schema/bco/error_domain.py` & `galaxy-schema-24.0.0/galaxy/schema/bco/error_domain.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,22 +7,21 @@
 from typing import (
     Any,
     Dict,
 )
 
 from pydantic import (
     BaseModel,
-    Extra,
+    ConfigDict,
     Field,
 )
 
 
 class ErrorDomain(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     empirical_error: Dict[str, Any] = Field(
         ...,
         description="empirically determined values such as limits of detectability, false positives, false negatives, statistical confidence of outcomes, etc. This can be measured by running the algorithm on multiple data samples of the usability domain or through the use of carefully designed in-silico data.",
         title="Empirical Error",
     )
     algorithmic_error: Dict[str, Any] = Field(
```

### Comparing `galaxy-schema-23.2.1/galaxy/schema/bco/execution_domain.py` & `galaxy-schema-24.0.0/galaxy/schema/bco/execution_domain.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,50 +11,49 @@
     List,
     Optional,
 )
 
 from pydantic import (
     AnyUrl,
     BaseModel,
+    ConfigDict,
     EmailStr,
-    Extra,
     Field,
+    RootModel,
 )
 
 
 class ExternalDataEndpoint(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     name: str = Field(
-        ..., description="Description of the service that is accessed", example=["HIVE", "access to e-utils"]
+        ..., description="Description of the service that is accessed", examples=["HIVE", "access to e-utils"]
     )
     url: str = Field(
         ...,
         description="The endpoint to be accessed.",
-        example=["https://hive.biochemistry.gwu.edu/dna.cgi?cmd=login"],
+        examples=["https://hive.biochemistry.gwu.edu/dna.cgi?cmd=login"],
     )
 
 
 class Uri(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     filename: Optional[str] = None
     uri: AnyUrl
     access_time: Optional[datetime] = Field(
         None, description="Time stamp of when the request for this data was submitted"
     )
     sha1_checksum: Optional[str] = Field(
-        None, description="output of hash function that produces a message digest", regex="[A-Za-z0-9]+"
+        None, description="output of hash function that produces a message digest", pattern="[A-Za-z0-9]+"
     )
 
 
-class ObjectId(BaseModel):
-    __root__: str = Field(
+class ObjectId(RootModel):
+    root: str = Field(
         ...,
         description="A unique identifier that should be applied to each IEEE-2791 Object instance, generated and assigned by a IEEE-2791 database engine. IDs should never be reused",
     )
 
 
 class ContributionEnum(Enum):
     authoredBy = "authoredBy"
@@ -69,64 +68,60 @@
     providedBy = "providedBy"
     retrievedBy = "retrievedBy"
     retrievedFrom = "retrievedFrom"
     sourceAccessedBy = "sourceAccessedBy"
 
 
 class Contributor(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
-    name: str = Field(..., description="Name of contributor", example=["Charles Darwin"])
+    name: str = Field(..., description="Name of contributor", examples=["Charles Darwin"])
     affiliation: Optional[str] = Field(
-        None, description="Organization the particular contributor is affiliated with", example=["HMS Beagle"]
+        None, description="Organization the particular contributor is affiliated with", examples=["HMS Beagle"]
     )
     email: Optional[EmailStr] = Field(
         None,
         description="electronic means for identification and communication purposes",
-        example=["name@example.edu"],
+        examples=["name@example.edu"],
     )
     contribution: List[ContributionEnum] = Field(
         ..., description="type of contribution determined according to PAV ontology"
     )
     orcid: Optional[AnyUrl] = Field(
         None,
         description="Field to record author information. ORCID identifiers allow for the author to curate their information after submission. ORCID identifiers must be valid and must have the prefix ‘https://orcid.org/’",
-        example=["http://orcid.org/0000-0002-1825-0097"],
+        examples=["http://orcid.org/0000-0002-1825-0097"],
     )
 
 
 class ScriptItem(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     uri: Optional[Uri] = None
 
 
 class SoftwarePrerequisite(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
-    name: str = Field(..., description="Names of software prerequisites", example=["HIVE-hexagon"])
-    version: str = Field(..., description="Versions of the software prerequisites", example=["babajanian.1"])
+    name: str = Field(..., description="Names of software prerequisites", examples=["HIVE-hexagon"])
+    version: str = Field(..., description="Versions of the software prerequisites", examples=["babajanian.1"])
     uri: Uri
 
 
 class ExecutionDomain(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     script: List[ScriptItem] = Field(
         ...,
         description="points to a script object or objects that was used to perform computations for this IEEE-2791 Object instance.",
     )
     script_driver: str = Field(
         ...,
         description="Indication of the kind of executable that can be launched in order to perform a sequence of commands described in the script in order to run the pipelin",
-        example=["hive", "cwl-runner", "shell"],
+        examples=["hive", "cwl-runner", "shell"],
     )
     software_prerequisites: List[SoftwarePrerequisite] = Field(
         ...,
         description="Minimal necessary prerequisites, library, tool versions needed to successfully run the script to produce this IEEE-2791 Object.",
     )
     external_data_endpoints: List[ExternalDataEndpoint] = Field(
         ...,
```

### Comparing `galaxy-schema-23.2.1/galaxy/schema/bco/io_domain.py` & `galaxy-schema-24.0.0/galaxy/schema/bco/io_domain.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,36 +10,36 @@
     List,
     Optional,
 )
 
 from pydantic import (
     AnyUrl,
     BaseModel,
+    ConfigDict,
     EmailStr,
-    Extra,
     Field,
+    RootModel,
 )
 
 
 class Uri(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     filename: Optional[str] = None
     uri: AnyUrl
     access_time: Optional[datetime] = Field(
         None, description="Time stamp of when the request for this data was submitted"
     )
     sha1_checksum: Optional[str] = Field(
-        None, description="output of hash function that produces a message digest", regex="[A-Za-z0-9]+"
+        None, description="output of hash function that produces a message digest", pattern="[A-Za-z0-9]+"
     )
 
 
-class ObjectId(BaseModel):
-    __root__: str = Field(
+class ObjectId(RootModel):
+    root: str = Field(
         ...,
         description="A unique identifier that should be applied to each IEEE-2791 Object instance, generated and assigned by a IEEE-2791 database engine. IDs should never be reused",
     )
 
 
 class ContributionEnum(Enum):
     authoredBy = "authoredBy"
@@ -54,49 +54,47 @@
     providedBy = "providedBy"
     retrievedBy = "retrievedBy"
     retrievedFrom = "retrievedFrom"
     sourceAccessedBy = "sourceAccessedBy"
 
 
 class Contributor(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
-    name: str = Field(..., description="Name of contributor", example=["Charles Darwin"])
+    name: str = Field(..., description="Name of contributor", examples=["Charles Darwin"])
     affiliation: Optional[str] = Field(
-        None, description="Organization the particular contributor is affiliated with", example=["HMS Beagle"]
+        None, description="Organization the particular contributor is affiliated with", examples=["HMS Beagle"]
     )
     email: Optional[EmailStr] = Field(
         None,
         description="electronic means for identification and communication purposes",
-        example=["name@example.edu"],
+        examples=["name@example.edu"],
     )
     contribution: List[ContributionEnum] = Field(
         ..., description="type of contribution determined according to PAV ontology"
     )
     orcid: Optional[AnyUrl] = Field(
         None,
         description="Field to record author information. ORCID identifiers allow for the author to curate their information after submission. ORCID identifiers must be valid and must have the prefix ‘https://orcid.org/’",
-        example=["http://orcid.org/0000-0002-1825-0097"],
+        examples=["http://orcid.org/0000-0002-1825-0097"],
     )
 
 
 class InputSubdomainItem(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     uri: Uri
 
 
 class OutputSubdomainItem(BaseModel):
     mediatype: str = Field(
         ...,
         description="https://www.iana.org/assignments/media-types/",
-        example=["text/csv"],
-        regex="^(.*)$",
+        examples=["text/csv"],
+        pattern="^(.*)$",
         title="mediatype",
     )
     uri: Uri
 
 
 class InputAndOutputDomain(BaseModel):
     input_subdomain: List[InputSubdomainItem] = Field(
```

### Comparing `galaxy-schema-23.2.1/galaxy/schema/bco/parametric_domain.py` & `galaxy-schema-24.0.0/galaxy/schema/bco/parametric_domain.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,40 +4,40 @@
 
 from __future__ import annotations
 
 from typing import List
 
 from pydantic import (
     BaseModel,
-    Extra,
+    ConfigDict,
     Field,
+    RootModel,
 )
 
 
 class ParametricDomainItem(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     param: str = Field(
-        ..., description="Specific variables for the computational workflow", example=["seed"], title="param"
+        ..., description="Specific variables for the computational workflow", examples=["seed"], title="param"
     )
     value: str = Field(
         ...,
         description="Specific (non-default) parameter values for the computational workflow",
-        example=["14"],
+        examples=["14"],
         title="value",
     )
     step: str = Field(
         ...,
         description="Refers to the specific step of the workflow relevant to the parameters specified in 'param' and 'value'",
-        example=["1"],
-        regex="^(.*)$",
+        examples=["1"],
+        pattern="^(.*)$",
         title="step",
     )
 
 
-class ParametricDomain(BaseModel):
-    __root__: List[ParametricDomainItem] = Field(
+class ParametricDomain(RootModel):
+    root: List[ParametricDomainItem] = Field(
         ...,
         description="This represents the list of NON-default parameters customizing the computational flow which can affect the output of the calculations. These fields can be custom to each kind of analysis and are tied to a particular pipeline implementation",
         title="Parametric Domain",
     )
```

### Comparing `galaxy-schema-23.2.1/galaxy/schema/bco/provenance_domain.py` & `galaxy-schema-24.0.0/galaxy/schema/bco/provenance_domain.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,31 +10,31 @@
     List,
     Optional,
 )
 
 from pydantic import (
     AnyUrl,
     BaseModel,
+    ConfigDict,
     EmailStr,
-    Extra,
     Field,
+    RootModel,
 )
 
 
 class Status(Enum):
     unreviewed = "unreviewed"
     in_review = "in-review"
     approved = "approved"
     rejected = "rejected"
     suspended = "suspended"
 
 
 class Embargo(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     start_time: Optional[datetime] = Field(None, description="Beginning date of embargo period.")
     end_time: Optional[datetime] = Field(None, description="End date of embargo period.")
 
 
 class ContributionEnum(Enum):
     authoredBy = "authoredBy"
@@ -49,84 +49,80 @@
     providedBy = "providedBy"
     retrievedBy = "retrievedBy"
     retrievedFrom = "retrievedFrom"
     sourceAccessedBy = "sourceAccessedBy"
 
 
 class Contributor(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
-    name: str = Field(..., description="Name of contributor", example=["Charles Darwin"])
+    name: str = Field(..., description="Name of contributor", examples=["Charles Darwin"])
     affiliation: Optional[str] = Field(
-        None, description="Organization the particular contributor is affiliated with", example=["HMS Beagle"]
+        None, description="Organization the particular contributor is affiliated with", examples=["HMS Beagle"]
     )
     email: Optional[EmailStr] = Field(
         None,
         description="electronic means for identification and communication purposes",
-        example=["name@example.edu"],
+        examples=["name@example.edu"],
     )
     contribution: List[ContributionEnum] = Field(
         ..., description="type of contribution determined according to PAV ontology"
     )
     orcid: Optional[AnyUrl] = Field(
         None,
         description="Field to record author information. ORCID identifiers allow for the author to curate their information after submission. ORCID identifiers must be valid and must have the prefix ‘https://orcid.org/’",
-        example=["http://orcid.org/0000-0002-1825-0097"],
+        examples=["http://orcid.org/0000-0002-1825-0097"],
     )
 
 
-class ObjectId(BaseModel):
-    __root__: str = Field(
+class ObjectId(RootModel):
+    root: str = Field(
         ...,
         description="A unique identifier that should be applied to each IEEE-2791 Object instance, generated and assigned by a IEEE-2791 database engine. IDs should never be reused",
     )
 
 
 class Uri(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     filename: Optional[str] = None
     uri: AnyUrl
     access_time: Optional[datetime] = Field(
         None, description="Time stamp of when the request for this data was submitted"
     )
     sha1_checksum: Optional[str] = Field(
-        None, description="output of hash function that produces a message digest", regex="[A-Za-z0-9]+"
+        None, description="output of hash function that produces a message digest", pattern="[A-Za-z0-9]+"
     )
 
 
 class ReviewItem(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     date: Optional[datetime] = None
     reviewer: Contributor = Field(..., description="Contributer that assigns IEEE-2791 review status.")
     reviewer_comment: Optional[str] = Field(
         None,
         description="Optional free text comment by reviewer",
-        example=["Approved by research institution staff. Waiting for approval from regulator"],
+        examples=["Approved by research institution staff. Waiting for approval from regulator"],
     )
     status: Status = Field(..., description="Current verification status of the IEEE-2791 Object")
 
 
 class ProvenanceDomain(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     name: str = Field(
         ...,
         description="Public searchable name for IEEE-2791 Object. This public field should take free text value using common biological research terminology supporting the terminology used in the usability_domain, external references (xref), and keywords sections.",
-        example=["HCV1a ledipasvir resistance SNP detection"],
+        examples=["HCV1a ledipasvir resistance SNP detection"],
     )
     version: str = Field(
         ...,
         description="Records the versioning of this IEEE-2791 Object instance. IEEE-2791 Object Version should adhere to semantic versioning as recommended by Semantic Versioning 2.0.0.",
-        example=["2.9"],
+        examples=["2.9"],
     )
     review: Optional[List[ReviewItem]] = Field(
         None,
         description="Description of the current verification status of an object in the review process. The unreviewed flag indicates that the object has been submitted, but no further evaluation or verification has occurred. The in-review flag indicates that verification is underway. The approved flag indicates that the IEEE-2791 Object has been verified and reviewed. The suspended flag indicates an object that was once valid is no longer considered valid. The rejected flag indicates that an error or inconsistency was detected in the IEEE-2791 Object, and it has been removed or rejected. The fields from the contributor object (described in section 2.1.10) is inherited to populate the reviewer section.",
     )
     derived_from: Optional[ObjectId] = Field(
         None,
@@ -145,9 +141,9 @@
     contributors: List[Contributor] = Field(
         ...,
         description="This is a list to hold contributor identifiers and a description of their type of contribution, including a field for ORCIDs to record author information, as they allow for the author to curate their information after submission. The contribution type is a choice taken from PAV ontology: provenance, authoring and versioning, which also maps to the PROV-O.",
     )
     license: str = Field(
         ...,
         description="Creative Commons license or other license information (text) space. The default or recommended license can be Attribution 4.0 International as shown in example",
-        example=["https://spdx.org/licenses/CC-BY-4.0.html"],
+        examples=["https://spdx.org/licenses/CC-BY-4.0.html"],
     )
```

### Comparing `galaxy-schema-23.2.1/galaxy/schema/bco/usability_domain.py` & `galaxy-schema-24.0.0/galaxy/schema/bco/usability_domain.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 #   timestamp: 2022-09-13T23:51:56+00:00
 
 from __future__ import annotations
 
 from typing import List
 
 from pydantic import (
-    BaseModel,
     Field,
+    RootModel,
 )
 
 
-class UsabilityDomain(BaseModel):
-    __root__: List[str] = Field(
+class UsabilityDomain(RootModel):
+    root: List[str] = Field(
         ...,
         description="Author-defined usability domain of the IEEE-2791 Object. This field is to aid in search-ability and provide a specific description of the function of the object.",
         title="Usability Domain",
     )
```

### Comparing `galaxy-schema-23.2.1/galaxy/schema/bco/util.py` & `galaxy-schema-24.0.0/galaxy/schema/bco/util.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Utilities for working with BCO models.
 
 We don't have a lot of functional code in this schema module so this may belong
 somewhere else in another galaxy-data package.
 """
+
 import hashlib
 from typing import (
     Any,
     Dict,
     List,
     Optional,
 )
@@ -60,18 +61,18 @@
         environment_variables=environment_variables or {},
     )
     return execution_domain
 
 
 def write_to_file(object_id: str, core_object: BioComputeObjectCore, output: StrOrBytesPath) -> None:
     # core_dict = core_object.dict()
-    etag = hashlib.sha256(core_object.json(indent=4, sort_keys=True).encode()).hexdigest()
-    object = BioComputeObject(object_id=object_id, etag=etag, **core_object.dict())
+    etag = hashlib.sha256(core_object.model_dump_json(indent=4).encode()).hexdigest()
+    object = BioComputeObject(object_id=object_id, etag=etag, **core_object.model_dump())
     with open(output, "w") as f:
-        f.write(object.json(indent=4, sort_keys=True, exclude_none=True))
+        f.write(object.model_dump_json(indent=4, exclude_none=True))
 
 
 def get_contributors(creator_metadata: Optional[List[Dict[str, Any]]]):
     contributors: List[Contributor] = []
     if creator_metadata:
         for creator in creator_metadata:
             name = None
```

### Comparing `galaxy-schema-23.2.1/galaxy/schema/cloud.py` & `galaxy-schema-24.0.0/galaxy/schema/cloud.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     List,
     Optional,
     Union,
 )
 
 from pydantic import (
     Field,
-    Required,
+    RootModel,
 )
 from typing_extensions import Literal
 
 from galaxy.schema.fields import DecodedDatabaseIdField
 from galaxy.schema.schema import (
     DatasetSummary,
     Model,
@@ -38,53 +38,53 @@
         title="Spaces to tabs",
         description="A boolean value ('true' or 'false') that sets if spaces should be converted to tab in the objects being fetched to Galaxy. Applicable only if `to_posix_lines` is True",
     )
 
 
 class CloudObjects(Model):
     history_id: DecodedDatabaseIdField = Field(
-        default=Required,
+        default=...,
         title="History ID",
         description="The ID of history to which the object should be received to.",
     )
     bucket: str = Field(
-        default=Required,
+        default=...,
         title="Bucket",
         description="The name of a bucket from which data should be fetched from (e.g., a bucket name on AWS S3).",
     )
     objects: List[str] = Field(
-        default=Required,
+        default=...,
         title="Objects",
         description="A list of the names of objects to be fetched.",
     )
     authz_id: DecodedDatabaseIdField = Field(
-        default=Required,
+        default=...,
         title="Authentication ID",
         description="The ID of CloudAuthz to be used for authorizing access to the resource provider. You may get a list of the defined authorizations via `/api/cloud/authz`. Also, you can use `/api/cloud/authz/create` to define a new authorization.",
     )
     input_args: Optional[InputArguments] = Field(
         default=None,
         title="Input arguments",
         description="A summary of the input arguments, which is optional and will default to {}.",
     )
 
 
 class CloudDatasets(Model):
     history_id: DecodedDatabaseIdField = Field(
-        default=Required,
+        default=...,
         title="History ID",
         description="The ID of history from which the object should be downloaded",
     )
     bucket: str = Field(
-        default=Required,
+        default=...,
         title="Bucket",
         description="The name of a bucket to which data should be sent (e.g., a bucket name on AWS S3).",
     )
     authz_id: DecodedDatabaseIdField = Field(
-        default=Required,
+        default=...,
         title="Authentication ID",
         description="The ID of CloudAuthz to be used for authorizing access to the resource provider. You may get a list of the defined authorizations via `/api/cloud/authz`. Also, you can use `/api/cloud/authz/create` to define a new authorization.",
     )
     dataset_ids: Optional[List[DecodedDatabaseIdField]] = Field(
         default=None,
         title="Objects",
         description="A list of dataset IDs belonging to the specified history that should be sent to the given bucket. If not provided, Galaxy sends all the datasets belonging the specified history.",
@@ -94,38 +94,38 @@
         title="Spaces to tabs",
         description="A boolean value. If set to 'True', and an object with same name of the dataset to be sent already exist in the bucket, Galaxy replaces the existing object with the dataset to be sent. If set to 'False', Galaxy appends datetime to the dataset name to prevent overwriting an existing object.",
     )
 
 
 class CloudDatasetsResponse(Model):
     sent_dataset_labels: List[str] = Field(
-        default=Required,
+        default=...,
         title="Send datasets",
         description="The datasets for which Galaxy succeeded to create (and queue) send job",
     )
     failed_dataset_labels: List[str] = Field(
-        default=Required,
+        default=...,
         title="Failed datasets",
         description="The datasets for which Galaxy failed to create (and queue) send job",
     )
     bucket_name: str = Field(
-        default=Required,
+        default=...,
         title="Bucket",
         description="The name of bucket to which the listed datasets are queued to be sent",
     )
 
 
 class StatusCode(Model):
     detail: str = Field(
-        default=Required,
+        default=...,
         title="Detail",
         description="The detail to expand on the status code",
     )
     status: int = Field(
-        default=Required,
+        default=...,
         title="Code",
         description="The actual status code",
     )
 
 
-class DatasetSummaryList(Model):
-    __root__: List[DatasetSummary]
+class DatasetSummaryList(RootModel):
+    root: List[DatasetSummary]
```

### Comparing `galaxy-schema-23.2.1/galaxy/schema/drs/DrsObject.py` & `galaxy-schema-24.0.0/galaxy/schema/workflows.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,137 +1,225 @@
-# generated by datamodel-codegen:
-#   filename:  https://raw.githubusercontent.com/ga4gh/data-repository-service-schemas/master/openapi/components/schemas/DrsObject.yaml
-#   timestamp: 2022-05-21T22:19:09+00:00
-
-from __future__ import annotations
-
-from datetime import datetime
-from enum import Enum
+import json
 from typing import (
+    Any,
+    Dict,
     List,
     Optional,
+    Union,
 )
 
 from pydantic import (
-    BaseModel,
     Field,
+    field_validator,
 )
 
-
-class Checksum(BaseModel):
-    checksum: str = Field(..., description="The hex-string encoded checksum for the data")
-    type: str = Field(
-        ...,
-        description="The digest method used to create the checksum.\nThe value (e.g. `sha-256`) SHOULD be listed as `Hash Name String` in the https://www.iana.org/assignments/named-information/named-information.xhtml#hash-alg[IANA Named Information Hash Algorithm Registry]. Other values MAY be used, as long as implementors are aware of the issues discussed in https://tools.ietf.org/html/rfc6920#section-9.4[RFC6920].\nGA4GH may provide more explicit guidance for use of non-IANA-registered algorithms in the future. Until then, if implementors do choose such an algorithm (e.g. because it's implemented by their storage provider), they SHOULD use an existing standard `type` value such as `md5`, `etag`, `crc32c`, `trunc512`, or `sha1`.",
-        example="sha-256",
-    )
-
-
-class Type(Enum):
-    s3 = "s3"
-    gs = "gs"
-    ftp = "ftp"
-    gsiftp = "gsiftp"
-    globus = "globus"
-    htsget = "htsget"
-    https = "https"
-    file = "file"
-
-
-class AccessURL(BaseModel):
-    url: str = Field(..., description="A fully resolvable URL that can be used to fetch the actual object bytes.")
-    headers: Optional[List[str]] = Field(
-        None,
-        description="An optional list of headers to include in the HTTP request to `url`. These headers can be used to provide auth tokens required to fetch the object bytes.",
-        example="Authorization: Basic Z2E0Z2g6ZHJz",
-    )
+from galaxy.schema.schema import (
+    AnnotationField,
+    InputDataCollectionStep,
+    InputDataStep,
+    InputParameterStep,
+    Model,
+    Organization,
+    PauseStep,
+    Person,
+    PreferredObjectStoreIdField,
+    StoredWorkflowSummary,
+    SubworkflowStep,
+    ToolStep,
+    WorkflowInput,
+)
 
 
-class ContentsObject(BaseModel):
-    name: str = Field(
-        ...,
-        description="A name declared by the bundle author that must be used when materialising this object, overriding any name directly associated with the object itself. The name must be unique with the containing bundle. This string is made up of uppercase and lowercase letters, decimal digits, hyphen, period, and underscore [A-Za-z0-9.-_]. See http://pubs.opengroup.org/onlinepubs/9699919799/basedefs/V1_chap03.html#tag_03_282[portable filenames].",
-    )
-    id: Optional[str] = Field(
+class GetTargetHistoryPayload(Model):
+    # TODO - Are the descriptions correct?
+    history: Optional[str] = Field(
         None,
-        description="A DRS identifier of a `DrsObject` (either a single blob or a nested bundle). If this ContentsObject is an object within a nested bundle, then the id is optional. Otherwise, the id is required.",
+        title="History",
+        # description="The encoded history id - passed exactly like this 'hist_id=...' -  to import the workflow into. Or the name of the new history to import the workflow into.",
+        description="The encoded history id - passed exactly like this 'hist_id=...' -  into which to import. Or the name of the new history into which to import.",
     )
-    drs_uri: Optional[List[str]] = Field(
+    history_id: Optional[str] = Field(
         None,
-        description="A list of full DRS identifier URI paths that may be used to obtain the object. These URIs may be external to this DRS instance.",
-        example="drs://drs.example.org/314159",
+        title="History ID",
+        # description="The history to import the workflow into.",
+        description="The encoded history id into which to import.",
     )
-    contents: Optional[List[ContentsObject]] = Field(
+    new_history_name: Optional[str] = Field(
         None,
-        description='If this ContentsObject describes a nested bundle and the caller specified "?expand=true" on the request, then this contents array must be present and describe the objects within the nested bundle.',
+        title="New History Name",
+        # description="The name of the new history to import the workflow into.",
+        description="The name of the new history into which to import.",
     )
 
 
-class AccessMethod(BaseModel):
-    type: Type = Field(..., description="Type of the access method.")
-    access_url: Optional[AccessURL] = Field(
-        None,
-        description="An `AccessURL` that can be used to fetch the actual object bytes. Note that at least one of `access_url` and `access_id` must be provided.",
+class InvokeWorkflowPayload(GetTargetHistoryPayload):
+    # TODO - Are the descriptions correct?
+    instance: Optional[bool] = Field(
+        False,
+        title="Is instance",
+        description="True when fetching by Workflow ID, False when fetching by StoredWorkflow ID",
     )
-    access_id: Optional[str] = Field(
+    scheduler: Optional[str] = Field(
         None,
-        description="An arbitrary string to be passed to the `/access` method to get an `AccessURL`. This string must be unique within the scope of a single object. Note that at least one of `access_url` and `access_id` must be provided.",
+        title="Scheduler",
+        description="Scheduler to use for workflow invocation.",
     )
-    region: Optional[str] = Field(
-        None,
-        description="Name of the region in the cloud service provider that the object belongs to.",
-        example="us-east-1",
+    batch: Optional[bool] = Field(
+        False,
+        title="Batch",
+        description="Indicates if the workflow is invoked as a batch.",
+    )
+    require_exact_tool_versions: Optional[bool] = Field(
+        True,
+        title="Require Exact Tool Versions",
+        description="If true, exact tool versions are required for workflow invocation.",
+        # description="TODO",
+    )
+    allow_tool_state_corrections: Optional[bool] = Field(
+        False,
+        title="Allow tool state corrections",
+        description="Indicates if tool state corrections are allowed for workflow invocation.",
+    )
+    use_cached_job: Optional[bool] = Field(
+        False,
+        title="Use cached job",
+        description="Indicated whether to use a cached job for workflow invocation.",
+    )
+    parameters_normalized: Optional[bool] = Field(
+        False,
+        title="Parameters Normalized",
+        description="Indicates if parameters are already normalized for workflow invocation.",
     )
 
+    @field_validator(
+        "parameters",
+        "inputs",
+        "ds_map",
+        "resource_params",
+        "replacement_params",
+        "step_parameters",
+        mode="before",
+        check_fields=False,
+    )
+    @classmethod
+    def inputs_string_to_json(cls, v):
+        if isinstance(v, str):
+            return json.loads(v)
+        return v
 
-class Model(BaseModel):
-    id: str = Field(..., description="An identifier unique to this `DrsObject`")
-    name: Optional[str] = Field(
+    parameters: Optional[Dict[str, Any]] = Field(
+        {},
+        title="Parameters",
+        description="The raw parameters for the workflow invocation.",
+    )
+    inputs: Optional[Dict[str, Any]] = Field(
         None,
-        description="A string that can be used to name a `DrsObject`.\nThis string is made up of uppercase and lowercase letters, decimal digits, hyphen, period, and underscore [A-Za-z0-9.-_]. See http://pubs.opengroup.org/onlinepubs/9699919799/basedefs/V1_chap03.html#tag_03_282[portable filenames].",
+        title="Inputs",
+        description="TODO",
     )
-    self_uri: str = Field(
-        ...,
-        description="A drs:// hostname-based URI, as defined in the DRS documentation, that tells clients how to access this object.\nThe intent of this field is to make DRS objects self-contained, and therefore easier for clients to store and pass around.  For example, if you arrive at this DRS JSON by resolving a compact identifier-based DRS URI, the `self_uri` presents you with a hostname and properly encoded DRS ID for use in subsequent `access` endpoint calls.",
-        example="drs://drs.example.org/314159",
+    ds_map: Optional[Dict[str, Dict[str, Any]]] = Field(
+        {},
+        title="Dataset Map",
+        description="TODO",
     )
-    size: int = Field(
-        ...,
-        description="For blobs, the blob size in bytes.\nFor bundles, the cumulative size, in bytes, of items in the `contents` field.",
+    resource_params: Optional[Dict[str, Any]] = Field(
+        {},
+        title="Resource Parameters",
+        description="TODO",
     )
-    created_time: datetime = Field(
-        ...,
-        description="Timestamp of content creation in RFC3339.\n(This is the creation time of the underlying content, not of the JSON object.)",
+    replacement_params: Optional[Dict[str, Any]] = Field(
+        {},
+        title="Replacement Parameters",
+        description="TODO",
     )
-    updated_time: Optional[datetime] = Field(
+    step_parameters: Optional[Dict[str, Any]] = Field(
         None,
-        description="Timestamp of content update in RFC3339, identical to `created_time` in systems that do not support updates. (This is the update time of the underlying content, not of the JSON object.)",
+        title="Step Parameters",
+        description="TODO",
     )
-    version: Optional[str] = Field(
-        None,
-        description="A string representing a version.\n(Some systems may use checksum, a RFC3339 timestamp, or an incrementing version number.)",
+    no_add_to_history: Optional[bool] = Field(
+        False,
+        title="No Add to History",
+        description="Indicates if the workflow invocation should not be added to the history.",
     )
-    mime_type: Optional[str] = Field(
-        None, description="A string providing the mime-type of the `DrsObject`.", example="application/json"
+    legacy: Optional[bool] = Field(
+        False,
+        title="Legacy",
+        description="Indicating if to use legacy workflow invocation.",
     )
-    checksums: List[Checksum] = Field(
-        ...,
-        description="The checksum of the `DrsObject`. At least one checksum must be provided.\nFor blobs, the checksum is computed over the bytes in the blob.\nFor bundles, the checksum is computed over a sorted concatenation of the checksums of its top-level contained objects (not recursive, names not included). The list of checksums is sorted alphabetically (hex-code) before concatenation and a further checksum is performed on the concatenated checksum value.\nFor example, if a bundle contains blobs with the following checksums:\nmd5(blob1) = 72794b6d\nmd5(blob2) = 5e089d29\nThen the checksum of the bundle is:\nmd5( concat( sort( md5(blob1), md5(blob2) ) ) )\n= md5( concat( sort( 72794b6d, 5e089d29 ) ) )\n= md5( concat( 5e089d29, 72794b6d ) )\n= md5( 5e089d2972794b6d )\n= f7a29a04",
-        min_items=1,
+    inputs_by: Optional[str] = Field(
+        None,
+        title="Inputs By",
+        # lib/galaxy/workflow/run_request.py - see line 60
+        description="How inputs maps to inputs (datasets/collections) to workflows steps.",
     )
-    access_methods: Optional[List[AccessMethod]] = Field(
+    effective_outputs: Optional[Any] = Field(
         None,
-        description="The list of access methods that can be used to fetch the `DrsObject`.\nRequired for single blobs; optional for bundles.",
-        min_items=1,
+        title="Effective Outputs",
+        # lib/galaxy/workflow/run_request.py - see line 455
+        description="TODO",
     )
-    contents: Optional[List[ContentsObject]] = Field(
+    preferred_intermediate_object_store_id: Optional[str] = Field(
         None,
-        description="If not set, this `DrsObject` is a single blob.\nIf set, this `DrsObject` is a bundle containing the listed `ContentsObject` s (some of which may be further nested).",
+        title="Preferred Intermediate Object Store ID",
+        description="The ID of the ? object store that should be used to store ? datasets in this history.",
     )
-    description: Optional[str] = Field(None, description="A human readable description of the `DrsObject`.")
-    aliases: Optional[List[str]] = Field(
+    preferred_outputs_object_store_id: Optional[str] = Field(
         None,
-        description="A list of strings that can be used to find other metadata about this `DrsObject` from external metadata sources. These aliases can be used to represent secondary accession numbers or external GUIDs.",
+        title="Preferred Outputs Object Store ID",
+        description="The ID of the object store that should be used to store ? datasets in this history.",
     )
+    preferred_object_store_id: Optional[str] = PreferredObjectStoreIdField
 
 
-ContentsObject.update_forward_refs()
+class StoredWorkflowDetailed(StoredWorkflowSummary):
+    annotation: Optional[str] = AnnotationField  # Inconsistency? See comment on StoredWorkflowSummary.annotations
+    license: Optional[str] = Field(
+        None, title="License", description="SPDX Identifier of the license associated with this workflow."
+    )
+    version: int = Field(
+        ..., title="Version", description="The version of the workflow represented by an incremental number."
+    )
+    inputs: Dict[int, WorkflowInput] = Field(
+        {}, title="Inputs", description="A dictionary containing information about all the inputs of the workflow."
+    )
+    creator: Optional[List[Union[Person, Organization]]] = Field(
+        None,
+        title="Creator",
+        description=("Additional information about the creator (or multiple creators) of this workflow."),
+    )
+    steps: Dict[
+        int,
+        Union[
+            InputDataStep,
+            InputDataCollectionStep,
+            InputParameterStep,
+            PauseStep,
+            ToolStep,
+            SubworkflowStep,
+        ],
+    ] = Field(
+        {},
+        title="Steps",
+        description="A dictionary with information about all the steps of the workflow.",
+        discriminator="type",
+    )
+    importable: Optional[bool] = Field(
+        ...,
+        title="Importable",
+        description="Indicates if the workflow is importable by the current user.",
+    )
+    email_hash: Optional[str] = Field(
+        ...,
+        title="Email Hash",
+        description="The hash of the email of the creator of this workflow",
+    )
+    slug: Optional[str] = Field(
+        ...,
+        title="Slug",
+        description="The slug of the workflow.",
+    )
+    source_metadata: Optional[Dict[str, Any]] = Field(
+        ...,
+        title="Source Metadata",
+        description="The source metadata of the workflow.",
+    )
```

### Comparing `galaxy-schema-23.2.1/galaxy/schema/fetch_data.py` & `galaxy-schema-24.0.0/galaxy/schema/fetch_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,34 +3,31 @@
 from typing import (
     List,
     Optional,
     Union,
 )
 
 from pydantic import (
-    Extra,
+    ConfigDict,
     Field,
+    field_validator,
     Json,
-    validator,
 )
 from typing_extensions import (
     Annotated,
     Literal,
 )
 
 from galaxy.schema.fields import DecodedDatabaseIdField
-from galaxy.schema.schema import (
-    HistoryIdField,
-    Model,
-)
+from galaxy.schema.schema import Model
+from galaxy.schema.types import CoercedStringType
 
 
 class FetchBaseModel(Model):
-    class Config:
-        allow_population_by_field_name = True
+    model_config = ConfigDict(populate_by_name=True)
 
 
 class ElementsFromType(str, Enum):
     archive = "archive"
     bagit = "bagit"
     bagit_archive = "bagit_archive"
     directory = "directory"
@@ -79,118 +76,113 @@
 class LibraryFolderDestination(FetchBaseModel):
     type: Literal["library_folder"]
     library_folder_id: DecodedDatabaseIdField  # For some reason this folder ID must NOT have the 'F' prefix
 
 
 class BaseCollectionTarget(BaseFetchDataTarget):
     destination: HdcaDestination
-    collection_type: Optional[str]
-    tags: Optional[List[str]]
-    name: Optional[str]
+    collection_type: Optional[str] = None
+    tags: Optional[List[str]] = None
+    name: Optional[str] = None
 
 
 class LibraryDestination(FetchBaseModel):
     type: Literal["library"]
     name: str = Field(..., description="Must specify a library name")
     description: Optional[str] = Field(None, description="Description for library to create")
     synopsis: Optional[str] = Field(None, description="Description for library to create")
 
 
 class ExtraFiles(FetchBaseModel):
-    items_from: Optional[str]
+    items_from: Optional[str] = None
     src: Src
     fuzzy_root: Optional[bool] = Field(
         True,
         description="Prevent Galaxy from checking for a single file in a directory and re-interpreting the archive",
     )
 
 
 class BaseDataElement(FetchBaseModel):
-    name: Optional[str]
+    name: Optional[CoercedStringType] = None
     dbkey: str = Field("?")
-    info: Optional[str]
+    info: Optional[str] = None
     ext: str = Field("auto")
     space_to_tab: bool = False
     to_posix_lines: bool = False
     deferred: bool = False
-    tags: Optional[List[str]]
-    created_from_basename: Optional[str]
-    extra_files: Optional[ExtraFiles]
+    tags: Optional[List[str]] = None
+    created_from_basename: Optional[str] = None
+    extra_files: Optional[ExtraFiles] = None
     auto_decompress: bool = AutoDecompressField
-    items_from: Optional[ElementsFromType] = Field(alias="elements_from")
-    collection_type: Optional[str]
-    MD5: Optional[str]
-    description: Optional[str]
-
-    class Config:
-        # reject unknown extra attributes
-        extra = Extra.forbid
+    items_from: Optional[ElementsFromType] = Field(None, alias="elements_from")
+    collection_type: Optional[str] = None
+    MD5: Optional[str] = None
+    description: Optional[str] = None
+    model_config = ConfigDict(extra="forbid")
 
 
 class FileDataElement(BaseDataElement):
     src: Literal["files"]
 
 
 class PastedDataElement(BaseDataElement):
     src: Literal["pasted"]
-    paste_content: str = Field(..., description="Content to upload")
+    paste_content: CoercedStringType = Field(..., description="Content to upload")
 
 
 class UrlDataElement(BaseDataElement):
     src: Literal["url"]
     url: str = Field(..., description="URL to upload")
 
 
 class ServerDirElement(BaseDataElement):
     src: Literal["server_dir"]
     server_dir: str
-    link_data_only: Optional[bool]
+    link_data_only: Optional[bool] = None
 
 
 class FtpImportElement(BaseDataElement):
     src: Literal["ftp_import"]
     ftp_path: str
-    items_from: Optional[ElementsFromType] = Field(alias="elements_from")
-    name: Optional[str]
-    collection_type: Optional[str]
+    collection_type: Optional[str] = None
 
 
 class ItemsFromModel(Model):
     src: ItemsFromSrc
-    path: Optional[str]
-    ftp_path: Optional[str]
-    server_dir: Optional[str]
-    url: Optional[str]
+    path: Optional[str] = None
+    ftp_path: Optional[str] = None
+    server_dir: Optional[str] = None
+    url: Optional[str] = None
 
 
 class FtpImportTarget(BaseCollectionTarget):
     src: Literal["ftp_import"]
     ftp_path: str
-    items_from: Optional[ElementsFromType] = Field(alias="elements_from")
+    items_from: Optional[ElementsFromType] = Field(None, alias="elements_from")
 
 
 class PathDataElement(BaseDataElement):
     src: Literal["path"]
     path: str
-    items_from: Optional[ElementsFromType] = Field(alias="elements_from")
-    link_data_only: Optional[bool]
+    items_from: Optional[ElementsFromType] = Field(None, alias="elements_from")
+    link_data_only: Optional[bool] = None
 
 
 class CompositeDataElement(BaseDataElement):
     src: Literal["composite"]
     composite: "CompositeItems"
 
 
 class CompositeItems(FetchBaseModel):
     items: List[
         Union[FileDataElement, PastedDataElement, UrlDataElement, PathDataElement, ServerDirElement, FtpImportElement]
     ] = Field(..., alias="elements")
 
 
-CompositeDataElement.update_forward_refs()
+CompositeDataElement.model_rebuild()
 
 
 class NestedElement(BaseDataElement):
     items: List[Union["AnyElement", "NestedElement"]] = Field(..., alias="elements")
 
 
 AnyElement = Annotated[
@@ -217,15 +209,15 @@
         ServerDirElement,
         FtpImportElement,
         CompositeDataElement,
     ],
     Field(default_factory=None, discriminator="src"),
 ]
 
-NestedElement.update_forward_refs()
+NestedElement.model_rebuild()
 
 
 class BaseDataTarget(BaseFetchDataTarget):
     destination: Union[HdaDestination, LibraryFolderDestination, LibraryDestination] = Field(..., discriminator="type")
 
 
 class DataElementsTarget(BaseDataTarget):
@@ -246,21 +238,19 @@
 
 class FilesPayload(Model):
     filename: str
     local_filename: str
 
 
 class BaseDataPayload(FetchBaseModel):
-    history_id: DecodedDatabaseIdField = HistoryIdField
-
-    class Config:
-        # file payloads are just tacked on, so we need to allow everything
-        extra = Extra.allow
+    history_id: DecodedDatabaseIdField
+    model_config = ConfigDict(extra="allow")
 
-    @validator("targets", pre=True, check_fields=False)
+    @field_validator("targets", mode="before", check_fields=False)
+    @classmethod
     def targets_string_to_json(cls, v):
         if isinstance(v, str):
             return json.loads(v)
         return v
 
 
 Targets = List[
```

### Comparing `galaxy-schema-23.2.1/galaxy/schema/groups.py` & `galaxy-schema-24.0.0/galaxy/schema/groups.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,65 +1,68 @@
 from typing import (
     List,
     Optional,
 )
 
 from pydantic import (
     Field,
-    Required,
+    RootModel,
 )
 from typing_extensions import Literal
 
 from galaxy.schema.fields import (
     DecodedDatabaseIdField,
     EncodedDatabaseIdField,
     ModelClassField,
 )
-from galaxy.schema.schema import Model
+from galaxy.schema.schema import (
+    Model,
+    WithModelClass,
+)
 
 GROUP_MODEL_CLASS = Literal["Group"]
 
 
-class GroupResponse(Model):
+class GroupResponse(Model, WithModelClass):
     """Response schema for a group."""
 
     model_class: GROUP_MODEL_CLASS = ModelClassField(GROUP_MODEL_CLASS)
     id: EncodedDatabaseIdField = Field(
-        Required,
+        ...,
         title="group ID",
     )
     name: str = Field(
-        Required,
+        ...,
         title="name of the group",
     )
     url: str = Field(
-        Required,
+        ...,
         title="URL for the group",
     )
     roles_url: Optional[str] = Field(
         None,
         title="URL for the roles of the group",
     )
     users_url: Optional[str] = Field(
         None,
         title="URL for the users of the group",
     )
 
 
-class GroupListResponse(Model):
+class GroupListResponse(RootModel):
     """Response schema for listing groups."""
 
-    __root__: List[GroupResponse]
+    root: List[GroupResponse]
 
 
 class GroupCreatePayload(Model):
     """Payload schema for creating a group."""
 
     name: str = Field(
-        Required,
+        ...,
         title="name of the group",
     )
     user_ids: List[DecodedDatabaseIdField] = Field(
         [],
         title="user IDs",
     )
     role_ids: List[DecodedDatabaseIdField] = Field(
```

### Comparing `galaxy-schema-23.2.1/galaxy/schema/help.py` & `galaxy-schema-24.0.0/galaxy/schema/help.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 from typing import (
     Any,
     List,
     Optional,
 )
 
 from pydantic import (
-    Extra,
+    ConfigDict,
     Field,
 )
 from typing_extensions import Annotated
 
 from galaxy.schema.schema import Model
 
 # Schema manually typed from https://docs.discourse.org/
 # Discourse has an OpenApi schema (https://docs.discourse.org/openapi.json)
 # but at the time of writing it is mostly untyped, which makes the manually
 # created types preferable.
 
 
 # TODO: remove this class once we have a proper model for all temp models
 class HelpTempBaseModel(Model):
-    class Config:
-        extra = Extra.allow
+    model_config = ConfigDict(extra="allow")
 
 
 class HelpForumPost(HelpTempBaseModel):
     """Model for a post in the help forum."""
 
     id: Annotated[int, Field(description="The ID of the post.")]
     name: Annotated[str, Field(description="The name of the post.")]
@@ -51,22 +50,24 @@
     created_at: Annotated[str, Field(description="The creation date of the topic.")]
     last_posted_at: Annotated[str, Field(description="The date of the last post in the topic.")]
     bumped: Annotated[bool, Field(description="Whether the topic was bumped.")]
     bumped_at: Annotated[str, Field(description="The date of the last bump of the topic.")]
     archetype: Annotated[Any, Field(description="The archetype of the topic.")]
     unseen: Annotated[bool, Field(description="Whether the topic is unseen.")]
     pinned: Annotated[bool, Field(description="Whether the topic is pinned.")]
-    unpinned: Annotated[Optional[bool], Field(description="Whether the topic is unpinned.")]
+    unpinned: Annotated[Optional[bool], Field(default=None, description="Whether the topic is unpinned.")]
     visible: Annotated[bool, Field(description="Whether the topic is visible.")]
     closed: Annotated[bool, Field(description="Whether the topic is closed.")]
     archived: Annotated[bool, Field(description="Whether the topic is archived.")]
-    bookmarked: Annotated[Optional[bool], Field(description="Whether the topic is bookmarked.")]
-    liked: Annotated[Optional[bool], Field(description="Whether the topic is liked.")]
+    bookmarked: Annotated[Optional[bool], Field(default=None, description="Whether the topic is bookmarked.")]
+    liked: Annotated[Optional[bool], Field(default=None, description="Whether the topic is liked.")]
     tags: Annotated[List[str], Field(description="The tags of the topic.")]
-    tags_descriptions: Annotated[Optional[Any], Field(description="The descriptions of the tags of the topic.")]
+    tags_descriptions: Annotated[
+        Optional[Any], Field(default=None, description="The descriptions of the tags of the topic.")
+    ]
     category_id: Annotated[int, Field(description="The ID of the category of the topic.")]
     has_accepted_answer: Annotated[bool, Field(description="Whether the topic has an accepted answer.")]
 
 
 class HelpForumUser(HelpTempBaseModel):
     """Model for a user in the help forum."""
 
@@ -99,14 +100,27 @@
 
 class HelpForumSearchResponse(Model):
     """Response model for the help search API endpoint.
 
     This model is based on the Discourse API response for the search endpoint.
     """
 
-    posts: Optional[List[HelpForumPost]]
-    topics: Optional[List[HelpForumTopic]]
-    users: Optional[List[HelpForumUser]]
-    categories: Optional[List[HelpForumCategory]]
-    tags: Optional[List[HelpForumTag]]
-    groups: Optional[List[HelpForumGroup]]
-    grouped_search_result: Optional[HelpForumGroupedSearchResult]
+    posts: Annotated[List[HelpForumPost], Field(default=None, description="The list of posts returned by the search.")]
+    topics: Annotated[
+        List[HelpForumTopic], Field(default=None, description="The list of topics returned by the search.")
+    ]
+    users: Annotated[
+        Optional[List[HelpForumUser]], Field(default=None, description="The list of users returned by the search.")
+    ]
+    categories: Annotated[
+        Optional[List[HelpForumCategory]],
+        Field(default=None, description="The list of categories returned by the search."),
+    ]
+    tags: Annotated[
+        Optional[List[HelpForumTag]], Field(default=None, description="The list of tags returned by the search.")
+    ]
+    groups: Annotated[
+        Optional[List[HelpForumGroup]], Field(default=None, description="The list of groups returned by the search.")
+    ]
+    grouped_search_result: Annotated[
+        Optional[HelpForumGroupedSearchResult], Field(default=None, description="The grouped search result.")
+    ]
```

### Comparing `galaxy-schema-23.2.1/galaxy/schema/item_tags.py` & `galaxy-schema-24.0.0/galaxy/schema/item_tags.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 from typing import (
     List,
     Optional,
 )
 
 from pydantic import (
     Field,
-    Required,
+    RootModel,
 )
 
 from galaxy.schema.fields import EncodedDatabaseIdField
 from galaxy.schema.schema import Model
 
 
 class ItemTagsResponse(Model):
     """Response schema for showing an item tag."""
 
     model_class: str = Field(
-        Required,
+        ...,
         title="model class",
     )
     id: EncodedDatabaseIdField = Field(
-        Required,
+        ...,
         title="item tag ID",
     )
     user_tname: str = Field(
-        Required,
+        ...,
         title="name of the item tag",
     )
     user_value: Optional[str] = Field(
         None,
         title="value of the item tag",
     )
 
 
-class ItemTagsListResponse(Model):
+class ItemTagsListResponse(RootModel):
     """Response schema for listing item tags."""
 
-    __root__: List[ItemTagsResponse]
+    root: List[ItemTagsResponse]
 
 
 class ItemTagsCreatePayload(Model):
     """Payload schema for creating an item tag."""
 
     value: Optional[str] = Field(
         None,
```

### Comparing `galaxy-schema-23.2.1/galaxy/schema/jobs.py` & `galaxy-schema-24.0.0/galaxy/schema/jobs.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,93 +1,94 @@
 import json
 from typing import (
     Any,
     Dict,
     List,
     Optional,
+    Union,
 )
 
 from pydantic import (
-    Extra,
+    ConfigDict,
     Field,
-    Required,
+    field_validator,
     UUID4,
-    validator,
 )
 from typing_extensions import Literal
 
 from galaxy.schema.fields import (
     DecodedDatabaseIdField,
     EncodedDatabaseIdField,
 )
 from galaxy.schema.schema import (
     DataItemSourceType,
     EncodedDataItemSourceId,
-    EntityIdField,
+    EncodedJobParameterHistoryItem,
+    JobMetricCollection,
     JobState,
     JobSummary,
     Model,
 )
 
 
 class JobInputSummary(Model):
     has_empty_inputs: bool = Field(
-        default=Required,
+        default=...,
         title="Empty inputs",
         description="Job has empty inputs.",
     )
     has_duplicate_inputs: bool = Field(
-        default=Required,
+        default=...,
         title="Duplicate inputs",
         description="Job has duplicate inputs.",
     )
 
 
 # TODO: Use Tuple again when `make update-client-api-schema` supports them
 class JobErrorSummary(Model):
     # messages: List[Union[Tuple[str, str], List[str]]]
     messages: List[List[str]] = Field(
-        default=Required,
+        default=...,
         title="Error messages",
         description="The error messages for the specified job.",
     )
 
 
 class JobAssociation(Model):
     name: str = Field(
-        default=Required,
+        default=...,
         title="name",
         description="Name of the job parameter.",
     )
     dataset: EncodedDataItemSourceId = Field(
-        default=Required,
+        default=...,
         title="dataset",
         description="Reference to the associated item.",
     )
 
 
 class JobInputAssociation(JobAssociation):
     name: str = Field(
-        default=Required,
+        default=...,
         title="name",
         description="Name of the job input parameter.",
     )
 
 
 class JobOutputAssociation(JobAssociation):
     name: str = Field(
-        default=Required,
+        default=...,
         title="name",
         description="Name of the job output parameter.",
     )
 
 
 class ReportJobErrorPayload(Model):
     dataset_id: DecodedDatabaseIdField = Field(
-        default=Required,
+        default=...,
         title="History Dataset Association ID",
         description="The History Dataset Association ID related to the error.",
     )
     email: Optional[str] = Field(
         default=None,
         title="Email",
         description="Email address for communication with the user. Only required for anonymous users.",
@@ -97,72 +98,72 @@
         title="Message",
         description="The optional message sent with the error report.",
     )
 
 
 class SearchJobsPayload(Model):
     tool_id: str = Field(
-        default=Required,
+        default=...,
         title="Tool ID",
         description="The tool ID related to the job.",
     )
     inputs: Dict[str, Any] = Field(
-        default=Required,
+        default=...,
         title="Inputs",
         description="The inputs of the job.",
     )
     state: Optional[JobState] = Field(
         default=None,
         title="State",
         description="Current state of the job.",
     )
+    model_config = ConfigDict(extra="allow")  # This is used for items named file_ and __file_
 
-    @validator("inputs", pre=True)
+    @field_validator("inputs", mode="before")
+    @classmethod
     def decode_json(cls, v):
         if isinstance(v, str):
             return json.loads(v)
         return v
 
-    class Config:
-        extra = Extra.allow  # This is used for items named file_ and __file_
-
 
 class DeleteJobPayload(Model):
     message: Optional[str] = Field(
         default=None,
         title="Job message",
         description="Stop message",
     )
 
 
 class SrcItem(Model):
     src: DataItemSourceType
 
 
 class EncodedHdcaSourceId(SrcItem):
-    id: EncodedDatabaseIdField = EntityIdField
+    id: EncodedDatabaseIdField
     src: Literal[DataItemSourceType.hdca] = Field(
-        default=Required,
+        default=...,
         title="Source",
         description="The source of this dataset, which in the case of the model can only be `hdca`.",
     )
 
 
 class EncodedDatasetJobInfo(EncodedDataItemSourceId):
     uuid: Optional[UUID4] = Field(
         default=None,
-        deprecated=True,
+        # TODO: also deprecate on python side, https://github.com/pydantic/pydantic/issues/2255
+        json_schema_extra={"deprecated": True},
         title="UUID",
         description="Universal unique identifier for this dataset.",
     )
 
 
 class EncodedJobDetails(JobSummary):
     command_version: Optional[str] = Field(
-        ...,
+        default=None,
         title="Command Version",
         description="Tool version indicated during job execution.",
     )
     params: Any = Field(
         ...,
         title="Parameters",
         description=(
@@ -177,60 +178,117 @@
     )
     outputs: Dict[str, EncodedDatasetJobInfo] = Field(
         {},
         title="Outputs",
         description="Dictionary mapping all the tool outputs (by name) to the corresponding data references.",
     )
     copied_from_job_id: Optional[EncodedDatabaseIdField] = Field(
-        default=None, title="Copied from Job-ID", description="Reference to cached job if job execution was cached."
+        default=None,
+        title="Copied from Job-ID",
+        description="Reference to cached job if job execution was cached.",
+    )
+    output_collections: Dict[str, EncodedHdcaSourceId] = Field(
+        default={},
+        title="Output collections",
+        description="",
     )
-    output_collections: Dict[str, EncodedHdcaSourceId] = Field(default={}, title="Output collections", description="")
 
 
 class JobDestinationParams(Model):
     runner: Optional[str] = Field(None, title="Runner", description="Job runner class", alias="Runner")
     runner_job_id: Optional[str] = Field(
         None,
         title="Runner Job ID",
         description="ID assigned to submitted job by external job running system",
         alias="Runner Job ID",
     )
     handler: Optional[str] = Field(
         None, title="Handler", description="Name of the process that handled the job.", alias="Handler"
     )
-
-    class Config:
-        extra = Extra.allow  # JobDestinationParams can have extra fields
+    model_config = ConfigDict(extra="allow")  # JobDestinationParams can have extra fields
 
 
 class JobOutput(Model):
-    label: Any = Field(default=Required, title="Output label", description="The output label")  # check if this is true
-    value: EncodedDataItemSourceId = Field(default=Required, title="Dataset", description="The associated dataset.")
+    label: Any = Field(default=..., title="Output label", description="The output label")  # check if this is true
+    value: EncodedDataItemSourceId = Field(default=..., title="Dataset", description="The associated dataset.")
 
 
 class JobParameter(Model):
     text: str = Field(
-        default=Required,
+        default=...,
         title="Text",
         description="Text associated with the job parameter.",
     )
     depth: int = Field(
-        default=Required,
+        default=...,
         title="Depth",
         description="The depth of the job parameter.",
     )
-    value: Optional[Any] = Field(default=None, title="Value", description="The values of the job parameter")
+    value: Optional[Union[List[EncodedJobParameterHistoryItem], float, int, bool, str]] = Field(
+        default=None, title="Value", description="The values of the job parameter", union_mode="left_to_right"
+    )
     notes: Optional[str] = Field(default=None, title="Notes", description="Notes associated with the job parameter.")
 
 
 class JobDisplayParametersSummary(Model):
     parameters: List[JobParameter] = Field(
-        default=Required, title="Parameters", description="The parameters of the job in a nested format."
+        default=..., title="Parameters", description="The parameters of the job in a nested format."
     )
     has_parameter_errors: bool = Field(
-        default=Required, title="Has parameter errors", description="The job has parameter errors"
+        default=..., title="Has parameter errors", description="The job has parameter errors"
     )
     outputs: Dict[str, List[JobOutput]] = Field(
-        default=Required,
+        default=...,
         title="Outputs",
         description="Dictionary mapping all the tool outputs (by name) with the corresponding dataset information in a nested format.",
     )
+
+
+class ShowFullJobResponse(EncodedJobDetails):
+    tool_stdout: Optional[str] = Field(
+        default=None,
+        title="Tool Standard Output",
+        description="The captured standard output of the tool executed by the job.",
+    )
+    tool_stderr: Optional[str] = Field(
+        default=None,
+        title="Tool Standard Error",
+        description="The captured standard error of the tool executed by the job.",
+    )
+    job_stdout: Optional[str] = Field(
+        default=None,
+        title="Job Standard Output",
+        description="The captured standard output of the job execution.",
+    )
+    job_stderr: Optional[str] = Field(
+        default=None,
+        title="Job Standard Error",
+        description="The captured standard error of the job execution.",
+    )
+    stdout: Optional[str] = Field(  # Redundant? it seems to be (tool_stdout + "\n" + job_stdout)
+        default=None,
+        title="Standard Output",
+        description="Combined tool and job standard output streams.",
+    )
+    stderr: Optional[str] = Field(  # Redundant? it seems to be (tool_stderr + "\n" + job_stderr)
+        default=None,
+        title="Standard Error",
+        description="Combined tool and job standard error streams.",
+    )
+    job_messages: Optional[List[Any]] = Field(
+        default=None,
+        title="Job Messages",
+        description="List with additional information and possible reasons for a failed job.",
+    )
+    dependencies: Optional[List[Any]] = Field(
+        default=None,
+        title="Job dependencies",
+        description="The dependencies of the job.",
+    )
+    job_metrics: Optional[JobMetricCollection] = Field(
+        default=None,
+        title="Job Metrics",
+        description=(
+            "Collections of metrics provided by `JobInstrumenter` plugins on a particular job. "
+            "Only administrators can see these metrics."
+        ),
+    )
```

### Comparing `galaxy-schema-23.2.1/galaxy/schema/notifications.py` & `galaxy-schema-24.0.0/galaxy/schema/notifications.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from datetime import datetime
 from enum import Enum
 from typing import (
+    Any,
     Dict,
     List,
     Optional,
     Union,
 )
 
 from pydantic import (
+    ConfigDict,
     Field,
-    Required,
+    RootModel,
 )
 from typing_extensions import (
     Annotated,
     Literal,
 )
 
 from galaxy.schema.fields import (
@@ -61,26 +63,24 @@
     # workflow_execution_completed = "workflow_execution_completed"
 
 
 NotificationCategory = Union[MandatoryNotificationCategory, PersonalNotificationCategory]
 
 
 class MessageNotificationContentBase(Model):
-    subject: str = Field(Required, title="Subject", description="The subject of the notification.")
-    message: str = Field(Required, title="Message", description="The message of the notification (supports Markdown).")
+    subject: str = Field(..., title="Subject", description="The subject of the notification.")
+    message: str = Field(..., title="Message", description="The message of the notification (supports Markdown).")
 
 
 class ActionLink(Model):
     """An action link to be displayed in the notification as a button."""
 
-    action_name: str = Field(
-        Required, title="Action name", description="The name of the action, will be the button title."
-    )
+    action_name: str = Field(..., title="Action name", description="The name of the action, will be the button title.")
     link: AbsoluteOrRelativeUrl = Field(
-        Required, title="Link", description="The link to be opened when the button is clicked."
+        ..., title="Link", description="The link to be opened when the button is clicked."
     )
 
 
 # Create the corresponding model for the registered category below and
 # add it to AnyNotificationContent Union.
 
 
@@ -103,72 +103,72 @@
     "visualization",
     "page",
 ]
 
 
 class NewSharedItemNotificationContent(Model):
     category: Literal[PersonalNotificationCategory.new_shared_item] = PersonalNotificationCategory.new_shared_item
-    item_type: SharableItemType = Field(Required, title="Item type", description="The type of the shared item.")
-    item_name: str = Field(Required, title="Item name", description="The name of the shared item.")
-    owner_name: str = Field(Required, title="Owner name", description="The name of the owner of the shared item.")
-    slug: str = Field(Required, title="Slug", description="The slug of the shared item. Used for the link to the item.")
+    item_type: SharableItemType = Field(..., title="Item type", description="The type of the shared item.")
+    item_name: str = Field(..., title="Item name", description="The name of the shared item.")
+    owner_name: str = Field(..., title="Owner name", description="The name of the owner of the shared item.")
+    slug: str = Field(..., title="Slug", description="The slug of the shared item. Used for the link to the item.")
 
 
 AnyNotificationContent = Annotated[
     Union[
         MessageNotificationContent,
         NewSharedItemNotificationContent,
         BroadcastNotificationContent,
     ],
     Field(
-        default=Required,
+        default=...,
         discriminator="category",
         title="Content",
         description="The content of the notification. The structure depends on the category.",
     ),
 ]
 
 NotificationIdField = Field(
-    Required,
+    ...,
     title="ID",
     description="The encoded ID of the notification.",
 )
 
 NotificationSourceField = Field(
-    Required,
+    ...,
     title="Source",
     description="The source of the notification. Represents the agent that created the notification. E.g. 'galaxy' or 'admin'.",
 )
 
 NotificationCategoryField = Field(
-    Required,
+    ...,
     title="Category",
     description="The category of the notification. Represents the type of the notification. E.g. 'message' or 'new_shared_item'.",
 )
 
 NotificationVariantField = Field(
-    Required,
+    ...,
     title="Variant",
     description="The variant of the notification. Represents the intent or relevance of the notification. E.g. 'info' or 'urgent'.",
 )
 
 NotificationCreateTimeField = Field(
-    Required,
+    ...,
     title="Create time",
     description="The time when the notification was created.",
 )
 
 NotificationUpdateTimeField = Field(
-    Required,
+    ...,
     title="Update time",
     description="The time when the notification was last updated.",
 )
 
 NotificationPublicationTimeField = Field(
-    Required,
+    ...,
     title="Publication time",
     description="The time when the notification was published. Notifications can be created and then published at a later time.",
 )
 
 NotificationExpirationTimeField = Field(
     None,
     title="Expiration time",
@@ -184,65 +184,63 @@
     category: NotificationCategory = NotificationCategoryField
     variant: NotificationVariant = NotificationVariantField
     create_time: datetime = NotificationCreateTimeField
     update_time: datetime = NotificationUpdateTimeField
     publication_time: datetime = NotificationPublicationTimeField
     expiration_time: Optional[datetime] = NotificationExpirationTimeField
     content: AnyNotificationContent
-
-    class Config:
-        orm_mode = True
+    model_config = ConfigDict(from_attributes=True)
 
 
 class UserNotificationResponse(NotificationResponse):
     """A notification response specific to the user."""
 
     category: PersonalNotificationCategory = NotificationCategoryField
     seen_time: Optional[datetime] = Field(
         None,
         title="Seen time",
         description="The time when the notification was seen by the user. If not set, the notification was not seen yet.",
     )
     deleted: bool = Field(
-        Required,
+        ...,
         title="Deleted",
         description="Whether the notification is marked as deleted by the user. Deleted notifications don't show up in the notification list.",
     )
 
 
 class BroadcastNotificationResponse(NotificationResponse):
     """A notification response specific for broadcasting."""
 
     category: Literal[MandatoryNotificationCategory.broadcast] = MandatoryNotificationCategory.broadcast
     content: BroadcastNotificationContent
 
 
-class UserNotificationListResponse(Model):
+class UserNotificationListResponse(RootModel):
     """A list of user notifications."""
 
-    __root__: List[UserNotificationResponse]
+    root: List[UserNotificationResponse]
 
 
-class BroadcastNotificationListResponse(Model):
+class BroadcastNotificationListResponse(RootModel):
     """A list of broadcast notifications."""
 
-    __root__: List[BroadcastNotificationResponse]
+    root: List[BroadcastNotificationResponse]
 
 
 class NotificationStatusSummary(Model):
     """A summary of the notification status for a user. Contains only updates since a particular timestamp."""
 
     total_unread_count: int = Field(
-        Required, title="Total unread count", description="The total number of unread notifications for the user."
+        ..., title="Total unread count", description="The total number of unread notifications for the user."
     )
     notifications: List[UserNotificationResponse] = Field(
-        Required, title="Notifications", description="The list of updated notifications for the user."
+        ..., title="Notifications", description="The list of updated notifications for the user."
     )
     broadcasts: List[BroadcastNotificationResponse] = Field(
-        Required, title="Broadcasts", description="The list of updated broadcasts."
+        ..., title="Broadcasts", description="The list of updated broadcasts."
     )
 
 
 class NotificationCreateData(Model):
     """Basic common fields for all notification create requests."""
 
     source: str = NotificationSourceField
@@ -281,44 +279,44 @@
     )
 
 
 class NotificationCreateRequest(Model):
     """Contains the recipients and the notification to create."""
 
     recipients: NotificationRecipients = Field(
-        Required,
+        ...,
         title="Recipients",
         description="The recipients of the notification. Can be a combination of users, groups and roles.",
     )
     notification: NotificationCreateData = Field(
-        Required,
+        ...,
         title="Notification",
         description="The notification to create. The structure depends on the category.",
     )
 
 
 class BroadcastNotificationCreateRequest(NotificationCreateData):
     """A notification create request specific for broadcasting."""
 
     category: Literal[MandatoryNotificationCategory.broadcast] = MandatoryNotificationCategory.broadcast
     content: BroadcastNotificationContent = Field(
-        Required,
+        ...,
         title="Content",
         description="The content of the broadcast notification. Broadcast notifications are displayed prominently to all users and can contain action links to redirect the user to a specific page.",
     )
 
 
 class NotificationCreatedResponse(Model):
     total_notifications_sent: int = Field(
-        Required,
+        ...,
         title="Total notifications sent",
         description="The total number of notifications that were sent to the recipients.",
     )
     notification: NotificationResponse = Field(
-        Required,
+        ...,
         title="Notification",
         description="The notification that was created. The structure depends on the category.",
     )
 
 
 class NotificationUpdateRequest(Model):
     def has_changes(self) -> bool:
@@ -369,35 +367,35 @@
         title="Content",
         description="The content of the broadcast notification. Broadcast notifications are displayed prominently to all users and can contain action links to redirect the user to a specific page.",
     )
 
 
 class NotificationsBatchRequest(Model):
     notification_ids: List[DecodedDatabaseIdField] = Field(
-        Required,
+        ...,
         title="Notification IDs",
         description="The list of encoded notification IDs of the notifications that should be updated.",
     )
 
 
 class UserNotificationsBatchUpdateRequest(NotificationsBatchRequest):
     """A batch update request specific for user notifications."""
 
     changes: UserNotificationUpdateRequest = Field(
-        Required,
+        ...,
         title="Changes",
         description="The changes that should be applied to the notifications. Only the fields that are set will be changed.",
     )
 
 
 class NotificationsBatchUpdateResponse(Model):
     """The response of a batch update request."""
 
     updated_count: int = Field(
-        Required,
+        ...,
         title="Updated count",
         description="The number of notifications that were updated.",
     )
 
 
 class NotificationChannelSettings(Model):
     """The settings for each channel of a notification category."""
@@ -429,19 +427,26 @@
 
 
 def get_default_personal_notification_preferences() -> PersonalNotificationPreferences:
     """Get the default personal notification preferences."""
     return {category: NotificationCategorySettings() for category in PersonalNotificationCategory.__members__.values()}
 
 
+def get_default_personal_notification_preferences_example() -> Dict[str, Any]:
+    return {
+        category: NotificationCategorySettings().model_dump()
+        for category in PersonalNotificationCategory.__members__.values()
+    }
+
+
 class UserNotificationPreferences(Model):
     """Contains the full notification preferences of a user."""
 
     preferences: PersonalNotificationPreferences = Field(
-        Required,
+        ...,
         title="Preferences",
         description="The notification preferences of the user.",
     )
 
     def update(
         self,
         other: Union["UserNotificationPreferences", PersonalNotificationPreferences],
@@ -457,30 +462,35 @@
         return self.preferences[category]
 
     @classmethod
     def default(cls):
         """Create a new instance with default preferences."""
         return cls(preferences=get_default_personal_notification_preferences())
 
-    class Config:
-        schema_extra = {
-            "example": {
-                "preferences": get_default_personal_notification_preferences(),
-            }
+    model_config = ConfigDict(
+        json_schema_extra={
+            "examples": [
+                {
+                    "preferences": get_default_personal_notification_preferences_example(),
+                }
+            ]
         }
+    )
 
 
 class UpdateUserNotificationPreferencesRequest(Model):
     """Contains the new notification preferences of a user."""
 
     preferences: PersonalNotificationPreferences = Field(
-        Required,
+        ...,
         title="Preferences",
         description="The new notification preferences of the user.",
     )
-
-    class Config:
-        schema_extra = {
-            "example": {
-                "preferences": get_default_personal_notification_preferences(),
-            }
+    model_config = ConfigDict(
+        json_schema_extra={
+            "examples": [
+                {
+                    "preferences": get_default_personal_notification_preferences_example(),
+                }
+            ]
         }
+    )
```

### Comparing `galaxy-schema-23.2.1/galaxy/schema/remote_files.py` & `galaxy-schema-24.0.0/galaxy/schema/remote_files.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,16 +3,17 @@
     Any,
     List,
     Optional,
     Union,
 )
 
 from pydantic import (
+    ConfigDict,
     Field,
-    Required,
+    RootModel,
 )
 from typing_extensions import (
     Annotated,
     Literal,
 )
 
 from galaxy.schema.schema import Model
@@ -33,47 +34,47 @@
 class RemoteFilesDisableMode(str, Enum):
     folders = "folders"
     files = "files"
 
 
 class FilesSourcePlugin(Model):
     id: str = Field(
-        Required,
+        ...,
         title="ID",
         description="The `FilesSource` plugin identifier",
-        example="_import",
+        examples=["_import"],
     )
     type: str = Field(
-        Required,
+        ...,
         title="Type",
         description="The type of the plugin.",
-        example="gximport",
+        examples=["gximport"],
     )
     label: str = Field(
-        Required,
+        ...,
         title="Label",
         description="The display label for this plugin.",
-        example="Library Import Directory",
+        examples=["Library Import Directory"],
     )
     doc: str = Field(
-        Required,
+        ...,
         title="Documentation",
         description="Documentation or extended description for this plugin.",
-        example="Galaxy's library import directory",
+        examples=["Galaxy's library import directory"],
     )
     browsable: bool = Field(
-        Required,
+        ...,
         title="Browsable",
         description="Whether this file source plugin can list items.",
     )
     writable: bool = Field(
-        Required,
+        ...,
         title="Writeable",
         description="Whether this files source plugin allows write access.",
-        example=False,
+        examples=[False],
     )
     requires_roles: Optional[str] = Field(
         None,
         title="Requires roles",
         description="Only users with the roles specified here can access this files source.",
     )
     requires_groups: Optional[str] = Field(
@@ -82,106 +83,108 @@
         description="Only users belonging to the groups specified here can access this files source.",
     )
 
 
 class BrowsableFilesSourcePlugin(FilesSourcePlugin):
     browsable: Literal[True]
     uri_root: str = Field(
-        Required,
+        ...,
         title="URI root",
         description="The URI root used by this type of plugin.",
-        example="gximport://",
+        examples=["gximport://"],
     )
+    model_config = ConfigDict(extra="allow")
 
 
-class FilesSourcePluginList(Model):
-    __root__: List[Union[BrowsableFilesSourcePlugin, FilesSourcePlugin]] = Field(
+class FilesSourcePluginList(RootModel):
+    root: List[Union[BrowsableFilesSourcePlugin, FilesSourcePlugin]] = Field(
         default=[],
         title="List of files source plugins",
-        example=[
+        examples=[
             {
                 "id": "_import",
                 "type": "gximport",
                 "uri_root": "gximport://",
                 "label": "Library Import Directory",
                 "doc": "Galaxy's library import directory",
                 "writable": False,
                 "browsable": True,
             }
         ],
     )
 
 
 class RemoteEntry(Model):
-    name: str = Field(Required, title="Name", description="The name of the entry.")
-    uri: str = Field(Required, title="URI", description="The URI of the entry.")
-    path: str = Field(Required, title="Path", description="The path of the entry.")
+    name: str = Field(..., title="Name", description="The name of the entry.")
+    uri: str = Field(..., title="URI", description="The URI of the entry.")
+    path: str = Field(..., title="Path", description="The path of the entry.")
 
 
 class RemoteDirectory(RemoteEntry):
-    class_: Literal["Directory"] = Field(Required, alias="class", const=True)
+    class_: Literal["Directory"] = Field(..., alias="class")
 
 
 class RemoteFile(RemoteEntry):
-    class_: Literal["File"] = Field(Required, alias="class", const=True)
-    size: int = Field(Required, title="Size", description="The size of the file in bytes.")
-    ctime: str = Field(Required, title="Creation time", description="The creation time of the file.")
+    class_: Literal["File"] = Field(..., alias="class")
+    size: int = Field(..., title="Size", description="The size of the file in bytes.")
+    ctime: str = Field(..., title="Creation time", description="The creation time of the file.")
 
 
-class ListJstreeResponse(Model):
-    __root__: List[Any] = Field(
+class ListJstreeResponse(RootModel):
+    root: List[Any] = Field(
         default=[],
         title="List of files",
         description="List of files in Jstree format.",
-        deprecated=True,
+        # TODO: also deprecate on python side, https://github.com/pydantic/pydantic/issues/2255
+        json_schema_extra={"deprecated": True},
     )
 
 
 AnyRemoteEntry = Annotated[
     Union[RemoteFile, RemoteDirectory],
     Field(discriminator="class_"),
 ]
 
 
-class ListUriResponse(Model):
-    __root__: List[AnyRemoteEntry] = Field(
+class ListUriResponse(RootModel):
+    root: List[AnyRemoteEntry] = Field(
         default=[],
         title="List of remote entries",
         description="List of directories and files.",
     )
 
 
 AnyRemoteFilesListResponse = Union[ListUriResponse, ListJstreeResponse]
 
 
 class CreateEntryPayload(Model):
     target: str = Field(
-        Required,
+        ...,
         title="Target",
         description="The target file source to create the entry in.",
     )
     name: str = Field(
-        Required,
+        ...,
         title="Name",
         description="The name of the entry to create.",
-        example="my_new_entry",
+        examples=["my_new_entry"],
     )
 
 
 class CreatedEntryResponse(Model):
     name: str = Field(
-        Required,
+        ...,
         title="Name",
         description="The name of the created entry.",
-        example="my_new_entry",
+        examples=["my_new_entry"],
     )
     uri: str = Field(
-        Required,
+        ...,
         title="URI",
         description="The URI of the created entry.",
-        example="gxfiles://my_new_entry",
+        examples=["gxfiles://my_new_entry"],
     )
     external_link: Optional[str] = Field(
         default=None,
         title="External link",
         description="An optional external link to the created entry if available.",
     )
```

### Comparing `galaxy-schema-23.2.1/galaxy/schema/schema.py` & `galaxy-schema-24.0.0/galaxy/schema/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """This module contains general pydantic models and common schema field annotations for them."""
 
-import re
 from datetime import (
     date,
     datetime,
 )
 from enum import Enum
 from typing import (
     Any,
@@ -17,32 +16,36 @@
 )
 from uuid import UUID
 
 from pydantic import (
     AnyHttpUrl,
     AnyUrl,
     BaseModel,
-    ConstrainedStr,
-    Extra,
+    BeforeValidator,
+    ConfigDict,
     Field,
     Json,
-    Required,
+    model_validator,
+    RootModel,
     UUID4,
 )
 from typing_extensions import (
     Annotated,
     Literal,
 )
 
+from galaxy.schema import partial_model
 from galaxy.schema.bco import XrefItem
 from galaxy.schema.fields import (
     DecodedDatabaseIdField,
     EncodedDatabaseIdField,
     EncodedLibraryFolderDatabaseIdField,
+    is_optional,
     LibraryFolderDatabaseIdField,
+    literal_to_value,
     ModelClassField,
 )
 from galaxy.schema.types import (
     OffsetNaiveDatetime,
     RelativeUrl,
 )
 
@@ -52,16 +55,20 @@
 DC_MODEL_CLASS = Literal["DatasetCollection"]
 DCE_MODEL_CLASS = Literal["DatasetCollectionElement"]
 HDCA_MODEL_CLASS = Literal["HistoryDatasetCollectionAssociation"]
 HISTORY_MODEL_CLASS = Literal["History"]
 JOB_MODEL_CLASS = Literal["Job"]
 STORED_WORKFLOW_MODEL_CLASS = Literal["StoredWorkflow"]
 PAGE_MODEL_CLASS = Literal["Page"]
+INVOCATION_MODEL_CLASS = Literal["WorkflowInvocation"]
+INVOCATION_STEP_MODEL_CLASS = Literal["WorkflowInvocationStep"]
+INVOCATION_REPORT_MODEL_CLASS = Literal["Report"]
+IMPLICIT_COLLECTION_JOBS_MODEL_CLASS = Literal["ImplicitCollectionJobs"]
 
-OptionalNumberT = Optional[Union[int, float]]
+OptionalNumberT = Annotated[Optional[Union[int, float]], Field(None)]
 
 
 class DatasetState(str, Enum):
     NEW = "new"
     UPLOAD = "upload"
     QUEUED = "queued"
     RUNNING = "running"
@@ -105,22 +112,35 @@
 
 class DatasetCollectionPopulatedState(str, Enum):
     NEW = "new"  # New dataset collection, unpopulated elements
     OK = "ok"  # Collection elements populated (HDAs may or may not have errors)
     FAILED = "failed"  # some problem populating state, won't be populated
 
 
+class HashFunctionNames(str, Enum):
+    """Hash function names that can be used to generate checksums for datasets."""
+
+    md5 = "MD5"
+    sha1 = "SHA-1"
+    sha256 = "SHA-256"
+    sha512 = "SHA-512"
+
+
 # Generic and common Field annotations that can be reused across models
 
-RelativeUrlField: RelativeUrl = Field(
-    ...,
-    title="URL",
-    description="The relative URL to access this item.",
-    deprecated=True,
-)
+RelativeUrlField = Annotated[
+    RelativeUrl,
+    Field(
+        ...,
+        title="URL",
+        description="The relative URL to access this item.",
+        # TODO: also deprecate on python side, https://github.com/pydantic/pydantic/issues/2255
+        json_schema_extra={"deprecated": True},
+    ),
+]
 
 DownloadUrlField: RelativeUrl = Field(
     ...,
     title="Download URL",
     description="The URL to download this item from the server.",
 )
 
@@ -132,26 +152,26 @@
 
 AccessibleField: bool = Field(
     ...,
     title="Accessible",
     description="Whether this item is accessible to the current user due to permissions.",
 )
 
+DatasetCollectionId = Annotated[EncodedDatabaseIdField, Field(..., title="Dataset Collection ID")]
+DatasetCollectionElementId = Annotated[EncodedDatabaseIdField, Field(..., title="Dataset Collection Element ID")]
+HistoryID = Annotated[EncodedDatabaseIdField, Field(..., title="History ID")]
+HistoryDatasetAssociationId = Annotated[EncodedDatabaseIdField, Field(..., title="History Dataset Association ID")]
+JobId = Annotated[EncodedDatabaseIdField, Field(..., title="Job ID")]
 
-EntityIdField = Field(
-    ...,
-    title="ID",
-    description="The encoded ID of this entity.",
-)
 
-DatasetStateField: DatasetState = Field(
-    ...,
-    title="State",
-    description="The current state of this dataset.",
-)
+DatasetStateField = Annotated[
+    DatasetState,
+    BeforeValidator(lambda v: "discarded" if v == "deleted" else v),
+    Field(..., title="State", description="The current state of this dataset."),
+]
 
 CreateTimeField = Field(
     title="Create Time",
     description="The time and date this item was created.",
 )
 
 UpdateTimeField = Field(
@@ -165,14 +185,23 @@
     title="Collection Type",
     description=(
         "The type of the collection, can be `list`, `paired`, or define subcollections using `:` "
         "as separator like `list:paired` or `list:list`."
     ),
 )
 
+OptionalCollectionTypeField = Field(
+    None,
+    title="Collection Type",
+    description=(
+        "The type of the collection, can be `list`, `paired`, or define subcollections using `:` "
+        "as separator like `list:paired` or `list:list`."
+    ),
+)
+
 PopulatedStateField: DatasetCollectionPopulatedState = Field(
     ...,
     title="Populated State",
     description=(
         "Indicates the general state of the elements in the dataset collection:"
         "- 'new': new dataset collection, unpopulated elements."
         "- 'ok': collection elements populated (HDAs may or may not have errors)."
@@ -182,141 +211,144 @@
 
 PopulatedStateMessageField: Optional[str] = Field(
     None,
     title="Populated State Message",
     description="Optional message with further information in case the population of the dataset collection failed.",
 )
 
-ElementCountField: Optional[int] = Field(
-    None,
-    title="Element Count",
-    description=(
-        "The number of elements contained in the dataset collection. "
-        "It may be None or undefined if the collection could not be populated."
+ElementCountField = Annotated[
+    Optional[int],
+    Field(
+        None,
+        title="Element Count",
+        description=(
+            "The number of elements contained in the dataset collection. "
+            "It may be None or undefined if the collection could not be populated."
+        ),
     ),
-)
+]
 
-PopulatedField: bool = Field(
-    title="Populated",
-    description="Whether the dataset collection elements (and any subcollections elements) were successfully populated.",
-)
+PopulatedField = Annotated[
+    bool,
+    Field(
+        None,
+        title="Populated",
+        description="Whether the dataset collection elements (and any subcollections elements) were successfully populated.",
+    ),
+]
 
 ElementsField = Field(
     [],
     title="Elements",
     description="The summary information of each of the elements inside the dataset collection.",
 )
 
-HistoryIdField: DecodedDatabaseIdField = Field(
-    ...,
-    title="History ID",
-    description="The encoded ID of the history associated with this item.",
-)
-
-UuidField: UUID4 = Field(
-    ...,
-    title="UUID",
-    description="Universal unique identifier for this dataset.",
-)
+UuidField = Annotated[
+    UUID4,
+    Field(
+        ...,
+        title="UUID",
+        description="Universal unique identifier for this dataset.",
+    ),
+]
 
 GenomeBuildField: Optional[str] = Field(
     "?",
     title="Genome Build",
     description="TODO",
 )
 
-ContentsUrlField = Field(
-    title="Contents URL",
-    description="The relative URL to access the contents of this History.",
-)
+ContentsUrlField = Annotated[
+    RelativeUrl,
+    Field(
+        ...,
+        title="Contents URL",
+        description="The relative URL to access the contents of this History.",
+    ),
+]
 
-UserIdField = Field(title="ID", description="Encoded ID of the user")
+UserId = Annotated[EncodedDatabaseIdField, Field(title="ID", description="Encoded ID of the user")]
 UserEmailField = Field(title="Email", description="Email of the user")
 UserDescriptionField = Field(title="Description", description="Description of the user")
-UserNameField = Field(default=Required, title="user_name", description="The name of the user.")
+UserNameField = Field(default=..., title="user_name", description="The name of the user.")
 QuotaPercentField = Field(
     default=None, title="Quota percent", description="Percentage of the storage quota applicable to the user."
 )
-UserDeletedField = Field(default=Required, title="Deleted", description=" User is deleted")
+UserDeletedField = Field(default=..., title="Deleted", description=" User is deleted")
 PreferredObjectStoreIdField = Field(
     default=None,
     title="Preferred Object Store ID",
     description="The ID of the object store that should be used to store new datasets in this history.",
 )
 
 TotalDiskUsageField = Field(
-    default=Required,
+    default=...,
     title="Total disk usage",
     description="Size of all non-purged, unique datasets of the user in bytes.",
 )
 NiceTotalDiskUsageField = Field(
-    default=Required,
+    default=...,
     title="Nice total disc usage",
     description="Size of all non-purged, unique datasets of the user in a nice format.",
 )
 FlexibleUserIdType = Union[DecodedDatabaseIdField, Literal["current"]]
 
 
 class Model(BaseModel):
-    class Config:
-        use_enum_values = True  # when using .dict()
-        allow_population_by_field_name = True
-        json_encoders = {
-            # This will ensure all IDs are encoded when serialized to JSON
-            DecodedDatabaseIdField: lambda v: DecodedDatabaseIdField.encode(v),
-            LibraryFolderDatabaseIdField: lambda v: LibraryFolderDatabaseIdField.encode(v),
-        }
+    """Base model definition with common configuration used by all derived models."""
+
+    model_config = ConfigDict(populate_by_name=True, use_enum_values=True, protected_namespaces=())
 
-        @staticmethod
-        def schema_extra(schema: Dict[str, Any], model) -> None:
-            # pydantic doesn't currently allow creating a constant that isn't optional,
-            # which makes sense for validation, but an openapi schema that describes
-            # a response should be able to declare that a field is always present,
-            # even if it is generated from a default value.
-            # Pass `mark_required_in_schema=True` when constructing a pydantic Field instance
-            # to indicate that the field is always present.
-            remove_prop_keys = set()  # hidden items shouldn't be added to schema
-            properties = schema.get("properties", {})
-            for prop_key, prop in properties.items():
-                required_in_schema = prop.pop("mark_required_in_schema", None)
-                hidden = prop.get("hidden")
-                if hidden:
-                    remove_prop_keys.add(prop_key)
-                if required_in_schema:
-                    # const is not valid in response?
-                    prop.pop("const", None)
-                    if "required" in schema:
-                        schema["required"].append(prop_key)
-                    else:
-                        schema["required"] = [prop_key]
-            for prop_key_to_remove in remove_prop_keys:
-                del properties[prop_key_to_remove]
+
+class RequireOneSetOption(Model):
+    # TODO: model in json schema
+    @model_validator(mode="after")
+    def check_some_ids_passed(self):
+        if not self.model_fields_set:
+            raise ValueError("Specify at least one ID to apply actions to")
+        return self
 
 
 class BaseUserModel(Model):
-    id: EncodedDatabaseIdField = UserIdField
+    id: UserId
     username: str = UserNameField
     email: str = UserEmailField
     deleted: bool = UserDeletedField
 
 
-class UserModel(BaseUserModel):
+class WithModelClass:
+    model_class: str
+
+    @model_validator(mode="before")
+    @classmethod
+    def set_default(cls, data):
+        if isinstance(data, dict):
+            if "model_class" not in data and issubclass(cls, BaseModel):
+                model_class_annotation = cls.model_fields["model_class"].annotation
+                if is_optional(model_class_annotation):
+                    return data
+                data = data.copy()
+                data["model_class"] = literal_to_value(model_class_annotation)
+        return data
+
+
+class UserModel(BaseUserModel, WithModelClass):
     """User in a transaction context."""
 
     active: bool = Field(title="Active", description="User is active")
     model_class: USER_MODEL_CLASS = ModelClassField(USER_MODEL_CLASS)
     last_password_change: Optional[datetime] = Field(title="Last password change", description="")
 
 
 class LimitedUserModel(Model):
     """This is used when config options (expose_user_name and expose_user_email) are in place."""
 
-    id: EncodedDatabaseIdField = UserIdField
-    username: Optional[str]
-    email: Optional[str]
+    id: UserId
+    username: Optional[str] = None
+    email: Optional[str] = None
 
 
 class DiskUsageUserModel(Model):
     total_disk_usage: float = TotalDiskUsageField
     nice_total_disk_usage: str = NiceTotalDiskUsageField
 
 
@@ -325,119 +357,115 @@
 
 
 class AnonUserModel(DiskUsageUserModel):
     quota_percent: Any = QuotaPercentField
 
 
 class DetailedUserModel(BaseUserModel, AnonUserModel):
-    is_admin: bool = Field(default=Required, title="Is admin", description="User is admin")
-    purged: bool = Field(default=Required, title="Purged", description="User is purged")
-    preferences: Dict[Any, Any] = Field(default=Required, title="Preferences", description="Preferences of the user")
+    is_admin: bool = Field(default=..., title="Is admin", description="User is admin")
+    purged: bool = Field(default=..., title="Purged", description="User is purged")
+    preferences: Dict[Any, Any] = Field(default=..., title="Preferences", description="Preferences of the user")
     preferred_object_store_id: Optional[str] = PreferredObjectStoreIdField
-    quota: str = Field(default=Required, title="Quota", description="Quota applicable to the user")
-    quota_bytes: Any = Field(
-        default=Required, title="Quota in bytes", description="Quota applicable to the user in bytes."
-    )
-    tags_used: List[str] = Field(default=Required, title="Tags used", description="Tags used by the user")
+    quota: str = Field(default=..., title="Quota", description="Quota applicable to the user")
+    quota_bytes: Any = Field(default=..., title="Quota in bytes", description="Quota applicable to the user in bytes.")
+    tags_used: List[str] = Field(default=..., title="Tags used", description="Tags used by the user")
 
 
 class UserCreationPayload(Model):
-    password: str = Field(default=Required, title="user_password", description="The password of the user.")
+    password: str = Field(default=..., title="user_password", description="The password of the user.")
     email: str = UserEmailField
     username: str = UserNameField
 
 
 class RemoteUserCreationPayload(Model):
     remote_user_email: str = UserEmailField
 
 
 class UserDeletionPayload(Model):
-    purge: bool = Field(default=Required, title="Purge user", description="Purge the user")
+    purge: bool = Field(default=..., title="Purge user", description="Purge the user")
 
 
 class FavoriteObject(Model):
     object_id: str = Field(
-        default=Required, title="Object ID", description="The id of an object the user wants to favorite."
+        default=..., title="Object ID", description="The id of an object the user wants to favorite."
     )
 
 
 class FavoriteObjectsSummary(Model):
-    tools: List[str] = Field(
-        default=Required, title="Favorite tools", description="The name of the tools the user favored."
-    )
+    tools: List[str] = Field(default=..., title="Favorite tools", description="The name of the tools the user favored.")
 
 
 class FavoriteObjectType(str, Enum):
     tools = "tools"
 
 
 class DeletedCustomBuild(Model):
     message: str = Field(
-        default=Required, title="Deletion message", description="Confirmation of the custom build deletion."
+        default=..., title="Deletion message", description="Confirmation of the custom build deletion."
     )
 
 
 class CustomBuildBaseModel(Model):
-    name: str = Field(default=Required, title="Name", description="The name of the custom build.")
+    name: str = Field(default=..., title="Name", description="The name of the custom build.")
 
 
 class CustomBuildLenType(str, Enum):
     file = "file"
     fasta = "fasta"
     text = "text"
 
 
 # TODO Evaluate if the titles and descriptions are fitting
 class CustomBuildCreationPayload(CustomBuildBaseModel):
     len_type: CustomBuildLenType = Field(
-        default=Required,
+        default=...,
         alias="len|type",
         title="Length type",
         description="The type of the len file.",
     )
     len_value: str = Field(
-        default=Required,
+        default=...,
         alias="len|value",
         title="Length value",
         description="The content of the length file.",
     )
 
 
 class CreatedCustomBuild(CustomBuildBaseModel):
-    len: EncodedDatabaseIdField = Field(default=Required, title="Length", description="The primary id of the len file.")
+    len: EncodedDatabaseIdField = Field(default=..., title="Length", description="The primary id of the len file.")
     count: Optional[str] = Field(default=None, title="Count", description="The number of chromosomes/contigs.")
     fasta: Optional[EncodedDatabaseIdField] = Field(
         default=None, title="Fasta", description="The primary id of the fasta file from a history."
     )
     linecount: Optional[EncodedDatabaseIdField] = Field(
         default=None, title="Line count", description="The primary id of a linecount dataset."
     )
 
 
 class CustomBuildModel(CreatedCustomBuild):
-    id: str = Field(default=Required, title="ID", description="The ID of the custom build.")
+    id: str = Field(default=..., title="ID", description="The ID of the custom build.")
 
 
-class CustomBuildsCollection(Model):
-    __root__: List[CustomBuildModel] = Field(
-        default=Required, title="Custom builds collection", description="The custom builds associated with the user."
+class CustomBuildsCollection(RootModel):
+    root: List[CustomBuildModel] = Field(
+        default=..., title="Custom builds collection", description="The custom builds associated with the user."
     )
 
 
-class GroupModel(Model):
+class GroupModel(Model, WithModelClass):
     """User group model"""
 
     model_class: GROUP_MODEL_CLASS = ModelClassField(GROUP_MODEL_CLASS)
     id: DecodedDatabaseIdField = Field(
-        ...,  # Required
+        ...,  # ...
         title="ID",
         description="Encoded group ID",
     )
     name: str = Field(
-        ...,  # Required
+        ...,  # ...
         title="Name",
         description="The name of the group.",
     )
 
 
 class JobSourceType(str, Enum):
     """Available types of job sources (model classes) that produce dataset collections."""
@@ -495,26 +523,25 @@
     library_folder = "library_folder"
     new_collection = "new_collection"
 
 
 DatasetCollectionInstanceType = Literal["history", "library"]
 
 
-class TagItem(ConstrainedStr):
-    regex = re.compile(r"^([^\s.:])+(.[^\s.:]+)*(:[^\s.:]+)?$")
+TagItem = Annotated[str, Field(..., pattern=r"^([^\s.:])+(.[^\s.:]+)*(:[^\s.:]+)?$")]
 
 
-class TagCollection(Model):
+class TagCollection(RootModel):
     """Represents the collection of tags associated with an item."""
 
-    __root__: List[TagItem] = Field(
+    root: List[TagItem] = Field(
         default=...,
         title="Tags",
         description="The collection of tags associated with an item.",
-        example=["COVID-19", "#myFancyTag", "covid19.galaxyproject.org"],
+        examples=["COVID-19", "#myFancyTag", "covid19.galaxyproject.org"],
     )
 
 
 class MetadataFile(Model):
     """Metadata file associated with a dataset."""
 
     file_type: str = Field(
@@ -540,21 +567,17 @@
     )
 
 
 class Hyperlink(Model):
     """Represents some text with an Hyperlink."""
 
     target: str = Field(
-        ..., title="Target", description="Specifies where to open the linked document.", example="_blank"
-    )
-    href: AnyUrl = Field(
-        ...,
-        title="HRef",
-        description="Specifies the linked document, resource, or location.",
+        ..., title="Target", description="Specifies where to open the linked document.", examples=["_blank"]
     )
+    href: Annotated[RelativeUrl, Field(..., title="Href", description="The URL of the linked document.")]
     text: str = Field(
         ...,
         title="Text",
         description="The text placeholder for the link.",
     )
 
 
@@ -570,27 +593,31 @@
         ...,
         title="Links",
         description="The collection of link details for this Display Application.",
     )
 
 
 class Visualization(Model):  # TODO annotate this model
-    class Config:
-        extra = Extra.allow  # Allow any fields temporarily until the model is annotated
+    # TODO[pydantic]: The following keys were removed: `json_encoders`.
+    # Check https://docs.pydantic.dev/dev-v2/migration/#changes-to-config for more information.
+    model_config = ConfigDict(
+        use_enum_values=True,
+        populate_by_name=True,
+    )
 
 
 class HistoryItemBase(Model):
     """Basic information provided by items contained in a History."""
 
-    id: DecodedDatabaseIdField = EntityIdField
+    id: EncodedDatabaseIdField
     name: Optional[str] = Field(
         title="Name",
         description="The name of the item.",
     )
-    history_id: DecodedDatabaseIdField = HistoryIdField
+    history_id: HistoryID
     hid: int = Field(
         ...,
         title="HID",
         description="The index position of this item in the History.",
     )
     deleted: bool = Field(
         ...,
@@ -603,95 +630,135 @@
         description="Whether this item is visible or hidden to the user by default.",
     )
 
 
 class HistoryItemCommon(HistoryItemBase):
     """Common information provided by items contained in a History."""
 
-    class Config:
-        extra = Extra.allow
-
     type_id: Optional[str] = Field(
         default=None,
         title="Type - ID",
         description="The type and the encoded ID of this item. Used for caching.",
-        example="dataset-616e371b2cc6c62e",
+        examples=["dataset-616e371b2cc6c62e"],
     )
     type: str = Field(
         ...,
         title="Type",
         description="The type of this item.",
     )
     create_time: Optional[datetime] = CreateTimeField
     update_time: Optional[datetime] = UpdateTimeField
-    url: RelativeUrl = RelativeUrlField
+    url: RelativeUrlField
     tags: TagCollection
 
 
 class HDACommon(HistoryItemCommon):
     history_content_type: Annotated[
         Literal["dataset"],
         Field(
             title="History Content Type",
             description="This is always `dataset` for datasets.",
         ),
     ]
+    copied_from_ldda_id: Optional[EncodedDatabaseIdField] = None
 
 
 class HDASummary(HDACommon):
     """History Dataset Association summary information."""
 
-    dataset_id: DecodedDatabaseIdField = Field(
+    dataset_id: EncodedDatabaseIdField = Field(
         ...,
         title="Dataset ID",
         description="The encoded ID of the dataset associated with this item.",
     )
-    state: DatasetState = DatasetStateField
-    extension: str = Field(
+    state: DatasetStateField
+    extension: Optional[str] = Field(
         ...,
         title="Extension",
         description="The extension of the dataset.",
-        example="txt",
+        examples=["txt"],
     )
     purged: bool = Field(
         ...,
         title="Purged",
         description="Whether this dataset has been removed from disk.",
     )
+    genome_build: Optional[str] = GenomeBuildField
 
 
 class HDAInaccessible(HDACommon):
     """History Dataset Association information when the user can not access it."""
 
     accessible: bool = AccessibleField
-    state: DatasetState = DatasetStateField
+    state: DatasetStateField
 
 
 HdaLddaField = Field(
     DatasetSourceType.hda,
-    const=True,
     title="HDA or LDDA",
     description="Whether this dataset belongs to a history (HDA) or a library (LDDA).",
-    deprecated=False,  # TODO Should this field be deprecated in favor of model_class?
 )
 
 
 class DatasetValidatedState(str, Enum):
     UNKNOWN = "unknown"
     INVALID = "invalid"
     OK = "ok"
 
 
-class HDADetailed(HDASummary):
+class DatasetHash(Model):
+    model_class: Literal["DatasetHash"] = ModelClassField(Literal["DatasetHash"])
+    id: EncodedDatabaseIdField = Field(
+        ...,
+        title="ID",
+        description="Encoded ID of the dataset hash.",
+    )
+    hash_function: HashFunctionNames = Field(
+        ...,
+        title="Hash Function",
+        description="The hash function used to generate the hash.",
+    )
+    hash_value: str = Field(
+        ...,
+        title="Hash Value",
+        description="The hash value.",
+    )
+    extra_files_path: Optional[str] = Field(
+        None,
+        title="Extra Files Path",
+        description="The path to the extra files used to generate the hash.",
+    )
+
+
+class DatasetSource(Model):
+    id: EncodedDatabaseIdField = Field(
+        ...,
+        title="ID",
+        description="Encoded ID of the dataset source.",
+    )
+    source_uri: Annotated[RelativeUrl, Field(..., title="Source URI", description="The URI of the dataset source.")]
+    extra_files_path: Annotated[
+        Optional[str], Field(None, title="Extra Files Path", description="The path to the extra files.")
+    ]
+    transform: Annotated[
+        Optional[List[Any]],  # TODO: type this
+        Field(
+            None,
+            title="Transform",
+            description="The transformations applied to the dataset source.",
+        ),
+    ]
+
+
+class HDADetailed(HDASummary, WithModelClass):
     """History Dataset Association detailed information."""
 
-    model_class: Annotated[HDA_MODEL_CLASS, ModelClassField()]
+    model_class: Annotated[HDA_MODEL_CLASS, ModelClassField(HDA_MODEL_CLASS)]
     hda_ldda: DatasetSourceType = HdaLddaField
     accessible: bool = AccessibleField
-    genome_build: Optional[str] = GenomeBuildField
     misc_info: Optional[str] = Field(
         default=None,
         title="Miscellaneous Information",
         description="TODO",
     )
     misc_blurb: Optional[str] = Field(
         default=None,
@@ -714,34 +781,24 @@
         description="Whether the job creating this dataset has been resubmitted.",
     )
     metadata: Optional[Any] = Field(  # TODO: create pydantic model for metadata?
         default=None,
         title="Metadata",
         description="The metadata associated with this dataset.",
     )
-    metadata_dbkey: Optional[str] = Field(
-        "?",
-        title="Metadata DBKey",
-        description="TODO",
-    )
-    metadata_data_lines: int = Field(
-        0,
-        title="Metadata Data Lines",
-        description="TODO",
-    )
     meta_files: List[MetadataFile] = Field(
         ...,
         title="Metadata Files",
         description="Collection of metadata files associated with this dataset.",
     )
     data_type: str = Field(
         ...,
         title="Data Type",
         description="The fully qualified name of the class implementing the data type of this dataset.",
-        example="galaxy.datatypes.data.Text",
+        examples=["galaxy.datatypes.data.Text"],
     )
     peek: Optional[str] = Field(
         default=None,
         title="Peek",
         description="A few lines of contents from the start of the file.",
     )
     creating_job: str = Field(
@@ -750,15 +807,15 @@
         description="The encoded ID of the job that created this dataset.",
     )
     rerunnable: bool = Field(
         ...,
         title="Rerunnable",
         description="Whether the job creating this dataset can be run again.",
     )
-    uuid: UUID4 = UuidField
+    uuid: UuidField
     permissions: DatasetPermissions = Field(
         ...,
         title="Permissions",
         description="Role-based access and manage control permissions for the dataset.",
     )
     file_name: Optional[str] = Field(
         default=None,
@@ -770,28 +827,24 @@
         title="Display Applications",
         description="Contains new-style display app urls.",
     )
     display_types: List[DisplayApp] = Field(
         ...,
         title="Legacy Display Applications",
         description="Contains old-style display app urls.",
-        deprecated=False,  # TODO: Should this field be deprecated in favor of display_apps?
-    )
-    visualizations: List[Visualization] = Field(
-        ...,
-        title="Visualizations",
-        description="The collection of visualizations that can be applied to this dataset.",
+        # https://github.com/pydantic/pydantic/issues/2255
+        # deprecated=False,  # TODO: Should this field be deprecated in favor of display_apps?
     )
     validated_state: DatasetValidatedState = Field(
         ...,
         title="Validated State",
         description="The state of the datatype validation for this dataset.",
     )
     validated_state_message: Optional[str] = Field(
-        ...,
+        None,
         title="Validated State Message",
         description="The message with details about the datatype validation result for this dataset.",
     )
     annotation: Optional[str] = AnnotationField
     download_url: RelativeUrl = DownloadUrlField
     type: Annotated[
         Literal["file"],
@@ -801,22 +854,48 @@
         ),
     ] = "file"
     api_type: Annotated[
         Literal["file"],
         Field(
             title="API Type",
             description="TODO",
-            deprecated=False,  # TODO: Should this field be deprecated as announced in release 16.04?
+            json_schema_extra={
+                "deprecated": True
+            },  # TODO: Should this field be deprecated as announced in release 16.04?
         ),
     ] = "file"
     created_from_basename: Optional[str] = Field(
         None,
         title="Created from basename",
         description="The basename of the output that produced this dataset.",  # TODO: is that correct?
     )
+    hashes: Annotated[
+        List[DatasetHash],
+        Field(
+            ...,
+            title="Hashes",
+            description="The list of hashes associated with this dataset.",
+        ),
+    ]
+    drs_id: Annotated[
+        str,
+        Field(
+            ...,
+            title="DRS ID",
+            description="The DRS ID of the dataset.",
+        ),
+    ]
+    sources: Annotated[
+        List[DatasetSource],
+        Field(
+            ...,
+            title="Sources",
+            description="The list of sources associated with this dataset.",
+        ),
+    ]
 
 
 class HDAExtended(HDADetailed):
     """History Dataset Association extended information."""
 
     tool_version: str = Field(
         ...,
@@ -831,57 +910,58 @@
     designation: Optional[str] = Field(
         None,
         title="Designation",
         description="TODO",
     )
 
 
-class DCSummary(Model):
+class DCSummary(Model, WithModelClass):
     """Dataset Collection summary information."""
 
     model_class: DC_MODEL_CLASS = ModelClassField(DC_MODEL_CLASS)
-    id: DecodedDatabaseIdField = EntityIdField
+    id: DatasetCollectionId
     create_time: datetime = CreateTimeField
     update_time: datetime = UpdateTimeField
     collection_type: CollectionType = CollectionTypeField
     populated_state: DatasetCollectionPopulatedState = PopulatedStateField
     populated_state_message: Optional[str] = PopulatedStateMessageField
-    element_count: Optional[int] = ElementCountField
+    element_count: ElementCountField
 
 
-class HDAObject(Model):
+class HDAObject(Model, WithModelClass):
     """History Dataset Association Object"""
 
-    id: DecodedDatabaseIdField = EntityIdField
+    # TODO: Does it need to be serialized differently from HDASummary ?
+    # If so at least merge models
+    id: HistoryDatasetAssociationId
     model_class: HDA_MODEL_CLASS = ModelClassField(HDA_MODEL_CLASS)
-    state: DatasetState = DatasetStateField
+    state: DatasetStateField
     hda_ldda: DatasetSourceType = HdaLddaField
-    history_id: DecodedDatabaseIdField = HistoryIdField
+    history_id: HistoryID
     tags: List[str]
-
-    class Config:
-        extra = Extra.allow  # Can contain more fields like metadata_*
+    copied_from_ldda_id: Optional[EncodedDatabaseIdField] = None
+    model_config = ConfigDict(extra="allow")
 
 
-class DCObject(Model):
+class DCObject(Model, WithModelClass):
     """Dataset Collection Object"""
 
-    id: DecodedDatabaseIdField = EntityIdField
+    id: DatasetCollectionId
     model_class: DC_MODEL_CLASS = ModelClassField(DC_MODEL_CLASS)
     collection_type: CollectionType = CollectionTypeField
-    populated: Optional[bool] = PopulatedField
-    element_count: Optional[int] = ElementCountField
-    contents_url: Optional[RelativeUrl] = ContentsUrlField
+    populated: PopulatedField
+    element_count: ElementCountField
+    contents_url: Optional[ContentsUrlField] = None
     elements: List["DCESummary"] = ElementsField
 
 
-class DCESummary(Model):
+class DCESummary(Model, WithModelClass):
     """Dataset Collection Element summary information."""
 
-    id: DecodedDatabaseIdField = EntityIdField
+    id: DatasetCollectionElementId
     model_class: DCE_MODEL_CLASS = ModelClassField(DCE_MODEL_CLASS)
     element_index: int = Field(
         ...,
         title="Element Index",
         description="The position index of this element inside the collection.",
     )
     element_identifier: str = Field(
@@ -897,21 +977,21 @@
     object: Union[HDAObject, HDADetailed, DCObject] = Field(
         ...,
         title="Object",
         description="The element's specific data depending on the value of `element_type`.",
     )
 
 
-DCObject.update_forward_refs()
+DCObject.model_rebuild()
 
 
 class DCDetailed(DCSummary):
     """Dataset Collection detailed information."""
 
-    populated: bool = PopulatedField
+    populated: PopulatedField
     elements: List[DCESummary] = ElementsField
 
 
 class HDCJobStateSummary(Model):
     """Overview of the job states working inside a dataset collection."""
 
     all_jobs: int = Field(
@@ -992,112 +1072,104 @@
         Field(
             title="History Content Type",
             description="This is always `dataset_collection` for dataset collections.",
         ),
     ]
 
 
-class HDCASummary(HDCACommon):
+class HDCASummary(HDCACommon, WithModelClass):
     """History Dataset Collection Association summary information."""
 
     model_class: HDCA_MODEL_CLASS = ModelClassField(HDCA_MODEL_CLASS)
     type: Annotated[
         Literal["collection"],
         Field(
             title="Type",
             description="This is always `collection` for dataset collections.",
         ),
     ] = "collection"
 
     collection_type: CollectionType = CollectionTypeField
     populated_state: DatasetCollectionPopulatedState = PopulatedStateField
     populated_state_message: Optional[str] = PopulatedStateMessageField
-    element_count: Optional[int] = ElementCountField
-    job_source_id: Optional[DecodedDatabaseIdField] = Field(
+    element_count: ElementCountField
+    job_source_id: Optional[EncodedDatabaseIdField] = Field(
         None,
         title="Job Source ID",
         description="The encoded ID of the Job that produced this dataset collection. Used to track the state of the job.",
     )
     job_source_type: Optional[JobSourceType] = Field(
         None,
         title="Job Source Type",
         description="The type of job (model class) that produced this dataset collection. Used to track the state of the job.",
     )
     job_state_summary: Optional[HDCJobStateSummary] = Field(
         None,
         title="Job State Summary",
         description="Overview of the job states working inside the dataset collection.",
     )
-    contents_url: RelativeUrl = ContentsUrlField
-    collection_id: DecodedDatabaseIdField = Field(
-        ...,
-        title="Collection ID",
-        description="The encoded ID of the dataset collection associated with this HDCA.",
-    )
+    contents_url: ContentsUrlField
+    collection_id: DatasetCollectionId
 
 
 class HDCADetailed(HDCASummary):
     """History Dataset Collection Association detailed information."""
 
-    populated: bool = PopulatedField
+    populated: PopulatedField
     elements: List[DCESummary] = ElementsField
     elements_datatypes: Set[str] = Field(
         ..., description="A set containing all the different element datatypes in the collection."
     )
-
-
-class HistoryBase(Model):
-    """Provides basic configuration for all the History models."""
-
-    class Config:
-        extra = Extra.allow  # Allow any other extra fields
+    implicit_collection_jobs_id: Optional[EncodedDatabaseIdField] = Field(
+        None,
+        description="Encoded ID for the ICJ object describing the collection of jobs corresponding to this collection",
+    )
 
 
 class HistoryContentItemBase(Model):
     """Identifies a dataset or collection contained in a History."""
 
     history_content_type: HistoryContentType = Field(
         ...,
         title="Content Type",
         description="The type of this item.",
     )
 
 
 class HistoryContentItem(HistoryContentItemBase):
-    id: DecodedDatabaseIdField = EntityIdField
+    id: DecodedDatabaseIdField
 
 
 class EncodedHistoryContentItem(HistoryContentItemBase):
-    id: EncodedDatabaseIdField = EntityIdField
+    id: EncodedDatabaseIdField
 
 
 class UpdateContentItem(HistoryContentItem):
     """Used for updating a particular history item. All fields are optional."""
 
-    class Config:
-        use_enum_values = True  # When using .dict()
-        extra = Extra.allow  # Allow any other extra fields
+    model_config = ConfigDict(use_enum_values=True, extra="allow")
 
 
-class UpdateHistoryContentsBatchPayload(HistoryBase):
+class UpdateHistoryContentsBatchPayload(Model):
     """Contains property values that will be updated for all the history `items` provided."""
 
     items: List[UpdateContentItem] = Field(
         ...,
         title="Items",
         description="A list of content items to update with the changes.",
     )
-
-    class Config:
-        schema_extra = {
+    model_config = ConfigDict(
+        extra="allow",
+        json_schema_extra={
             "example": {
                 "items": [{"history_content_type": "dataset", "id": "string"}],
                 "visible": False,
             }
-        }
+        },
+    )
 
 
 class HistoryContentItemOperation(str, Enum):
     hide = "hide"
     unhide = "unhide"
     delete = "delete"
     undelete = "undelete"
@@ -1132,29 +1204,29 @@
     ChangeDbkeyOperationParams,
     TagOperationParams,
 ]
 
 
 class HistoryContentBulkOperationPayload(Model):
     operation: HistoryContentItemOperation
-    items: Optional[List[HistoryContentItem]]
-    params: Optional[AnyBulkOperationParams]
+    items: Optional[List[HistoryContentItem]] = None
+    params: Optional[AnyBulkOperationParams] = None
 
 
 class BulkOperationItemError(Model):
     item: EncodedHistoryContentItem
     error: str
 
 
 class HistoryContentBulkOperationResult(Model):
     success_count: int
     errors: List[BulkOperationItemError]
 
 
-class UpdateHistoryContentsPayload(HistoryBase):
+class UpdateHistoryContentsPayload(Model):
     """Can contain arbitrary/dynamic fields that will be updated for a particular history item."""
 
     name: Optional[str] = Field(
         None,
         title="Name",
         description="The new name of the item.",
     )
@@ -1174,29 +1246,30 @@
         description="A user-defined annotation for this item.",
     )
     tags: Optional[TagCollection] = Field(
         None,
         title="Tags",
         description="A list of tags to add to this item.",
     )
-
-    class Config:
-        schema_extra = {
+    model_config = ConfigDict(
+        extra="allow",
+        json_schema_extra={
             "example": {
                 "visible": False,
                 "annotation": "Test",
             }
-        }
+        },
+    )
 
 
-class HistorySummary(HistoryBase):
+class HistorySummary(Model, WithModelClass):
     """History summary information."""
 
     model_class: HISTORY_MODEL_CLASS = ModelClassField(HISTORY_MODEL_CLASS)
-    id: DecodedDatabaseIdField = EntityIdField
+    id: HistoryID
     name: str = Field(
         ...,
         title="Name",
         description="The name of the history.",
     )
     deleted: bool = Field(
         ...,
@@ -1209,15 +1282,15 @@
         description="Whether this item has been permanently removed.",
     )
     archived: bool = Field(
         ...,
         title="Archived",
         description="Whether this item has been archived and is no longer active.",
     )
-    url: RelativeUrl = RelativeUrlField
+    url: RelativeUrlField
     published: bool = Field(
         ...,
         title="Published",
         description="Whether this resource is currently publicly available to all users.",
     )
     count: int = Field(
         ...,
@@ -1246,43 +1319,52 @@
     deleted: int = Field(
         ...,
         title="Deleted",
         description="Number of deleted datasets.",
     )
 
 
+# TODO: https://github.com/galaxyproject/galaxy/issues/17785
 HistoryStateCounts = Dict[DatasetState, int]
 HistoryStateIds = Dict[DatasetState, List[DecodedDatabaseIdField]]
 
+HistoryContentStates = Union[DatasetState, DatasetCollectionPopulatedState]
+HistoryContentStateCounts = Dict[HistoryContentStates, int]
+
 
 class HistoryDetailed(HistorySummary):  # Equivalent to 'dev-detailed' view, which seems the default
     """History detailed information."""
 
-    contents_url: RelativeUrl = ContentsUrlField
+    contents_url: ContentsUrlField
     size: int = Field(
         ...,
         title="Size",
         description="The total size of the contents of this history in bytes.",
     )
-    user_id: DecodedDatabaseIdField = Field(
-        ...,
+    user_id: Optional[EncodedDatabaseIdField] = Field(
+        None,
         title="User ID",
         description="The encoded ID of the user that owns this History.",
     )
     create_time: datetime = CreateTimeField
     importable: bool = Field(
         ...,
         title="Importable",
         description="Whether this History can be imported by other users with a shared link.",
     )
     slug: Optional[str] = Field(
         None,
         title="Slug",
         description="Part of the URL to uniquely identify this History by link in a readable way.",
     )
+    username: Optional[str] = Field(
+        None,
+        title="Username",
+        description="Owner of the history",
+    )
     username_and_slug: Optional[str] = Field(
         None,
         title="Username and slug",
         description="The relative URL in the form of /u/{username}/h/{slug}",
     )
     genome_build: Optional[str] = GenomeBuildField
     state: DatasetState = Field(
@@ -1304,20 +1386,48 @@
         description=(
             "A dictionary keyed to possible dataset states and valued with the number "
             "of datasets in this history that have those states."
         ),
     )
 
 
-AnyHistoryView = Union[
-    HistorySummary,
-    HistoryDetailed,
-    # Any will cover those cases in which only specific `keys` are requested
-    # otherwise the validation will fail because the required fields are not returned
-    Any,
+@partial_model()
+class CustomHistoryView(HistoryDetailed):
+    """History Response with all optional fields.
+
+    It is used for serializing only specific attributes using the "keys"
+    query parameter. Unfortunately, we cannot know the exact fields that
+    will be requested, so we have to allow all fields to be optional.
+    """
+
+    # Define a few more useful fields to be optional that are not part of HistoryDetailed
+    contents_active: Optional[HistoryActiveContentCounts] = Field(
+        default=None,
+        title="Contents Active",
+        description=("Contains the number of active, deleted or hidden items in a History."),
+    )
+    contents_states: Optional[HistoryContentStateCounts] = Field(
+        default=None,
+        title="Contents States",
+        description="A dictionary keyed to possible dataset states and valued with the number of datasets in this history that have those states.",
+    )
+    nice_size: Optional[str] = Field(
+        default=None,
+        title="Nice Size",
+        description="The total size of the contents of this history in a human-readable format.",
+    )
+
+
+AnyHistoryView = Annotated[
+    Union[
+        CustomHistoryView,
+        HistoryDetailed,
+        HistorySummary,
+    ],
+    Field(union_mode="left_to_right"),
 ]
 
 
 class ExportHistoryArchivePayload(Model):
     gzip: Optional[bool] = Field(
         default=True,
         title="GZip",
@@ -1346,15 +1456,14 @@
             "using the `galaxy.files` URI infrastructure."
         ),
     )
     force: Optional[bool] = Field(  # Hack to force rebuild everytime during dev
         default=None,
         title="Force Rebuild",
         description="Whether to force a rebuild of the history archive.",
-        hidden=True,  # Avoids displaying this field in the documentation
     )
 
 
 WorkflowSortByEnum = Literal["create_time", "update_time", "name"]
 
 
 class WorkflowIndexQueryPayload(Model):
@@ -1387,64 +1496,63 @@
     tool_ids: Optional[List[str]] = None
     tool_ids_like: Optional[List[str]] = None
     date_range_min: Optional[Union[OffsetNaiveDatetime, date]] = None
     date_range_max: Optional[Union[OffsetNaiveDatetime, date]] = None
     history_id: Optional[DecodedDatabaseIdField] = None
     workflow_id: Optional[DecodedDatabaseIdField] = None
     invocation_id: Optional[DecodedDatabaseIdField] = None
+    implicit_collection_jobs_id: Optional[DecodedDatabaseIdField] = None
     order_by: JobIndexSortByEnum = JobIndexSortByEnum.update_time
     search: Optional[str] = None
     limit: int = 500
     offset: int = 0
 
 
 class InvocationSortByEnum(str, Enum):
     create_time = "create_time"
     update_time = "update_time"
     none = None
 
 
 class InvocationIndexQueryPayload(Model):
-    workflow_id: Optional[DecodedDatabaseIdField] = Field(
-        title="Workflow ID", description="Return only invocations for this Workflow ID"
+    workflow_id: Optional[int] = Field(
+        None, title="Workflow ID", description="Return only invocations for this Workflow ID"
     )
-    history_id: Optional[DecodedDatabaseIdField] = Field(
-        title="History ID", description="Return only invocations for this History ID"
-    )
-    job_id: Optional[DecodedDatabaseIdField] = Field(
-        title="Job ID", description="Return only invocations for this Job ID"
-    )
-    user_id: Optional[DecodedDatabaseIdField] = Field(
-        title="User ID", description="Return invocations for this User ID"
+    history_id: Optional[int] = Field(
+        None, title="History ID", description="Return only invocations for this History ID"
     )
+    job_id: Optional[int] = Field(None, title="Job ID", description="Return only invocations for this Job ID")
+    user_id: Optional[int] = Field(None, title="User ID", description="Return invocations for this User ID")
     sort_by: Optional[InvocationSortByEnum] = Field(
-        title="Sort By", description="Sort Workflow Invocations by this attribute"
+        None, title="Sort By", description="Sort Workflow Invocations by this attribute"
     )
     sort_desc: bool = Field(default=False, description="Sort in descending order?")
     include_terminal: bool = Field(default=True, description="Set to false to only include terminal Invocations.")
     limit: Optional[int] = Field(
         default=100,
         lt=1000,
     )
     offset: Optional[int] = Field(default=0, description="Number of invocations to skip")
+    include_nested_invocations: bool = True
 
 
-PageSortByEnum = Literal["update_time", "title", "username"]
+PageSortByEnum = Literal["create_time", "title", "update_time", "username"]
 
 
 class PageIndexQueryPayload(Model):
     deleted: bool = False
+    limit: Optional[int] = Field(default=100, lt=1000, title="Limit", description="Maximum number of pages to return.")
+    offset: Optional[int] = Field(default=0, title="Offset", description="Number of pages to skip.")
+    show_own: Optional[bool] = None
     show_published: Optional[bool] = None
     show_shared: Optional[bool] = None
-    user_id: Optional[DecodedDatabaseIdField] = None
+    search: Optional[str] = Field(default=None, title="Filter text", description="Freetext to search.")
     sort_by: PageSortByEnum = Field("update_time", title="Sort By", description="Sort pages by this attribute.")
     sort_desc: Optional[bool] = Field(default=False, title="Sort descending", description="Sort in descending order.")
-    search: Optional[str] = Field(default=None, title="Filter text", description="Freetext to search.")
-    limit: Optional[int] = Field(default=100, lt=1000, title="Limit", description="Maximum number of pages to return.")
-    offset: Optional[int] = Field(default=0, title="Offset", description="Number of pages to skip.")
+    user_id: Optional[DecodedDatabaseIdField] = None
 
 
 class CreateHistoryPayload(Model):
     name: Optional[str] = Field(
         default=None,
         title="Name",
         description="The new history name.",
@@ -1492,34 +1600,29 @@
         description="The source of the element.",
     )
     id: Optional[DecodedDatabaseIdField] = Field(
         default=None,
         title="ID",
         description="The encoded ID of the element.",
     )
-    collection_type: Optional[CollectionType] = CollectionTypeField
+    collection_type: Optional[CollectionType] = OptionalCollectionTypeField
     element_identifiers: Optional[List["CollectionElementIdentifier"]] = Field(
         default=None,
         title="Element Identifiers",
         description="List of elements that should be in the new sub-collection.",
     )
     tags: Optional[List[str]] = Field(
         default=None,
         title="Tags",
         description="The list of tags associated with the element.",
     )
 
 
-# Required for self-referencing models
-# See https://pydantic-docs.helpmanual.io/usage/postponed_annotations/#self-referencing-models
-CollectionElementIdentifier.update_forward_refs()
-
-
 class CreateNewCollectionPayload(Model):
-    collection_type: Optional[CollectionType] = CollectionTypeField
+    collection_type: Optional[CollectionType] = OptionalCollectionTypeField
     element_identifiers: Optional[List[CollectionElementIdentifier]] = Field(
         default=None,
         title="Element Identifiers",
         description="List of elements that should be in the new collection.",
     )
     name: Optional[str] = Field(
         default=None,
@@ -1569,16 +1672,16 @@
 
     @classmethod
     def is_bag(cls, value: "ModelStoreFormat"):
         return value in [cls.BAG_DOT_TAR, cls.BAG_DOT_TGZ, cls.BAG_DOT_ZIP]
 
 
 class StoreContentSource(Model):
-    store_content_uri: Optional[str]
-    store_dict: Optional[Dict[str, Any]]
+    store_content_uri: Optional[str] = None
+    store_dict: Optional[Dict[str, Any]] = None
     model_store_format: Optional["ModelStoreFormat"] = None
 
 
 class CreateHistoryFromStore(StoreContentSource):
     pass
 
 
@@ -1601,15 +1704,15 @@
         title="Include hidden",
         description="Include file contents for hidden datasets (if include_files is True).",
     )
 
 
 class ShortTermStoreExportPayload(StoreExportPayload):
     short_term_storage_request_id: UUID
-    duration: OptionalNumberT
+    duration: OptionalNumberT = None
 
 
 class BcoGenerationParametersMixin(BaseModel):
     bco_merge_history_metadata: bool = Field(
         default=False, description="When reading tags/annotations to generate BCO object include history metadata."
     )
     bco_override_environment_variables: Optional[Dict[str, str]] = Field(
@@ -1690,26 +1793,26 @@
     HISTORY = "history"
     INVOCATION = "invocation"
 
 
 class ExportObjectRequestMetadata(Model):
     object_id: EncodedDatabaseIdField
     object_type: ExportObjectType
-    user_id: Optional[EncodedDatabaseIdField]
+    user_id: Optional[EncodedDatabaseIdField] = None
     payload: Union[WriteStoreToPayload, ShortTermStoreExportPayload]
 
 
 class ExportObjectResultMetadata(Model):
     success: bool
-    error: Optional[str]
+    error: Optional[str] = None
 
 
 class ExportObjectMetadata(Model):
     request_data: ExportObjectRequestMetadata
-    result_data: Optional[ExportObjectResultMetadata]
+    result_data: Optional[ExportObjectResultMetadata] = None
 
     def is_short_term(self):
         """Whether the export is a short term export."""
         return isinstance(self.request_data.payload, ShortTermStoreExportPayload)
 
     def is_ready(self):
         """Whether the export has finished and it's ready to be used."""
@@ -1719,23 +1822,23 @@
 class ObjectExportTaskResponse(ObjectExportResponseBase):
     task_uuid: UUID4 = Field(
         ...,
         title="Task ID",
         description="The identifier of the task processing the export.",
     )
     create_time: datetime = CreateTimeField
-    export_metadata: Optional[ExportObjectMetadata]
+    export_metadata: Optional[ExportObjectMetadata] = None
 
 
-class JobExportHistoryArchiveListResponse(Model):
-    __root__: List[JobExportHistoryArchiveModel]
+class JobExportHistoryArchiveListResponse(RootModel):
+    root: List[JobExportHistoryArchiveModel]
 
 
-class ExportTaskListResponse(Model):
-    __root__: List[ObjectExportTaskResponse]
+class ExportTaskListResponse(RootModel):
+    root: List[ObjectExportTaskResponse]
     __accept_type__ = "application/vnd.galaxy.task.export+json"
 
 
 class ArchiveHistoryRequestPayload(Model):
     archive_export_id: Optional[DecodedDatabaseIdField] = Field(
         default=None,
         title="Export Record ID",
@@ -1815,23 +1918,19 @@
         ),
     )
 
 
 class JobIdResponse(Model):
     """Contains the ID of the job associated with a particular request."""
 
-    job_id: EncodedDatabaseIdField = Field(
-        ...,
-        title="Job ID",
-        description="The encoded database ID of the job that is currently processing a particular request.",
-    )
+    job_id: JobId
 
 
-class JobBaseModel(Model):
-    id: EncodedDatabaseIdField = EntityIdField
+class JobBaseModel(Model, WithModelClass):
+    id: JobId
     history_id: Optional[EncodedDatabaseIdField] = Field(
         None,
         title="History ID",
         description="The encoded ID of the history associated with this item.",
     )
     model_class: JOB_MODEL_CLASS = ModelClassField(JOB_MODEL_CLASS)
     tool_id: str = Field(
@@ -1847,59 +1946,67 @@
     exit_code: Optional[int] = Field(
         None,
         title="Exit Code",
         description="The exit code returned by the tool. Can be unset if the job is not completed yet.",
     )
     create_time: datetime = CreateTimeField
     update_time: datetime = UpdateTimeField
-    galaxy_version: str = Field(
-        ...,
+    galaxy_version: Optional[str] = Field(
+        default=None,
         title="Galaxy Version",
         description="The (major) version of Galaxy used to create this job.",
-        example="21.05",
+        examples=["21.05"],
     )
 
 
 class JobImportHistoryResponse(JobBaseModel):
     message: str = Field(
         ...,
         title="Message",
         description="Text message containing information about the history import.",
     )
 
 
 class ItemStateSummary(Model):
-    id: DecodedDatabaseIdField = EntityIdField
+    id: EncodedDatabaseIdField
     populated_state: DatasetCollectionPopulatedState = PopulatedStateField
     states: Dict[JobState, int] = Field(
         {}, title="States", description=("A dictionary of job states and the number of jobs in that state.")
     )
 
 
 class JobStateSummary(ItemStateSummary):
-    model: Literal["Job"] = ModelClassField("Job")
+    model: Literal["Job"] = ModelClassField(Literal["Job"])
 
 
 class ImplicitCollectionJobsStateSummary(ItemStateSummary):
-    model: Literal["ImplicitCollectionJobs"] = ModelClassField("ImplicitCollectionJobs")
+    model: Literal["ImplicitCollectionJobs"] = ModelClassField(Literal["ImplicitCollectionJobs"])
 
 
 class WorkflowInvocationStateSummary(ItemStateSummary):
-    model: Literal["WorkflowInvocation"] = ModelClassField("WorkflowInvocation")
+    model: Literal["WorkflowInvocation"] = ModelClassField(Literal["WorkflowInvocation"])
 
 
 class JobSummary(JobBaseModel):
     """Basic information about a job."""
 
     external_id: Optional[str] = Field(
         None,
         title="External ID",
-        description=(
-            "The job id used by the external job runner (Condor, Pulsar, etc.)" "Only administrator can see this value."
-        ),
+        description="The job id used by the external job runner (Condor, Pulsar, etc.). Only administrator can see this value.",
+    )
+    handler: Optional[str] = Field(
+        None,
+        title="Job Handler",
+        description="The job handler process assigned to handle this job. Only administrator can see this value.",
+    )
+    job_runner_name: Optional[str] = Field(
+        None,
+        title="Job Runner Name",
+        description="Name of the job runner plugin that handles this job. Only administrator can see this value.",
     )
     command_line: Optional[str] = Field(
         None,
         title="Command Line",
         description=(
             "The command line produced by the job. "
             "Users can see this value if allowed in the configuration, administrator can always see this value."
@@ -1920,42 +2027,47 @@
         ...,
         title="Source",
         description="The source of this dataset, either `hda` or `ldda` depending of its origin.",
     )
 
 
 class DatasetSourceId(DatasetSourceIdBase):
-    id: DecodedDatabaseIdField = EntityIdField
+    id: DecodedDatabaseIdField
 
 
 class EncodedDatasetSourceId(DatasetSourceIdBase):
-    id: EncodedDatabaseIdField = EntityIdField
+    id: EncodedDatabaseIdField
 
 
 class EncodedDataItemSourceId(Model):
-    id: EncodedDatabaseIdField = EntityIdField
+    id: EncodedDatabaseIdField
     src: DataItemSourceType = Field(
         ...,
         title="Source",
         description="The source of this dataset, either `hda`, `ldda`, `hdca`, `dce` or `dc` depending of its origin.",
     )
 
 
+class EncodedJobParameterHistoryItem(EncodedDataItemSourceId):
+    hid: Optional[int] = None
+    name: str
+
+
 class DatasetJobInfo(DatasetSourceId):
-    uuid: UUID4 = UuidField
+    uuid: UuidField
 
 
 class JobDetails(JobSummary):
     command_version: str = Field(
         ...,
         title="Command Version",
         description="Tool version indicated during job execution.",
     )
     params: Any = Field(
-        ...,
+        None,
         title="Parameters",
         description=(
             "Object containing all the parameters of the tool associated with this job. "
             "The specific parameters depend on the tool itself."
         ),
     )
     inputs: Dict[str, DatasetJobInfo] = Field(
@@ -1992,31 +2104,31 @@
         description="The name of the metric variable.",
     )
     raw_value: str = Field(
         ...,
         title="Raw Value",
         description="The raw value of the metric as a string.",
     )
-
-    class Config:
-        schema_extra = {
+    model_config = ConfigDict(
+        json_schema_extra={
             "example": {
                 "title": "Job Start Time",
                 "value": "2021-02-25 14:55:40",
                 "plugin": "core",
                 "name": "start_epoch",
                 "raw_value": "1614261340.0000000",
             }
         }
+    )
 
 
-class JobMetricCollection(Model):
+class JobMetricCollection(RootModel):
     """Represents a collection of metrics associated with a Job."""
 
-    __root__: List[JobMetric] = Field(
+    root: List[JobMetric] = Field(
         [],
         title="Job Metrics",
         description="Collections of metrics provided by `JobInstrumenter` plugins on a particular job.",
     )
 
 
 class JobFullDetails(JobDetails):
@@ -2061,34 +2173,36 @@
         description=(
             "Collections of metrics provided by `JobInstrumenter` plugins on a particular job. "
             "Only administrators can see these metrics."
         ),
     )
 
 
-class StoredWorkflowSummary(Model):
-    id: DecodedDatabaseIdField = EntityIdField
+class StoredWorkflowSummary(Model, WithModelClass):
+    id: EncodedDatabaseIdField
     model_class: STORED_WORKFLOW_MODEL_CLASS = ModelClassField(STORED_WORKFLOW_MODEL_CLASS)
     create_time: datetime = CreateTimeField
     update_time: datetime = UpdateTimeField
     name: str = Field(
         ...,
         title="Name",
         description="The name of the history.",
     )
-    url: RelativeUrl = RelativeUrlField
+    url: RelativeUrlField
     published: bool = Field(
         ...,
         title="Published",
         description="Whether this workflow is currently publicly available to all users.",
     )
-    annotations: List[str] = Field(  # Inconsistency? Why workflows summaries use a list instead of an optional string?
-        ...,
-        title="Annotations",
-        description="An list of annotations to provide details or to help understand the purpose and usage of this workflow.",
+    annotations: Optional[List[str]] = (
+        Field(  # Inconsistency? Why workflows summaries use a list instead of an optional string?
+            None,
+            title="Annotations",
+            description="An list of annotations to provide details or to help understand the purpose and usage of this workflow.",
+        )
     )
     tags: TagCollection
     deleted: bool = Field(
         ...,
         title="Deleted",
         description="Whether this item is marked as deleted.",
     )
@@ -2098,43 +2212,43 @@
         description="TODO",
     )
     owner: str = Field(
         ...,
         title="Owner",
         description="The name of the user who owns this workflow.",
     )
-    latest_workflow_uuid: UUID4 = Field(  # Is this really used?
-        ...,
+    latest_workflow_uuid: Optional[UUID4] = Field(
+        None,
         title="Latest workflow UUID",
         description="TODO",
     )
-    number_of_steps: int = Field(
-        ...,
+    number_of_steps: Optional[int] = Field(
+        None,
         title="Number of Steps",
         description="The number of steps that make up this workflow.",
     )
-    show_in_tool_panel: bool = Field(
-        ...,
+    show_in_tool_panel: Optional[bool] = Field(
+        None,
         title="Show in Tool Panel",
         description="Whether to display this workflow in the Tools Panel.",
     )
 
 
 class WorkflowInput(Model):
-    label: str = Field(
+    label: Optional[str] = Field(
         ...,
         title="Label",
         description="Label of the input.",
     )
-    value: str = Field(
+    value: Optional[Any] = Field(
         ...,
         title="Value",
         description="TODO",
     )
-    uuid: UUID4 = Field(
+    uuid: Optional[UUID4] = Field(
         ...,
         title="UUID",
         description="Universal unique identifier of the input.",
     )
 
 
 class WorkflowOutput(Model):
@@ -2145,15 +2259,15 @@
     )
     output_name: str = Field(
         ...,
         title="Output Name",
         description="The name assigned to the output.",
     )
     uuid: Optional[UUID4] = Field(
-        ...,
+        None,
         title="UUID",
         description="Universal unique identifier of the output.",
     )
 
 
 class InputStep(Model):
     source_step: int = Field(
@@ -2164,92 +2278,68 @@
     step_output: str = Field(
         ...,
         title="Step Output",
         description="The name of the output generated by the source step.",
     )
 
 
-class WorkflowModuleType(str, Enum):
-    """Available types of modules that represent a step in a Workflow."""
-
-    data_input = "data_input"
-    data_collection_input = "data_collection_input"
-    parameter_input = "parameter_input"
-    subworkflow = "subworkflow"
-    tool = "tool"
-    pause = "pause"  # Experimental
-
-
 class WorkflowStepBase(Model):
     id: int = Field(
         ...,
         title="ID",
         description="The identifier of the step. It matches the index order of the step inside the workflow.",
     )
-    type: WorkflowModuleType = Field(..., title="Type", description="The type of workflow module.")
     annotation: Optional[str] = AnnotationField
     input_steps: Dict[str, InputStep] = Field(
         ...,
         title="Input Steps",
         description="A dictionary containing information about the inputs connected to this workflow step.",
     )
-
-
-class ToolBasedWorkflowStep(WorkflowStepBase):
+    when: Optional[str]
+    # TODO: these should move to ToolStep, however we might be breaking scripts that iterate over steps and
+    # assume tool_id is a valid key for every step.
     tool_id: Optional[str] = Field(
         None, title="Tool ID", description="The unique name of the tool associated with this step."
     )
     tool_version: Optional[str] = Field(
         None, title="Tool Version", description="The version of the tool associated with this step."
     )
-    tool_inputs: Any = Field(..., title="Tool Inputs", description="TODO")
+    tool_inputs: Any = Field(None, title="Tool Inputs", description="TODO")
 
 
-class InputDataStep(ToolBasedWorkflowStep):
-    type: WorkflowModuleType = Field(
-        WorkflowModuleType.data_input, const=True, title="Type", description="The type of workflow module."
-    )
+class InputDataStep(WorkflowStepBase):
+    type: Literal["data_input"]
 
 
-class InputDataCollectionStep(ToolBasedWorkflowStep):
-    type: WorkflowModuleType = Field(
-        WorkflowModuleType.data_collection_input, const=True, title="Type", description="The type of workflow module."
-    )
+class InputDataCollectionStep(WorkflowStepBase):
+    type: Literal["data_collection_input"]
 
 
-class InputParameterStep(ToolBasedWorkflowStep):
-    type: WorkflowModuleType = Field(
-        WorkflowModuleType.parameter_input, const=True, title="Type", description="The type of workflow module."
-    )
+class InputParameterStep(WorkflowStepBase):
+    type: Literal["parameter_input"]
 
 
 class PauseStep(WorkflowStepBase):
-    type: WorkflowModuleType = Field(
-        WorkflowModuleType.pause, const=True, title="Type", description="The type of workflow module."
-    )
+    type: Literal["pause"]
 
 
-class ToolStep(ToolBasedWorkflowStep):
-    type: WorkflowModuleType = Field(
-        WorkflowModuleType.tool, const=True, title="Type", description="The type of workflow module."
-    )
+class ToolStep(WorkflowStepBase):
+    type: Literal["tool"]
 
 
 class SubworkflowStep(WorkflowStepBase):
-    type: WorkflowModuleType = Field(
-        WorkflowModuleType.subworkflow, const=True, title="Type", description="The type of workflow module."
-    )
-    workflow_id: DecodedDatabaseIdField = Field(
+    type: Literal["subworkflow"]
+    workflow_id: EncodedDatabaseIdField = Field(
         ..., title="Workflow ID", description="The encoded ID of the workflow that will be run on this step."
     )
 
 
 class Creator(Model):
     class_: str = Field(..., alias="class", title="Class", description="The class representing this creator.")
-    name: str = Field(..., title="Name", description="The name of the creator.")
+    name: Optional[str] = Field(None, title="Name", description="The name of the creator.")
     address: Optional[str] = Field(
         None,
         title="Address",
     )
     alternate_name: Optional[str] = Field(
         None,
         alias="alternateName",
@@ -2278,23 +2368,21 @@
         title="URL",
     )
 
 
 class Organization(Creator):
     class_: str = Field(
         "Organization",
-        const=True,
         alias="class",
     )
 
 
 class Person(Creator):
     class_: str = Field(
         "Person",
-        const=True,
         alias="class",
     )
     family_name: Optional[str] = Field(
         None,
         alias="familyName",
         title="Family Name",
     )
@@ -2315,43 +2403,14 @@
     job_title: Optional[str] = Field(
         None,
         alias="jobTitle",
         title="Job Title",
     )
 
 
-class StoredWorkflowDetailed(StoredWorkflowSummary):
-    annotation: Optional[str] = AnnotationField  # Inconsistency? See comment on StoredWorkflowSummary.annotations
-    license: Optional[str] = Field(
-        None, title="License", description="SPDX Identifier of the license associated with this workflow."
-    )
-    version: int = Field(
-        ..., title="Version", description="The version of the workflow represented by an incremental number."
-    )
-    inputs: Dict[int, WorkflowInput] = Field(
-        {}, title="Inputs", description="A dictionary containing information about all the inputs of the workflow."
-    )
-    creator: Optional[List[Union[Person, Organization]]] = Field(
-        None,
-        title="Creator",
-        description=("Additional information about the creator (or multiple creators) of this workflow."),
-    )
-    steps: Dict[
-        int,
-        Union[
-            InputDataStep,
-            InputDataCollectionStep,
-            InputParameterStep,
-            PauseStep,
-            ToolStep,
-            SubworkflowStep,
-        ],
-    ] = Field({}, title="Steps", description="A dictionary with information about all the steps of the workflow.")
-
-
 class Input(Model):
     name: str = Field(..., title="Name", description="The name of the input.")
     description: str = Field(..., title="Description", description="The annotation or description of the input.")
 
 
 class Output(Model):
     name: str = Field(..., title="Name", description="The name of the output.")
@@ -2381,14 +2440,17 @@
     right: int = Field(..., title="Right", description="Right margin or right-most position of the box.")
     x: int = Field(..., title="X", description="Horizontal pixel coordinate of the top right corner of the box.")
     y: int = Field(..., title="Y", description="Vertical pixel coordinate of the top right corner of the box.")
     height: int = Field(..., title="Height", description="Height of the box in pixels.")
     width: int = Field(..., title="Width", description="Width of the box in pixels.")
 
 
+InvocationsStateCounts = RootModel[Dict[str, int]]
+
+
 class WorkflowStepToExportBase(Model):
     id: int = Field(
         ...,
         title="ID",
         description="The identifier of the step. It matches the index order of the step inside the workflow.",
     )
     type: str = Field(..., title="Type", description="The type of workflow module.")
@@ -2423,15 +2485,15 @@
     )
     position: WorkflowStepLayoutPosition = Field(
         ...,
         title="Position",
         description="Layout position of this step in the graph",
     )
     workflow_outputs: List[WorkflowOutput] = Field(
-        [], title="Workflow Outputs", description="The version of the tool associated with this step."
+        [], title="Workflow Outputs", description="Workflow outputs associated with this step."
     )
 
 
 class WorkflowStepToExport(WorkflowStepToExportBase):
     content_id: Optional[str] = Field(  # Duplicate of `tool_id` or viceversa?
         None, title="Content ID", description="TODO"
     )
@@ -2538,87 +2600,87 @@
     steps: Dict[int, Union[SubworkflowStepToExport, WorkflowToolStepToExport, WorkflowStepToExport]] = Field(
         {}, title="Steps", description="A dictionary with information about all the steps of the workflow."
     )
 
 
 # Roles -----------------------------------------------------------------
 
-RoleIdField = Field(title="ID", description="Encoded ID of the role")
-RoleNameField = Field(title="Name", description="Name of the role")
-RoleDescriptionField = Field(title="Description", description="Description of the role")
+RoleIdField = Annotated[EncodedDatabaseIdField, Field(title="ID", description="Encoded ID of the role")]
+RoleNameField = Annotated[str, Field(title="Name", description="Name of the role")]
+RoleDescriptionField = Annotated[str, Field(title="Description", description="Description of the role")]
 
 
 class BasicRoleModel(Model):
-    id: EncodedDatabaseIdField = RoleIdField
-    name: str = RoleNameField
+    id: RoleIdField
+    name: RoleNameField
     type: str = Field(title="Type", description="Type or category of the role")
 
 
-class RoleModelResponse(BasicRoleModel):
-    description: Optional[str] = RoleDescriptionField
-    url: RelativeUrl = RelativeUrlField
-    model_class: Literal["Role"] = ModelClassField("Role")
+class RoleModelResponse(BasicRoleModel, WithModelClass):
+    description: Optional[RoleDescriptionField]
+    url: RelativeUrlField
+    model_class: Literal["Role"] = ModelClassField(Literal["Role"])
 
 
 class RoleDefinitionModel(Model):
-    name: str = RoleNameField
-    description: str = RoleDescriptionField
+    name: RoleNameField
+    description: RoleDescriptionField
     user_ids: Optional[List[DecodedDatabaseIdField]] = Field(title="User IDs", default=[])
     group_ids: Optional[List[DecodedDatabaseIdField]] = Field(title="Group IDs", default=[])
 
 
-class RoleListResponse(Model):
-    __root__: List[RoleModelResponse]
+class RoleListResponse(RootModel):
+    root: List[RoleModelResponse]
 
 
 # The tuple should probably be another proper model instead?
 # Keeping it as a Tuple for now for backward compatibility
 # TODO: Use Tuple again when `make update-client-api-schema` supports them
 RoleNameIdTuple = List[str]  # Tuple[str, DecodedDatabaseIdField]
 
 # Group_Roles -----------------------------------------------------------------
 
 
 class GroupRoleResponse(Model):
-    id: EncodedDatabaseIdField = RoleIdField
-    name: str = RoleNameField
-    url: RelativeUrl = RelativeUrlField
+    id: RoleIdField
+    name: RoleNameField
+    url: RelativeUrlField
 
 
-class GroupRoleListResponse(Model):
-    __root__: List[GroupRoleResponse]
+class GroupRoleListResponse(RootModel):
+    root: List[GroupRoleResponse]
 
 
 # Users -----------------------------------------------------------------------
 # Group_Users -----------------------------------------------------------------
 
 
 class GroupUserResponse(Model):
-    id: EncodedDatabaseIdField = UserIdField
+    id: EncodedDatabaseIdField
     email: str = UserEmailField
-    url: RelativeUrl = RelativeUrlField
+    url: RelativeUrlField
 
 
-class GroupUserListResponse(Model):
-    __root__: List[GroupUserResponse]
+class GroupUserListResponse(RootModel):
+    root: List[GroupUserResponse]
 
 
 class ImportToolDataBundleUriSource(Model):
     src: Literal["uri"] = Field(title="src", description="Indicates that the tool data should be resolved by a URI.")
     uri: str = Field(
         title="uri",
         description="URI to fetch tool data bundle from (file:// URIs are fine because this is an admin-only operation)",
     )
 
 
 class ImportToolDataBundleDatasetSource(Model):
     src: Literal["hda", "ldda"] = Field(
         title="src", description="Indicates that the tool data should be resolved from a dataset."
     )
-    id: DecodedDatabaseIdField = EntityIdField
+    id: DecodedDatabaseIdField
 
 
 ImportToolDataBundleSource = Union[ImportToolDataBundleDatasetSource, ImportToolDataBundleUriSource]
 
 
 class ToolShedRepository(Model):
     tool_shed_url: str = Field(
@@ -2635,22 +2697,22 @@
 class InstalledRepositoryToolShedStatus(Model):
     # See https://github.com/galaxyproject/galaxy/issues/10453 , bad booleans
     # See https://github.com/galaxyproject/galaxy/issues/16135 , optional fields
     latest_installable_revision: Optional[str] = Field(
         title="Latest installed revision", description="Most recent version available on the tool shed"
     )
     revision_update: str
-    revision_upgrade: Optional[str]
+    revision_upgrade: Optional[str] = None
     repository_deprecated: Optional[str] = Field(
         title="Repository deprecated", description="Repository has been depreciated on the tool shed"
     )
 
 
-class InstalledToolShedRepository(Model):
-    model_class: Literal["ToolShedRepository"] = ModelClassField("ToolShedRepository")
+class InstalledToolShedRepository(Model, WithModelClass):
+    model_class: Literal["ToolShedRepository"] = ModelClassField(Literal["ToolShedRepository"])
     id: EncodedDatabaseIdField = Field(
         ...,
         title="ID",
         description="Encoded ID of the install tool shed repository.",
     )
     status: str
     name: str = Field(title="Name", description="Name of repository")
@@ -2673,16 +2735,16 @@
         title="Changeset revision", description="Changeset revision of the repository - a mercurial commit hash"
     )
     tool_shed_status: Optional[InstalledRepositoryToolShedStatus] = Field(
         title="Latest updated status from the tool shed"
     )
 
 
-class InstalledToolShedRepositories(Model):
-    __root__: List[InstalledToolShedRepository]
+class InstalledToolShedRepositories(RootModel):
+    root: List[InstalledToolShedRepository]
 
 
 CheckForUpdatesResponseStatusT = Literal["ok", "error"]
 
 
 class CheckForUpdatesResponse(Model):
     status: CheckForUpdatesResponseStatusT = Field(title="Status", description="'ok' or 'error'")
@@ -2695,16 +2757,16 @@
 
 
 class LibraryPermissionScope(str, Enum):
     current = "current"
     available = "available"
 
 
-class LibraryLegacySummary(Model):
-    model_class: Literal["Library"] = ModelClassField("Library")
+class LibraryLegacySummary(Model, WithModelClass):
+    model_class: Literal["Library"] = ModelClassField(Literal["Library"])
     id: EncodedDatabaseIdField = Field(
         ...,
         title="ID",
         description="Encoded ID of the Library.",
     )
     name: str = Field(
         ...,
@@ -2739,15 +2801,15 @@
 
 
 class LibrarySummary(LibraryLegacySummary):
     create_time_pretty: str = Field(  # This is somewhat redundant, maybe the client can do this with `create_time`?
         ...,
         title="Create Time Pretty",
         description="Nice time representation of the creation date.",
-        example="2 months ago",
+        examples=["2 months ago"],
     )
     public: bool = Field(
         ...,
         title="Public",
         description="Whether this Library has been deleted.",
     )
     can_user_add: bool = Field(
@@ -2763,16 +2825,16 @@
     can_user_manage: bool = Field(
         ...,
         title="Can User Manage",
         description="Whether the current user can manage the Library and its contents.",
     )
 
 
-class LibrarySummaryList(Model):
-    __root__: List[LibrarySummary] = Field(
+class LibrarySummaryList(RootModel):
+    root: List[LibrarySummary] = Field(
         default=[],
         title="List with summary information of Libraries.",
     )
 
 
 class CreateLibraryPayload(Model):
     name: str = Field(
@@ -2846,15 +2908,15 @@
 
 
 RoleIdList = Union[
     List[DecodedDatabaseIdField], DecodedDatabaseIdField
 ]  # Should we support just List[DecodedDatabaseIdField] in the future?
 
 
-class LegacyLibraryPermissionsPayload(Model):
+class LegacyLibraryPermissionsPayload(RequireOneSetOption):
     LIBRARY_ACCESS_in: Optional[RoleIdList] = Field(
         [],
         title="Access IDs",
         description="A list of role encoded IDs defining roles that should have access permission on the library.",
     )
     LIBRARY_MODIFY_in: Optional[RoleIdList] = Field(
         [],
@@ -2880,15 +2942,15 @@
 
 class DatasetPermissionAction(str, Enum):
     set_permissions = "set_permissions"
     make_private = "make_private"
     remove_restrictions = "remove_restrictions"
 
 
-class LibraryPermissionsPayloadBase(Model):
+class LibraryPermissionsPayloadBase(RequireOneSetOption):
     add_ids: Optional[RoleIdList] = Field(
         [],
         alias="add_ids[]",
         title="Add IDs",
         description="A list of role encoded IDs defining roles that should be able to add items to the library.",
     )
     manage_ids: Optional[RoleIdList] = Field(
@@ -2903,15 +2965,15 @@
         title="Modify IDs",
         description="A list of role encoded IDs defining roles that should have modify permission on the library.",
     )
 
 
 class LibraryPermissionsPayload(LibraryPermissionsPayloadBase):
     action: Optional[LibraryPermissionAction] = Field(
-        ...,
+        None,
         title="Action",
         description="Indicates what action should be performed on the Library.",
     )
     access_ids: Optional[RoleIdList] = Field(
         [],
         alias="access_ids[]",  # Added for backward compatibility but it looks really ugly...
         title="Access IDs",
@@ -2942,34 +3004,34 @@
     action: Optional[LibraryFolderPermissionAction] = Field(
         None,
         title="Action",
         description="Indicates what action should be performed on the library folder.",
     )
 
 
-class LibraryFolderDetails(Model):
-    model_class: Literal["LibraryFolder"] = ModelClassField("LibraryFolder")
-    id: LibraryFolderDatabaseIdField = Field(
+class LibraryFolderDetails(Model, WithModelClass):
+    model_class: Literal["LibraryFolder"] = ModelClassField(Literal["LibraryFolder"])
+    id: EncodedLibraryFolderDatabaseIdField = Field(
         ...,
         title="ID",
         description="Encoded ID of the library folder.",
     )
     name: str = FolderNameField
     description: Optional[str] = FolderDescriptionField
     item_count: int = Field(
         ...,
         title="Item Count",
         description="A detailed description of the library folder.",
     )
-    parent_library_id: DecodedDatabaseIdField = Field(
+    parent_library_id: EncodedDatabaseIdField = Field(
         ...,
         title="Parent Library ID",
         description="Encoded ID of the Library this folder belongs to.",
     )
-    parent_id: Optional[LibraryFolderDatabaseIdField] = Field(
+    parent_id: Optional[EncodedLibraryFolderDatabaseIdField] = Field(
         None,
         title="Parent Folder ID",
         description="Encoded ID of the parent folder. Empty if it's the root folder.",
     )
     genome_build: Optional[str] = GenomeBuildField
     update_time: datetime = UpdateTimeField
     deleted: bool = Field(
@@ -3074,33 +3136,33 @@
 class FileLibraryFolderItem(LibraryFolderItemBase):
     id: EncodedDatabaseIdField
     type: Literal["file"]
     file_ext: str
     date_uploaded: datetime
     is_unrestricted: bool
     is_private: bool
-    state: DatasetState = DatasetStateField
+    state: DatasetStateField
     file_size: str
     raw_size: int
     ldda_id: EncodedDatabaseIdField
     tags: TagCollection
-    message: Optional[str]
+    message: Optional[str] = None
 
 
 AnyLibraryFolderItem = Annotated[Union[FileLibraryFolderItem, FolderLibraryFolderItem], Field(discriminator="type")]
 
 
 class LibraryFolderMetadata(Model):
     parent_library_id: EncodedDatabaseIdField
     folder_name: str
     folder_description: str
     total_rows: int
     can_modify_folder: bool
     can_add_library_item: bool
-    full_path: List[List[str]]
+    full_path: List[Tuple[EncodedLibraryFolderDatabaseIdField, str]]
 
 
 class LibraryFolderContentsIndexResult(Model):
     metadata: LibraryFolderMetadata
     folder_contents: List[AnyLibraryFolderItem]
 
 
@@ -3177,31 +3239,50 @@
         [],
         alias="modify_ids[]",
         title="Modify IDs",
         description="A list of role encoded IDs defining roles that should have modify permission on the dataset.",
     )
 
 
-class CustomHistoryItem(Model):
-    """Can contain any serializable property of the item.
+@partial_model()
+class HDACustom(HDADetailed):
+    """Can contain any serializable property of an HDA.
 
     Allows arbitrary custom keys to be specified in the serialization
     parameters without a particular view (predefined set of keys).
     """
 
-    class Config:
-        extra = Extra.allow
+    # TODO: Fix this workaround for partial_model not supporting UUID fields for some reason.
+    # The error otherwise is: `PydanticUserError: 'UuidVersion' cannot annotate 'nullable'.`
+    # Also ignoring mypy complaints about the type redefinition.
+    uuid: Optional[UUID4]  # type: ignore
+
+    # Add fields that are not part of any view here
+    visualizations: Annotated[
+        Optional[List[Visualization]],
+        Field(
+            None,
+            title="Visualizations",
+            description="The collection of visualizations that can be applied to this dataset.",
+        ),
+    ]
+
+    # We need to allow extra fields so we can have the metadata_* fields serialized.
+    # TODO: try to find a better way to handle this.
+    model_config = ConfigDict(extra="allow")
 
 
-AnyHDA = Union[HDADetailed, HDASummary]
+AnyHDA = Union[HDACustom, HDADetailed, HDASummary]
 AnyHDCA = Union[HDCADetailed, HDCASummary]
-AnyHistoryContentItem = Union[
-    AnyHDA,
-    AnyHDCA,
-    CustomHistoryItem,
+AnyHistoryContentItem = Annotated[
+    Union[
+        AnyHDA,
+        AnyHDCA,
+    ],
+    Field(union_mode="left_to_right"),
 ]
 
 
 AnyJobStateSummary = Annotated[
     Union[
         JobStateSummary,
         ImplicitCollectionJobsStateSummary,
@@ -3228,15 +3309,15 @@
     stop_job: bool = Field(
         default=False,
         title="Stop Job",
         description="Whether to stop the creating job if all the job's outputs are deleted.",
     )
 
 
-class DeleteHistoryContentResult(CustomHistoryItem):
+class DeleteHistoryContentResult(Model):
     """Contains minimum information about the deletion state of a history item.
 
     Can also contain any other properties of the item."""
 
     id: DecodedDatabaseIdField = Field(
         ...,
         title="ID",
@@ -3250,41 +3331,41 @@
     purged: Optional[bool] = Field(
         default=None,
         title="Purged",
         description="True if the item was successfully removed from disk.",
     )
 
 
-class HistoryContentsArchiveDryRunResult(Model):
+class HistoryContentsArchiveDryRunResult(RootModel):
     """
     Contains a collection of filepath/filename entries that represent
     the contents that would have been included in the archive.
     This is returned when the `dry_run` flag is active when
     creating an archive with the contents of the history.
 
     This is used for debugging purposes.
     """
 
-    __root__: List[Tuple[str, str]]
+    root: List[Tuple[str, str]]
 
 
 class HistoryContentStats(Model):
     total_matches: int = Field(
         ...,
         title="Total Matches",
         description=("The total number of items that match the search query without any pagination"),
     )
 
 
-class HistoryContentsResult(Model):
+class HistoryContentsResult(RootModel):
     """List of history content items.
     Can contain different views and kinds of items.
     """
 
-    __root__: List[AnyHistoryContentItem]
+    root: List[AnyHistoryContentItem]
 
 
 class HistoryContentsWithStatsResult(Model):
     """Includes stats with items counting"""
 
     stats: HistoryContentStats = Field(
         ...,
@@ -3315,17 +3396,14 @@
 class ShareWithExtra(Model):
     can_share: bool = Field(
         False,
         title="Can Share",
         description="Indicates whether the resource can be directly shared or requires further actions.",
     )
 
-    class Config:
-        extra = Extra.allow
-
 
 UserIdentifier = Union[DecodedDatabaseIdField, str]
 
 
 class ShareWithPayload(Model):
     user_ids: List[UserIdentifier] = Field(
         ...,
@@ -3352,15 +3430,15 @@
         ...,
         title="New Slug",
         description="The slug that will be used to access this shared item.",
     )
 
 
 class UserEmail(Model):
-    id: DecodedDatabaseIdField = Field(
+    id: EncodedDatabaseIdField = Field(
         ...,
         title="User ID",
         description="The encoded ID of the user.",
     )
     email: str = Field(
         ...,
         title="Email",
@@ -3373,15 +3451,15 @@
         ...,
         title="Enabled",
         description="True if beacon sharing is enabled",
     )
 
 
 class SharingStatus(Model):
-    id: DecodedDatabaseIdField = Field(
+    id: EncodedDatabaseIdField = Field(
         ...,
         title="ID",
         description="The encoded ID of the resource to be shared.",
     )
     title: str = Field(
         ...,
         title="Title",
@@ -3415,32 +3493,16 @@
     username_and_slug: Optional[str] = Field(
         None,
         title="Username and slug",
         description="The relative URL in the form of /u/{username}/{resource_single_char}/{slug}",
     )
 
 
-class ShareWithStatus(SharingStatus):
-    errors: List[str] = Field(
-        [],
-        title="Errors",
-        description="Collection of messages indicating that the resource was not shared with some (or all users) due to an error.",
-    )
-    extra: Optional[ShareWithExtra] = Field(
-        None,
-        title="Extra",
-        description=(
-            "Optional extra information about this shareable resource that may be of interest. "
-            "The contents of this field depend on the particular resource."
-        ),
-    )
-
-
 class HDABasicInfo(Model):
-    id: DecodedDatabaseIdField
+    id: EncodedDatabaseIdField
     name: str
 
 
 class ShareHistoryExtra(ShareWithExtra):
     can_change: List[HDABasicInfo] = Field(
         [],
         title="Can Change",
@@ -3460,14 +3522,41 @@
     accessible_count: int = Field(
         0,
         title="Accessible Count",
         description=("The number of datasets in the history that are public or accessible by all the target users."),
     )
 
 
+class ShareWithStatus(SharingStatus):
+    errors: List[str] = Field(
+        [],
+        title="Errors",
+        description="Collection of messages indicating that the resource was not shared with some (or all users) due to an error.",
+    )
+    extra: Optional[ShareWithExtra] = Field(
+        None,
+        title="Extra",
+        description=(
+            "Optional extra information about this shareable resource that may be of interest. "
+            "The contents of this field depend on the particular resource."
+        ),
+    )
+
+
+class ShareHistoryWithStatus(ShareWithStatus):
+    extra: ShareHistoryExtra = Field(
+        ...,
+        title="Extra",
+        description=(
+            "Optional extra information about this shareable resource that may be of interest. "
+            "The contents of this field depend on the particular resource."
+        ),
+    )
+
+
 # Pages -------------------------------------------------------
 
 
 class PageContentFormat(str, Enum):
     markdown = "markdown"
     html = "html"
 
@@ -3477,29 +3566,29 @@
     title="Content format",
     description="Either `markdown` or `html`.",
 )
 
 ContentField: Optional[str] = Field(
     default="",
     title="Content",
-    description="Raw text contents of the first page revision (type dependent on content_format).",
+    description="Raw text contents of the last page revision (type dependent on content_format).",
 )
 
 
 class PageSummaryBase(Model):
     title: str = Field(
         ...,  # Required
         title="Title",
         description="The name of the page.",
     )
     slug: str = Field(
         ...,  # Required
         title="Identifier",
         description="The title slug for the page URL, must be unique.",
-        regex=r"^[a-z0-9\-]+$",
+        pattern=r"^[a-z0-9\-]+$",
     )
 
 
 class MaterializeDatasetInstanceAPIRequest(Model):
     source: DatasetSourceType = Field(
         title="Source",
         description="The source of the content. Can be other history element to be copied or library elements.",
@@ -3527,18 +3616,15 @@
         description="Annotation that will be attached to the page.",
     )
     invocation_id: Optional[DecodedDatabaseIdField] = Field(
         None,
         title="Workflow invocation ID",
         description="Encoded ID used by workflow generated reports.",
     )
-
-    class Config:
-        use_enum_values = True  # When using .dict()
-        extra = Extra.allow  # Allow any other extra fields
+    model_config = ConfigDict(use_enum_values=True, extra="allow")
 
 
 class AsyncTaskResultSummary(Model):
     id: str = Field(
         ...,
         title="ID",
         description="Celery AsyncResult ID for this task",
@@ -3559,16 +3645,16 @@
 
 
 class AsyncFile(Model):
     storage_request_id: UUID
     task: AsyncTaskResultSummary
 
 
-class PageSummary(PageSummaryBase):
-    id: DecodedDatabaseIdField = Field(
+class PageSummary(PageSummaryBase, WithModelClass):
+    id: EncodedDatabaseIdField = Field(
         ...,  # Required
         title="ID",
         description="Encoded ID of the Page.",
     )
     model_class: PAGE_MODEL_CLASS = ModelClassField(PAGE_MODEL_CLASS)
     username: str = Field(
         ...,  # Required
@@ -3591,58 +3677,60 @@
         description="Whether this Page can be imported.",
     )
     deleted: bool = Field(
         ...,  # Required
         title="Deleted",
         description="Whether this Page has been deleted.",
     )
-    latest_revision_id: DecodedDatabaseIdField = Field(
+    latest_revision_id: EncodedDatabaseIdField = Field(
         ...,  # Required
         title="Latest revision ID",
         description="The encoded ID of the last revision of this Page.",
     )
-    revision_ids: List[DecodedDatabaseIdField] = Field(
+    revision_ids: List[EncodedDatabaseIdField] = Field(
         ...,  # Required
         title="List of revisions",
         description="The history with the encoded ID of each revision of the Page.",
     )
-    create_time: Optional[datetime] = CreateTimeField
-    update_time: Optional[datetime] = UpdateTimeField
+    create_time: datetime = CreateTimeField
+    update_time: datetime = UpdateTimeField
     tags: TagCollection
 
 
+GenerateVersionField = Field(
+    None,
+    title="Galaxy Version",
+    description="The version of Galaxy this object was generated with.",
+)
+GenerateTimeField = Field(
+    None,
+    title="Galaxy Version",
+    description="The version of Galaxy this object was generated with.",
+)
+
+
 class PageDetails(PageSummary):
     content_format: PageContentFormat = ContentFormatField
     content: Optional[str] = ContentField
-    generate_version: Optional[str] = Field(
-        None,
-        title="Galaxy Version",
-        description="The version of Galaxy this page was generated with.",
-    )
-    generate_time: Optional[str] = Field(
-        None,
-        title="Generate Date",
-        description="The date this page was generated.",
-    )
+    generate_version: Optional[str] = GenerateVersionField
+    generate_time: Optional[str] = GenerateTimeField
+    model_config = ConfigDict(extra="allow")
 
-    class Config:
-        extra = Extra.allow  # Allow any other extra fields
 
-
-class PageSummaryList(Model):
-    __root__: List[PageSummary] = Field(
+class PageSummaryList(RootModel):
+    root: List[PageSummary] = Field(
         default=[],
         title="List with summary information of Pages.",
     )
 
 
 class DatasetSummary(Model):
-    id: EncodedDatabaseIdField = EntityIdField
+    id: EncodedDatabaseIdField
     create_time: Optional[datetime] = CreateTimeField
     update_time: Optional[datetime] = UpdateTimeField
-    state: DatasetState = DatasetStateField
+    state: DatasetStateField
     deleted: bool
     purged: bool
     purgable: bool
     file_size: int
     total_size: int
-    uuid: UUID4 = UuidField
+    uuid: UuidField
```

### Comparing `galaxy-schema-23.2.1/galaxy/schema/storage_cleaner.py` & `galaxy-schema-24.0.0/galaxy/schema/storage_cleaner.py`

 * *Files identical despite different names*

### Comparing `galaxy-schema-23.2.1/galaxy/schema/visualization.py` & `galaxy-schema-24.0.0/galaxy/schema/visualization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from datetime import datetime
 from typing import (
     List,
     Optional,
 )
 
 from pydantic import (
-    Extra,
+    ConfigDict,
     Field,
+    RootModel,
 )
 from typing_extensions import Literal
 
 from galaxy.schema.fields import (
     DecodedDatabaseIdField,
     EncodedDatabaseIdField,
 )
@@ -87,17 +88,15 @@
     username: str = Field(
         ...,  # Required
         title="Username",
         description="The name of the user owning this Visualization.",
     )
     create_time: Optional[datetime] = CreateTimeField
     update_time: Optional[datetime] = UpdateTimeField
+    model_config = ConfigDict(extra="allow")
 
-    class Config:
-        extra = Extra.allow  # Allow any other extra fields
 
-
-class VisualizationSummaryList(Model):
-    __root__: List[VisualizationSummary] = Field(
+class VisualizationSummaryList(RootModel):
+    root: List[VisualizationSummary] = Field(
         default=[],
         title="List with detailed information of Visualizations.",
     )
```

### Comparing `galaxy-schema-23.2.1/galaxy/schema/workflow/comments.py` & `galaxy-schema-24.0.0/galaxy/schema/workflow/comments.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,30 +4,35 @@
     Tuple,
     Union,
 )
 
 from pydantic import (
     BaseModel,
     Field,
+    RootModel,
 )
 from typing_extensions import Literal
 
 
 class BaseComment(BaseModel):
     id: int = Field(..., description="Unique identifier for this comment. Determined by the comments order")
     color: Literal["none", "black", "blue", "turquoise", "green", "lime", "orange", "yellow", "red", "pink"] = Field(
         ..., description="Color this comment is displayed as. The exact color hex is determined by the client"
     )
     position: Tuple[float, float] = Field(..., description="[x, y] position of this comment in the Workflow")
     size: Tuple[float, float] = Field(..., description="[width, height] size of this comment")
 
 
 class TextCommentData(BaseModel):
-    bold: Optional[bool] = Field(description="If the Comments text is bold. Absent is interpreted as false")
-    italic: Optional[bool] = Field(description="If the Comments text is italic. Absent is interpreted as false")
+    bold: Optional[bool] = Field(
+        default=None, description="If the Comments text is bold. Absent is interpreted as false"
+    )
+    italic: Optional[bool] = Field(
+        default=None, description="If the Comments text is italic. Absent is interpreted as false"
+    )
     size: int = Field(..., description="Relative size (1 -> 100%) of the text compared to the default text sitz")
     text: str = Field(..., description="The plaintext text of this comment")
 
 
 class TextComment(BaseComment):
     type: Literal["text"]
     data: TextCommentData
@@ -46,18 +51,18 @@
     title: str = Field(..., description="The Frames title")
 
 
 class FrameComment(BaseComment):
     type: Literal["frame"]
     data: FrameCommentData
     child_comments: Optional[List[int]] = Field(
-        description="A list of ids (see `id`) of all Comments which are encompassed by this Frame"
+        default=None, description="A list of ids (see `id`) of all Comments which are encompassed by this Frame"
     )
     child_steps: Optional[List[int]] = Field(
-        description="A list of ids of all Steps (see WorkflowStep.id) which are encompassed by this Frame"
+        default=None, description="A list of ids of all Steps (see WorkflowStep.id) which are encompassed by this Frame"
     )
 
 
 class FreehandCommentData(BaseModel):
     thickness: int = Field(..., description="Width of the Line in pixels")
     line: List[Tuple[float, float]] = Field(
         ...,
@@ -66,9 +71,9 @@
 
 
 class FreehandComment(BaseComment):
     type: Literal["freehand"]
     data: FreehandCommentData
 
 
-class WorkflowCommentModel(BaseModel):
-    __root__: Union[TextComment, MarkdownComment, FrameComment, FreehandComment]
+class WorkflowCommentModel(RootModel):
+    root: Union[TextComment, MarkdownComment, FrameComment, FreehandComment] = Field(..., discriminator="type")
```

### Comparing `galaxy-schema-23.2.1/galaxy_schema.egg-info/SOURCES.txt` & `galaxy-schema-24.0.0/galaxy_schema.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -10,41 +10,35 @@
 galaxy/py.typed
 galaxy/schema/__init__.py
 galaxy/schema/cloud.py
 galaxy/schema/fetch_data.py
 galaxy/schema/fields.py
 galaxy/schema/groups.py
 galaxy/schema/help.py
+galaxy/schema/history.py
 galaxy/schema/invocation.py
 galaxy/schema/item_tags.py
 galaxy/schema/jobs.py
 galaxy/schema/notifications.py
 galaxy/schema/remote_files.py
 galaxy/schema/schema.py
 galaxy/schema/storage_cleaner.py
 galaxy/schema/tasks.py
 galaxy/schema/types.py
 galaxy/schema/visualization.py
+galaxy/schema/workflows.py
 galaxy/schema/bco/__init__.py
 galaxy/schema/bco/description_domain.py
 galaxy/schema/bco/error_domain.py
 galaxy/schema/bco/execution_domain.py
 galaxy/schema/bco/io_domain.py
 galaxy/schema/bco/parametric_domain.py
 galaxy/schema/bco/provenance_domain.py
 galaxy/schema/bco/usability_domain.py
 galaxy/schema/bco/util.py
-galaxy/schema/drs/AccessMethod.py
-galaxy/schema/drs/AccessURL.py
-galaxy/schema/drs/Checksum.py
-galaxy/schema/drs/ContentsObject.py
-galaxy/schema/drs/DrsObject.py
-galaxy/schema/drs/DrsService.py
-galaxy/schema/drs/Error.py
-galaxy/schema/drs/Service.py
 galaxy/schema/drs/__init__.py
 galaxy/schema/workflow/__init__.py
 galaxy/schema/workflow/comments.py
 galaxy_schema.egg-info/PKG-INFO
 galaxy_schema.egg-info/SOURCES.txt
 galaxy_schema.egg-info/dependency_links.txt
 galaxy_schema.egg-info/requires.txt
```

### Comparing `galaxy-schema-23.2.1/setup.cfg` & `galaxy-schema-24.0.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -5,40 +5,41 @@
 	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Intended Audience :: Developers
 	License :: OSI Approved :: Academic Free License (AFL)
 	Natural Language :: English
 	Operating System :: POSIX
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Software Development
 	Topic :: Software Development :: Code Generators
 	Topic :: Software Development :: Testing
 description = Galaxy auth framework and implementations
 keywords = 
 	Galaxy
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-schema
 url = https://github.com/galaxyproject/galaxy
-version = 23.2.1
+version = 24.0.0
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-util
-	pydantic[email]
+	pydantic[email]>=2,!=2.6.0,!=2.6.1
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.packages.find]
 exclude = 
 	tests*
 
 [egg_info]
 tag_build =
```

