# Comparing `tmp/nvcc4jupyter-1.2.0.tar.gz` & `tmp/nvcc4jupyter-1.2.1.tar.gz`

## Comparing `nvcc4jupyter-1.2.0.tar` & `nvcc4jupyter-1.2.1.tar`

### file list

```diff
@@ -1,44 +1,45 @@
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/.flake8
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/.readthedocs.yaml
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/.devcontainer/Dockerfile
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/.devcontainer/post_create.sh
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/.github/workflows/code-quality-master.yml
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/.github/workflows/code-quality-pr.yml
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/.vscode/settings.json
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/docs/Makefile
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/docs/make.bat
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/docs/requirements.txt
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/docs/source/conf.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/docs/source/index.rst
--rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/docs/source/magics.rst
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/docs/source/notebooks.rst
--rw-r--r--   0        0        0    11271 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/docs/source/usage.rst
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/nvcc4jupyter/__init__.py
--rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/nvcc4jupyter/parsers.py
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/nvcc4jupyter/path_utils.py
--rw-r--r--   0        0        0    12451 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/nvcc4jupyter/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/tests/conftest.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/tests/requirements.txt
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/tests/test_path_utils.py
--rw-r--r--   0        0        0    10121 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/tests/test_plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/tests/fixtures/fixtures.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/tests/fixtures/compiler/cpp_17.cu
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/tests/fixtures/compiler/opencv.cu
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/tests/fixtures/multiple_files/hello.cu
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/tests/fixtures/multiple_files/hello.h
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/tests/fixtures/multiple_files/main.cu
--rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/tests/fixtures/scripts/ncu
--rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/tests/fixtures/scripts/nsys
--rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/tests/fixtures/scripts/searchforme
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/tests/fixtures/single_file/hello.cu
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/LICENSE
--rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/README.md
--rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     5084 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/.flake8
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/.devcontainer/post_create.sh
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/.github/workflows/code-quality-master.yml
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/.github/workflows/code-quality-pr.yml
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/.vscode/settings.json
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/docs/Makefile
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/docs/make.bat
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/docs/requirements.txt
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/docs/source/conf.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/docs/source/index.rst
+-rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/docs/source/magics.rst
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/docs/source/notebooks.rst
+-rw-r--r--   0        0        0    11271 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/docs/source/usage.rst
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/nvcc4jupyter/__init__.py
+-rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/nvcc4jupyter/parsers.py
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/nvcc4jupyter/path_utils.py
+-rw-r--r--   0        0        0    12516 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/nvcc4jupyter/plugin.py
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/nvcc4jupyter/setup_env.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/tests/__init__.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/tests/conftest.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/tests/requirements.txt
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/tests/test_path_utils.py
+-rw-r--r--   0        0        0    10121 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/tests/test_plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/tests/fixtures/fixtures.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/tests/fixtures/compiler/cpp_17.cu
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/tests/fixtures/compiler/opencv.cu
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/tests/fixtures/multiple_files/hello.cu
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/tests/fixtures/multiple_files/hello.h
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/tests/fixtures/multiple_files/main.cu
+-rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/tests/fixtures/scripts/ncu
+-rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/tests/fixtures/scripts/nsys
+-rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/tests/fixtures/scripts/searchforme
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/tests/fixtures/single_file/hello.cu
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/LICENSE
+-rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/README.md
+-rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5084 2020-02-02 00:00:00.000000 nvcc4jupyter-1.2.1/PKG-INFO
```

### Comparing `nvcc4jupyter-1.2.0/.pre-commit-config.yaml` & `nvcc4jupyter-1.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nvcc4jupyter-1.2.0/.readthedocs.yaml` & `nvcc4jupyter-1.2.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `nvcc4jupyter-1.2.0/.devcontainer/Dockerfile` & `nvcc4jupyter-1.2.1/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `nvcc4jupyter-1.2.0/.devcontainer/devcontainer.json` & `nvcc4jupyter-1.2.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `nvcc4jupyter-1.2.0/.github/workflows/code-quality-pr.yml` & `nvcc4jupyter-1.2.1/.github/workflows/code-quality-pr.yml`

 * *Files identical despite different names*

### Comparing `nvcc4jupyter-1.2.0/.github/workflows/publish-to-pypi.yml` & `nvcc4jupyter-1.2.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `nvcc4jupyter-1.2.0/.github/workflows/test.yml` & `nvcc4jupyter-1.2.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `nvcc4jupyter-1.2.0/.vscode/settings.json` & `nvcc4jupyter-1.2.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `nvcc4jupyter-1.2.0/docs/Makefile` & `nvcc4jupyter-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nvcc4jupyter-1.2.0/docs/make.bat` & `nvcc4jupyter-1.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nvcc4jupyter-1.2.0/docs/source/conf.py` & `nvcc4jupyter-1.2.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nvcc4jupyter-1.2.0/docs/source/magics.rst` & `nvcc4jupyter-1.2.1/docs/source/magics.rst`

 * *Files identical despite different names*

### Comparing `nvcc4jupyter-1.2.0/docs/source/notebooks.rst` & `nvcc4jupyter-1.2.1/docs/source/notebooks.rst`

 * *Files identical despite different names*

### Comparing `nvcc4jupyter-1.2.0/docs/source/usage.rst` & `nvcc4jupyter-1.2.1/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `nvcc4jupyter-1.2.0/nvcc4jupyter/parsers.py` & `nvcc4jupyter-1.2.1/nvcc4jupyter/parsers.py`

 * *Files identical despite different names*

### Comparing `nvcc4jupyter-1.2.0/nvcc4jupyter/path_utils.py` & `nvcc4jupyter-1.2.1/nvcc4jupyter/path_utils.py`

 * *Files identical despite different names*

### Comparing `nvcc4jupyter-1.2.0/nvcc4jupyter/plugin.py` & `nvcc4jupyter-1.2.1/nvcc4jupyter/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     Profiler,
     get_parser_cuda,
     get_parser_cuda_group_delete,
     get_parser_cuda_group_run,
     get_parser_cuda_group_save,
 )
 from .path_utils import CUDA_SEARCH_PATHS, find_executable
+from .setup_env import setup_environment
 
 DEFAULT_EXEC_FNAME = "cuda_exec.out"
 SHARED_GROUP_NAME = "shared"
 
 
 def print_out(out: str):
     """Print string line by line."""
@@ -360,9 +361,10 @@
         self._delete_group(args.group)
 
 
 def load_ipython_extension(shell: InteractiveShell):
     """
     Method used by IPython to load the extension.
     """
+    setup_environment()
     nvcc_plugin = NVCCPlugin(shell)
     shell.register_magics(nvcc_plugin)
```

### Comparing `nvcc4jupyter-1.2.0/tests/test_plugin.py` & `nvcc4jupyter-1.2.1/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `nvcc4jupyter-1.2.0/tests/fixtures/fixtures.py` & `nvcc4jupyter-1.2.1/tests/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `nvcc4jupyter-1.2.0/tests/fixtures/compiler/cpp_17.cu` & `nvcc4jupyter-1.2.1/tests/fixtures/compiler/cpp_17.cu`

 * *Files identical despite different names*

### Comparing `nvcc4jupyter-1.2.0/LICENSE` & `nvcc4jupyter-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nvcc4jupyter-1.2.0/README.md` & `nvcc4jupyter-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nvcc4jupyter-1.2.0/pyproject.toml` & `nvcc4jupyter-1.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -84,14 +84,18 @@
 line-length = 79
 fast = true
 preview = true
 enable-unstable-feature = ["string_processing"]
 
 [tool.coverage.run]
 branch = true
+omit = [
+    # cannot test installing dependencies on platforms such as kaggle
+    "nvcc4jupyter/setup_env.py",
+]
 
 [tool.pyright]
 include = ["src"]
 exclude = [
     "**/node_modules",
     "**/__pycache__",
 ]
```

### Comparing `nvcc4jupyter-1.2.0/PKG-INFO` & `nvcc4jupyter-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nvcc4jupyter
-Version: 1.2.0
+Version: 1.2.1
 Summary: Jupyter notebook plugin to run CUDA C/C++ code
 Project-URL: documentation, https://nvcc4jupyter.readthedocs.io/
 Project-URL: repository, https://github.com/andreinechaev/nvcc4jupyter
 Author-email: Andrei Nechaev <lyfaradey@yahoo.com>, Cosmin Stefan Ciocan <ciocan.cosmin98@gmail.com>
 License: MIT License
 License-File: LICENSE
 Classifier: Environment :: GPU
```

