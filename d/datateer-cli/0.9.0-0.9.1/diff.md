# Comparing `tmp/datateer-cli-0.9.0.tar.gz` & `tmp/datateer-cli-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datateer-cli-0.9.0.tar", max compression
+gzip compressed data, was "datateer-cli-0.9.1.tar", max compression
```

## Comparing `datateer-cli-0.9.0.tar` & `datateer-cli-0.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       22 2022-03-10 03:32:24.769383 datateer-cli-0.9.0/datateer_cli/__init__.py
--rw-r--r--   0        0        0      654 2022-03-10 03:32:24.045377 datateer-cli-0.9.0/datateer_cli/cli.py
--rw-r--r--   0        0        0     8233 2022-03-10 03:32:24.045377 datateer-cli-0.9.0/datateer_cli/cli_old.py
--rw-r--r--   0        0        0     1663 2022-03-10 03:32:24.045377 datateer-cli-0.9.0/datateer_cli/commands/config/commands.py
--rw-r--r--   0        0        0     6733 2022-03-10 03:32:24.045377 datateer-cli-0.9.0/datateer_cli/commands/config/operations.py
--rw-r--r--   0        0        0      901 2022-03-10 03:32:24.045377 datateer-cli-0.9.0/datateer_cli/commands/docs/commands.py
--rw-r--r--   0        0        0     2777 2022-03-10 03:32:24.045377 datateer-cli-0.9.0/datateer_cli/commands/docs/docs.py
--rw-r--r--   0        0        0     8059 2022-03-10 03:32:24.045377 datateer-cli-0.9.0/datateer_cli/commands/docs/generate_erd.py
--rw-r--r--   0        0        0      173 2022-03-10 03:32:24.045377 datateer-cli-0.9.0/datateer_cli/commands/echo/echo_commands.py
--rw-r--r--   0        0        0     1069 2022-03-10 03:32:24.045377 datateer-cli-0.9.0/datateer_cli/commands/infra/commands.py
--rw-r--r--   0        0        0     1906 2022-03-10 03:32:24.045377 datateer-cli-0.9.0/datateer_cli/commands/infra/terraform_util.py
--rw-r--r--   0        0        0     5218 2022-03-10 03:32:24.045377 datateer-cli-0.9.0/datateer_cli/commands/pipeline/commands.py
--rw-r--r--   0        0        0     6526 2022-03-10 03:32:24.045377 datateer-cli-0.9.0/datateer_cli/commands/pipeline/deploy_flow.py
--rw-r--r--   0        0        0      218 2022-03-10 03:32:24.045377 datateer-cli-0.9.0/datateer_cli/commands/pipeline/flow/.dockerignore
--rw-r--r--   0        0        0     1629 2022-03-10 03:32:24.045377 datateer-cli-0.9.0/datateer_cli/commands/pipeline/flow/Dockerfile
--rw-r--r--   0        0        0     3415 2022-03-10 03:32:24.045377 datateer-cli-0.9.0/datateer_cli/developer_setup.py
--rw-r--r--   0        0        0     2889 2022-03-10 03:32:24.045377 datateer-cli-0.9.0/datateer_cli/docker_util.py
--rw-r--r--   0        0        0      292 2022-03-10 03:32:24.045377 datateer-cli-0.9.0/datateer_cli/efs.py
--rw-r--r--   0        0        0      564 2022-03-10 03:32:24.045377 datateer-cli-0.9.0/datateer_cli/install_bfg.sh
--rw-r--r--   0        0        0      291 2022-03-10 03:32:24.045377 datateer-cli-0.9.0/datateer_cli/logging.py
--rw-r--r--   0        0        0     1134 2022-03-10 03:32:24.045377 datateer-cli-0.9.0/datateer_cli/orchestration/pipeline_test.py
--rw-r--r--   0        0        0     1213 2022-03-10 03:32:24.045377 datateer-cli-0.9.0/datateer_cli/prefect_ops.py
--rw-r--r--   0        0        0     1356 2022-03-10 03:32:24.045377 datateer-cli-0.9.0/datateer_cli/security_scan_no_forbidden_files.py
--rw-r--r--   0        0        0      411 2022-03-10 03:32:24.045377 datateer-cli-0.9.0/datateer_cli/ssh/datateer-machine-key
--rw-r--r--   0        0        0       98 2022-03-10 03:32:24.045377 datateer-cli-0.9.0/datateer_cli/ssh/datateer-machine-key.pub
--rw-r--r--   0        0        0      441 2022-03-10 03:32:24.045377 datateer-cli-0.9.0/datateer_cli/ssh/readme
--rw-r--r--   0        0        0      872 2022-03-10 03:32:24.769383 datateer-cli-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     1111 2022-03-10 03:32:34.861738 datateer-cli-0.9.0/setup.py
--rw-r--r--   0        0        0      583 2022-03-10 03:32:34.862002 datateer-cli-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2022-03-10 05:45:52.521174 datateer-cli-0.9.1/datateer_cli/__init__.py
+-rw-r--r--   0        0        0      654 2022-03-10 05:45:51.881184 datateer-cli-0.9.1/datateer_cli/cli.py
+-rw-r--r--   0        0        0     8233 2022-03-10 05:45:51.885184 datateer-cli-0.9.1/datateer_cli/cli_old.py
+-rw-r--r--   0        0        0     1663 2022-03-10 05:45:51.885184 datateer-cli-0.9.1/datateer_cli/commands/config/commands.py
+-rw-r--r--   0        0        0     6733 2022-03-10 05:45:51.885184 datateer-cli-0.9.1/datateer_cli/commands/config/operations.py
+-rw-r--r--   0        0        0      901 2022-03-10 05:45:51.885184 datateer-cli-0.9.1/datateer_cli/commands/docs/commands.py
+-rw-r--r--   0        0        0     2777 2022-03-10 05:45:51.885184 datateer-cli-0.9.1/datateer_cli/commands/docs/docs.py
+-rw-r--r--   0        0        0     8059 2022-03-10 05:45:51.885184 datateer-cli-0.9.1/datateer_cli/commands/docs/generate_erd.py
+-rw-r--r--   0        0        0      173 2022-03-10 05:45:51.885184 datateer-cli-0.9.1/datateer_cli/commands/echo/echo_commands.py
+-rw-r--r--   0        0        0     1069 2022-03-10 05:45:51.885184 datateer-cli-0.9.1/datateer_cli/commands/infra/commands.py
+-rw-r--r--   0        0        0     1906 2022-03-10 05:45:51.885184 datateer-cli-0.9.1/datateer_cli/commands/infra/terraform_util.py
+-rw-r--r--   0        0        0     5218 2022-03-10 05:45:51.885184 datateer-cli-0.9.1/datateer_cli/commands/pipeline/commands.py
+-rw-r--r--   0        0        0     6514 2022-03-10 05:45:51.885184 datateer-cli-0.9.1/datateer_cli/commands/pipeline/deploy_flow.py
+-rw-r--r--   0        0        0      218 2022-03-10 05:45:51.885184 datateer-cli-0.9.1/datateer_cli/commands/pipeline/flow/.dockerignore
+-rw-r--r--   0        0        0     1629 2022-03-10 05:45:51.885184 datateer-cli-0.9.1/datateer_cli/commands/pipeline/flow/Dockerfile
+-rw-r--r--   0        0        0     3415 2022-03-10 05:45:51.885184 datateer-cli-0.9.1/datateer_cli/developer_setup.py
+-rw-r--r--   0        0        0     2889 2022-03-10 05:45:51.885184 datateer-cli-0.9.1/datateer_cli/docker_util.py
+-rw-r--r--   0        0        0      292 2022-03-10 05:45:51.885184 datateer-cli-0.9.1/datateer_cli/efs.py
+-rw-r--r--   0        0        0      564 2022-03-10 05:45:51.885184 datateer-cli-0.9.1/datateer_cli/install_bfg.sh
+-rw-r--r--   0        0        0      291 2022-03-10 05:45:51.885184 datateer-cli-0.9.1/datateer_cli/logging.py
+-rw-r--r--   0        0        0     1134 2022-03-10 05:45:51.885184 datateer-cli-0.9.1/datateer_cli/orchestration/pipeline_test.py
+-rw-r--r--   0        0        0     1213 2022-03-10 05:45:51.885184 datateer-cli-0.9.1/datateer_cli/prefect_ops.py
+-rw-r--r--   0        0        0     1356 2022-03-10 05:45:51.885184 datateer-cli-0.9.1/datateer_cli/security_scan_no_forbidden_files.py
+-rw-r--r--   0        0        0      411 2022-03-10 05:45:51.885184 datateer-cli-0.9.1/datateer_cli/ssh/datateer-machine-key
+-rw-r--r--   0        0        0       98 2022-03-10 05:45:51.885184 datateer-cli-0.9.1/datateer_cli/ssh/datateer-machine-key.pub
+-rw-r--r--   0        0        0      441 2022-03-10 05:45:51.885184 datateer-cli-0.9.1/datateer_cli/ssh/readme
+-rw-r--r--   0        0        0      872 2022-03-10 05:45:52.521174 datateer-cli-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1111 2022-03-10 05:46:00.886412 datateer-cli-0.9.1/setup.py
+-rw-r--r--   0        0        0      583 2022-03-10 05:46:00.886691 datateer-cli-0.9.1/PKG-INFO
```

### Comparing `datateer-cli-0.9.0/datateer_cli/cli.py` & `datateer-cli-0.9.1/datateer_cli/cli.py`

 * *Files identical despite different names*

### Comparing `datateer-cli-0.9.0/datateer_cli/cli_old.py` & `datateer-cli-0.9.1/datateer_cli/cli_old.py`

 * *Files identical despite different names*

### Comparing `datateer-cli-0.9.0/datateer_cli/commands/config/commands.py` & `datateer-cli-0.9.1/datateer_cli/commands/config/commands.py`

 * *Files identical despite different names*

### Comparing `datateer-cli-0.9.0/datateer_cli/commands/config/operations.py` & `datateer-cli-0.9.1/datateer_cli/commands/config/operations.py`

 * *Files identical despite different names*

### Comparing `datateer-cli-0.9.0/datateer_cli/commands/docs/commands.py` & `datateer-cli-0.9.1/datateer_cli/commands/docs/commands.py`

 * *Files identical despite different names*

### Comparing `datateer-cli-0.9.0/datateer_cli/commands/docs/docs.py` & `datateer-cli-0.9.1/datateer_cli/commands/docs/docs.py`

 * *Files identical despite different names*

### Comparing `datateer-cli-0.9.0/datateer_cli/commands/docs/generate_erd.py` & `datateer-cli-0.9.1/datateer_cli/commands/docs/generate_erd.py`

 * *Files identical despite different names*

### Comparing `datateer-cli-0.9.0/datateer_cli/commands/infra/commands.py` & `datateer-cli-0.9.1/datateer_cli/commands/infra/commands.py`

 * *Files identical despite different names*

### Comparing `datateer-cli-0.9.0/datateer_cli/commands/infra/terraform_util.py` & `datateer-cli-0.9.1/datateer_cli/commands/infra/terraform_util.py`

 * *Files identical despite different names*

### Comparing `datateer-cli-0.9.0/datateer_cli/commands/pipeline/commands.py` & `datateer-cli-0.9.1/datateer_cli/commands/pipeline/commands.py`

 * *Files identical despite different names*

### Comparing `datateer-cli-0.9.0/datateer_cli/commands/pipeline/deploy_flow.py` & `datateer-cli-0.9.1/datateer_cli/commands/pipeline/deploy_flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,15 @@
         include_https {bool} -- True to include the https:// prefix, false to leave off (default: {False})
 
     Returns:
         string -- A well formed docker registry URL
     """
     # aws_account_id = boto3.client("sts").get_caller_identity()["Account"]
     registry = f"{aws_account_id}.dkr.ecr.{aws_region}.amazonaws.com"
-    return f"https://{registry}" if include_https else f"http://{registry}"
+    return f"https://{registry}" if include_https else registry
 
 
 # def validate_environment(ctx, name, environment):
 #     path = '.env' if environment == 'local' else f'.env.{environment}'
 #     if not os.path.exists(path):
 #         raise click.BadParameter(f'Could not locate an .env file at {path}')
 #     return environment
```

### Comparing `datateer-cli-0.9.0/datateer_cli/commands/pipeline/flow/Dockerfile` & `datateer-cli-0.9.1/datateer_cli/commands/pipeline/flow/Dockerfile`

 * *Files identical despite different names*

### Comparing `datateer-cli-0.9.0/datateer_cli/developer_setup.py` & `datateer-cli-0.9.1/datateer_cli/developer_setup.py`

 * *Files identical despite different names*

### Comparing `datateer-cli-0.9.0/datateer_cli/docker_util.py` & `datateer-cli-0.9.1/datateer_cli/docker_util.py`

 * *Files identical despite different names*

### Comparing `datateer-cli-0.9.0/datateer_cli/install_bfg.sh` & `datateer-cli-0.9.1/datateer_cli/install_bfg.sh`

 * *Files identical despite different names*

### Comparing `datateer-cli-0.9.0/datateer_cli/orchestration/pipeline_test.py` & `datateer-cli-0.9.1/datateer_cli/orchestration/pipeline_test.py`

 * *Files identical despite different names*

### Comparing `datateer-cli-0.9.0/datateer_cli/prefect_ops.py` & `datateer-cli-0.9.1/datateer_cli/prefect_ops.py`

 * *Files identical despite different names*

### Comparing `datateer-cli-0.9.0/datateer_cli/security_scan_no_forbidden_files.py` & `datateer-cli-0.9.1/datateer_cli/security_scan_no_forbidden_files.py`

 * *Files identical despite different names*

### Comparing `datateer-cli-0.9.0/pyproject.toml` & `datateer-cli-0.9.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datateer-cli"
-version = "0.9.0"
+version = "0.9.1"
 description = "Datateer CLI to support devops and infrastructure"
 authors = ["Datateer <dev@datateer.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 boto3 = "^1.20.37"
 click = ">=7.0"
```

### Comparing `datateer-cli-0.9.0/setup.py` & `datateer-cli-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
  'pathspec>=0.9.0,<0.10.0']
 
 entry_points = \
 {'console_scripts': ['datateer = datateer_cli.cli:main']}
 
 setup_kwargs = {
     'name': 'datateer-cli',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'Datateer CLI to support devops and infrastructure',
     'long_description': None,
     'author': 'Datateer',
     'author_email': 'dev@datateer.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `datateer-cli-0.9.0/PKG-INFO` & `datateer-cli-0.9.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datateer-cli
-Version: 0.9.0
+Version: 0.9.1
 Summary: Datateer CLI to support devops and infrastructure
 Author: Datateer
 Author-email: dev@datateer.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
```

