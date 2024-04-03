# Comparing `tmp/fast_dev_cli-0.6.2.tar.gz` & `tmp/fast_dev_cli-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_dev_cli-0.6.2.tar", max compression
+gzip compressed data, was "fast_dev_cli-0.6.4.tar", max compression
```

## Comparing `fast_dev_cli-0.6.2.tar` & `fast_dev_cli-0.6.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2024-03-06 06:08:37.265617 fast_dev_cli-0.6.2/LICENSE
--rw-r--r--   0        0        0     1663 2024-03-07 02:13:22.157917 fast_dev_cli-0.6.2/README.md
--rw-r--r--   0        0        0       76 2024-03-06 06:08:37.265993 fast_dev_cli-0.6.2/fast_dev_cli/__init__.py
--rw-r--r--   0        0        0       28 2024-03-06 06:08:37.266125 fast_dev_cli-0.6.2/fast_dev_cli/__main__.py
--rw-r--r--   0        0        0    19833 2024-03-12 14:15:24.546794 fast_dev_cli-0.6.2/fast_dev_cli/cli.py
--rw-r--r--   0        0        0        0 2024-03-06 06:08:37.266469 fast_dev_cli-0.6.2/fast_dev_cli/py.typed
--rw-r--r--   0        0        0     1374 2024-03-12 14:18:58.422789 fast_dev_cli-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     2467 1970-01-01 00:00:00.000000 fast_dev_cli-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-03-06 06:08:37.265617 fast_dev_cli-0.6.4/LICENSE
+-rw-r--r--   0        0        0     1663 2024-03-07 02:13:22.157917 fast_dev_cli-0.6.4/README.md
+-rw-r--r--   0        0        0       76 2024-03-06 06:08:37.265993 fast_dev_cli-0.6.4/fast_dev_cli/__init__.py
+-rw-r--r--   0        0        0       28 2024-03-06 06:08:37.266125 fast_dev_cli-0.6.4/fast_dev_cli/__main__.py
+-rw-r--r--   0        0        0    19833 2024-03-12 14:15:24.546794 fast_dev_cli-0.6.4/fast_dev_cli/cli.py
+-rw-r--r--   0        0        0        0 2024-03-06 06:08:37.266469 fast_dev_cli-0.6.4/fast_dev_cli/py.typed
+-rw-r--r--   0        0        0     1357 2024-04-03 14:29:18.885217 fast_dev_cli-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     2463 1970-01-01 00:00:00.000000 fast_dev_cli-0.6.4/PKG-INFO
```

### Comparing `fast_dev_cli-0.6.2/LICENSE` & `fast_dev_cli-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_dev_cli-0.6.2/README.md` & `fast_dev_cli-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `fast_dev_cli-0.6.2/fast_dev_cli/cli.py` & `fast_dev_cli-0.6.4/fast_dev_cli/cli.py`

 * *Files identical despite different names*

### Comparing `fast_dev_cli-0.6.2/pyproject.toml` & `fast_dev_cli-0.6.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 [tool.poetry]
 name = "fast-dev-cli"
-version = "0.6.2"
+version = "0.6.4"
 description = ""
 authors = ["Waket Zheng <waketzheng@gmail.com>"]
 readme = "README.md"
 packages = [{include = "fast_dev_cli"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 click = ">=7.1.1"
 isort = {version = ">=5.12.0", optional = true}
 black = {version = ">=23.9.1", optional = true}
 ruff = {version = ">=0.3", optional = true}
-typer = {extras = ["all"], version = ">=0.9.0", optional = true}
 mypy = {version = ">=1.5.0", optional = true}
 coverage = {version = ">=6.5.0", optional = true}
 bumpversion = {version = "^0.6.0", optional = true}
-pytest = {version = "^8.0.2", optional = true}
+pytest = {version = "^8.1.1", optional = true}
+typer = {version = ">=0.12.0", optional = true}
 
 [tool.poetry.extras]
 all = ["isort", "black", "ruff", "typer", "mypy", "bumpversion", "pytest", "coverage"]
 
 [tool.poetry.group.dev.dependencies]
 isort = "*"
 black = "*"
 ruff = ">=0.3"
 mypy = "*"
 pytest = "*"
 coverage = "*"
 bumpversion = "*"
 typer = {extras = ["all"], version = "*"}
-ipython = "^8.22.2"
+ipython = "^8.23.0"
 coveralls = "^3.3.1"
-pytest-mock = "^3.12.0"
+pytest-mock = "^3.14.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 fast = "fast_dev_cli:cli"
```

### Comparing `fast_dev_cli-0.6.2/PKG-INFO` & `fast_dev_cli-0.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: fast-dev-cli
-Version: 0.6.2
+Version: 0.6.4
 Summary: 
 Author: Waket Zheng
 Author-email: waketzheng@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: all
 Requires-Dist: black (>=23.9.1) ; extra == "all"
 Requires-Dist: bumpversion (>=0.6.0,<0.7.0) ; extra == "all"
 Requires-Dist: click (>=7.1.1)
 Requires-Dist: coverage (>=6.5.0) ; extra == "all"
 Requires-Dist: isort (>=5.12.0) ; extra == "all"
 Requires-Dist: mypy (>=1.5.0) ; extra == "all"
-Requires-Dist: pytest (>=8.0.2,<9.0.0) ; extra == "all"
+Requires-Dist: pytest (>=8.1.1,<9.0.0) ; extra == "all"
 Requires-Dist: ruff (>=0.3) ; extra == "all"
-Requires-Dist: typer[all] (>=0.9.0) ; extra == "all"
+Requires-Dist: typer (>=0.12.0) ; extra == "all"
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://fastdevcli.waketzheng.top/img/logo-margin/logo-teal.png" alt="FastDevCli">
 </p>
 <p align="center">
     <em>Toolkit for python code lint/test/bump ...</em>
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: fast-dev-cli Version: 0.6.2 Summary: Author: Waket
+Metadata-Version: 2.1 Name: fast-dev-cli Version: 0.6.4 Summary: Author: Waket
 Zheng Author-email: waketzheng@gmail.com Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: all Requires-Dist: black (>=23.9.1) ; extra == "all" Requires-
 Dist: bumpversion (>=0.6.0,<0.7.0) ; extra == "all" Requires-Dist: click
 (>=7.1.1) Requires-Dist: coverage (>=6.5.0) ; extra == "all" Requires-Dist:
 isort (>=5.12.0) ; extra == "all" Requires-Dist: mypy (>=1.5.0) ; extra ==
-"all" Requires-Dist: pytest (>=8.0.2,<9.0.0) ; extra == "all" Requires-Dist:
-ruff (>=0.3) ; extra == "all" Requires-Dist: typer[all] (>=0.9.0) ; extra ==
-"all" Description-Content-Type: text/markdown
+"all" Requires-Dist: pytest (>=8.1.1,<9.0.0) ; extra == "all" Requires-Dist:
+ruff (>=0.3) ; extra == "all" Requires-Dist: typer (>=0.12.0) ; extra == "all"
+Description-Content-Type: text/markdown
                                  [FastDevCli]
                   TToooollkkiitt ffoorr ppyytthhoonn ccooddee lliinntt//tteesstt//bbuummpp ......
    _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_G_i_t_h_u_b_A_c_t_i_o_n_R_e_s_u_l_t_]_[_C_o_v_e_r_a_g_e
                                     _S_t_a_t_u_s_]
 --- **Source Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_w_a_k_e_t_z_h_e_n_g_/_f_a_s_t_-_d_e_v_-_c_l_i ## Requirements
 Python 3.11+ ## Installation
 ```console $ pip install "fast-dev-cli[all]" ---> 100% Successfully installed
```

