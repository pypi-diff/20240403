# Comparing `tmp/rcplus_alloy_common-4.0.3.tar.gz` & `tmp/rcplus_alloy_common-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcplus_alloy_common-4.0.3.tar", max compression
+gzip compressed data, was "rcplus_alloy_common-4.0.4.tar", max compression
```

## Comparing `rcplus_alloy_common-4.0.3.tar` & `rcplus_alloy_common-4.0.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0       77 2024-03-28 13:40:23.614498 rcplus_alloy_common-4.0.3/LICENSE
--rw-r--r--   0        0        0      571 2024-03-28 13:40:23.614498 rcplus_alloy_common-4.0.3/README.md
--rw-r--r--   0        0        0     3017 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/pyproject.toml
--rw-r--r--   0        0        0     2668 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/__init__.py
--rw-r--r--   0        0        0     1072 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/airflow/__init__.py
--rw-r--r--   0        0        0     4256 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/airflow/dag.py
--rw-r--r--   0        0        0     2998 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/airflow/decorators.py
--rw-r--r--   0        0        0      703 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/airflow/hooks.py
--rw-r--r--   0        0        0     8258 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/airflow/locking.py
--rw-r--r--   0        0        0    11749 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/airflow/observability.py
--rw-r--r--   0        0        0    26453 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/airflow/operators.py
--rw-r--r--   0        0        0        0 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/airflow/py.typed
--rw-r--r--   0        0        0     2186 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/airflow/sensors.py
--rw-r--r--   0        0        0     5997 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/airflow/utils.py
--rw-r--r--   0        0        0       98 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/aws/__init__.py
--rw-r--r--   0        0        0     4051 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/aws/dynamodb.py
--rw-r--r--   0        0        0     2720 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/aws/utils.py
--rw-r--r--   0        0        0    12254 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/aws/wr.py
--rw-r--r--   0        0        0     2750 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/aws/wr_utils.py
--rw-r--r--   0        0        0     2475 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/constants.py
--rw-r--r--   0        0        0      710 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/encoder.py
--rw-r--r--   0        0        0      616 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/gam/__init__.py
--rw-r--r--   0        0        0     7223 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/gam/audience.py
--rw-r--r--   0        0        0       80 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/gam/constants.py
--rw-r--r--   0        0        0    10291 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/gam/keyvalues.py
--rw-r--r--   0        0        0        0 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/gam/mock/__init__.py
--rw-r--r--   0        0        0    18267 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/gam/mock/services.py
--rw-r--r--   0        0        0     2170 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/gam/network.py
--rw-r--r--   0        0        0        0 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/gam/py.typed
--rw-r--r--   0        0        0      494 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/gam/utils.py
--rw-r--r--   0        0        0     8397 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/logging.py
--rw-r--r--   0        0        0     6968 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/metrics.py
--rw-r--r--   0        0        0     1250 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/multitenancy.py
--rw-r--r--   0        0        0        0 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/py.typed
--rw-r--r--   0        0        0     3925 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/retry.py
--rw-r--r--   0        0        0       19 2024-03-28 13:40:23.618497 rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/version.py
--rw-r--r--   0        0        0     2181 1970-01-01 00:00:00.000000 rcplus_alloy_common-4.0.3/PKG-INFO
+-rw-r--r--   0        0        0       77 2024-04-03 12:33:51.460947 rcplus_alloy_common-4.0.4/LICENSE
+-rw-r--r--   0        0        0      571 2024-04-03 12:33:51.460947 rcplus_alloy_common-4.0.4/README.md
+-rw-r--r--   0        0        0     3017 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2668 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/__init__.py
+-rw-r--r--   0        0        0     1072 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/__init__.py
+-rw-r--r--   0        0        0     4256 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/dag.py
+-rw-r--r--   0        0        0     2998 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/decorators.py
+-rw-r--r--   0        0        0      703 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/hooks.py
+-rw-r--r--   0        0        0     8258 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/locking.py
+-rw-r--r--   0        0        0    11749 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/observability.py
+-rw-r--r--   0        0        0    26534 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/operators.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/py.typed
+-rw-r--r--   0        0        0     2186 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/sensors.py
+-rw-r--r--   0        0        0     5997 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/utils.py
+-rw-r--r--   0        0        0       98 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/aws/__init__.py
+-rw-r--r--   0        0        0     4051 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/aws/dynamodb.py
+-rw-r--r--   0        0        0     2720 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/aws/utils.py
+-rw-r--r--   0        0        0    12430 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/aws/wr.py
+-rw-r--r--   0        0        0     2750 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/aws/wr_utils.py
+-rw-r--r--   0        0        0     2475 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/constants.py
+-rw-r--r--   0        0        0      710 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/encoder.py
+-rw-r--r--   0        0        0      616 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/gam/__init__.py
+-rw-r--r--   0        0        0     7223 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/gam/audience.py
+-rw-r--r--   0        0        0       80 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/gam/constants.py
+-rw-r--r--   0        0        0    10291 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/gam/keyvalues.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/gam/mock/__init__.py
+-rw-r--r--   0        0        0    18267 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/gam/mock/services.py
+-rw-r--r--   0        0        0     2170 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/gam/network.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/gam/py.typed
+-rw-r--r--   0        0        0      494 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/gam/utils.py
+-rw-r--r--   0        0        0     8397 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/logging.py
+-rw-r--r--   0        0        0     6968 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/metrics.py
+-rw-r--r--   0        0        0     1250 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/multitenancy.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/py.typed
+-rw-r--r--   0        0        0     3925 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/retry.py
+-rw-r--r--   0        0        0       19 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/version.py
+-rw-r--r--   0        0        0     2181 1970-01-01 00:00:00.000000 rcplus_alloy_common-4.0.4/PKG-INFO
```

### Comparing `rcplus_alloy_common-4.0.3/README.md` & `rcplus_alloy_common-4.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # rcplus-alloy-lib-py-common
 
 ![PyPI](https://img.shields.io/pypi/v/rcplus-alloy-common)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rcplus-alloy-common)
 ![Coverage badge](./coverage.svg)
 
-Current version: **v4.0.3**
+Current version: **v4.0.4**
 
 ---
 
 Python utilities for RC+/Alloy.
 
 _**NOTE**_: This Python package is published to PyPI.org as publicly available package.
```

### Comparing `rcplus_alloy_common-4.0.3/pyproject.toml` & `rcplus_alloy_common-4.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 max-args = 11
 
 [tool.ruff.flake8-quotes]
 docstring-quotes = "double"
 
 [tool.poetry]
 name = "rcplus_alloy_common"
-version = "4.0.3"
+version = "4.0.4"
 description = "RC+/Alloy helpers functions for Python"
 readme = "README.md"
 authors = [
     "Ringier AG <info@rcplus.io>",
 ]
 license = "Proprietary"
 repository = "https://github.com/ringier-data/rcplus-alloy-lib-py-common"
```

### Comparing `rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/__init__.py` & `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/__init__.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/airflow/__init__.py` & `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/__init__.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/airflow/dag.py` & `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/dag.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/airflow/decorators.py` & `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/decorators.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/airflow/hooks.py` & `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/hooks.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/airflow/locking.py` & `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/locking.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/airflow/observability.py` & `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/observability.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/airflow/operators.py` & `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,14 @@
         # read the log4j2.properties file from S3 as a template
         s3 = boto3_session.client("s3")
         templ = BytesIO()
         s3.download_fileobj(s3_bucket_name, s3_key_src, templ)
         #
         # inject the extra attributes into the template and upload the result back to S3
         extra_attrs = (
-            f"type=fluentd;"
             f"env={self.project.get('env', 'dev')};"
             f"version={self.project.get('project_version', 'undefined')};"
             f"repository={self.project.get('git_repo_name', 'undefined')};"
             f"software_component={self.project.get('software_component', 'undefined')};"
             f"dag_id={dag_id or 'undefined'};"
             f"dag_run_id={dag_run_id or 'undefined'};"
             f"task_id={self.task_id or 'undefined'};"
@@ -200,52 +199,53 @@
         #   2. `containerOverrides` might not exist
         #   3. the logger sidecar normally has no override in the definition (but it could have)
         #   4. `environment` might not exist
         if "containerOverrides" not in self.overrides:
             self.overrides["containerOverrides"] = []
         primary_container = None
         logging_sidecar = None
+        project_id = self.project.config.get("project_id", "unknown")
         for c in self.overrides["containerOverrides"]:
             # NOTE: the convention is that the primary container is named after the task definition
             if c["name"] == self.task_definition:
                 # NOTE-zw: so far we do not have a reason to inject the logging context into the primary app container!
                 primary_container = c
-            elif c["name"] == "logzio-logs-router":
+            elif c["name"] == f"{project_id}-logs-router":
                 # NOTE-zw: we need to inject the logging context into the logger sidecar because this is where the
                 # fluent-bit runs.
                 logging_sidecar = c
         if primary_container is None:
             if len(self.overrides["containerOverrides"]) > int(logging_sidecar is not None):
                 additional_container_names = [
                     c["name"]
                     for c in self.overrides["containerOverrides"]
-                    if c["name"] not in ["logzio-logs-router", self.task_definition]
+                    if c["name"] not in [f"{project_id}-logs-router", self.task_definition]
                 ]
                 self.log.warning(
                     "containerOverrides contains containers other than "
-                    f"['logzio-logs-router', '{self.task_definition}']: {additional_container_names}"
+                    f"['{project_id}-logs-router', '{self.task_definition}']: {additional_container_names}"
                 )
             primary_container = {
                 "name": self.task_definition,
                 "environment": [],
             }
             self.overrides["containerOverrides"].append(primary_container)
         if logging_sidecar is None:
             if len(self.overrides["containerOverrides"]) > 1:
                 additional_container_names = [
                     c["name"]
                     for c in self.overrides["containerOverrides"]
-                    if c["name"] not in ["logzio-logs-router", self.task_definition]
+                    if c["name"] not in [f"{project_id}-logs-router", self.task_definition]
                 ]
                 self.log.warning(
                     "containerOverrides contains containers other than "
-                    f"['logzio-logs-router', '{self.task_definition}']: {additional_container_names}"
+                    f"['{project_id}-logs-router', '{self.task_definition}']: {additional_container_names}"
                 )
             logging_sidecar = {
-                "name": "logzio-logs-router",
+                "name": f"{project_id}-logs-router",
                 "environment": [],
             }
             self.overrides["containerOverrides"].append(logging_sidecar)
         if "environment" not in logging_sidecar:
             logging_sidecar["environment"] = []
         logging_sidecar["environment"].extend(
             [
```

### Comparing `rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/airflow/sensors.py` & `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/sensors.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/airflow/utils.py` & `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/utils.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/aws/dynamodb.py` & `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/aws/dynamodb.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/aws/utils.py` & `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/aws/utils.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/aws/wr.py` & `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/aws/wr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 from typing import Literal, Iterator, Any, overload
+import logging
 
 import pandas as pd
 import awswrangler as wr
 from awswrangler.athena._utils import _QueryMetadata
 from awswrangler.typing import GlueTableSettings, _S3WriteDataReturnValue
 
 from rcplus_alloy_common.aws.wr_utils import (
@@ -12,14 +13,17 @@
     get_partition_columns_list,
     get_partition_columns_with_type,
     get_sql_columns_with_comments,
     read_table_from_yaml_schema,
 )
 
 
+logger = logging.getLogger(__name__)
+
+
 def get_database() -> str | None:
     database = os.getenv("TENANT", os.getenv("WR_DATABASE", None))
     return database
 
 
 def get_s3_output(workgroup=None) -> str | None:
     tenant = os.getenv("TENANT", None)
@@ -112,14 +116,17 @@
     workgroup: str | None = None,
     wait: bool = False,
     **kwargs,
 ) -> str | dict[str, Any]:
     """s3_output is required in order to ensure we separate tenant specific outputs in different locations"""
     database = database if database is not None else get_database()
     s3_output = s3_output if s3_output is not None else get_s3_output(workgroup=workgroup)
+
+    logger.debug(sql)
+
     return wr.athena.start_query_execution(
         sql=sql,
         database=database,
         s3_output=s3_output,
         workgroup=workgroup,
         wait=wait,
         **kwargs
@@ -356,40 +363,43 @@
     path: str,
     schema_file_path: str,
     database: str,
     s3_output: str | None = None,
     workgroup: str | None = None,
     wait: Literal[True, False] = False,
     skip_path_validation: bool = False,
+    **kwargs,
 ) -> str | dict[str, Any]:
     """Helper to create an iceberg table from a schema file."""
 
     database = database if database is not None else get_database()
     if database is None:
         raise ValueError("Database is not set")
 
     if not skip_path_validation:
         validate_path(table, database, path)
 
     table_schema = read_table_from_yaml_schema(schema_file_path, table)
     columns = get_sql_columns_with_comments(table_schema)
     partition_columns = ", ".join(get_partition_columns_list(table_schema))
 
+    partition_by = f"PARTITIONED BY ({partition_columns})" if partition_columns else ""
     sql = f"""
     CREATE TABLE IF NOT EXISTS {table} (
             {columns})
         COMMENT '{table_schema["description"]}'
-        PARTITIONED BY ({partition_columns})
+        {partition_by}
         LOCATION '{path}'
         TBLPROPERTIES (
                 'format'='parquet',
                 'table_type' ='ICEBERG'
                 )
     """
 
     return start_query_execution(
         sql=sql,
         database=database,
         s3_output=s3_output,
         workgroup=workgroup,
         wait=wait,
+        **kwargs,
     )
```

### Comparing `rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/aws/wr_utils.py` & `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/aws/wr_utils.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/constants.py` & `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/constants.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/encoder.py` & `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/encoder.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/exceptions.py` & `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/exceptions.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/gam/audience.py` & `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/gam/audience.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/gam/keyvalues.py` & `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/gam/keyvalues.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/gam/mock/services.py` & `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/gam/mock/services.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/gam/network.py` & `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/gam/network.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/logging.py` & `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/logging.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/metrics.py` & `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/metrics.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/multitenancy.py` & `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/multitenancy.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.3/src/rcplus_alloy_common/retry.py` & `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/retry.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.3/PKG-INFO` & `rcplus_alloy_common-4.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcplus_alloy_common
-Version: 4.0.3
+Version: 4.0.4
 Summary: RC+/Alloy helpers functions for Python
 Home-page: https://github.com/ringier-data/rcplus-alloy-lib-py-common
 License: Proprietary
 Keywords: rcplus,alloy,logging,metrics,utilities
 Author: Ringier AG
 Author-email: info@rcplus.io
 Requires-Python: >=3.10,<4
@@ -37,15 +37,15 @@
 
 # rcplus-alloy-lib-py-common
 
 ![PyPI](https://img.shields.io/pypi/v/rcplus-alloy-common)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rcplus-alloy-common)
 ![Coverage badge](./coverage.svg)
 
-Current version: **v4.0.3**
+Current version: **v4.0.4**
 
 ---
 
 Python utilities for RC+/Alloy.
 
 _**NOTE**_: This Python package is published to PyPI.org as publicly available package.
```

