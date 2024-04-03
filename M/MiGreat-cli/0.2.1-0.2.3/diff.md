# Comparing `tmp/migreat_cli-0.2.1.tar.gz` & `tmp/migreat_cli-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "migreat_cli-0.2.1.tar", max compression
+gzip compressed data, was "migreat_cli-0.2.3.tar", max compression
```

## Comparing `migreat_cli-0.2.1.tar` & `migreat_cli-0.2.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1069 2024-04-01 00:37:40.162398 migreat_cli-0.2.1/LICENSE
--rw-r--r--   0        0        0     7603 2024-04-01 00:37:40.166398 migreat_cli-0.2.1/README.md
--rw-r--r--   0        0        0      563 2024-04-01 00:37:40.166398 migreat_cli-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    23042 2024-04-01 00:37:40.166398 migreat_cli-0.2.1/src/migreat/MiGreat.py
--rw-r--r--   0        0        0       23 2024-04-01 00:37:40.166398 migreat_cli-0.2.1/src/migreat/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 00:37:40.166398 migreat_cli-0.2.1/src/migreat/bin/__init__.py
--rw-r--r--   0        0        0       66 2024-04-01 00:37:40.166398 migreat_cli-0.2.1/src/migreat/bin/migreat
--rw-r--r--   0        0        0      105 2024-04-01 00:37:40.166398 migreat_cli-0.2.1/src/migreat/bin/migreat.py
--rw-r--r--   0        0        0      952 2024-04-01 00:37:40.166398 migreat_cli-0.2.1/src/migreat/example/docker-compose.yml
--rw-r--r--   0        0        0      371 2024-04-01 00:37:40.166398 migreat_cli-0.2.1/src/migreat/example/svc1/Dockerfile
--rw-r--r--   0        0        0      303 2024-04-01 00:37:40.166398 migreat_cli-0.2.1/src/migreat/example/svc1/MiGreat.yaml
--rw-r--r--   0        0        0       17 2024-04-01 00:37:40.166398 migreat_cli-0.2.1/src/migreat/example/svc1/requirements.txt
--rw-r--r--   0        0        0      338 2024-04-01 00:37:40.166398 migreat_cli-0.2.1/src/migreat/example/svc1/versions/0001_create_user_table.py
--rw-r--r--   0        0        0      251 2024-04-01 00:37:40.166398 migreat_cli-0.2.1/src/migreat/example/svc1/versions/0002_create_enum_type.py
--rw-r--r--   0        0        0      129 2024-04-01 00:37:40.166398 migreat_cli-0.2.1/src/migreat/example/svc1/versions/0003_alter_enum_type.py
--rw-r--r--   0        0        0      492 2024-04-01 00:37:40.166398 migreat_cli-0.2.1/src/migreat/example/svc1/versions/0004_create_shared_table.py
--rw-r--r--   0        0        0      384 2024-04-01 00:37:40.166398 migreat_cli-0.2.1/src/migreat/example/svc2/Dockerfile
--rw-r--r--   0        0        0      320 2024-04-01 00:37:40.166398 migreat_cli-0.2.1/src/migreat/example/svc2/MiGreat.yaml
--rw-r--r--   0        0        0       17 2024-04-01 00:37:40.166398 migreat_cli-0.2.1/src/migreat/example/svc2/requirements.txt
--rwxr-xr-x   0        0        0      240 2024-04-01 00:37:40.166398 migreat_cli-0.2.1/src/migreat/example/svc2/start.sh
--rw-r--r--   0        0        0      324 2024-04-01 00:37:40.166398 migreat_cli-0.2.1/src/migreat/example/svc2/versions/0001_create_fun_table.py
--rw-r--r--   0        0        0     1087 2024-04-01 00:37:40.166398 migreat_cli-0.2.1/src/migreat/templates/MiGreat.yaml
--rw-r--r--   0        0        0      622 2024-04-01 00:37:40.166398 migreat_cli-0.2.1/src/migreat/templates/migrator.tmpl
--rw-r--r--   0        0        0     8309 1970-01-01 00:00:00.000000 migreat_cli-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-03 20:19:23.019521 migreat_cli-0.2.3/LICENSE
+-rw-r--r--   0        0        0     7738 2024-04-03 20:19:23.019521 migreat_cli-0.2.3/README.md
+-rw-r--r--   0        0        0      563 2024-04-03 20:19:23.019521 migreat_cli-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0    23316 2024-04-03 20:19:23.019521 migreat_cli-0.2.3/src/migreat/MiGreat.py
+-rw-r--r--   0        0        0       23 2024-04-03 20:19:23.019521 migreat_cli-0.2.3/src/migreat/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 20:19:23.019521 migreat_cli-0.2.3/src/migreat/bin/__init__.py
+-rw-r--r--   0        0        0       66 2024-04-03 20:19:23.019521 migreat_cli-0.2.3/src/migreat/bin/migreat
+-rw-r--r--   0        0        0      105 2024-04-03 20:19:23.019521 migreat_cli-0.2.3/src/migreat/bin/migreat.py
+-rw-r--r--   0        0        0      952 2024-04-03 20:19:23.019521 migreat_cli-0.2.3/src/migreat/example/docker-compose.yml
+-rw-r--r--   0        0        0      371 2024-04-03 20:19:23.019521 migreat_cli-0.2.3/src/migreat/example/svc1/Dockerfile
+-rw-r--r--   0        0        0      303 2024-04-03 20:19:23.019521 migreat_cli-0.2.3/src/migreat/example/svc1/MiGreat.yaml
+-rw-r--r--   0        0        0       17 2024-04-03 20:19:23.019521 migreat_cli-0.2.3/src/migreat/example/svc1/requirements.txt
+-rw-r--r--   0        0        0      338 2024-04-03 20:19:23.019521 migreat_cli-0.2.3/src/migreat/example/svc1/versions/0001_create_user_table.py
+-rw-r--r--   0        0        0      251 2024-04-03 20:19:23.019521 migreat_cli-0.2.3/src/migreat/example/svc1/versions/0002_create_enum_type.py
+-rw-r--r--   0        0        0      129 2024-04-03 20:19:23.019521 migreat_cli-0.2.3/src/migreat/example/svc1/versions/0003_alter_enum_type.py
+-rw-r--r--   0        0        0      492 2024-04-03 20:19:23.019521 migreat_cli-0.2.3/src/migreat/example/svc1/versions/0004_create_shared_table.py
+-rw-r--r--   0        0        0      384 2024-04-03 20:19:23.019521 migreat_cli-0.2.3/src/migreat/example/svc2/Dockerfile
+-rw-r--r--   0        0        0      320 2024-04-03 20:19:23.019521 migreat_cli-0.2.3/src/migreat/example/svc2/MiGreat.yaml
+-rw-r--r--   0        0        0       17 2024-04-03 20:19:23.019521 migreat_cli-0.2.3/src/migreat/example/svc2/requirements.txt
+-rwxr-xr-x   0        0        0      240 2024-04-03 20:19:23.019521 migreat_cli-0.2.3/src/migreat/example/svc2/start.sh
+-rw-r--r--   0        0        0      324 2024-04-03 20:19:23.019521 migreat_cli-0.2.3/src/migreat/example/svc2/versions/0001_create_fun_table.py
+-rw-r--r--   0        0        0     1087 2024-04-03 20:19:23.019521 migreat_cli-0.2.3/src/migreat/templates/MiGreat.yaml
+-rw-r--r--   0        0        0      622 2024-04-03 20:19:23.019521 migreat_cli-0.2.3/src/migreat/templates/migrator.tmpl
+-rw-r--r--   0        0        0     8444 1970-01-01 00:00:00.000000 migreat_cli-0.2.3/PKG-INFO
```

### Comparing `migreat_cli-0.2.1/LICENSE` & `migreat_cli-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `migreat_cli-0.2.1/README.md` & `migreat_cli-0.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,18 @@
 # Wraps the entire upgrade process in a PG advisory lock, ensuring mutual exclusion on concurrent
 # migrators.
 use_advisory_lock: false
 ```
 
 `legacy_sqlalchemy` assumes the pre v2 way of writing SQL queries (meaning, largely, they don't need to be wrapped in `text()`).  The other options should be fairly self explanatory.
 
+Adjusting log level:
+
+Set `MIGREAT_LOG_LEVEL` environment variable to one of `error`, `warning`, `info`, `debug`.  Default is `info`.
+
 ## FAQ
 ---
 
 Q) Why called migreat?
 
 A) Because this functionality is great... why else :)
```

### Comparing `migreat_cli-0.2.1/pyproject.toml` & `migreat_cli-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "MiGreat-cli"
-version = "0.2.1"
+version = "0.2.3"
 description = "A schema isolated Postgres migrator for shared database micro services"
 authors = ["Flying Hashibuto <hashibuto@noreply.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "migreat", from = "src" }]
 
 [tool.poetry.scripts]
```

### Comparing `migreat_cli-0.2.1/src/migreat/MiGreat.py` & `migreat_cli-0.2.3/src/migreat/MiGreat.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,29 @@
 from sqlalchemy.exc import OperationalError
 from sqlalchemy.orm import Session
 import sys
 import random
 import time
 import yaml
 
+LOG_LEVEL = os.getenv("MIGREAT_LOG_LEVEL", "info")
+
+log_level = None
+if LOG_LEVEL == "error":
+    log_level = logging.ERROR
+elif LOG_LEVEL == "warning":
+    log_level = logging.WARNING
+elif LOG_LEVEL == "info":
+    log_level = logging.INFO
+else:
+    log_level = logging.DEBUG
+
 # Log config
 logger = logging.getLogger('MiGreat')
-logger.setLevel(logging.INFO)
+logger.setLevel(log_level)
 ch = logging.StreamHandler()
 ch.setFormatter(logging.Formatter("%(levelname)s: %(asctime)s - %(message)s"))
 logger.addHandler(ch)
 
 
 class Config(BaseModel):
     """
```

### Comparing `migreat_cli-0.2.1/src/migreat/example/docker-compose.yml` & `migreat_cli-0.2.3/src/migreat/example/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `migreat_cli-0.2.1/src/migreat/templates/MiGreat.yaml` & `migreat_cli-0.2.3/src/migreat/templates/MiGreat.yaml`

 * *Files identical despite different names*

### Comparing `migreat_cli-0.2.1/src/migreat/templates/migrator.tmpl` & `migreat_cli-0.2.3/src/migreat/templates/migrator.tmpl`

 * *Files identical despite different names*

### Comparing `migreat_cli-0.2.1/PKG-INFO` & `migreat_cli-0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MiGreat-cli
-Version: 0.2.1
+Version: 0.2.3
 Summary: A schema isolated Postgres migrator for shared database micro services
 License: MIT
 Author: Flying Hashibuto
 Author-email: hashibuto@noreply.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -135,14 +135,18 @@
 # Wraps the entire upgrade process in a PG advisory lock, ensuring mutual exclusion on concurrent
 # migrators.
 use_advisory_lock: false
 ```
 
 `legacy_sqlalchemy` assumes the pre v2 way of writing SQL queries (meaning, largely, they don't need to be wrapped in `text()`).  The other options should be fairly self explanatory.
 
+Adjusting log level:
+
+Set `MIGREAT_LOG_LEVEL` environment variable to one of `error`, `warning`, `info`, `debug`.  Default is `info`.
+
 ## FAQ
 ---
 
 Q) Why called migreat?
 
 A) Because this functionality is great... why else :)
```

