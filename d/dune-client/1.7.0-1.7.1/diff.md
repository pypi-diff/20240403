# Comparing `tmp/dune_client-1.7.0.tar.gz` & `tmp/dune_client-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_client-1.7.0.tar", last modified: Tue Apr  2 12:09:40 2024, max compression
+gzip compressed data, was "dune_client-1.7.1.tar", last modified: Wed Apr  3 18:44:49 2024, max compression
```

## Comparing `dune_client-1.7.0.tar` & `dune_client-1.7.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:40.863785 dune_client-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-02 12:09:33.000000 dune_client-1.7.0/.env.sample
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:40.851785 dune_client-1.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:40.855785 dune_client-1.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-02 12:09:33.000000 dune_client-1.7.0/.github/workflows/pull-request.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-02 12:09:33.000000 dune_client-1.7.0/.github/workflows/py-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-02 12:09:33.000000 dune_client-1.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-02 12:09:33.000000 dune_client-1.7.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-02 12:09:33.000000 dune_client-1.7.0/COPYRIGHT.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 12:09:33.000000 dune_client-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-02 12:09:33.000000 dune_client-1.7.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-04-02 12:09:40.863785 dune_client-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-04-02 12:09:33.000000 dune_client-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:40.855785 dune_client-1.7.0/dune_client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:40.859785 dune_client-1.7.0/dune_client/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/api/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7356 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/api/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)    16080 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/api/extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/api/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/api/table.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    20167 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/client_async.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:40.859785 dune_client-1.7.0/dune_client/file/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/file/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/file/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    11897 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     6559 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:40.859785 dune_client-1.7.0/dune_client/viz/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/viz/graphs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:40.863785 dune_client-1.7.0/dune_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-04-02 12:09:40.000000 dune_client-1.7.0/dune_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-02 12:09:40.000000 dune_client-1.7.0/dune_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 12:09:40.000000 dune_client-1.7.0/dune_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 12:09:40.000000 dune_client-1.7.0/dune_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-02 12:09:40.000000 dune_client-1.7.0/dune_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 12:09:40.000000 dune_client-1.7.0/dune_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-02 12:09:33.000000 dune_client-1.7.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:40.859785 dune_client-1.7.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-02 12:09:33.000000 dune_client-1.7.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-02 12:09:33.000000 dune_client-1.7.0/requirements/prod.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-02 12:09:40.863785 dune_client-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 12:09:33.000000 dune_client-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:40.851785 dune_client-1.7.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:40.859785 dune_client-1.7.0/tests/e2e/
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-02 12:09:33.000000 dune_client-1.7.0/tests/e2e/test_async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16613 2024-04-02 12:09:33.000000 dune_client-1.7.0/tests/e2e/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:40.859785 dune_client-1.7.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 12:09:33.000000 dune_client-1.7.0/tests/fixtures/sample_table_insert.csv
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 12:09:33.000000 dune_client-1.7.0/tests/fixtures/sample_table_insert.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:40.863785 dune_client-1.7.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-04-02 12:09:33.000000 dune_client-1.7.0/tests/unit/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-04-02 12:09:33.000000 dune_client-1.7.0/tests/unit/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-02 12:09:33.000000 dune_client-1.7.0/tests/unit/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-02 12:09:33.000000 dune_client-1.7.0/tests/unit/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-02 12:09:33.000000 dune_client-1.7.0/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-02 12:09:33.000000 dune_client-1.7.0/tests/unit/test_viz_sankey.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:44:49.077237 dune_client-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-03 18:44:42.000000 dune_client-1.7.1/.env.sample
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:44:49.065237 dune_client-1.7.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:44:49.069237 dune_client-1.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-03 18:44:42.000000 dune_client-1.7.1/.github/workflows/pull-request.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-03 18:44:42.000000 dune_client-1.7.1/.github/workflows/py-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 18:44:42.000000 dune_client-1.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-03 18:44:42.000000 dune_client-1.7.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-03 18:44:42.000000 dune_client-1.7.1/COPYRIGHT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-03 18:44:42.000000 dune_client-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-03 18:44:42.000000 dune_client-1.7.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-04-03 18:44:49.077237 dune_client-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-04-03 18:44:42.000000 dune_client-1.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:44:49.069237 dune_client-1.7.1/dune_client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:44:42.000000 dune_client-1.7.1/dune_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:44:49.073238 dune_client-1.7.1/dune_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:44:42.000000 dune_client-1.7.1/dune_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-04-03 18:44:42.000000 dune_client-1.7.1/dune_client/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7356 2024-04-03 18:44:42.000000 dune_client-1.7.1/dune_client/api/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16080 2024-04-03 18:44:42.000000 dune_client-1.7.1/dune_client/api/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-04-03 18:44:42.000000 dune_client-1.7.1/dune_client/api/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-03 18:44:42.000000 dune_client-1.7.1/dune_client/api/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-03 18:44:42.000000 dune_client-1.7.1/dune_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20167 2024-04-03 18:44:42.000000 dune_client-1.7.1/dune_client/client_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:44:49.073238 dune_client-1.7.1/dune_client/file/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:44:42.000000 dune_client-1.7.1/dune_client/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-03 18:44:42.000000 dune_client-1.7.1/dune_client/file/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-04-03 18:44:42.000000 dune_client-1.7.1/dune_client/file/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-03 18:44:42.000000 dune_client-1.7.1/dune_client/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11897 2024-04-03 18:44:42.000000 dune_client-1.7.1/dune_client/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:44:42.000000 dune_client-1.7.1/dune_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-03 18:44:42.000000 dune_client-1.7.1/dune_client/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6559 2024-04-03 18:44:42.000000 dune_client-1.7.1/dune_client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-03 18:44:42.000000 dune_client-1.7.1/dune_client/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:44:49.073238 dune_client-1.7.1/dune_client/viz/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:44:42.000000 dune_client-1.7.1/dune_client/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-03 18:44:42.000000 dune_client-1.7.1/dune_client/viz/graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:44:49.073238 dune_client-1.7.1/dune_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-04-03 18:44:49.000000 dune_client-1.7.1/dune_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-03 18:44:49.000000 dune_client-1.7.1/dune_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:44:49.000000 dune_client-1.7.1/dune_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:44:49.000000 dune_client-1.7.1/dune_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-03 18:44:49.000000 dune_client-1.7.1/dune_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 18:44:49.000000 dune_client-1.7.1/dune_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-03 18:44:42.000000 dune_client-1.7.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:44:49.073238 dune_client-1.7.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-03 18:44:42.000000 dune_client-1.7.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-03 18:44:42.000000 dune_client-1.7.1/requirements/prod.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-03 18:44:49.077237 dune_client-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-03 18:44:42.000000 dune_client-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:44:49.065237 dune_client-1.7.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:44:49.073238 dune_client-1.7.1/tests/e2e/
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-03 18:44:42.000000 dune_client-1.7.1/tests/e2e/test_async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16613 2024-04-03 18:44:42.000000 dune_client-1.7.1/tests/e2e/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:44:49.073238 dune_client-1.7.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-03 18:44:42.000000 dune_client-1.7.1/tests/fixtures/sample_table_insert.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-03 18:44:42.000000 dune_client-1.7.1/tests/fixtures/sample_table_insert.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:44:49.073238 dune_client-1.7.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-04-03 18:44:42.000000 dune_client-1.7.1/tests/unit/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-04-03 18:44:42.000000 dune_client-1.7.1/tests/unit/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-03 18:44:42.000000 dune_client-1.7.1/tests/unit/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-03 18:44:42.000000 dune_client-1.7.1/tests/unit/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-03 18:44:42.000000 dune_client-1.7.1/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-03 18:44:42.000000 dune_client-1.7.1/tests/unit/test_viz_sankey.py
```

### Comparing `dune_client-1.7.0/.github/workflows/pull-request.yaml` & `dune_client-1.7.1/.github/workflows/pull-request.yaml`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.0/.github/workflows/py-publish.yaml` & `dune_client-1.7.1/.github/workflows/py-publish.yaml`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.0/LICENSE` & `dune_client-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.0/PKG-INFO` & `dune_client-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune_client
-Version: 1.7.0
+Version: 1.7.1
 Summary: A simple framework for interacting with Dune Analytics official API service.
 Home-page: https://github.com/duneanalytics/dune-client
 Author: Benjamin H. Smith & Dune Analytics
 Author-email: ben@cow.fi
 License: Apache License Version 2.0
 Project-URL: Tracker, https://github.com/duneanalytics/dune-client/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dune_client-1.7.0/README.md` & `dune_client-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.0/dune_client/api/base.py` & `dune_client-1.7.1/dune_client/api/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,21 +108,15 @@
             sample_count is None
             # We are sampling and don't use filters or pagination
             or (limit is None and offset is None and filters is None)
         ), "sampling cannot be combined with filters or pagination"
 
         params = params or {}
         if columns is not None and len(columns) > 0:
-            output = []
-            for column in columns:
-                # Escape all quotes and add quotes around it
-                col = '"' + column.replace('"', '\\"') + '"'
-                output.append(col)
-
-            params["columns"] = ",".join(output)
+            params["columns"] = ",".join(columns)
         if sample_count is not None:
             params["sample_count"] = sample_count
         if filters is not None:
             params["filters"] = filters
         if sort_by is not None and len(sort_by) > 0:
             params["sort_by"] = ",".join(sort_by)
         if limit is not None:
```

### Comparing `dune_client-1.7.0/dune_client/api/execution.py` & `dune_client-1.7.1/dune_client/api/execution.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.0/dune_client/api/extensions.py` & `dune_client-1.7.1/dune_client/api/extensions.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.0/dune_client/api/query.py` & `dune_client-1.7.1/dune_client/api/query.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.0/dune_client/api/table.py` & `dune_client-1.7.1/dune_client/api/table.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.0/dune_client/client.py` & `dune_client-1.7.1/dune_client/client.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.0/dune_client/client_async.py` & `dune_client-1.7.1/dune_client/client_async.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.0/dune_client/file/base.py` & `dune_client-1.7.1/dune_client/file/base.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.0/dune_client/file/interface.py` & `dune_client-1.7.1/dune_client/file/interface.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.0/dune_client/interface.py` & `dune_client-1.7.1/dune_client/interface.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.0/dune_client/models.py` & `dune_client-1.7.1/dune_client/models.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.0/dune_client/query.py` & `dune_client-1.7.1/dune_client/query.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.0/dune_client/types.py` & `dune_client-1.7.1/dune_client/types.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.0/dune_client/util.py` & `dune_client-1.7.1/dune_client/util.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.0/dune_client/viz/graphs.py` & `dune_client-1.7.1/dune_client/viz/graphs.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.0/dune_client.egg-info/PKG-INFO` & `dune_client-1.7.1/dune_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune_client
-Version: 1.7.0
+Version: 1.7.1
 Summary: A simple framework for interacting with Dune Analytics official API service.
 Home-page: https://github.com/duneanalytics/dune-client
 Author: Benjamin H. Smith & Dune Analytics
 Author-email: ben@cow.fi
 License: Apache License Version 2.0
 Project-URL: Tracker, https://github.com/duneanalytics/dune-client/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dune_client-1.7.0/dune_client.egg-info/SOURCES.txt` & `dune_client-1.7.1/dune_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.0/setup.cfg` & `dune_client-1.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.0/tests/e2e/test_async_client.py` & `dune_client-1.7.1/tests/e2e/test_async_client.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.0/tests/e2e/test_client.py` & `dune_client-1.7.1/tests/e2e/test_client.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.0/tests/unit/test_file.py` & `dune_client-1.7.1/tests/unit/test_file.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.0/tests/unit/test_models.py` & `dune_client-1.7.1/tests/unit/test_models.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.0/tests/unit/test_query.py` & `dune_client-1.7.1/tests/unit/test_query.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.0/tests/unit/test_types.py` & `dune_client-1.7.1/tests/unit/test_types.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.0/tests/unit/test_utils.py` & `dune_client-1.7.1/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.0/tests/unit/test_viz_sankey.py` & `dune_client-1.7.1/tests/unit/test_viz_sankey.py`

 * *Files identical despite different names*

