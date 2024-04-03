# Comparing `tmp/pytest_jupyter-0.9.0.tar.gz` & `tmp/pytest_jupyter-0.9.1.tar.gz`

## Comparing `pytest_jupyter-0.9.0.tar` & `pytest_jupyter-0.9.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.0/pytest_jupyter/__init__.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.0/pytest_jupyter/_version.py
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.0/pytest_jupyter/echo_kernel.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.0/pytest_jupyter/jupyter_client.py
--rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.0/pytest_jupyter/jupyter_core.py
--rw-r--r--   0        0        0    16256 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.0/pytest_jupyter/jupyter_server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.0/pytest_jupyter/py.typed
--rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.0/pytest_jupyter/pytest_tornasync.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.0/pytest_jupyter/utils.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.0/tests/conftest.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.0/tests/test_jupyter_client.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.0/tests/test_jupyter_core.py
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.0/tests/test_jupyter_server.py
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.0/.gitignore
--rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.0/LICENSE
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.0/README.md
--rw-r--r--   0        0        0     4978 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     9270 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.1/pytest_jupyter/__init__.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.1/pytest_jupyter/_version.py
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.1/pytest_jupyter/echo_kernel.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.1/pytest_jupyter/jupyter_client.py
+-rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.1/pytest_jupyter/jupyter_core.py
+-rw-r--r--   0        0        0    16256 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.1/pytest_jupyter/jupyter_server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.1/pytest_jupyter/py.typed
+-rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.1/pytest_jupyter/pytest_tornasync.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.1/pytest_jupyter/utils.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.1/tests/conftest.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.1/tests/test_jupyter_client.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.1/tests/test_jupyter_core.py
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.1/tests/test_jupyter_server.py
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.1/.gitignore
+-rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.1/LICENSE
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.1/README.md
+-rw-r--r--   0        0        0     4978 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     9270 2020-02-02 00:00:00.000000 pytest_jupyter-0.9.1/PKG-INFO
```

### Comparing `pytest_jupyter-0.9.0/pytest_jupyter/echo_kernel.py` & `pytest_jupyter-0.9.1/pytest_jupyter/echo_kernel.py`

 * *Files identical despite different names*

### Comparing `pytest_jupyter-0.9.0/pytest_jupyter/jupyter_client.py` & `pytest_jupyter-0.9.1/pytest_jupyter/jupyter_client.py`

 * *Files identical despite different names*

### Comparing `pytest_jupyter-0.9.0/pytest_jupyter/jupyter_core.py` & `pytest_jupyter-0.9.1/pytest_jupyter/jupyter_core.py`

 * *Files identical despite different names*

### Comparing `pytest_jupyter-0.9.0/pytest_jupyter/jupyter_server.py` & `pytest_jupyter-0.9.1/pytest_jupyter/jupyter_server.py`

 * *Files identical despite different names*

### Comparing `pytest_jupyter-0.9.0/pytest_jupyter/pytest_tornasync.py` & `pytest_jupyter-0.9.1/pytest_jupyter/pytest_tornasync.py`

 * *Files identical despite different names*

### Comparing `pytest_jupyter-0.9.0/tests/test_jupyter_client.py` & `pytest_jupyter-0.9.1/tests/test_jupyter_client.py`

 * *Files identical despite different names*

### Comparing `pytest_jupyter-0.9.0/tests/test_jupyter_server.py` & `pytest_jupyter-0.9.1/tests/test_jupyter_server.py`

 * *Files identical despite different names*

### Comparing `pytest_jupyter-0.9.0/.gitignore` & `pytest_jupyter-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_jupyter-0.9.0/LICENSE` & `pytest_jupyter-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_jupyter-0.9.0/README.md` & `pytest_jupyter-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pytest_jupyter-0.9.0/pyproject.toml` & `pytest_jupyter-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest_jupyter-0.9.0/PKG-INFO` & `pytest_jupyter-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-jupyter
-Version: 0.9.0
+Version: 0.9.1
 Summary: A pytest plugin for testing Jupyter libraries and extensions.
 Project-URL: Homepage, http://jupyter.org
 Project-URL: Funding, https://numfocus.org/donate
 Project-URL: Source, https://github.com/jupyter-server/pytest-jupyter
 Project-URL: Tracker, https://github.com/jupyter-server/pytest-jupyter/issues
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: # Licensing terms
```

