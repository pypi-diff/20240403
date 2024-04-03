# Comparing `tmp/async-lambda-unstable-0.3.5.tar.gz` & `tmp/async-lambda-unstable-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async-lambda-unstable-0.3.5.tar", last modified: Mon Mar 25 20:52:40 2024, max compression
+gzip compressed data, was "async-lambda-unstable-0.3.6.tar", last modified: Wed Apr  3 15:46:53 2024, max compression
```

## Comparing `async-lambda-unstable-0.3.5.tar` & `async-lambda-unstable-0.3.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-03-25 20:52:40.727303 async-lambda-unstable-0.3.5/
--rw-r--r--   0 henryjones   (501) staff       (20)    14546 2024-03-25 20:52:40.726912 async-lambda-unstable-0.3.5/PKG-INFO
--rw-r--r--   0 henryjones   (501) staff       (20)    14286 2024-03-25 20:21:32.000000 async-lambda-unstable-0.3.5/README.md
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-03-25 20:52:40.724213 async-lambda-unstable-0.3.5/async_lambda/
--rw-r--r--   0 henryjones   (501) staff       (20)      692 2024-03-25 19:23:25.000000 async-lambda-unstable-0.3.5/async_lambda/__init__.py
--rw-r--r--   0 henryjones   (501) staff       (20)     3388 2024-03-25 20:13:13.000000 async-lambda-unstable-0.3.5/async_lambda/build_config.py
--rw-r--r--   0 henryjones   (501) staff       (20)    10311 2024-01-24 02:07:27.000000 async-lambda-unstable-0.3.5/async_lambda/cli.py
--rw-r--r--   0 henryjones   (501) staff       (20)      750 2024-03-15 17:38:55.000000 async-lambda-unstable-0.3.5/async_lambda/client.py
--rw-r--r--   0 henryjones   (501) staff       (20)      350 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.5/async_lambda/config.py
--rw-r--r--   0 henryjones   (501) staff       (20)    19117 2024-03-25 20:51:58.000000 async-lambda-unstable-0.3.5/async_lambda/controller.py
--rw-r--r--   0 henryjones   (501) staff       (20)      723 2024-03-15 17:38:55.000000 async-lambda-unstable-0.3.5/async_lambda/env.py
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-03-25 20:52:40.724630 async-lambda-unstable-0.3.5/async_lambda/models/
--rw-r--r--   0 henryjones   (501) staff       (20)        0 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.5/async_lambda/models/__init__.py
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-03-25 20:52:40.725599 async-lambda-unstable-0.3.5/async_lambda/models/events/
--rw-r--r--   0 henryjones   (501) staff       (20)        0 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.5/async_lambda/models/events/__init__.py
--rw-r--r--   0 henryjones   (501) staff       (20)     1118 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.5/async_lambda/models/events/api_event.py
--rw-r--r--   0 henryjones   (501) staff       (20)      929 2024-03-15 17:38:55.000000 async-lambda-unstable-0.3.5/async_lambda/models/events/base_event.py
--rw-r--r--   0 henryjones   (501) staff       (20)     1884 2024-03-18 21:28:52.000000 async-lambda-unstable-0.3.5/async_lambda/models/events/managed_sqs_event.py
--rw-r--r--   0 henryjones   (501) staff       (20)       77 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.5/async_lambda/models/events/scheduled_event.py
--rw-r--r--   0 henryjones   (501) staff       (20)     1086 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.5/async_lambda/models/events/unmanaged_sqs_event.py
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-03-25 20:52:40.725881 async-lambda-unstable-0.3.5/async_lambda/models/mock/
--rw-r--r--   0 henryjones   (501) staff       (20)      508 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.5/async_lambda/models/mock/mock_context.py
--rw-r--r--   0 henryjones   (501) staff       (20)     2030 2024-03-25 19:06:55.000000 async-lambda-unstable-0.3.5/async_lambda/models/mock/mock_event.py
--rw-r--r--   0 henryjones   (501) staff       (20)    17633 2024-03-25 19:54:46.000000 async-lambda-unstable-0.3.5/async_lambda/models/task.py
--rw-r--r--   0 henryjones   (501) staff       (20)        0 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.5/async_lambda/py.typed
--rw-r--r--   0 henryjones   (501) staff       (20)      215 2024-03-25 19:15:10.000000 async-lambda-unstable-0.3.5/async_lambda/util.py
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-03-25 20:52:40.726730 async-lambda-unstable-0.3.5/async_lambda_unstable.egg-info/
--rw-r--r--   0 henryjones   (501) staff       (20)    14546 2024-03-25 20:52:40.000000 async-lambda-unstable-0.3.5/async_lambda_unstable.egg-info/PKG-INFO
--rw-r--r--   0 henryjones   (501) staff       (20)      910 2024-03-25 20:52:40.000000 async-lambda-unstable-0.3.5/async_lambda_unstable.egg-info/SOURCES.txt
--rw-r--r--   0 henryjones   (501) staff       (20)        1 2024-03-25 20:52:40.000000 async-lambda-unstable-0.3.5/async_lambda_unstable.egg-info/dependency_links.txt
--rw-r--r--   0 henryjones   (501) staff       (20)       54 2024-03-25 20:52:40.000000 async-lambda-unstable-0.3.5/async_lambda_unstable.egg-info/entry_points.txt
--rw-r--r--   0 henryjones   (501) staff       (20)       48 2024-03-25 20:52:40.000000 async-lambda-unstable-0.3.5/async_lambda_unstable.egg-info/requires.txt
--rw-r--r--   0 henryjones   (501) staff       (20)       13 2024-03-25 20:52:40.000000 async-lambda-unstable-0.3.5/async_lambda_unstable.egg-info/top_level.txt
--rw-r--r--   0 henryjones   (501) staff       (20)      821 2024-03-15 17:38:55.000000 async-lambda-unstable-0.3.5/pyproject.toml
--rw-r--r--   0 henryjones   (501) staff       (20)       38 2024-03-25 20:52:40.727355 async-lambda-unstable-0.3.5/setup.cfg
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-04-03 15:46:53.174629 async-lambda-unstable-0.3.6/
+-rw-r--r--   0 henryjones   (501) staff       (20)    14546 2024-04-03 15:46:53.174422 async-lambda-unstable-0.3.6/PKG-INFO
+-rw-r--r--   0 henryjones   (501) staff       (20)    14286 2024-03-25 20:21:32.000000 async-lambda-unstable-0.3.6/README.md
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-04-03 15:46:53.170789 async-lambda-unstable-0.3.6/async_lambda/
+-rw-r--r--   0 henryjones   (501) staff       (20)      692 2024-04-03 15:45:53.000000 async-lambda-unstable-0.3.6/async_lambda/__init__.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     3388 2024-03-25 20:13:13.000000 async-lambda-unstable-0.3.6/async_lambda/build_config.py
+-rw-r--r--   0 henryjones   (501) staff       (20)    11395 2024-04-03 15:45:25.000000 async-lambda-unstable-0.3.6/async_lambda/cli.py
+-rw-r--r--   0 henryjones   (501) staff       (20)      750 2024-03-15 17:38:55.000000 async-lambda-unstable-0.3.6/async_lambda/client.py
+-rw-r--r--   0 henryjones   (501) staff       (20)      350 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.6/async_lambda/config.py
+-rw-r--r--   0 henryjones   (501) staff       (20)    19117 2024-03-25 20:51:58.000000 async-lambda-unstable-0.3.6/async_lambda/controller.py
+-rw-r--r--   0 henryjones   (501) staff       (20)      723 2024-03-15 17:38:55.000000 async-lambda-unstable-0.3.6/async_lambda/env.py
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-04-03 15:46:53.171303 async-lambda-unstable-0.3.6/async_lambda/models/
+-rw-r--r--   0 henryjones   (501) staff       (20)        0 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.6/async_lambda/models/__init__.py
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-04-03 15:46:53.172856 async-lambda-unstable-0.3.6/async_lambda/models/events/
+-rw-r--r--   0 henryjones   (501) staff       (20)        0 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.6/async_lambda/models/events/__init__.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     1118 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.6/async_lambda/models/events/api_event.py
+-rw-r--r--   0 henryjones   (501) staff       (20)      929 2024-03-15 17:38:55.000000 async-lambda-unstable-0.3.6/async_lambda/models/events/base_event.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     1884 2024-03-18 21:28:52.000000 async-lambda-unstable-0.3.6/async_lambda/models/events/managed_sqs_event.py
+-rw-r--r--   0 henryjones   (501) staff       (20)       77 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.6/async_lambda/models/events/scheduled_event.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     1086 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.6/async_lambda/models/events/unmanaged_sqs_event.py
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-04-03 15:46:53.173267 async-lambda-unstable-0.3.6/async_lambda/models/mock/
+-rw-r--r--   0 henryjones   (501) staff       (20)      508 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.6/async_lambda/models/mock/mock_context.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     2030 2024-03-25 19:06:55.000000 async-lambda-unstable-0.3.6/async_lambda/models/mock/mock_event.py
+-rw-r--r--   0 henryjones   (501) staff       (20)    17705 2024-04-03 15:42:11.000000 async-lambda-unstable-0.3.6/async_lambda/models/task.py
+-rw-r--r--   0 henryjones   (501) staff       (20)        0 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.6/async_lambda/py.typed
+-rw-r--r--   0 henryjones   (501) staff       (20)      514 2024-03-27 19:59:17.000000 async-lambda-unstable-0.3.6/async_lambda/util.py
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-04-03 15:46:53.174259 async-lambda-unstable-0.3.6/async_lambda_unstable.egg-info/
+-rw-r--r--   0 henryjones   (501) staff       (20)    14546 2024-04-03 15:46:53.000000 async-lambda-unstable-0.3.6/async_lambda_unstable.egg-info/PKG-INFO
+-rw-r--r--   0 henryjones   (501) staff       (20)      910 2024-04-03 15:46:53.000000 async-lambda-unstable-0.3.6/async_lambda_unstable.egg-info/SOURCES.txt
+-rw-r--r--   0 henryjones   (501) staff       (20)        1 2024-04-03 15:46:53.000000 async-lambda-unstable-0.3.6/async_lambda_unstable.egg-info/dependency_links.txt
+-rw-r--r--   0 henryjones   (501) staff       (20)       54 2024-04-03 15:46:53.000000 async-lambda-unstable-0.3.6/async_lambda_unstable.egg-info/entry_points.txt
+-rw-r--r--   0 henryjones   (501) staff       (20)       48 2024-04-03 15:46:53.000000 async-lambda-unstable-0.3.6/async_lambda_unstable.egg-info/requires.txt
+-rw-r--r--   0 henryjones   (501) staff       (20)       13 2024-04-03 15:46:53.000000 async-lambda-unstable-0.3.6/async_lambda_unstable.egg-info/top_level.txt
+-rw-r--r--   0 henryjones   (501) staff       (20)      821 2024-03-15 17:38:55.000000 async-lambda-unstable-0.3.6/pyproject.toml
+-rw-r--r--   0 henryjones   (501) staff       (20)       38 2024-04-03 15:46:53.174682 async-lambda-unstable-0.3.6/setup.cfg
```

### Comparing `async-lambda-unstable-0.3.5/PKG-INFO` & `async-lambda-unstable-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-lambda-unstable
-Version: 0.3.5
+Version: 0.3.6
 Summary: A framework for creating AWS Lambda Async Workflows. - Unstable Branch
 Author-email: "Nuclei, Inc" <engineering@nuclei.ai>
 Description-Content-Type: text/markdown
 Provides-Extra: local
 
 # async-lambda
```

### Comparing `async-lambda-unstable-0.3.5/README.md` & `async-lambda-unstable-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.3.5/async_lambda/__init__.py` & `async-lambda-unstable-0.3.6/async_lambda/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,8 +5,8 @@
 from .env import enable_force_sync_mode as enable_force_sync_mode
 from .env import is_build_mode as is_build_mode
 from .models.events.api_event import APIEvent as APIEvent
 from .models.events.managed_sqs_event import ManagedSQSEvent as ManagedSQSEvent
 from .models.events.scheduled_event import ScheduledEvent as ScheduledEvent
 from .models.events.unmanaged_sqs_event import UnmanagedSQSEvent as UnmanagedSQSEvent
 
-__version__ = "0.3.5"
+__version__ = "0.3.6"
```

### Comparing `async-lambda-unstable-0.3.5/async_lambda/build_config.py` & `async-lambda-unstable-0.3.6/async_lambda/build_config.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.3.5/async_lambda/cli.py` & `async-lambda-unstable-0.3.6/async_lambda/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 import inspect
 import json
 import logging
 import os
 import shutil
 import subprocess
 import sys
+import traceback
 import zipfile
 from pathlib import Path
 from typing import Callable, List, Optional, Tuple
 from uuid import uuid4
 
 import click
 
 from . import __version__
 from .build_config import get_build_config_for_stage
 from .controller import AsyncLambdaController
 from .env import enable_force_sync_mode
 from .models.mock.mock_context import MockLambdaContext
 from .models.mock.mock_event import MockAPILambdaEvent, MockSQSLambdaEvent
 from .models.task import TaskTriggerType
+from .util import nested_update
 
 
 @click.group()
 @click.option("-d", "--debug", help="Turn on debug logs", is_flag=True, default=False)
 def cli(debug: bool):
     """
     async-lambda CLI. For building async-lambda applications.
@@ -68,32 +70,58 @@
 @click.option("-s", "--stage", help="The stage to build the app for.")
 @click.option(
     "-o",
     "--output",
     default="template.json",
     help="The name of the file for the output template.",
 )
-def build(module: str, output: str, stage: Optional[str] = None):
+@click.option(
+    "-e", "--extras", help="The path to a json file to merge the output template with."
+)
+def build(
+    module: str, output: str, stage: Optional[str] = None, extras: Optional[str] = None
+):
     """
     Builds/generates the SAM template for the given module.
     """
     dir = Path.cwd()
     config = {}
     config_file = dir.joinpath(".async_lambda/config.json")
     if config_file.exists():
         config = json.loads(config_file.read_bytes())
     controller = import_module_get_controller(
         module_name=module, config=config, stage=stage
     )
-    click.echo("Generating SAM template...")
 
+    extras_json = None
+    if extras is not None:
+        extras_file = dir.joinpath(extras)
+        if not extras_file.exists():
+            raise click.ClickException(
+                f"Unable to find extras file {extras_file.as_posix()}"
+            )
+        click.echo("Collecting extras...")
+        try:
+            extras_json = json.loads(extras_file.read_text())
+        except json.JSONDecodeError:
+            click.echo(traceback.format_exc(), err=True)
+            raise click.ClickException("Extras file contains invalid formatted data.")
+        if not isinstance(extras_json, dict):
+            raise click.ClickException("Extras file contains invalid formatted data.")
+
+    click.echo("Generating SAM template...")
+    template = controller.generate_sam_template(module, config, stage=stage)
+    if extras_json is not None:
+        click.echo("Merging template with extras...")
+        nested_update(template, extras_json)
+    click.echo(f"Writing template to {output}...")
     with open(os.path.join(os.getcwd(), output), "w") as template_file:
         template_file.write(
             json.dumps(
-                controller.generate_sam_template(module, config, stage=stage),
+                template,
                 indent=2,
             )
         )
 
     if os.path.exists(".async_lambda/build"):
         shutil.rmtree(".async_lambda/build")
     os.makedirs(".async_lambda/build/packages", exist_ok=True)
```

### Comparing `async-lambda-unstable-0.3.5/async_lambda/client.py` & `async-lambda-unstable-0.3.6/async_lambda/client.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.3.5/async_lambda/controller.py` & `async-lambda-unstable-0.3.6/async_lambda/controller.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.3.5/async_lambda/env.py` & `async-lambda-unstable-0.3.6/async_lambda/env.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.3.5/async_lambda/models/events/api_event.py` & `async-lambda-unstable-0.3.6/async_lambda/models/events/api_event.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.3.5/async_lambda/models/events/base_event.py` & `async-lambda-unstable-0.3.6/async_lambda/models/events/base_event.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.3.5/async_lambda/models/events/managed_sqs_event.py` & `async-lambda-unstable-0.3.6/async_lambda/models/events/managed_sqs_event.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.3.5/async_lambda/models/events/unmanaged_sqs_event.py` & `async-lambda-unstable-0.3.6/async_lambda/models/events/unmanaged_sqs_event.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.3.5/async_lambda/models/mock/mock_event.py` & `async-lambda-unstable-0.3.6/async_lambda/models/mock/mock_event.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.3.5/async_lambda/models/task.py` & `async-lambda-unstable-0.3.6/async_lambda/models/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -393,14 +393,15 @@
                         "Tags": make_cf_tags({**build_config.tags, **_extra_tags}),
                         "QueueName": self.get_managed_queue_name(lane=lane_index),
                         "RedrivePolicy": {
                             "deadLetterTargetArn": dead_letter_target_arn,
                             "maxReceiveCount": self.trigger_config["max_receive_count"],
                         },
                         "VisibilityTimeout": self.timeout,
+                        "MessageRetentionPeriod": 1_209_600,  # 14 days
                     },
                 }
                 for extra_index, extra in enumerate(build_config.managed_queue_extras):
                     template[
                         self.get_managed_queue_extra_logical_id(
                             extra_index, lane=lane_index
                         )
```

### Comparing `async-lambda-unstable-0.3.5/async_lambda_unstable.egg-info/PKG-INFO` & `async-lambda-unstable-0.3.6/async_lambda_unstable.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-lambda-unstable
-Version: 0.3.5
+Version: 0.3.6
 Summary: A framework for creating AWS Lambda Async Workflows. - Unstable Branch
 Author-email: "Nuclei, Inc" <engineering@nuclei.ai>
 Description-Content-Type: text/markdown
 Provides-Extra: local
 
 # async-lambda
```

### Comparing `async-lambda-unstable-0.3.5/async_lambda_unstable.egg-info/SOURCES.txt` & `async-lambda-unstable-0.3.6/async_lambda_unstable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.3.5/pyproject.toml` & `async-lambda-unstable-0.3.6/pyproject.toml`

 * *Files identical despite different names*

