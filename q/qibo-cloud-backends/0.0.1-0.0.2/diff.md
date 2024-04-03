# Comparing `tmp/qibo_cloud_backends-0.0.1.tar.gz` & `tmp/qibo_cloud_backends-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qibo_cloud_backends-0.0.1.tar", max compression
+gzip compressed data, was "qibo_cloud_backends-0.0.2.tar", max compression
```

## Comparing `qibo_cloud_backends-0.0.1.tar` & `qibo_cloud_backends-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2024-02-18 09:41:31.057675 qibo_cloud_backends-0.0.1/LICENSE
--rw-r--r--   0        0        0     1557 2024-03-02 09:02:26.554542 qibo_cloud_backends-0.0.1/README.md
--rw-r--r--   0        0        0     1548 2024-03-03 16:31:49.252389 qibo_cloud_backends-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      200 2024-03-02 09:02:26.556218 qibo_cloud_backends-0.0.1/src/qibo_cloud_backends/__init__.py
--rw-r--r--   0        0        0     1437 2024-03-02 09:02:26.556285 qibo_cloud_backends-0.0.1/src/qibo_cloud_backends/qibo_client.py
--rw-r--r--   0        0        0     2407 2024-03-02 09:02:26.556347 qibo_cloud_backends-0.0.1/src/qibo_cloud_backends/qiskit_client.py
--rw-r--r--   0        0        0     2434 1970-01-01 00:00:00.000000 qibo_cloud_backends-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-03 09:23:37.642500 qibo_cloud_backends-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1557 2024-04-03 09:23:37.642500 qibo_cloud_backends-0.0.2/README.md
+-rw-r--r--   0        0        0     1548 2024-04-03 09:23:37.646500 qibo_cloud_backends-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      200 2024-04-03 09:23:37.646500 qibo_cloud_backends-0.0.2/src/qibo_cloud_backends/__init__.py
+-rw-r--r--   0        0        0     1437 2024-04-03 09:23:37.646500 qibo_cloud_backends-0.0.2/src/qibo_cloud_backends/qibo_client.py
+-rw-r--r--   0        0        0     2407 2024-04-03 09:23:37.646500 qibo_cloud_backends-0.0.2/src/qibo_cloud_backends/qiskit_client.py
+-rw-r--r--   0        0        0     2434 1970-01-01 00:00:00.000000 qibo_cloud_backends-0.0.2/PKG-INFO
```

### Comparing `qibo_cloud_backends-0.0.1/LICENSE` & `qibo_cloud_backends-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qibo_cloud_backends-0.0.1/README.md` & `qibo_cloud_backends-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `qibo_cloud_backends-0.0.1/pyproject.toml` & `qibo_cloud_backends-0.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "qibo-cloud-backends"
-version = "0.0.1"
+version = "0.0.2"
 description = "Qibo backends for client interface."
 authors = ["The Qibo team"]
 license = "Apache License 2.0"
 readme = "README.md"
 homepage = "https://qibo.science/"
 repository = "https://github.com/qiboteam/qibo-cloud-backends/"
 documentation = "https://qibo.science/qibo-cloud-backends/stable"
@@ -18,15 +18,15 @@
   "Topic :: Scientific/Engineering :: Physics",
 ]
 packages = [{ include = "qibo_cloud_backends", from = "src" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 qibo = ">=0.2.4"
-qibo_client = ">=0.0.3"
+qibo_client = ">=0.0.4"
 qiskit_ibm_runtime = ">=0.17"
 qiskit_ibm_provider = ">=0.8.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.3"
 pytest-cov = "^4.1.0"
 pylint = "^3.0.3"
```

### Comparing `qibo_cloud_backends-0.0.1/src/qibo_cloud_backends/qibo_client.py` & `qibo_cloud_backends-0.0.2/src/qibo_cloud_backends/qibo_client.py`

 * *Files identical despite different names*

### Comparing `qibo_cloud_backends-0.0.1/src/qibo_cloud_backends/qiskit_client.py` & `qibo_cloud_backends-0.0.2/src/qibo_cloud_backends/qiskit_client.py`

 * *Files identical despite different names*

### Comparing `qibo_cloud_backends-0.0.1/PKG-INFO` & `qibo_cloud_backends-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: qibo-cloud-backends
-Version: 0.0.1
+Version: 0.0.2
 Summary: Qibo backends for client interface.
 Home-page: https://qibo.science/
 License: Apache-2.0
 Author: The Qibo team
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Dist: qibo (>=0.2.4)
-Requires-Dist: qibo_client (>=0.0.3)
+Requires-Dist: qibo_client (>=0.0.4)
 Requires-Dist: qiskit_ibm_provider (>=0.8.0)
 Requires-Dist: qiskit_ibm_runtime (>=0.17)
 Project-URL: Documentation, https://qibo.science/qibo-cloud-backends/stable
 Project-URL: Repository, https://github.com/qiboteam/qibo-cloud-backends/
 Description-Content-Type: text/markdown
 
 # Qibo cloud backends
```

