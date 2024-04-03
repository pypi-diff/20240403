# Comparing `tmp/ipython-ngql-0.8.0.tar.gz` & `tmp/ipython-ngql-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipython-ngql-0.8.0.tar", last modified: Mon Jan 29 07:54:56 2024, max compression
+gzip compressed data, was "ipython-ngql-0.9.0.tar", last modified: Wed Apr  3 10:59:17 2024, max compression
```

## Comparing `ipython-ngql-0.8.0.tar` & `ipython-ngql-0.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 07:54:56.462535 ipython-ngql-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-01-29 07:54:41.000000 ipython-ngql-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-01-29 07:54:56.462535 ipython-ngql-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-01-29 07:54:41.000000 ipython-ngql-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 07:54:56.462535 ipython-ngql-0.8.0/ipython_ngql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-01-29 07:54:56.000000 ipython-ngql-0.8.0/ipython_ngql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-01-29 07:54:56.000000 ipython-ngql-0.8.0/ipython_ngql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 07:54:56.000000 ipython-ngql-0.8.0/ipython_ngql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-29 07:54:56.000000 ipython-ngql-0.8.0/ipython_ngql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-29 07:54:56.000000 ipython-ngql-0.8.0/ipython_ngql.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 07:54:56.462535 ipython-ngql-0.8.0/ngql/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-01-29 07:54:41.000000 ipython-ngql-0.8.0/ngql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22171 2024-01-29 07:54:41.000000 ipython-ngql-0.8.0/ngql/magic.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-29 07:54:56.462535 ipython-ngql-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-01-29 07:54:41.000000 ipython-ngql-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:59:17.463383 ipython-ngql-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-03 10:59:12.000000 ipython-ngql-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8542 2024-04-03 10:59:17.463383 ipython-ngql-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-04-03 10:59:12.000000 ipython-ngql-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:59:17.463383 ipython-ngql-0.9.0/ipython_ngql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8542 2024-04-03 10:59:17.000000 ipython-ngql-0.9.0/ipython_ngql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-03 10:59:17.000000 ipython-ngql-0.9.0/ipython_ngql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 10:59:17.000000 ipython-ngql-0.9.0/ipython_ngql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 10:59:17.000000 ipython-ngql-0.9.0/ipython_ngql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-03 10:59:17.000000 ipython-ngql-0.9.0/ipython_ngql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:59:17.459383 ipython-ngql-0.9.0/ngql/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-03 10:59:12.000000 ipython-ngql-0.9.0/ngql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35833 2024-04-03 10:59:12.000000 ipython-ngql-0.9.0/ngql/magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 10:59:17.463383 ipython-ngql-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-03 10:59:12.000000 ipython-ngql-0.9.0/setup.py
```

### Comparing `ipython-ngql-0.8.0/LICENSE` & `ipython-ngql-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipython-ngql-0.8.0/PKG-INFO` & `ipython-ngql-0.9.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: ipython-ngql
-Version: 0.8.0
-Summary: Jupyter and iPython extension for NebulaGraph
-Home-page: https://github.com/wey-gu/ipython-ngql
-Author: Wey Gu
-Author-email: weyl.gu@gmail.com
-Project-URL: Bug Tracker, https://github.com/wey-gu/ipython-ngql/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: Jinja2
-Requires-Dist: nebula3-python>=3.5.0
-Requires-Dist: pandas
-
 
 [![for NebulaGraph](https://img.shields.io/badge/Toolchain-NebulaGraph-blue)](https://github.com/vesoft-inc/nebula) [![Jupyter](https://img.shields.io/badge/Jupyter-Supported-brightgreen)](https://github.com/jupyterlab/jupyterlab) [![Docker Image](https://img.shields.io/docker/v/weygu/nebulagraph-jupyter?label=Image&logo=docker)](https://hub.docker.com/r/weygu/nebulagraph-jupyter) [![Docker Extension](https://img.shields.io/badge/Docker-Extension-blue?logo=docker)](https://hub.docker.com/extensions/weygu/nebulagraph-dd-ext) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/wey-gu/ipython-ngql?label=Version)](https://github.com/wey-gu/ipython-ngql/releases)
 [![pypi-version](https://img.shields.io/pypi/v/ipython-ngql)](https://pypi.org/project/ipython-ngql/)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/wey-gu/ipython-ngql/blob/main/examples/get_started.ipynb)
 
 
 https://github.com/wey-gu/ipython-ngql/assets/1651790/10135264-77b5-4d3c-b68f-c5810257feeb
@@ -138,14 +120,45 @@
 
 ### Draw Graph Schema
 
 ```python
 %ng_draw_schema
 ```
 
+![](https://github.com/wey-gu/ipython-ngql/assets/1651790/81fd71b5-61e7-4c65-93be-c2f4e507611b)
+
+### Load Data from CSV
+
+It's supported to load data from a CSV file into NebulaGraph with the help of `ng_load_csv` magic.
+
+For example, to load data from a CSV file `actor.csv` into a space `basketballplayer` with tag `player` and vid in column `0`, and props in column `1` and `2`:
+
+```csv
+"player999","Tom Hanks",30
+"player1000","Tom Cruise",40
+"player1001","Jimmy X",33
+```
+
+Just run the below line:
+
+```python
+%ng_load --source actor.csv --tag player --vid 0 --props 1:name,2:age --space basketballplayer
+```
+
+Some other examples:
+
+```python
+# load CSV from a URL
+%ng_load --source https://github.com/wey-gu/ipython-ngql/raw/main/examples/actor.csv --tag player --vid 0 --props 1:name,2:age --space demo_basketballplayer -b 2
+# with rank column
+%ng_load --source follow_with_rank.csv --edge follow --src 0 --dst 1 --props 2:degree --rank 3 --space basketballplayer
+# without rank column
+%ng_load --source follow.csv --edge follow --src 0 --dst 1 --props 2:degree --space basketballplayer
+```
+
 ### Configure `ngql_result_style`
 
 By default, `ipython-ngql` will use pandas dataframe as output style to enable more human-readable output, while it's supported to use the raw thrift data format that comes from the `nebula3-python` itself.
 
 This can be done ad-hoc with below one line:
 
 ```python
```

### Comparing `ipython-ngql-0.8.0/README.md` & `ipython-ngql-0.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: ipython-ngql
+Version: 0.9.0
+Summary: Jupyter and iPython extension for NebulaGraph
+Home-page: https://github.com/wey-gu/ipython-ngql
+Author: Wey Gu
+Author-email: weyl.gu@gmail.com
+Project-URL: Bug Tracker, https://github.com/wey-gu/ipython-ngql/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: Jinja2
+Requires-Dist: nebula3-python>=3.5.0
+Requires-Dist: pandas
+
 
 [![for NebulaGraph](https://img.shields.io/badge/Toolchain-NebulaGraph-blue)](https://github.com/vesoft-inc/nebula) [![Jupyter](https://img.shields.io/badge/Jupyter-Supported-brightgreen)](https://github.com/jupyterlab/jupyterlab) [![Docker Image](https://img.shields.io/docker/v/weygu/nebulagraph-jupyter?label=Image&logo=docker)](https://hub.docker.com/r/weygu/nebulagraph-jupyter) [![Docker Extension](https://img.shields.io/badge/Docker-Extension-blue?logo=docker)](https://hub.docker.com/extensions/weygu/nebulagraph-dd-ext) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/wey-gu/ipython-ngql?label=Version)](https://github.com/wey-gu/ipython-ngql/releases)
 [![pypi-version](https://img.shields.io/pypi/v/ipython-ngql)](https://pypi.org/project/ipython-ngql/)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/wey-gu/ipython-ngql/blob/main/examples/get_started.ipynb)
 
 
 https://github.com/wey-gu/ipython-ngql/assets/1651790/10135264-77b5-4d3c-b68f-c5810257feeb
@@ -120,14 +138,45 @@
 
 ### Draw Graph Schema
 
 ```python
 %ng_draw_schema
 ```
 
+![](https://github.com/wey-gu/ipython-ngql/assets/1651790/81fd71b5-61e7-4c65-93be-c2f4e507611b)
+
+### Load Data from CSV
+
+It's supported to load data from a CSV file into NebulaGraph with the help of `ng_load_csv` magic.
+
+For example, to load data from a CSV file `actor.csv` into a space `basketballplayer` with tag `player` and vid in column `0`, and props in column `1` and `2`:
+
+```csv
+"player999","Tom Hanks",30
+"player1000","Tom Cruise",40
+"player1001","Jimmy X",33
+```
+
+Just run the below line:
+
+```python
+%ng_load --source actor.csv --tag player --vid 0 --props 1:name,2:age --space basketballplayer
+```
+
+Some other examples:
+
+```python
+# load CSV from a URL
+%ng_load --source https://github.com/wey-gu/ipython-ngql/raw/main/examples/actor.csv --tag player --vid 0 --props 1:name,2:age --space demo_basketballplayer -b 2
+# with rank column
+%ng_load --source follow_with_rank.csv --edge follow --src 0 --dst 1 --props 2:degree --rank 3 --space basketballplayer
+# without rank column
+%ng_load --source follow.csv --edge follow --src 0 --dst 1 --props 2:degree --space basketballplayer
+```
+
 ### Configure `ngql_result_style`
 
 By default, `ipython-ngql` will use pandas dataframe as output style to enable more human-readable output, while it's supported to use the raw thrift data format that comes from the `nebula3-python` itself.
 
 This can be done ad-hoc with below one line:
 
 ```python
```

### Comparing `ipython-ngql-0.8.0/ipython_ngql.egg-info/PKG-INFO` & `ipython-ngql-0.9.0/ipython_ngql.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipython-ngql
-Version: 0.8.0
+Version: 0.9.0
 Summary: Jupyter and iPython extension for NebulaGraph
 Home-page: https://github.com/wey-gu/ipython-ngql
 Author: Wey Gu
 Author-email: weyl.gu@gmail.com
 Project-URL: Bug Tracker, https://github.com/wey-gu/ipython-ngql/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -138,14 +138,45 @@
 
 ### Draw Graph Schema
 
 ```python
 %ng_draw_schema
 ```
 
+![](https://github.com/wey-gu/ipython-ngql/assets/1651790/81fd71b5-61e7-4c65-93be-c2f4e507611b)
+
+### Load Data from CSV
+
+It's supported to load data from a CSV file into NebulaGraph with the help of `ng_load_csv` magic.
+
+For example, to load data from a CSV file `actor.csv` into a space `basketballplayer` with tag `player` and vid in column `0`, and props in column `1` and `2`:
+
+```csv
+"player999","Tom Hanks",30
+"player1000","Tom Cruise",40
+"player1001","Jimmy X",33
+```
+
+Just run the below line:
+
+```python
+%ng_load --source actor.csv --tag player --vid 0 --props 1:name,2:age --space basketballplayer
+```
+
+Some other examples:
+
+```python
+# load CSV from a URL
+%ng_load --source https://github.com/wey-gu/ipython-ngql/raw/main/examples/actor.csv --tag player --vid 0 --props 1:name,2:age --space demo_basketballplayer -b 2
+# with rank column
+%ng_load --source follow_with_rank.csv --edge follow --src 0 --dst 1 --props 2:degree --rank 3 --space basketballplayer
+# without rank column
+%ng_load --source follow.csv --edge follow --src 0 --dst 1 --props 2:degree --space basketballplayer
+```
+
 ### Configure `ngql_result_style`
 
 By default, `ipython-ngql` will use pandas dataframe as output style to enable more human-readable output, while it's supported to use the raw thrift data format that comes from the `nebula3-python` itself.
 
 This can be done ad-hoc with below one line:
 
 ```python
```

### Comparing `ipython-ngql-0.8.0/setup.py` & `ipython-ngql-0.9.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ipython-ngql",
-    version="0.8.0",
+    version="0.9.0",
     author="Wey Gu",
     author_email="weyl.gu@gmail.com",
     description="Jupyter and iPython extension for NebulaGraph",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wey-gu/ipython-ngql",
     project_urls={
```

