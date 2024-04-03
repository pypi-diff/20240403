# Comparing `tmp/cto_cli-0.1.2.tar.gz` & `tmp/cto_cli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cto_cli-0.1.2.tar", max compression
+gzip compressed data, was "cto_cli-0.1.3.tar", max compression
```

## Comparing `cto_cli-0.1.2.tar` & `cto_cli-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2024-04-03 10:28:39.776182 cto_cli-0.1.2/LICENSE
--rw-r--r--   0        0        0      233 2024-04-03 10:28:39.776182 cto_cli-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-04-03 10:28:39.776182 cto_cli-0.1.2/cto_cli/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 10:28:39.776182 cto_cli-0.1.2/cto_cli/ecs/api/__init__.py
--rw-r--r--   0        0        0     7306 2024-04-03 10:28:39.776182 cto_cli-0.1.2/cto_cli/ecs/api/connector.py
--rw-r--r--   0        0        0        0 2024-04-03 10:28:39.776182 cto_cli-0.1.2/cto_cli/ecs/commands/__init__.py
--rw-r--r--   0        0        0     3273 2024-04-03 10:28:39.776182 cto_cli-0.1.2/cto_cli/ecs/commands/config.py
--rw-r--r--   0        0        0     2047 2024-04-03 10:28:39.776182 cto_cli-0.1.2/cto_cli/ecs/commands/users.py
--rw-r--r--   0        0        0        0 2024-04-03 10:28:39.776182 cto_cli-0.1.2/cto_cli/ecs/local/__init__.py
--rw-r--r--   0        0        0      451 2024-04-03 10:28:39.776182 cto_cli-0.1.2/cto_cli/ecs/local/commands.py
--rw-r--r--   0        0        0     6279 2024-04-03 10:28:39.776182 cto_cli-0.1.2/cto_cli/ecs/local/files.py
--rw-r--r--   0        0        0     7277 2024-04-03 10:28:39.776182 cto_cli-0.1.2/cto_cli/ecs/local/operations.py
--rw-r--r--   0        0        0     2922 2024-04-03 10:28:39.776182 cto_cli-0.1.2/cto_cli/ecs/local/settings.py
--rw-r--r--   0        0        0     1789 2024-04-03 10:28:39.776182 cto_cli-0.1.2/cto_cli/ecs/local/validators.py
--rw-r--r--   0        0        0     2949 2024-04-03 10:28:39.776182 cto_cli-0.1.2/cto_cli/ecs/main.py
--rw-r--r--   0        0        0      652 2024-04-03 10:28:39.776182 cto_cli-0.1.2/cto_cli/main.py
--rw-r--r--   0        0        0      213 2024-04-03 10:28:39.776182 cto_cli-0.1.2/cto_cli/utils/errors.py
--rw-r--r--   0        0        0     1612 2024-04-03 10:28:40.608181 cto_cli-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 cto_cli-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-03 10:47:36.966879 cto_cli-0.1.3/LICENSE
+-rw-r--r--   0        0        0      233 2024-04-03 10:47:36.966879 cto_cli-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 10:47:36.966879 cto_cli-0.1.3/cto_cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:47:36.966879 cto_cli-0.1.3/cto_cli/ecs/api/__init__.py
+-rw-r--r--   0        0        0     7306 2024-04-03 10:47:36.966879 cto_cli-0.1.3/cto_cli/ecs/api/connector.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:47:36.966879 cto_cli-0.1.3/cto_cli/ecs/commands/__init__.py
+-rw-r--r--   0        0        0     3273 2024-04-03 10:47:36.966879 cto_cli-0.1.3/cto_cli/ecs/commands/config.py
+-rw-r--r--   0        0        0     2047 2024-04-03 10:47:36.966879 cto_cli-0.1.3/cto_cli/ecs/commands/users.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:47:36.966879 cto_cli-0.1.3/cto_cli/ecs/local/__init__.py
+-rw-r--r--   0        0        0      451 2024-04-03 10:47:36.966879 cto_cli-0.1.3/cto_cli/ecs/local/commands.py
+-rw-r--r--   0        0        0     6279 2024-04-03 10:47:36.966879 cto_cli-0.1.3/cto_cli/ecs/local/files.py
+-rw-r--r--   0        0        0     7277 2024-04-03 10:47:36.966879 cto_cli-0.1.3/cto_cli/ecs/local/operations.py
+-rw-r--r--   0        0        0     2922 2024-04-03 10:47:36.966879 cto_cli-0.1.3/cto_cli/ecs/local/settings.py
+-rw-r--r--   0        0        0     1789 2024-04-03 10:47:36.966879 cto_cli-0.1.3/cto_cli/ecs/local/validators.py
+-rw-r--r--   0        0        0     2949 2024-04-03 10:47:36.966879 cto_cli-0.1.3/cto_cli/ecs/main.py
+-rw-r--r--   0        0        0      652 2024-04-03 10:47:36.966879 cto_cli-0.1.3/cto_cli/main.py
+-rw-r--r--   0        0        0      213 2024-04-03 10:47:36.966879 cto_cli-0.1.3/cto_cli/utils/errors.py
+-rw-r--r--   0        0        0     1580 2024-04-03 10:47:37.918884 cto_cli-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 cto_cli-0.1.3/PKG-INFO
```

### Comparing `cto_cli-0.1.2/LICENSE` & `cto_cli-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cto_cli-0.1.2/cto_cli/ecs/api/connector.py` & `cto_cli-0.1.3/cto_cli/ecs/api/connector.py`

 * *Files identical despite different names*

### Comparing `cto_cli-0.1.2/cto_cli/ecs/commands/config.py` & `cto_cli-0.1.3/cto_cli/ecs/commands/config.py`

 * *Files identical despite different names*

### Comparing `cto_cli-0.1.2/cto_cli/ecs/commands/users.py` & `cto_cli-0.1.3/cto_cli/ecs/commands/users.py`

 * *Files identical despite different names*

### Comparing `cto_cli-0.1.2/cto_cli/ecs/local/files.py` & `cto_cli-0.1.3/cto_cli/ecs/local/files.py`

 * *Files identical despite different names*

### Comparing `cto_cli-0.1.2/cto_cli/ecs/local/operations.py` & `cto_cli-0.1.3/cto_cli/ecs/local/operations.py`

 * *Files identical despite different names*

### Comparing `cto_cli-0.1.2/cto_cli/ecs/local/settings.py` & `cto_cli-0.1.3/cto_cli/ecs/local/settings.py`

 * *Files identical despite different names*

### Comparing `cto_cli-0.1.2/cto_cli/ecs/local/validators.py` & `cto_cli-0.1.3/cto_cli/ecs/local/validators.py`

 * *Files identical despite different names*

### Comparing `cto_cli-0.1.2/cto_cli/ecs/main.py` & `cto_cli-0.1.3/cto_cli/ecs/main.py`

 * *Files identical despite different names*

### Comparing `cto_cli-0.1.2/cto_cli/main.py` & `cto_cli-0.1.3/cto_cli/main.py`

 * *Files identical despite different names*

### Comparing `cto_cli-0.1.2/pyproject.toml` & `cto_cli-0.1.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 [tool.poetry]
 name = "cto-cli"
-version = "0.1.2"
+version = "0.1.3"
 description = "The CTO cli"
 authors = ["CTO <support@cloudtechnologyoffice.com>"]
 readme = "README.md"
-
-[project]
-license = { file = "LICENSE" }
-
-[project.urls]
-Homepage = "https://doc.cloudtechnologyoffice.com/ecs/latest/"
-Source = "https://github.com/Cloud-Technology-Office/cto-cli"
+homepage = "https://doc.cloudtechnologyoffice.com/ecs/latest"
+repository = "https://github.com/Cloud-Technology-Office/cto-cli"
+license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 typer = "0.9.0"
 rich = "13.6.0"
 requests = "2.31.0"
 PyYAML = "6.0.1"
```

### Comparing `cto_cli-0.1.2/PKG-INFO` & `cto_cli-0.1.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: cto-cli
-Version: 0.1.2
+Version: 0.1.3
 Summary: The CTO cli
+Home-page: https://doc.cloudtechnologyoffice.com/ecs/latest
+License: Apache-2.0
 Author: CTO
 Author-email: support@cloudtechnologyoffice.com
 Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyYAML (==6.0.1)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: rich (==13.6.0)
 Requires-Dist: typer (==0.9.0)
+Project-URL: Repository, https://github.com/Cloud-Technology-Office/cto-cli
 Description-Content-Type: text/markdown
 
 # CTO cli
 
 CLI for ECS by CTO.
 
 ## Installation
```

