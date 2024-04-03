# Comparing `tmp/cerebrium-1.9.5.tar.gz` & `tmp/cerebrium-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerebrium-1.9.5.tar", max compression
+gzip compressed data, was "cerebrium-1.9.6.tar", max compression
```

## Comparing `cerebrium-1.9.5.tar` & `cerebrium-1.9.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    34594 2023-11-06 16:31:35.379943 cerebrium-1.9.5/LICENSE
--rw-r--r--   0        0        0      372 2023-11-06 16:31:35.379943 cerebrium-1.9.5/README.md
--rw-r--r--   0        0        0      201 2023-11-06 16:34:58.783985 cerebrium-1.9.5/cerebrium/__init__.py
--rw-r--r--   0        0        0    13823 2023-11-06 16:31:35.379943 cerebrium-1.9.5/cerebrium/api.py
--rwxr-xr-x   0        0        0      317 2023-11-06 16:31:35.379943 cerebrium-1.9.5/cerebrium/cli.py
--rw-r--r--   0        0        0    21567 2023-11-06 16:31:35.383942 cerebrium-1.9.5/cerebrium/commands/cortex.py
--rw-r--r--   0        0        0     1819 2023-11-06 16:31:35.383942 cerebrium-1.9.5/cerebrium/commands/storage.py
--rw-r--r--   0        0        0     4654 2023-11-06 16:31:35.383942 cerebrium-1.9.5/cerebrium/commands/utilities.py
--rw-r--r--   0        0        0      714 2023-11-06 16:31:35.383942 cerebrium-1.9.5/cerebrium/core.py
--rw-r--r--   0        0        0     3175 2023-11-06 16:31:35.383942 cerebrium-1.9.5/cerebrium/datatypes.py
--rw-r--r--   0        0        0     1739 2023-11-06 16:31:35.383942 cerebrium-1.9.5/cerebrium/errors.py
--rw-r--r--   0        0        0     6823 2023-11-06 16:31:35.383942 cerebrium-1.9.5/cerebrium/utils.py
--rw-r--r--   0        0        0     4019 2023-11-06 16:31:35.383942 cerebrium-1.9.5/cerebrium/verification.py
--rw-r--r--   0        0        0     1403 2023-11-06 16:34:58.779985 cerebrium-1.9.5/pyproject.toml
--rw-r--r--   0        0        0     1458 1970-01-01 00:00:00.000000 cerebrium-1.9.5/PKG-INFO
+-rw-r--r--   0        0        0    34594 2023-11-10 16:00:27.902035 cerebrium-1.9.6/LICENSE
+-rw-r--r--   0        0        0      372 2023-11-10 16:00:27.902035 cerebrium-1.9.6/README.md
+-rw-r--r--   0        0        0      201 2023-11-10 16:03:32.480090 cerebrium-1.9.6/cerebrium/__init__.py
+-rw-r--r--   0        0        0    13823 2023-11-10 16:00:27.902035 cerebrium-1.9.6/cerebrium/api.py
+-rwxr-xr-x   0        0        0      317 2023-11-10 16:00:27.902035 cerebrium-1.9.6/cerebrium/cli.py
+-rw-r--r--   0        0        0    21719 2023-11-10 16:00:27.902035 cerebrium-1.9.6/cerebrium/commands/cortex.py
+-rw-r--r--   0        0        0     1819 2023-11-10 16:00:27.902035 cerebrium-1.9.6/cerebrium/commands/storage.py
+-rw-r--r--   0        0        0     4654 2023-11-10 16:00:27.902035 cerebrium-1.9.6/cerebrium/commands/utilities.py
+-rw-r--r--   0        0        0      714 2023-11-10 16:00:27.902035 cerebrium-1.9.6/cerebrium/core.py
+-rw-r--r--   0        0        0     3175 2023-11-10 16:00:27.902035 cerebrium-1.9.6/cerebrium/datatypes.py
+-rw-r--r--   0        0        0     1739 2023-11-10 16:00:27.902035 cerebrium-1.9.6/cerebrium/errors.py
+-rw-r--r--   0        0        0     6823 2023-11-10 16:00:27.902035 cerebrium-1.9.6/cerebrium/utils.py
+-rw-r--r--   0        0        0     4019 2023-11-10 16:00:27.902035 cerebrium-1.9.6/cerebrium/verification.py
+-rw-r--r--   0        0        0     1403 2023-11-10 16:03:32.476090 cerebrium-1.9.6/pyproject.toml
+-rw-r--r--   0        0        0     1458 1970-01-01 00:00:00.000000 cerebrium-1.9.6/PKG-INFO
```

### Comparing `cerebrium-1.9.5/LICENSE` & `cerebrium-1.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cerebrium-1.9.5/cerebrium/api.py` & `cerebrium-1.9.6/cerebrium/api.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.9.5/cerebrium/commands/cortex.py` & `cerebrium-1.9.6/cerebrium/commands/cortex.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,27 +218,30 @@
         "exclude": "[./.*, ./__*]",  # ignore .git etc. by default
         "init_debug": False,
         "pre_init_debug": False,
         "disable_animation": os.getenv("CI", None),
     }
 
     # If a config file is provided, load it in.
-    if config_file:
+    if config_file == "" or config_file is None:
+        config_file = "config.yaml"
+    else:
         if not os.path.exists(config_file):
             utils.cerebriumLog(
                 level="ERROR",
                 message=f"Config file {config_file} not found.",
                 prefix="Argument Error:",
             )
-            config = {}
-        else:
-            with open(config_file, "r") as f:
-                config = yaml.safe_load(f)
+
+    if os.path.exists(config_file):
+        with open(config_file, "r") as f:
+            config = yaml.safe_load(f)
     else:
         config = {}
+        
     config = utils.remove_null_values(config)
     disable_animation = disable_animation if disable_animation is not None else False
     # Override the default params with the config file params
     params.update(config)
     params = assign_param(params, "name", name)
     params = assign_param(params, "hardware", hardware)
     params = assign_param(params, "cpu", cpu)
@@ -321,15 +324,19 @@
         print(json.dumps(params, indent=2)[2:-1])
 
     if predict_data is not None:
         print("🔮 Running predict function with the following data:")
         try:
             print(json.dumps(json.loads(predict_data), indent=4)[2:-1])
         except json.decoder.JSONDecodeError:
-            utils.cerebriumLog(message="Invalid JSON string", level="ERROR", prefix="Could not parse predict data:")
+            utils.cerebriumLog(
+                message="Invalid JSON string",
+                level="ERROR",
+                prefix="Could not parse predict data:",
+            )
 
     setup_response = api._setup_app(
         headers={"Authorization": api_key},
         body=params,
     )
     build_status = setup_response["status"]
     project_id = setup_response["projectId"]
@@ -595,15 +602,17 @@
         None,
         help="Force rebuild. Clears rebuilds deployment from scratch as if it's a clean deployment.",
     ),
     config_file: str = typer.Option(
         "",
         help="Path to config.yaml file. You can generate a config using `cerebrium init-cortex`. The contents of the deployment config file are overridden by the command line arguments.",
     ),
-    log_level: Union[str, None] = typer.Option(None, help="Log level for the Cortex build. Can be one of 'DEBUG' or 'INFO'"),
+    log_level: Union[str, None] = typer.Option(
+        None, help="Log level for the Cortex build. Can be one of 'DEBUG' or 'INFO'"
+    ),
     disable_animation: Union[bool, None] = typer.Option(
         None,
         help="Whether to use TQDM and yaspin animations.",
     ),
     disable_build_logs: bool = typer.Option(
         False, help="Whether to disable build logs during a deployment."
     ),
```

### Comparing `cerebrium-1.9.5/cerebrium/commands/storage.py` & `cerebrium-1.9.6/cerebrium/commands/storage.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.9.5/cerebrium/commands/utilities.py` & `cerebrium-1.9.6/cerebrium/commands/utilities.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.9.5/cerebrium/core.py` & `cerebrium-1.9.6/cerebrium/core.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.9.5/cerebrium/datatypes.py` & `cerebrium-1.9.6/cerebrium/datatypes.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.9.5/cerebrium/errors.py` & `cerebrium-1.9.6/cerebrium/errors.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.9.5/cerebrium/utils.py` & `cerebrium-1.9.6/cerebrium/utils.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.9.5/cerebrium/verification.py` & `cerebrium-1.9.6/cerebrium/verification.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.9.5/pyproject.toml` & `cerebrium-1.9.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cerebrium"
-version = "1.9.5"
+version = "1.9.6"
 description = ""
 authors = ["Elijah Roussos <elijah@cerebrium.ai>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 exclude = ["tests/*", "dist/*", "examples/*"]
 
 [tool.poetry.urls]
```

### Comparing `cerebrium-1.9.5/PKG-INFO` & `cerebrium-1.9.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerebrium
-Version: 1.9.5
+Version: 1.9.6
 Summary: 
 License: AGPL-3.0-only
 Author: Elijah Roussos
 Author-email: elijah@cerebrium.ai
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

