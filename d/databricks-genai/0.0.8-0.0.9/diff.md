# Comparing `tmp/databricks-genai-0.0.8.tar.gz` & `tmp/databricks-genai-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks-genai-0.0.8.tar", last modified: Wed Jan 24 20:42:31 2024, max compression
+gzip compressed data, was "databricks-genai-0.0.9.tar", last modified: Thu Feb  8 04:31:54 2024, max compression
```

## Comparing `databricks-genai-0.0.8.tar` & `databricks-genai-0.0.9.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-01-24 20:42:31.796906 databricks-genai-0.0.8/
--rw-r--r--   0 nancy.hung   (502) staff       (20)     1381 2024-01-24 20:42:31.796589 databricks-genai-0.0.8/PKG-INFO
--rw-r--r--   0 nancy.hung   (502) staff       (20)      273 2024-01-15 20:03:23.000000 databricks-genai-0.0.8/README.md
-drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-01-24 20:42:31.789388 databricks-genai-0.0.8/databricks_genai/
--rw-r--r--   0 nancy.hung   (502) staff       (20)      181 2024-01-15 20:03:23.000000 databricks-genai-0.0.8/databricks_genai/__init__.py
-drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-01-24 20:42:31.791254 databricks-genai-0.0.8/databricks_genai/api/
--rw-r--r--   0 nancy.hung   (502) staff       (20)        0 2023-12-08 18:20:10.000000 databricks-genai-0.0.8/databricks_genai/api/__init__.py
--rw-r--r--   0 nancy.hung   (502) staff       (20)     2676 2024-01-15 20:03:23.000000 databricks-genai-0.0.8/databricks_genai/api/config.py
-drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-01-24 20:42:31.793630 databricks-genai-0.0.8/databricks_genai/api/finetuning/
--rw-r--r--   0 nancy.hung   (502) staff       (20)      325 2024-01-15 20:03:23.000000 databricks-genai-0.0.8/databricks_genai/api/finetuning/__init__.py
--rw-r--r--   0 nancy.hung   (502) staff       (20)     1336 2024-01-24 20:40:46.000000 databricks-genai-0.0.8/databricks_genai/api/finetuning/cancel.py
--rw-r--r--   0 nancy.hung   (502) staff       (20)     6259 2024-01-24 20:40:46.000000 databricks-genai-0.0.8/databricks_genai/api/finetuning/create.py
--rw-r--r--   0 nancy.hung   (502) staff       (20)     1060 2024-01-15 20:03:23.000000 databricks-genai-0.0.8/databricks_genai/api/finetuning/delete.py
--rw-r--r--   0 nancy.hung   (502) staff       (20)     1022 2024-01-15 20:03:23.000000 databricks-genai-0.0.8/databricks_genai/api/finetuning/get.py
--rw-r--r--   0 nancy.hung   (502) staff       (20)      866 2024-01-15 20:03:23.000000 databricks-genai-0.0.8/databricks_genai/api/finetuning/get_events.py
--rw-r--r--   0 nancy.hung   (502) staff       (20)     1738 2024-01-15 20:04:36.000000 databricks-genai-0.0.8/databricks_genai/api/finetuning/list.py
--rw-r--r--   0 nancy.hung   (502) staff       (20)     8502 2024-01-24 20:40:46.000000 databricks-genai-0.0.8/databricks_genai/api/finetuning/utils.py
--rw-r--r--   0 nancy.hung   (502) staff       (20)      782 2024-01-15 20:03:23.000000 databricks-genai-0.0.8/databricks_genai/errors.py
-drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-01-24 20:42:31.794332 databricks-genai-0.0.8/databricks_genai/types/
--rw-r--r--   0 nancy.hung   (502) staff       (20)      106 2024-01-15 20:03:23.000000 databricks-genai-0.0.8/databricks_genai/types/__init__.py
--rw-r--r--   0 nancy.hung   (502) staff       (20)     2542 2024-01-15 20:03:23.000000 databricks-genai-0.0.8/databricks_genai/types/common.py
-drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-01-24 20:42:31.794849 databricks-genai-0.0.8/databricks_genai/types/finetuning/
--rw-r--r--   0 nancy.hung   (502) staff       (20)      143 2024-01-15 20:03:23.000000 databricks-genai-0.0.8/databricks_genai/types/finetuning/__init__.py
--rw-r--r--   0 nancy.hung   (502) staff       (20)     5380 2024-01-24 20:40:46.000000 databricks-genai-0.0.8/databricks_genai/types/finetuning/finetuning_run.py
--rw-r--r--   0 nancy.hung   (502) staff       (20)       53 2024-01-24 20:41:00.000000 databricks-genai-0.0.8/databricks_genai/version.py
-drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-01-24 20:42:31.795666 databricks-genai-0.0.8/databricks_genai.egg-info/
--rw-r--r--   0 nancy.hung   (502) staff       (20)     1381 2024-01-24 20:42:31.000000 databricks-genai-0.0.8/databricks_genai.egg-info/PKG-INFO
--rw-r--r--   0 nancy.hung   (502) staff       (20)      904 2024-01-24 20:42:31.000000 databricks-genai-0.0.8/databricks_genai.egg-info/SOURCES.txt
--rw-r--r--   0 nancy.hung   (502) staff       (20)        1 2024-01-24 20:42:31.000000 databricks-genai-0.0.8/databricks_genai.egg-info/dependency_links.txt
--rw-r--r--   0 nancy.hung   (502) staff       (20)      291 2024-01-24 20:42:31.000000 databricks-genai-0.0.8/databricks_genai.egg-info/requires.txt
--rw-r--r--   0 nancy.hung   (502) staff       (20)       17 2024-01-24 20:42:31.000000 databricks-genai-0.0.8/databricks_genai.egg-info/top_level.txt
--rw-r--r--   0 nancy.hung   (502) staff       (20)    31194 2024-01-15 20:03:23.000000 databricks-genai-0.0.8/pyproject.toml
--rw-r--r--   0 nancy.hung   (502) staff       (20)       38 2024-01-24 20:42:31.796978 databricks-genai-0.0.8/setup.cfg
--rw-r--r--   0 nancy.hung   (502) staff       (20)     1591 2024-01-24 20:40:46.000000 databricks-genai-0.0.8/setup.py
-drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-01-24 20:42:31.795133 databricks-genai-0.0.8/tests/
--rw-r--r--   0 nancy.hung   (502) staff       (20)      332 2024-01-15 20:03:23.000000 databricks-genai-0.0.8/tests/test_package.py
+drwxr-xr-x   0 nicholas.garcia   (502) staff       (20)        0 2024-02-08 04:31:54.391224 databricks-genai-0.0.9/
+-rw-r--r--   0 nicholas.garcia   (502) staff       (20)     1381 2024-02-08 04:31:54.390932 databricks-genai-0.0.9/PKG-INFO
+-rw-r--r--   0 nicholas.garcia   (502) staff       (20)      273 2024-01-09 18:19:25.000000 databricks-genai-0.0.9/README.md
+drwxr-xr-x   0 nicholas.garcia   (502) staff       (20)        0 2024-02-08 04:31:54.381879 databricks-genai-0.0.9/databricks_genai/
+-rw-r--r--   0 nicholas.garcia   (502) staff       (20)      181 2024-01-09 18:19:25.000000 databricks-genai-0.0.9/databricks_genai/__init__.py
+drwxr-xr-x   0 nicholas.garcia   (502) staff       (20)        0 2024-02-08 04:31:54.383660 databricks-genai-0.0.9/databricks_genai/api/
+-rw-r--r--   0 nicholas.garcia   (502) staff       (20)        0 2024-01-09 18:19:25.000000 databricks-genai-0.0.9/databricks_genai/api/__init__.py
+-rw-r--r--   0 nicholas.garcia   (502) staff       (20)     2695 2024-02-08 04:30:05.000000 databricks-genai-0.0.9/databricks_genai/api/config.py
+drwxr-xr-x   0 nicholas.garcia   (502) staff       (20)        0 2024-02-08 04:31:54.386563 databricks-genai-0.0.9/databricks_genai/api/finetuning/
+-rw-r--r--   0 nicholas.garcia   (502) staff       (20)      325 2024-01-09 18:19:25.000000 databricks-genai-0.0.9/databricks_genai/api/finetuning/__init__.py
+-rw-r--r--   0 nicholas.garcia   (502) staff       (20)     2700 2024-02-08 04:30:05.000000 databricks-genai-0.0.9/databricks_genai/api/finetuning/cancel.py
+-rw-r--r--   0 nicholas.garcia   (502) staff       (20)     7588 2024-02-08 04:30:05.000000 databricks-genai-0.0.9/databricks_genai/api/finetuning/create.py
+-rw-r--r--   0 nicholas.garcia   (502) staff       (20)     3498 2024-02-08 04:30:05.000000 databricks-genai-0.0.9/databricks_genai/api/finetuning/delete.py
+-rw-r--r--   0 nicholas.garcia   (502) staff       (20)     1048 2024-02-08 04:30:05.000000 databricks-genai-0.0.9/databricks_genai/api/finetuning/get.py
+-rw-r--r--   0 nicholas.garcia   (502) staff       (20)     1646 2024-02-08 04:30:05.000000 databricks-genai-0.0.9/databricks_genai/api/finetuning/get_events.py
+-rw-r--r--   0 nicholas.garcia   (502) staff       (20)     5447 2024-02-08 04:30:05.000000 databricks-genai-0.0.9/databricks_genai/api/finetuning/list.py
+-rw-r--r--   0 nicholas.garcia   (502) staff       (20)    12245 2024-02-08 04:30:05.000000 databricks-genai-0.0.9/databricks_genai/api/finetuning/utils.py
+-rw-r--r--   0 nicholas.garcia   (502) staff       (20)      782 2024-01-09 18:19:25.000000 databricks-genai-0.0.9/databricks_genai/errors.py
+drwxr-xr-x   0 nicholas.garcia   (502) staff       (20)        0 2024-02-08 04:31:54.388023 databricks-genai-0.0.9/databricks_genai/types/
+-rw-r--r--   0 nicholas.garcia   (502) staff       (20)      106 2024-01-09 18:19:25.000000 databricks-genai-0.0.9/databricks_genai/types/__init__.py
+-rw-r--r--   0 nicholas.garcia   (502) staff       (20)     3836 2024-02-08 04:30:05.000000 databricks-genai-0.0.9/databricks_genai/types/common.py
+drwxr-xr-x   0 nicholas.garcia   (502) staff       (20)        0 2024-02-08 04:31:54.389059 databricks-genai-0.0.9/databricks_genai/types/finetuning/
+-rw-r--r--   0 nicholas.garcia   (502) staff       (20)      143 2024-01-09 18:19:25.000000 databricks-genai-0.0.9/databricks_genai/types/finetuning/__init__.py
+-rw-r--r--   0 nicholas.garcia   (502) staff       (20)     5958 2024-02-08 04:30:05.000000 databricks-genai-0.0.9/databricks_genai/types/finetuning/finetune_config.py
+-rw-r--r--   0 nicholas.garcia   (502) staff       (20)     8518 2024-02-08 04:30:05.000000 databricks-genai-0.0.9/databricks_genai/types/finetuning/finetuning_run.py
+-rw-r--r--   0 nicholas.garcia   (502) staff       (20)      936 2024-02-08 04:30:05.000000 databricks-genai-0.0.9/databricks_genai/types/run_event.py
+-rw-r--r--   0 nicholas.garcia   (502) staff       (20)     5255 2024-02-08 04:30:05.000000 databricks-genai-0.0.9/databricks_genai/types/run_status.py
+-rw-r--r--   0 nicholas.garcia   (502) staff       (20)       53 2024-02-08 04:30:17.000000 databricks-genai-0.0.9/databricks_genai/version.py
+drwxr-xr-x   0 nicholas.garcia   (502) staff       (20)        0 2024-02-08 04:31:54.390064 databricks-genai-0.0.9/databricks_genai.egg-info/
+-rw-r--r--   0 nicholas.garcia   (502) staff       (20)     1381 2024-02-08 04:31:54.000000 databricks-genai-0.0.9/databricks_genai.egg-info/PKG-INFO
+-rw-r--r--   0 nicholas.garcia   (502) staff       (20)     1030 2024-02-08 04:31:54.000000 databricks-genai-0.0.9/databricks_genai.egg-info/SOURCES.txt
+-rw-r--r--   0 nicholas.garcia   (502) staff       (20)        1 2024-02-08 04:31:54.000000 databricks-genai-0.0.9/databricks_genai.egg-info/dependency_links.txt
+-rw-r--r--   0 nicholas.garcia   (502) staff       (20)      291 2024-02-08 04:31:54.000000 databricks-genai-0.0.9/databricks_genai.egg-info/requires.txt
+-rw-r--r--   0 nicholas.garcia   (502) staff       (20)       17 2024-02-08 04:31:54.000000 databricks-genai-0.0.9/databricks_genai.egg-info/top_level.txt
+-rw-r--r--   0 nicholas.garcia   (502) staff       (20)    31194 2024-01-09 18:19:25.000000 databricks-genai-0.0.9/pyproject.toml
+-rw-r--r--   0 nicholas.garcia   (502) staff       (20)       38 2024-02-08 04:31:54.391274 databricks-genai-0.0.9/setup.cfg
+-rw-r--r--   0 nicholas.garcia   (502) staff       (20)     1591 2024-02-08 04:30:05.000000 databricks-genai-0.0.9/setup.py
+drwxr-xr-x   0 nicholas.garcia   (502) staff       (20)        0 2024-02-08 04:31:54.389483 databricks-genai-0.0.9/tests/
+-rw-r--r--   0 nicholas.garcia   (502) staff       (20)      332 2024-01-09 18:19:25.000000 databricks-genai-0.0.9/tests/test_package.py
```

### Comparing `databricks-genai-0.0.8/PKG-INFO` & `databricks-genai-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: databricks-genai
-Version: 0.0.8
+Version: 0.0.9
 Summary: Interact with the Databricks Generative AI APIs in python
 Home-page: https://docs.mosaicml.com/projects/mcli/en/latest/finetuning/finetuning.html
 Author: Databricks
 Author-email: genai-eng-team@databricks.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Requires-Dist: databricks-sdk>=0.14.0
 Requires-Dist: typing_extensions>=4.7.1
-Requires-Dist: mosaicml-cli==0.6.2
+Requires-Dist: mosaicml-cli==0.6.5
 Requires-Dist: datasets>=2.16.1
 Requires-Dist: mlflow>=2.9.2
 Provides-Extra: dev
 Requires-Dist: isort>=5.9.3; extra == "dev"
 Requires-Dist: packaging<23,>=21; extra == "dev"
 Requires-Dist: pylint>=3.0.0; extra == "dev"
 Requires-Dist: pyright==1.1.256; extra == "dev"
 Requires-Dist: pytest>=7.4.0; extra == "dev"
 Requires-Dist: yapf>=0.40.0; extra == "dev"
 Provides-Extra: all
-Requires-Dist: pylint>=3.0.0; extra == "all"
 Requires-Dist: pyright==1.1.256; extra == "all"
-Requires-Dist: packaging<23,>=21; extra == "all"
 Requires-Dist: isort>=5.9.3; extra == "all"
-Requires-Dist: pytest>=7.4.0; extra == "all"
 Requires-Dist: yapf>=0.40.0; extra == "all"
+Requires-Dist: pytest>=7.4.0; extra == "all"
+Requires-Dist: packaging<23,>=21; extra == "all"
+Requires-Dist: pylint>=3.0.0; extra == "all"
```

### Comparing `databricks-genai-0.0.8/databricks_genai/api/config.py` & `databricks-genai-0.0.9/databricks_genai/api/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,8 +83,8 @@
         if previous_api_key:
             os.environ[config.MOSAICML_API_KEY_ENV] = previous_api_key
         if previous_endpoint:
             os.environ[config.MOSAICML_API_ENDPOINT_ENV] = previous_endpoint
 
         return res
 
-    return setup
+    return setup  # pyright: ignore
```

### Comparing `databricks-genai-0.0.8/databricks_genai/api/finetuning/create.py` & `databricks-genai-0.0.9/databricks_genai/api/finetuning/create.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,53 @@
 """Create a finetuning run"""
 
-from typing import List, Optional
+from typing import Dict, List, Optional, Union
 
-from mcli.api.finetuning_runs.api_create_finetuning_run import _db_create_finetuning_run
+from mcli.api.engine.engine import get_return_response, run_singular_mapi_request
 
 from databricks_genai.api.config import configure_request, get_me
-from databricks_genai.api.finetuning.utils import format_path, is_cluster_sql, validate_create_finetuning_run_inputs
+from databricks_genai.api.finetuning.utils import (SAVE_FOLDER_PATH, format_path, is_cluster_sql,
+                                                   validate_create_finetuning_run_inputs)
 from databricks_genai.types.finetuning import FinetuningRun
+from databricks_genai.types.finetuning.finetune_config import FinetuneConfig
+
+QUERY_FUNCTION = 'createFinetune'
+VARIABLE_DATA_NAME = 'createFinetuneData'
+# This returns the same data that the create_run function returns
+# for consistency when rendering the describe output
+QUERY = f"""
+mutation CreateFinetune(${VARIABLE_DATA_NAME}: CreateFinetuneInput!) {{
+  {QUERY_FUNCTION}({VARIABLE_DATA_NAME}: ${VARIABLE_DATA_NAME}) {{
+    id
+    name
+    status
+    createdById
+    createdByEmail
+    createdAt
+    updatedAt
+    startedAt
+    completedAt
+    reason
+    isDeleted
+    details {{
+        model
+        taskType
+        trainDataPath
+        saveFolder
+        evalDataPath
+        evalPrompts
+        trainingDuration
+        learningRate
+        contextLength
+        dataPrepConfig
+        experimentTracker
+        customWeightsPath
+    }}
+  }}
+}}"""
 
 
 @configure_request
 def create(
     model: str,
     train_data_path: str,
     register_to: str,
@@ -84,40 +121,54 @@
         'mlflow': {
             'experiment_path': f'/Users/{databricks_username}/{experiment_path}',
             'model_registry_path': register_to,
         }
     }
 
     train_data_path = format_path(train_data_path)
-    eval_data_path = format_path(eval_data_path)
-    custom_weights_path = format_path(custom_weights_path)
-    save_folder = 'dbfs:/databricks/mlflow-tracking/{mlflow_experiment_id}/{mlflow_run_id}/artifacts'
+    if eval_data_path is not None:
+        eval_data_path = format_path(eval_data_path)
+    if custom_weights_path is not None:
+        custom_weights_path = format_path(custom_weights_path)
+    save_folder = SAVE_FOLDER_PATH
     if validate_inputs:
         # don't validate experiment path if it's the default
         # TODO: create FinetuneConfig object for this SDK, so we can pass in object
         # instead of a list of params in the next line
         experiment_path_to_validate = experiment_tracker['mlflow'][
             'experiment_path'] if experiment_path != "{}" else None
         validate_create_finetuning_run_inputs(train_data_path, register_to, experiment_path_to_validate, eval_data_path,
-                                              data_prep_cluster_id)
-    data_prep_config = None
+                                              data_prep_cluster_id, custom_weights_path)
+    data_prep_config: Optional[Dict[str, Union[str, bool]]] = None
     # TODO: add translations for snake to camel case
     if data_prep_cluster_id is not None:
         data_prep_config = {'clusterId': data_prep_cluster_id}
         if is_cluster_sql(data_prep_cluster_id):
             data_prep_config['useSql'] = True
-    return FinetuningRun.from_mcli(
-        _db_create_finetuning_run(
-            model=model,
-            train_data_path=train_data_path,
-            task_type=task_type,
-            eval_data_path=eval_data_path,
-            eval_prompts=eval_prompts,
-            data_prep_config=data_prep_config,
-            custom_weights_path=custom_weights_path,
-            training_duration=training_duration,
-            learning_rate=learning_rate,
-            context_length=context_length,
-            save_folder=save_folder,
-            experiment_tracker=experiment_tracker,
-            disable_credentials_check=True,
-        ))
+
+    config = FinetuneConfig.from_dict({
+        'model': model,
+        'task_type': task_type,
+        'train_data_path': train_data_path,
+        'save_folder': save_folder,
+        'eval_data_path': eval_data_path,
+        'eval_prompts': eval_prompts,
+        'training_duration': training_duration,
+        'experiment_tracker': experiment_tracker,
+        'learning_rate': learning_rate,
+        'context_length': context_length,
+        'custom_weights_path': custom_weights_path,
+        'data_prep_config': data_prep_config,
+        'disable_credentials_check': not validate_inputs,
+    })
+    finetune_config = config.to_create_finetune_api_input()
+    variables = {
+        VARIABLE_DATA_NAME: finetune_config,
+    }
+
+    response = run_singular_mapi_request(
+        query=QUERY,
+        query_function=QUERY_FUNCTION,
+        return_model_type=FinetuningRun,
+        variables=variables,
+    )
+    return get_return_response(response)
```

### Comparing `databricks-genai-0.0.8/databricks_genai/api/finetuning/get.py` & `databricks-genai-0.0.9/databricks_genai/api/finetuning/get.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Get finetuning runs"""
 
 from typing import Union
 
-from mcli import get_finetuning_runs
-
 from databricks_genai.api.config import configure_request
+from databricks_genai.api.finetuning.list import get_finetuning_runs_paginated
 from databricks_genai.errors import DatabricksGenAIResponseError
 from databricks_genai.types.finetuning import FinetuningRun
 
 
 @configure_request
 def get(finetuning_run: Union[str, FinetuningRun]) -> FinetuningRun:
     """Get a single finetuning run by name or run object
@@ -16,17 +15,17 @@
     Args:
         finetuning_run (Union[str, FinetuningRun]): The finetuning run to get.
     
     Returns:
         FinetuningRun: The finetuning run
     """
     finetuning_runs = [finetuning_run] if isinstance(finetuning_run, str) else [finetuning_run.name]
-    run = get_finetuning_runs(
+    run = get_finetuning_runs_paginated(
         finetuning_runs=finetuning_runs,
         include_details=True,
     )
 
     if not run:
         name = finetuning_run if isinstance(finetuning_run, str) else finetuning_run.name
         raise DatabricksGenAIResponseError(f'Finetuning run {name} not found')
 
-    return FinetuningRun.from_mcli(run[0])
+    return run[0]
```

### Comparing `databricks-genai-0.0.8/databricks_genai/errors.py` & `databricks-genai-0.0.9/databricks_genai/errors.py`

 * *Files identical despite different names*

### Comparing `databricks-genai-0.0.8/databricks_genai/types/finetuning/finetuning_run.py` & `databricks-genai-0.0.9/databricks_genai/api/finetuning/list.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,174 +1,161 @@
-"""
-A Databricks finetuning run
-"""
+"""List multiple finetuning runs"""
 
-from dataclasses import dataclass
 from datetime import datetime
-from typing import Any, Dict, List, Optional
+from typing import List, Optional, Union
 
-from mcli import Finetune as McliFinetune
-from mcli.api.model.run_event import FormattedRunEvent as McliFinetuneEvent
-from mcli.utils.utils_run_status import RunStatus
+from mcli.api.engine.engine import get_return_response, run_paginated_mapi_request
+from mcli.config import MCLIConfig
 
-from databricks_genai.types.common import Object
-
-
-@dataclass
-class FinetuningEvent(Object):
-    """
-    An event that occurs during a finetuning run
-
-    Args:
-        type: The type of event
-        time: The time the event occurred
-        message: The message associated with the event
+from databricks_genai.api.config import configure_request
+from databricks_genai.types.common import ObjectList
+from databricks_genai.types.finetuning import FinetuningRun
+from databricks_genai.types.run_status import RunStatus
+
+QUERY_FUNCTION = 'getFinetunesPaginated'
+VARIABLE_DATA_NAME = 'getFinetunesPaginatedData'
+
+QUERY = f"""
+query GetFinetunesPaginated(${VARIABLE_DATA_NAME}: GetFinetunesPaginatedInput!) {{
+  {QUERY_FUNCTION}({VARIABLE_DATA_NAME}: ${VARIABLE_DATA_NAME}) {{
+    cursor
+    hasNextPage
+    finetunes {{
+        id
+        name
+        status
+        createdById
+        createdByEmail
+        createdAt
+        updatedAt
+        startedAt
+        completedAt
+        reason
+        estimatedEndTime
+        isDeleted
+    }}
+  }}
+}}"""
+
+QUERY_WITH_DETAILS_DB = f"""
+query GetFinetunesPaginated(${VARIABLE_DATA_NAME}: GetFinetunesPaginatedInput!) {{
+  {QUERY_FUNCTION}({VARIABLE_DATA_NAME}: ${VARIABLE_DATA_NAME}) {{
+    cursor
+    hasNextPage
+    finetunes {{
+        id
+        name
+        status
+        createdById
+        createdByEmail
+        createdAt
+        updatedAt
+        startedAt
+        completedAt
+        reason
+        estimatedEndTime
+        isDeleted
+        details {{
+            model
+            taskType
+            trainDataPath
+            saveFolder
+            evalDataPath
+            evalPrompts
+            trainingDuration
+            learningRate
+            contextLength
+            experimentTracker
+            customWeightsPath
+            dataPrepConfig
+            formattedFinetuningEvents {{
+                eventType
+                eventTime
+                eventMessage    
+            }}
+        }}
+    }}
+  }}
+}}"""
+
+
+@configure_request
+def list(  # pylint: disable=redefined-builtin
+    finetuning_runs: Optional[Union[List[str], List[FinetuningRun], ObjectList[FinetuningRun]]] = None,
+    *,
+    statuses: Optional[Union[List[str], List[RunStatus]]] = None,
+    user_emails: Optional[List[str]] = None,
+    before: Optional[Union[str, datetime]] = None,
+    after: Optional[Union[str, datetime]] = None,
+    limit: Optional[int] = None,
+):
+    """ 
+    Internal db get finetuning runs to include dataPrepConfig in details.
     """
-
-    type: str
-    time: datetime
-    message: str
-
-    @classmethod
-    def from_mcli(cls, obj: McliFinetuneEvent) -> 'FinetuningEvent':
-        return cls(
-            type=obj.event_type,
-            time=obj.event_time,
-            message=obj.event_message,
-        )
-
-    def _get_display_columns(self) -> Dict[str, str]:
-        return {
-            'type': 'Type',
-            'time': 'Time',
-            'message': 'Message',
-        }
-
-
-@dataclass
-class FinetuningRun:
-    """A Databricks finetuning run
+    return get_finetuning_runs_paginated(finetuning_runs=finetuning_runs,
+                                         statuses=statuses,
+                                         user_emails=user_emails,
+                                         before=before,
+                                         after=after,
+                                         limit=limit)
+
+
+def get_finetuning_runs_paginated(
+    finetuning_runs: Optional[Union[List[str], List[FinetuningRun], ObjectList[FinetuningRun]]] = None,
+    *,
+    statuses: Optional[Union[List[str], List[RunStatus]]] = None,
+    user_emails: Optional[List[str]] = None,
+    before: Optional[Union[str, datetime]] = None,
+    after: Optional[Union[str, datetime]] = None,
+    include_details: bool = False,
+    limit: Optional[int] = None,
+) -> List[FinetuningRun]:
+    """List finetuning runs
     
     Args:
-        name: The name of the finetuning run
-        created_by: The user email of who created the run
-        model: The model to finetune
-        train_data_path: The path to the training data
-        register_to: The location to the registered model
-        experiment_path: The path to save the MLflow experiment
-        created_at: The time the run was created
-        started_at: The time the run was started
-        estimated_end_time: The estimated time the run will complete
-        completed_at: The time the run was completed
+        finetuning_runs (Optional[Union[List[str], List[FinetuningRun], ObjectList[FinetuningRun]]], optional): 
+        The finetuning runs to list. Defaults to None.
+        statuses (Optional[Union[List[str], List[RunStatus]], optional): The statuses to filter by. Defaults to None.
+        user_emails (Optional[List[str]], optional): The user emails to filter by. Defaults to None.
+        before (Optional[Union[str, datetime]], optional): The date to filter before. Defaults to None.
+        after (Optional[Union[str, datetime]], optional): The date to filter after. Defaults to None.
+        limit (Optional[int], optional): The maximum number of runs to return. Defaults to None.
+    
+    Returns:
+        ObjectList[FinetuningRun]: A list of finetuning runs
     """
-
-    name: str
-    status: RunStatus
-    created_by: str
-
-    # User inputs
-    model: str
-    train_data_path: str
-    register_to: str
-    experiment_path: Optional[str] = None
-    data_prep_config: Optional[Dict[str, str]] = None
-
-    # Lifecycle
-    created_at: Optional[datetime] = None
-    started_at: Optional[datetime] = None
-    estimated_end_time: Optional[datetime] = None
-    completed_at: Optional[datetime] = None
-
-    # hyperparameters: Hyperparameters ## todo
-
-    @property
-    def submitted_config(self) -> Dict[str, Any]:
-        """The config originally submitted to the API to create this run"""
-        return {
-            'model': self.model,
-            'train_data_path': self.train_data_path,
-            'register_to': self.register_to,
-            'experiment_path': self.experiment_path,
-            # TODO: add the other inputs from create here
-        }
-
-    def _get_display_columns(self) -> Dict[str, str]:
-        return {
-            'name': 'Name',
-            'status': 'Status',
-            'created_by': 'Created By',
-            'model': 'Model',
-        }
-
-    @classmethod
-    def from_mcli(
-        cls,
-        obj: McliFinetune,
-    ) -> 'FinetuningRun':
-
-        # TODO: These should be top level properties, for now pull from the original yaml
-        submitted_config = obj.submitted_config
-        mlflow_tracker = submitted_config.experiment_tracker["mlflow"]
-        # The experiment path is auto-formatted to be '/Users/username/experiment_path'
-        _, _, _, *experiment_path = mlflow_tracker['experiment_path'].split('/')
-        experiment_path = '/'.join(experiment_path)
-        register_to = mlflow_tracker.get('model_registry_path')
-
-        return cls(
-            name=obj.name,
-            status=obj.status,
-            created_by=obj.created_by,
-            model=obj.model,
-            train_data_path=obj.train_data_path,
-            register_to=register_to,
-            experiment_path=experiment_path,
-            data_prep_config=submitted_config.data_prep_config,
-            created_at=obj.created_at,
-            started_at=obj.started_at,
-            completed_at=obj.completed_at,
-            estimated_end_time=obj.estimated_end_time,
-        )
-
-    def refresh(self) -> 'FinetuningRun':
-        """Refetches the finetuning run from the API
-
-        Returns:
-            FinetuningRun: The updated finetuning run
-        """
-
-        # pylint: disable=import-outside-toplevel, cyclic-import
-        from databricks_genai.api.finetuning.get import get
-        return get(self)
-
-    def cancel(self) -> int:
-        """Cancel the finetuning run
-        
-        Returns:
-            int: Will return 1 if the run was cancelled, 0 if it was already cancelled
-        """
-
-        # pylint: disable=import-outside-toplevel, cyclic-import
-        from databricks_genai.api.finetuning.cancel import cancel
-        return cancel(self)
-
-    def delete(self) -> int:
-        """Delete the finetuning run
-        
-        Returns:
-            int: Will return 1 if the run was deleted, 0 if it was already deleted
-        """
-
-        # pylint: disable=import-outside-toplevel, cyclic-import
-        from databricks_genai.api.finetuning.delete import delete
-        return delete(self)
-
-    def get_events(self) -> List[FinetuningEvent]:
-        """Get events for the finetuning run
-        
-        Returns:
-            List[FinetuningEvent]: A list of finetuning events. Each event has an event 
-                type, time, and message.
-        """
-
-        # pylint: disable=import-outside-toplevel, cyclic-import
-        from databricks_genai.api.finetuning.get_events import get_events
-        return get_events(self)
+    filters = {}
+    if finetuning_runs:
+        filters['name'] = {'in': [r.name if isinstance(r, FinetuningRun) else r for r in finetuning_runs]}
+    if statuses:
+        filters['status'] = {'in': [s.value if isinstance(s, RunStatus) else s for s in statuses]}
+    if before or after:
+        date_filters = {}
+        if before:
+            date_filters['lt'] = before.astimezone().isoformat() if isinstance(before, datetime) else before
+        if after:
+            date_filters['gte'] = after.astimezone().isoformat() if isinstance(after, datetime) else after
+        filters['createdAt'] = date_filters
+
+    variables = {
+        VARIABLE_DATA_NAME: {
+            'filters': filters,
+            'includeDeleted': False,
+            'limit': limit,
+        },
+    }
+
+    cfg = MCLIConfig.load_config()
+    cfg.update_entity(variables[VARIABLE_DATA_NAME])
+    if user_emails:
+        if variables[VARIABLE_DATA_NAME].get('entity'):
+            variables[VARIABLE_DATA_NAME]['entity']['emails'] = user_emails
+        else:
+            variables[VARIABLE_DATA_NAME]['entity'] = {'emails': user_emails}
+
+    response = run_paginated_mapi_request(
+        query=QUERY_WITH_DETAILS_DB if include_details else QUERY,
+        query_function=QUERY_FUNCTION,
+        return_model_type=FinetuningRun,
+        variables=variables,
+    )
+    return get_return_response(response)
```

### Comparing `databricks-genai-0.0.8/databricks_genai.egg-info/PKG-INFO` & `databricks-genai-0.0.9/databricks_genai.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: databricks-genai
-Version: 0.0.8
+Version: 0.0.9
 Summary: Interact with the Databricks Generative AI APIs in python
 Home-page: https://docs.mosaicml.com/projects/mcli/en/latest/finetuning/finetuning.html
 Author: Databricks
 Author-email: genai-eng-team@databricks.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Requires-Dist: databricks-sdk>=0.14.0
 Requires-Dist: typing_extensions>=4.7.1
-Requires-Dist: mosaicml-cli==0.6.2
+Requires-Dist: mosaicml-cli==0.6.5
 Requires-Dist: datasets>=2.16.1
 Requires-Dist: mlflow>=2.9.2
 Provides-Extra: dev
 Requires-Dist: isort>=5.9.3; extra == "dev"
 Requires-Dist: packaging<23,>=21; extra == "dev"
 Requires-Dist: pylint>=3.0.0; extra == "dev"
 Requires-Dist: pyright==1.1.256; extra == "dev"
 Requires-Dist: pytest>=7.4.0; extra == "dev"
 Requires-Dist: yapf>=0.40.0; extra == "dev"
 Provides-Extra: all
-Requires-Dist: pylint>=3.0.0; extra == "all"
 Requires-Dist: pyright==1.1.256; extra == "all"
-Requires-Dist: packaging<23,>=21; extra == "all"
 Requires-Dist: isort>=5.9.3; extra == "all"
-Requires-Dist: pytest>=7.4.0; extra == "all"
 Requires-Dist: yapf>=0.40.0; extra == "all"
+Requires-Dist: pytest>=7.4.0; extra == "all"
+Requires-Dist: packaging<23,>=21; extra == "all"
+Requires-Dist: pylint>=3.0.0; extra == "all"
```

### Comparing `databricks-genai-0.0.8/databricks_genai.egg-info/SOURCES.txt` & `databricks-genai-0.0.9/databricks_genai.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -17,10 +17,13 @@
 databricks_genai/api/finetuning/delete.py
 databricks_genai/api/finetuning/get.py
 databricks_genai/api/finetuning/get_events.py
 databricks_genai/api/finetuning/list.py
 databricks_genai/api/finetuning/utils.py
 databricks_genai/types/__init__.py
 databricks_genai/types/common.py
+databricks_genai/types/run_event.py
+databricks_genai/types/run_status.py
 databricks_genai/types/finetuning/__init__.py
+databricks_genai/types/finetuning/finetune_config.py
 databricks_genai/types/finetuning/finetuning_run.py
 tests/test_package.py
```

### Comparing `databricks-genai-0.0.8/pyproject.toml` & `databricks-genai-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `databricks-genai-0.0.8/setup.py` & `databricks-genai-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # pylint: disable-next=exec-used,consider-using-with
 exec(open('databricks_genai/version.py', 'r', encoding='utf-8').read())
 
 install_requires = [
     'databricks-sdk>=0.14.0',
     'typing_extensions>=4.7.1',
-    'mosaicml-cli==0.6.2',
+    'mosaicml-cli==0.6.5',
     'datasets>=2.16.1',
     'mlflow>=2.9.2'
 ]
 
 extra_deps = {}
 
 extra_deps['dev'] = [
```

