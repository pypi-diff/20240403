# Comparing `tmp/maap_jupyter_server_extension-1.3.0.tar.gz` & `tmp/maap_jupyter_server_extension-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maap_jupyter_server_extension-1.3.0.tar", last modified: Mon Mar 18 18:10:00 2024, max compression
+gzip compressed data, was "maap_jupyter_server_extension-1.3.4.tar", last modified: Wed Apr  3 20:19:40 2024, max compression
```

## Comparing `maap_jupyter_server_extension-1.3.0.tar` & `maap_jupyter_server_extension-1.3.4.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 mlucas     (503) staff       (20)        0 2024-03-18 18:10:00.237239 maap_jupyter_server_extension-1.3.0/
--rw-r--r--   0 mlucas     (503) staff       (20)       86 2022-07-22 16:01:37.000000 maap_jupyter_server_extension-1.3.0/CHANGELOG.md
--rw-r--r--   0 mlucas     (503) staff       (20)    10988 2023-02-13 22:24:25.000000 maap_jupyter_server_extension-1.3.0/LICENSE
--rw-r--r--   0 mlucas     (503) staff       (20)      512 2022-09-16 17:04:10.000000 maap_jupyter_server_extension-1.3.0/MANIFEST.in
--rw-r--r--   0 mlucas     (503) staff       (20)     5091 2024-03-18 18:10:00.236998 maap_jupyter_server_extension-1.3.0/PKG-INFO
--rw-r--r--   0 mlucas     (503) staff       (20)     3763 2023-01-20 01:31:26.000000 maap_jupyter_server_extension-1.3.0/README.md
--rw-r--r--   0 mlucas     (503) staff       (20)      211 2022-08-17 17:39:04.000000 maap_jupyter_server_extension-1.3.0/conftest.py
--rw-r--r--   0 mlucas     (503) staff       (20)      209 2022-08-17 17:39:15.000000 maap_jupyter_server_extension-1.3.0/install.json
-drwxr-xr-x   0 mlucas     (503) staff       (20)        0 2024-03-18 18:10:00.227248 maap_jupyter_server_extension-1.3.0/jupyter-config/
-drwxr-xr-x   0 mlucas     (503) staff       (20)        0 2024-03-18 18:10:00.230148 maap_jupyter_server_extension-1.3.0/jupyter-config/nb-config/
--rw-r--r--   0 mlucas     (503) staff       (20)      101 2022-08-17 17:42:45.000000 maap_jupyter_server_extension-1.3.0/jupyter-config/nb-config/dps_jupyter_server_extension.json
-drwxr-xr-x   0 mlucas     (503) staff       (20)        0 2024-03-18 18:10:00.230367 maap_jupyter_server_extension-1.3.0/jupyter-config/server-config/
--rw-r--r--   0 mlucas     (503) staff       (20)       99 2022-08-17 17:42:45.000000 maap_jupyter_server_extension-1.3.0/jupyter-config/server-config/dps_jupyter_server_extension.json
-drwxr-xr-x   0 mlucas     (503) staff       (20)        0 2024-03-18 18:10:00.231057 maap_jupyter_server_extension-1.3.0/jupyter_server_extension/
--rw-r--r--   0 mlucas     (503) staff       (20)     1007 2022-08-17 18:22:56.000000 maap_jupyter_server_extension-1.3.0/jupyter_server_extension/__init__.py
--rw-r--r--   0 mlucas     (503) staff       (20)      624 2022-08-17 18:21:56.000000 maap_jupyter_server_extension-1.3.0/jupyter_server_extension/_version.py
--rw-r--r--   0 mlucas     (503) staff       (20)    25136 2024-03-18 18:03:37.000000 maap_jupyter_server_extension-1.3.0/jupyter_server_extension/handlers.py
-drwxr-xr-x   0 mlucas     (503) staff       (20)        0 2024-03-18 18:10:00.231706 maap_jupyter_server_extension-1.3.0/jupyter_server_extension/labextension/
--rw-r--r--   0 mlucas     (503) staff       (20)    21481 2024-03-18 18:09:18.000000 maap_jupyter_server_extension-1.3.0/jupyter_server_extension/labextension/build_log.json
--rw-r--r--   0 mlucas     (503) staff       (20)     2891 2024-03-18 18:09:19.000000 maap_jupyter_server_extension-1.3.0/jupyter_server_extension/labextension/package.json
-drwxr-xr-x   0 mlucas     (503) staff       (20)        0 2024-03-18 18:10:00.233717 maap_jupyter_server_extension-1.3.0/jupyter_server_extension/labextension/static/
--rw-r--r--   0 mlucas     (503) staff       (20)     3775 2024-03-18 18:09:19.000000 maap_jupyter_server_extension-1.3.0/jupyter_server_extension/labextension/static/lib_index_js.f3563370867954312194.js
--rw-r--r--   0 mlucas     (503) staff       (20)     2459 2024-03-18 18:09:19.000000 maap_jupyter_server_extension-1.3.0/jupyter_server_extension/labextension/static/lib_index_js.f3563370867954312194.js.map
--rw-r--r--   0 mlucas     (503) staff       (20)    28202 2024-03-18 18:09:19.000000 maap_jupyter_server_extension-1.3.0/jupyter_server_extension/labextension/static/remoteEntry.6f9394f1d8ef18e972d0.js
--rw-r--r--   0 mlucas     (503) staff       (20)    27139 2024-03-18 18:09:19.000000 maap_jupyter_server_extension-1.3.0/jupyter_server_extension/labextension/static/remoteEntry.6f9394f1d8ef18e972d0.js.map
--rw-r--r--   0 mlucas     (503) staff       (20)      172 2024-03-18 18:09:18.000000 maap_jupyter_server_extension-1.3.0/jupyter_server_extension/labextension/static/style.js
--rw-r--r--   0 mlucas     (503) staff       (20)     4630 2024-03-18 18:09:19.000000 maap_jupyter_server_extension-1.3.0/jupyter_server_extension/labextension/static/style_index_js.985542941dd18f4568ee.js
--rw-r--r--   0 mlucas     (503) staff       (20)     1832 2024-03-18 18:09:19.000000 maap_jupyter_server_extension-1.3.0/jupyter_server_extension/labextension/static/style_index_js.985542941dd18f4568ee.js.map
--rw-r--r--   0 mlucas     (503) staff       (20)    12088 2024-03-18 18:09:19.000000 maap_jupyter_server_extension-1.3.0/jupyter_server_extension/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.265412ff30d319ce76fc.js
--rw-r--r--   0 mlucas     (503) staff       (20)    13835 2024-03-18 18:09:19.000000 maap_jupyter_server_extension-1.3.0/jupyter_server_extension/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.265412ff30d319ce76fc.js.map
-drwxr-xr-x   0 mlucas     (503) staff       (20)        0 2024-03-18 18:10:00.236479 maap_jupyter_server_extension-1.3.0/maap_jupyter_server_extension.egg-info/
--rw-r--r--   0 mlucas     (503) staff       (20)     5091 2024-03-18 18:10:00.000000 maap_jupyter_server_extension-1.3.0/maap_jupyter_server_extension.egg-info/PKG-INFO
--rw-r--r--   0 mlucas     (503) staff       (20)     1749 2024-03-18 18:10:00.000000 maap_jupyter_server_extension-1.3.0/maap_jupyter_server_extension.egg-info/SOURCES.txt
--rw-r--r--   0 mlucas     (503) staff       (20)        1 2024-03-18 18:10:00.000000 maap_jupyter_server_extension-1.3.0/maap_jupyter_server_extension.egg-info/dependency_links.txt
--rw-r--r--   0 mlucas     (503) staff       (20)        1 2024-03-18 18:08:32.000000 maap_jupyter_server_extension-1.3.0/maap_jupyter_server_extension.egg-info/not-zip-safe
--rw-r--r--   0 mlucas     (503) staff       (20)       90 2024-03-18 18:10:00.000000 maap_jupyter_server_extension-1.3.0/maap_jupyter_server_extension.egg-info/requires.txt
--rw-r--r--   0 mlucas     (503) staff       (20)       25 2024-03-18 18:10:00.000000 maap_jupyter_server_extension-1.3.0/maap_jupyter_server_extension.egg-info/top_level.txt
--rw-r--r--   0 mlucas     (503) staff       (20)     2749 2024-03-18 18:03:52.000000 maap_jupyter_server_extension-1.3.0/package.json
--rw-r--r--   0 mlucas     (503) staff       (20)      631 2023-03-30 20:17:57.000000 maap_jupyter_server_extension-1.3.0/pyproject.toml
--rw-r--r--   0 mlucas     (503) staff       (20)       38 2024-03-18 18:10:00.237287 maap_jupyter_server_extension-1.3.0/setup.cfg
--rw-r--r--   0 mlucas     (503) staff       (20)     3433 2024-03-15 20:51:32.000000 maap_jupyter_server_extension-1.3.0/setup.py
-drwxr-xr-x   0 mlucas     (503) staff       (20)        0 2024-03-18 18:10:00.235498 maap_jupyter_server_extension-1.3.0/src/
--rw-r--r--   0 mlucas     (503) staff       (20)     1111 2022-08-17 17:56:43.000000 maap_jupyter_server_extension-1.3.0/src/handler.ts
--rw-r--r--   0 mlucas     (503) staff       (20)      716 2022-08-17 17:56:43.000000 maap_jupyter_server_extension-1.3.0/src/index.ts
-drwxr-xr-x   0 mlucas     (503) staff       (20)        0 2024-03-18 18:10:00.236215 maap_jupyter_server_extension-1.3.0/style/
--rw-r--r--   0 mlucas     (503) staff       (20)      138 2022-07-22 16:01:37.000000 maap_jupyter_server_extension-1.3.0/style/base.css
--rw-r--r--   0 mlucas     (503) staff       (20)       25 2022-07-22 16:01:37.000000 maap_jupyter_server_extension-1.3.0/style/index.css
--rw-r--r--   0 mlucas     (503) staff       (20)       21 2022-07-22 16:01:37.000000 maap_jupyter_server_extension-1.3.0/style/index.js
--rw-r--r--   0 mlucas     (503) staff       (20)      669 2023-06-05 20:12:23.000000 maap_jupyter_server_extension-1.3.0/tsconfig.json
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-03 20:19:40.399308 maap_jupyter_server_extension-1.3.4/
+-rw-r--r--   0 root         (0) staff       (20)       86 2024-03-07 17:56:57.000000 maap_jupyter_server_extension-1.3.4/CHANGELOG.md
+-rw-r--r--   0 root         (0) staff       (20)    10988 2024-03-07 17:56:57.000000 maap_jupyter_server_extension-1.3.4/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)      512 2024-03-07 17:56:57.000000 maap_jupyter_server_extension-1.3.4/MANIFEST.in
+-rw-r--r--   0 root         (0) staff       (20)     5124 2024-04-03 20:19:40.398870 maap_jupyter_server_extension-1.3.4/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     3763 2024-03-07 17:56:57.000000 maap_jupyter_server_extension-1.3.4/README.md
+-rw-r--r--   0 root         (0) staff       (20)      211 2024-03-07 17:56:57.000000 maap_jupyter_server_extension-1.3.4/conftest.py
+-rw-r--r--   0 root         (0) staff       (20)      209 2024-03-07 17:56:57.000000 maap_jupyter_server_extension-1.3.4/install.json
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-03 20:19:40.374415 maap_jupyter_server_extension-1.3.4/jupyter-config/
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-03 20:19:40.384964 maap_jupyter_server_extension-1.3.4/jupyter-config/nb-config/
+-rw-r--r--   0 root         (0) staff       (20)      101 2024-03-07 17:56:57.000000 maap_jupyter_server_extension-1.3.4/jupyter-config/nb-config/dps_jupyter_server_extension.json
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-03 20:19:40.385966 maap_jupyter_server_extension-1.3.4/jupyter-config/server-config/
+-rw-r--r--   0 root         (0) staff       (20)       99 2024-03-07 17:56:57.000000 maap_jupyter_server_extension-1.3.4/jupyter-config/server-config/dps_jupyter_server_extension.json
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-03 20:19:40.387448 maap_jupyter_server_extension-1.3.4/jupyter_server_extension/
+-rw-r--r--   0 root         (0) staff       (20)     1007 2024-03-07 17:56:57.000000 maap_jupyter_server_extension-1.3.4/jupyter_server_extension/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      624 2024-03-07 17:56:57.000000 maap_jupyter_server_extension-1.3.4/jupyter_server_extension/_version.py
+-rw-r--r--   0 root         (0) staff       (20)    25136 2024-03-18 18:15:07.000000 maap_jupyter_server_extension-1.3.4/jupyter_server_extension/handlers.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-03 20:19:40.388732 maap_jupyter_server_extension-1.3.4/jupyter_server_extension/labextension/
+-rw-r--r--   0 root         (0) staff       (20)    21943 2024-03-28 21:07:48.000000 maap_jupyter_server_extension-1.3.4/jupyter_server_extension/labextension/build_log.json
+-rw-r--r--   0 root         (0) staff       (20)     2891 2024-03-28 21:07:48.000000 maap_jupyter_server_extension-1.3.4/jupyter_server_extension/labextension/package.json
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-03 20:19:40.393209 maap_jupyter_server_extension-1.3.4/jupyter_server_extension/labextension/static/
+-rw-r--r--   0 root         (0) staff       (20)     3775 2024-03-28 21:07:48.000000 maap_jupyter_server_extension-1.3.4/jupyter_server_extension/labextension/static/lib_index_js.f3563370867954312194.js
+-rw-r--r--   0 root         (0) staff       (20)     2459 2024-03-28 21:07:48.000000 maap_jupyter_server_extension-1.3.4/jupyter_server_extension/labextension/static/lib_index_js.f3563370867954312194.js.map
+-rw-r--r--   0 root         (0) staff       (20)    28202 2024-03-28 21:07:48.000000 maap_jupyter_server_extension-1.3.4/jupyter_server_extension/labextension/static/remoteEntry.6f9394f1d8ef18e972d0.js
+-rw-r--r--   0 root         (0) staff       (20)    27139 2024-03-28 21:07:48.000000 maap_jupyter_server_extension-1.3.4/jupyter_server_extension/labextension/static/remoteEntry.6f9394f1d8ef18e972d0.js.map
+-rw-r--r--   0 root         (0) staff       (20)      172 2024-03-28 21:07:48.000000 maap_jupyter_server_extension-1.3.4/jupyter_server_extension/labextension/static/style.js
+-rw-r--r--   0 root         (0) staff       (20)     4630 2024-03-28 21:07:48.000000 maap_jupyter_server_extension-1.3.4/jupyter_server_extension/labextension/static/style_index_js.985542941dd18f4568ee.js
+-rw-r--r--   0 root         (0) staff       (20)     1832 2024-03-28 21:07:48.000000 maap_jupyter_server_extension-1.3.4/jupyter_server_extension/labextension/static/style_index_js.985542941dd18f4568ee.js.map
+-rw-r--r--   0 root         (0) staff       (20)    12088 2024-03-28 21:07:48.000000 maap_jupyter_server_extension-1.3.4/jupyter_server_extension/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.265412ff30d319ce76fc.js
+-rw-r--r--   0 root         (0) staff       (20)    13835 2024-03-28 21:07:48.000000 maap_jupyter_server_extension-1.3.4/jupyter_server_extension/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.265412ff30d319ce76fc.js.map
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-03 20:19:40.397839 maap_jupyter_server_extension-1.3.4/maap_jupyter_server_extension.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     5124 2024-04-03 20:19:40.000000 maap_jupyter_server_extension-1.3.4/maap_jupyter_server_extension.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     1759 2024-04-03 20:19:40.000000 maap_jupyter_server_extension-1.3.4/maap_jupyter_server_extension.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-04-03 20:19:40.000000 maap_jupyter_server_extension-1.3.4/maap_jupyter_server_extension.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-03-07 17:58:46.000000 maap_jupyter_server_extension-1.3.4/maap_jupyter_server_extension.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) staff       (20)      108 2024-04-03 20:19:40.000000 maap_jupyter_server_extension-1.3.4/maap_jupyter_server_extension.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       25 2024-04-03 20:19:40.000000 maap_jupyter_server_extension-1.3.4/maap_jupyter_server_extension.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)     2749 2024-04-03 20:18:11.000000 maap_jupyter_server_extension-1.3.4/package.json
+-rw-r--r--   0 root         (0) staff       (20)      631 2024-03-07 17:56:57.000000 maap_jupyter_server_extension-1.3.4/pyproject.toml
+-rw-r--r--   0 root         (0) staff       (20)       38 2024-04-03 20:19:40.399403 maap_jupyter_server_extension-1.3.4/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     3462 2024-04-03 20:18:11.000000 maap_jupyter_server_extension-1.3.4/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-03 20:19:40.395941 maap_jupyter_server_extension-1.3.4/src/
+-rw-r--r--   0 root         (0) staff       (20)     1111 2024-03-07 17:56:57.000000 maap_jupyter_server_extension-1.3.4/src/handler.ts
+-rw-r--r--   0 root         (0) staff       (20)      716 2024-03-07 17:56:57.000000 maap_jupyter_server_extension-1.3.4/src/index.ts
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-03 20:19:40.397137 maap_jupyter_server_extension-1.3.4/style/
+-rw-r--r--   0 root         (0) staff       (20)      138 2024-03-07 17:56:57.000000 maap_jupyter_server_extension-1.3.4/style/base.css
+-rw-r--r--   0 root         (0) staff       (20)       25 2024-03-07 17:56:57.000000 maap_jupyter_server_extension-1.3.4/style/index.css
+-rw-r--r--   0 root         (0) staff       (20)       21 2024-03-07 17:56:57.000000 maap_jupyter_server_extension-1.3.4/style/index.js
+-rw-r--r--   0 root         (0) staff       (20)      669 2024-03-07 17:56:57.000000 maap_jupyter_server_extension-1.3.4/tsconfig.json
+-rw-r--r--   0 root         (0) staff       (20)   230492 2024-04-03 20:18:11.000000 maap_jupyter_server_extension-1.3.4/yarn.lock
```

### Comparing `maap_jupyter_server_extension-1.3.0/LICENSE` & `maap_jupyter_server_extension-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.3.0/MANIFEST.in` & `maap_jupyter_server_extension-1.3.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.3.0/PKG-INFO` & `maap_jupyter_server_extension-1.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maap_jupyter_server_extension
-Version: 1.3.0
+Version: 1.3.4
 Summary: A JupyterLab extension.
 Home-page: https://github.com/MAAP-Project/jupyter-server-extension
 Author: Marjorie Lucas
 Author-email: marjorie.j.lucas@jpl.nasa.gov
 License: Apache 2.0
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
@@ -22,14 +22,15 @@
 Classifier: Framework :: Jupyter :: JupyterLab :: 3
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jupyter_server==2.12.5
+Requires-Dist: xmltodict==0.13.0
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-tornasync; extra == "test"
```

### Comparing `maap_jupyter_server_extension-1.3.0/README.md` & `maap_jupyter_server_extension-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.3.0/jupyter_server_extension/__init__.py` & `maap_jupyter_server_extension-1.3.4/jupyter_server_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.3.0/jupyter_server_extension/_version.py` & `maap_jupyter_server_extension-1.3.4/jupyter_server_extension/_version.py`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.3.0/jupyter_server_extension/handlers.py` & `maap_jupyter_server_extension-1.3.4/jupyter_server_extension/handlers.py`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.3.0/jupyter_server_extension/labextension/build_log.json` & `maap_jupyter_server_extension-1.3.4/jupyter_server_extension/labextension/build_log.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9828696814373897%*

 * *Differences: {'0': "{'resolve': {'alias': {'@phosphor/algorithm$': "*

 * *      "'/Users/graceal/Documents/maap/extensions/jupyter-server-extension/node_modules/@lumino/algorithm/dist/index.js', "*

 * *      "'@phosphor/application$': "*

 * *      "'/Users/graceal/Documents/maap/extensions/jupyter-server-extension/node_modules/@lumino/application/dist/index.js', "*

 * *      "'@phosphor/commands$': "*

 * *      "'/Users/graceal/Documents/maap/extensions/jupyter-server-extension/node_modules/@lumino/commands/dist/index.js', "*

 * *      "'@phosphor/c […]*

```diff
@@ -91,29 +91,29 @@
                     ]
                 }
             ]
         },
         "output": {
             "filename": "[name].[contenthash].js",
             "hashFunction": "sha256",
-            "path": "/Users/mlucas/MAAP/jupyter_server_extension/jupyter_server_extension/labextension/static",
+            "path": "/Users/graceal/Documents/maap/extensions/jupyter-server-extension/jupyter_server_extension/labextension/static",
             "publicPath": "auto"
         },
         "plugins": [
             {
                 "definitions": {
                     "process": "process/browser"
                 }
             },
             {
                 "_options": {
                     "exposes": {
-                        "./extension": "/Users/mlucas/MAAP/jupyter_server_extension/lib/index.js",
-                        "./index": "/Users/mlucas/MAAP/jupyter_server_extension/lib/index.js",
-                        "./style": "/Users/mlucas/MAAP/jupyter_server_extension/style/index.js"
+                        "./extension": "/Users/graceal/Documents/maap/extensions/jupyter-server-extension/lib/index.js",
+                        "./index": "/Users/graceal/Documents/maap/extensions/jupyter-server-extension/lib/index.js",
+                        "./style": "/Users/graceal/Documents/maap/extensions/jupyter-server-extension/style/index.js"
                     },
                     "filename": "remoteEntry.[contenthash].js",
                     "library": {
                         "name": [
                             "_JUPYTERLAB",
                             "maap-jupyter-server-extension"
                         ],
@@ -599,15 +599,15 @@
                         },
                         "@lumino/widgets": {
                             "import": false,
                             "requiredVersion": "^1.37.2",
                             "singleton": true
                         },
                         "maap-jupyter-server-extension": {
-                            "import": "/Users/mlucas/MAAP/jupyter_server_extension/lib/index.js",
+                            "import": "/Users/graceal/Documents/maap/extensions/jupyter-server-extension/lib/index.js",
                             "singleton": true,
                             "version": "1.3.0"
                         },
                         "react": {
                             "import": false,
                             "requiredVersion": "^17.0.1",
                             "singleton": true
@@ -625,34 +625,34 @@
                     }
                 }
             },
             {}
         ],
         "resolve": {
             "alias": {
-                "@phosphor/algorithm$": "/Users/mlucas/MAAP/jupyter_server_extension/node_modules/@lumino/algorithm/dist/index.js",
-                "@phosphor/application$": "/Users/mlucas/MAAP/jupyter_server_extension/node_modules/@lumino/application/dist/index.js",
-                "@phosphor/commands$": "/Users/mlucas/MAAP/jupyter_server_extension/node_modules/@lumino/commands/dist/index.js",
-                "@phosphor/coreutils$": "/Users/mlucas/MAAP/jupyter_server_extension/node_modules/@lumino/coreutils/dist/index.node.js",
-                "@phosphor/disposable$": "/Users/mlucas/MAAP/jupyter_server_extension/node_modules/@lumino/disposable/dist/index.js",
-                "@phosphor/domutils$": "/Users/mlucas/MAAP/jupyter_server_extension/node_modules/@lumino/domutils/dist/index.js",
-                "@phosphor/dragdrop$": "/Users/mlucas/MAAP/jupyter_server_extension/node_modules/@lumino/dragdrop/dist/index.js",
-                "@phosphor/dragdrop/style": "/Users/mlucas/MAAP/jupyter_server_extension/node_modules/@lumino/widgets/style",
-                "@phosphor/messaging$": "/Users/mlucas/MAAP/jupyter_server_extension/node_modules/@lumino/messaging/dist/index.js",
-                "@phosphor/properties$": "/Users/mlucas/MAAP/jupyter_server_extension/node_modules/@lumino/properties/dist/index.js",
-                "@phosphor/signaling": "/Users/mlucas/MAAP/jupyter_server_extension/node_modules/@lumino/signaling/dist/index.js",
-                "@phosphor/virtualdom$": "/Users/mlucas/MAAP/jupyter_server_extension/node_modules/@lumino/virtualdom/dist/index.js",
-                "@phosphor/widgets$": "/Users/mlucas/MAAP/jupyter_server_extension/node_modules/@lumino/widgets/dist/index.js",
-                "@phosphor/widgets/style": "/Users/mlucas/MAAP/jupyter_server_extension/node_modules/@lumino/widgets/style"
+                "@phosphor/algorithm$": "/Users/graceal/Documents/maap/extensions/jupyter-server-extension/node_modules/@lumino/algorithm/dist/index.js",
+                "@phosphor/application$": "/Users/graceal/Documents/maap/extensions/jupyter-server-extension/node_modules/@lumino/application/dist/index.js",
+                "@phosphor/commands$": "/Users/graceal/Documents/maap/extensions/jupyter-server-extension/node_modules/@lumino/commands/dist/index.js",
+                "@phosphor/coreutils$": "/Users/graceal/Documents/maap/extensions/jupyter-server-extension/node_modules/@lumino/coreutils/dist/index.node.js",
+                "@phosphor/disposable$": "/Users/graceal/Documents/maap/extensions/jupyter-server-extension/node_modules/@lumino/disposable/dist/index.js",
+                "@phosphor/domutils$": "/Users/graceal/Documents/maap/extensions/jupyter-server-extension/node_modules/@lumino/domutils/dist/index.js",
+                "@phosphor/dragdrop$": "/Users/graceal/Documents/maap/extensions/jupyter-server-extension/node_modules/@lumino/dragdrop/dist/index.js",
+                "@phosphor/dragdrop/style": "/Users/graceal/Documents/maap/extensions/jupyter-server-extension/node_modules/@lumino/widgets/style",
+                "@phosphor/messaging$": "/Users/graceal/Documents/maap/extensions/jupyter-server-extension/node_modules/@lumino/messaging/dist/index.js",
+                "@phosphor/properties$": "/Users/graceal/Documents/maap/extensions/jupyter-server-extension/node_modules/@lumino/properties/dist/index.js",
+                "@phosphor/signaling": "/Users/graceal/Documents/maap/extensions/jupyter-server-extension/node_modules/@lumino/signaling/dist/index.js",
+                "@phosphor/virtualdom$": "/Users/graceal/Documents/maap/extensions/jupyter-server-extension/node_modules/@lumino/virtualdom/dist/index.js",
+                "@phosphor/widgets$": "/Users/graceal/Documents/maap/extensions/jupyter-server-extension/node_modules/@lumino/widgets/dist/index.js",
+                "@phosphor/widgets/style": "/Users/graceal/Documents/maap/extensions/jupyter-server-extension/node_modules/@lumino/widgets/style"
             },
             "fallback": {
                 "buffer": false,
                 "crypto": false,
-                "path": "/Users/mlucas/MAAP/jupyter_server_extension/node_modules/path-browserify/index.js",
-                "process": "/Users/mlucas/MAAP/jupyter_server_extension/node_modules/process/browser.js",
+                "path": "/Users/graceal/Documents/maap/extensions/jupyter-server-extension/node_modules/path-browserify/index.js",
+                "process": "/Users/graceal/Documents/maap/extensions/jupyter-server-extension/node_modules/process/browser.js",
                 "url": false
             }
         },
         "watchOptions": {
             "aggregateTimeout": 1000,
             "poll": 500
         }
```

### Comparing `maap_jupyter_server_extension-1.3.0/jupyter_server_extension/labextension/package.json` & `maap_jupyter_server_extension-1.3.4/jupyter_server_extension/labextension/package.json`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.3.0/jupyter_server_extension/labextension/static/lib_index_js.f3563370867954312194.js` & `maap_jupyter_server_extension-1.3.4/jupyter_server_extension/labextension/static/lib_index_js.f3563370867954312194.js`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.3.0/jupyter_server_extension/labextension/static/lib_index_js.f3563370867954312194.js.map` & `maap_jupyter_server_extension-1.3.4/jupyter_server_extension/labextension/static/lib_index_js.f3563370867954312194.js.map`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.3.0/jupyter_server_extension/labextension/static/remoteEntry.6f9394f1d8ef18e972d0.js` & `maap_jupyter_server_extension-1.3.4/jupyter_server_extension/labextension/static/remoteEntry.6f9394f1d8ef18e972d0.js`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.3.0/jupyter_server_extension/labextension/static/remoteEntry.6f9394f1d8ef18e972d0.js.map` & `maap_jupyter_server_extension-1.3.4/jupyter_server_extension/labextension/static/remoteEntry.6f9394f1d8ef18e972d0.js.map`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.3.0/jupyter_server_extension/labextension/static/style_index_js.985542941dd18f4568ee.js` & `maap_jupyter_server_extension-1.3.4/jupyter_server_extension/labextension/static/style_index_js.985542941dd18f4568ee.js`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.3.0/jupyter_server_extension/labextension/static/style_index_js.985542941dd18f4568ee.js.map` & `maap_jupyter_server_extension-1.3.4/jupyter_server_extension/labextension/static/style_index_js.985542941dd18f4568ee.js.map`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.3.0/jupyter_server_extension/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.265412ff30d319ce76fc.js` & `maap_jupyter_server_extension-1.3.4/jupyter_server_extension/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.265412ff30d319ce76fc.js`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.3.0/jupyter_server_extension/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.265412ff30d319ce76fc.js.map` & `maap_jupyter_server_extension-1.3.4/jupyter_server_extension/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.265412ff30d319ce76fc.js.map`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.3.0/maap_jupyter_server_extension.egg-info/PKG-INFO` & `maap_jupyter_server_extension-1.3.4/maap_jupyter_server_extension.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maap_jupyter_server_extension
-Version: 1.3.0
+Version: 1.3.4
 Summary: A JupyterLab extension.
 Home-page: https://github.com/MAAP-Project/jupyter-server-extension
 Author: Marjorie Lucas
 Author-email: marjorie.j.lucas@jpl.nasa.gov
 License: Apache 2.0
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
@@ -22,14 +22,15 @@
 Classifier: Framework :: Jupyter :: JupyterLab :: 3
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jupyter_server==2.12.5
+Requires-Dist: xmltodict==0.13.0
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-tornasync; extra == "test"
```

### Comparing `maap_jupyter_server_extension-1.3.0/maap_jupyter_server_extension.egg-info/SOURCES.txt` & `maap_jupyter_server_extension-1.3.4/maap_jupyter_server_extension.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 README.md
 conftest.py
 install.json
 package.json
 pyproject.toml
 setup.py
 tsconfig.json
+yarn.lock
 jupyter-config/nb-config/dps_jupyter_server_extension.json
 jupyter-config/server-config/dps_jupyter_server_extension.json
 jupyter_server_extension/__init__.py
 jupyter_server_extension/_version.py
 jupyter_server_extension/handlers.py
 jupyter_server_extension/labextension/build_log.json
 jupyter_server_extension/labextension/package.json
```

### Comparing `maap_jupyter_server_extension-1.3.0/package.json` & `maap_jupyter_server_extension-1.3.4/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'1.3.4'"}*

```diff
@@ -88,9 +88,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.3.0"
+    "version": "1.3.4"
 }
```

### Comparing `maap_jupyter_server_extension-1.3.0/pyproject.toml` & `maap_jupyter_server_extension-1.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.3.0/setup.py` & `maap_jupyter_server_extension-1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,16 @@
     description=pkg_json["description"],
     license=pkg_json["license"],
     license_file="LICENSE",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=[
-        "jupyter_server==2.12.5"
+        "jupyter_server==2.12.5",
+        "xmltodict==0.13.0"
     ],
     extras_require={
         "test": [
             "coverage",
             "pytest",
             "pytest-asyncio",
             "pytest-cov",
```

### Comparing `maap_jupyter_server_extension-1.3.0/src/handler.ts` & `maap_jupyter_server_extension-1.3.4/src/handler.ts`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.3.0/src/index.ts` & `maap_jupyter_server_extension-1.3.4/src/index.ts`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.3.0/tsconfig.json` & `maap_jupyter_server_extension-1.3.4/tsconfig.json`

 * *Files identical despite different names*

