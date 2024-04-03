# Comparing `tmp/pytest_pg-0.0.8.tar.gz` & `tmp/pytest_pg-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_pg-0.0.8.tar", last modified: Sun Dec 26 10:32:14 2021, max compression
+gzip compressed data, was "pytest_pg-0.0.9.tar", last modified: Tue Dec 28 09:03:47 2021, max compression
```

## Comparing `pytest_pg-0.0.8.tar` & `pytest_pg-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-26 10:32:14.194057 pytest_pg-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2021-12-26 10:32:03.000000 pytest_pg-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1266 2021-12-26 10:32:14.194057 pytest_pg-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-12-26 10:32:03.000000 pytest_pg-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-26 10:32:14.194057 pytest_pg-0.0.8/pytest_pg/
--rw-r--r--   0 runner    (1001) docker     (121)     1227 2021-12-26 10:32:03.000000 pytest_pg-0.0.8/pytest_pg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2021-12-26 10:32:03.000000 pytest_pg-0.0.8/pytest_pg/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (121)     2230 2021-12-26 10:32:03.000000 pytest_pg-0.0.8/pytest_pg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-26 10:32:14.194057 pytest_pg-0.0.8/pytest_pg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1266 2021-12-26 10:32:14.000000 pytest_pg-0.0.8/pytest_pg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      305 2021-12-26 10:32:14.000000 pytest_pg-0.0.8/pytest_pg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-26 10:32:14.000000 pytest_pg-0.0.8/pytest_pg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       34 2021-12-26 10:32:14.000000 pytest_pg-0.0.8/pytest_pg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-12-26 10:32:14.000000 pytest_pg-0.0.8/pytest_pg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-12-26 10:32:14.000000 pytest_pg-0.0.8/pytest_pg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-26 10:32:14.194057 pytest_pg-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2134 2021-12-26 10:32:03.000000 pytest_pg-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 09:03:47.505980 pytest_pg-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1068 2021-12-28 09:03:36.000000 pytest_pg-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1367 2021-12-28 09:03:47.505980 pytest_pg-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2021-12-28 09:03:36.000000 pytest_pg-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 09:03:47.501980 pytest_pg-0.0.9/pytest_pg/
+-rw-r--r--   0 runner    (1001) docker     (121)     1227 2021-12-28 09:03:36.000000 pytest_pg-0.0.9/pytest_pg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2617 2021-12-28 09:03:36.000000 pytest_pg-0.0.9/pytest_pg/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2230 2021-12-28 09:03:36.000000 pytest_pg-0.0.9/pytest_pg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 09:03:47.505980 pytest_pg-0.0.9/pytest_pg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1367 2021-12-28 09:03:47.000000 pytest_pg-0.0.9/pytest_pg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      305 2021-12-28 09:03:47.000000 pytest_pg-0.0.9/pytest_pg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-28 09:03:47.000000 pytest_pg-0.0.9/pytest_pg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2021-12-28 09:03:47.000000 pytest_pg-0.0.9/pytest_pg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2021-12-28 09:03:47.000000 pytest_pg-0.0.9/pytest_pg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2021-12-28 09:03:47.000000 pytest_pg-0.0.9/pytest_pg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-28 09:03:47.505980 pytest_pg-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2134 2021-12-28 09:03:36.000000 pytest_pg-0.0.9/setup.py
```

### Comparing `pytest_pg-0.0.8/LICENSE` & `pytest_pg-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_pg-0.0.8/PKG-INFO` & `pytest_pg-0.0.9/pytest_pg.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pytest_pg
-Version: 0.0.8
+Name: pytest-pg
+Version: 0.0.9
 Summary: Helps to run PostgreSQL in docker as pytest fixture
 Home-page: https://github.com/anna-money/pytest-pg
 Author: Yury Pliner
 Author-email: yury.pliner@gmail.com
 License: MIT
 Platform: macOS
 Platform: POSIX
@@ -21,14 +21,19 @@
 Classifier: Framework :: Pytest
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pytest-pg
 
+## v0.0.9 (2021-12-28)
+
+* Disable fsync, full_page_writes, synchronous_commit to speedup the tests
+
+
 ## v0.0.8 (2021-12-26)
 
 * Add typing marker, mypy. Run tests in CI
 
 
 ## v0.0.7 (2021-12-25)
```

### Comparing `pytest_pg-0.0.8/pytest_pg/__init__.py` & `pytest_pg-0.0.9/pytest_pg/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 from typing import Tuple
 
 from .fixtures import PG, pg, pg_11, pg_12, pg_13, pg_14, run_pg  # noqa
 
 __all__: Tuple[str, ...] = ("PG", "run_pg", "pg", "pg_11", "pg_12", "pg_13", "pg_14")
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 version = f"{__version__}, Python {sys.version}"
 
 VersionInfo = collections.namedtuple("VersionInfo", "major minor micro release_level serial")
 
 
 def _parse_version(v: str) -> VersionInfo:
```

### Comparing `pytest_pg-0.0.8/pytest_pg/fixtures.py` & `pytest_pg-0.0.9/pytest_pg/fixtures.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     container = docker_client.create_container(
         image=image,
         name=f"pytest-pg-{uuid.uuid4()}",
         ports=[5432],
         detach=True,
         host_config=docker_client.create_host_config(port_bindings={5432: (LOCALHOST, unused_port)}),
         environment={"POSTGRES_HOST_AUTH_METHOD": "trust"},
+        command="-c fsync=off -c full_page_writes=off -c synchronous_commit=off",
     )
 
     try:
         docker_client.start(container=container["Id"])
 
         started_at = time.time()
```

### Comparing `pytest_pg-0.0.8/pytest_pg/utils.py` & `pytest_pg-0.0.9/pytest_pg/utils.py`

 * *Files identical despite different names*

### Comparing `pytest_pg-0.0.8/pytest_pg.egg-info/PKG-INFO` & `pytest_pg-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pytest-pg
-Version: 0.0.8
+Name: pytest_pg
+Version: 0.0.9
 Summary: Helps to run PostgreSQL in docker as pytest fixture
 Home-page: https://github.com/anna-money/pytest-pg
 Author: Yury Pliner
 Author-email: yury.pliner@gmail.com
 License: MIT
 Platform: macOS
 Platform: POSIX
@@ -21,14 +21,19 @@
 Classifier: Framework :: Pytest
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pytest-pg
 
+## v0.0.9 (2021-12-28)
+
+* Disable fsync, full_page_writes, synchronous_commit to speedup the tests
+
+
 ## v0.0.8 (2021-12-26)
 
 * Add typing marker, mypy. Run tests in CI
 
 
 ## v0.0.7 (2021-12-25)
```

### Comparing `pytest_pg-0.0.8/setup.py` & `pytest_pg-0.0.9/setup.py`

 * *Files identical despite different names*

