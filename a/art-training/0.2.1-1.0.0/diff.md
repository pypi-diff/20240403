# Comparing `tmp/art_training-0.2.1.tar.gz` & `tmp/art_training-1.0.0.tar.gz`

## Comparing `art_training-0.2.1.tar` & `art_training-1.0.0.tar`

### file list

```diff
@@ -1,72 +1,77 @@
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 art_training-0.2.1/readthedocs.yml
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 art_training-0.2.1/setup.cfg
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 art_training-0.2.1/tox.ini
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 art_training-0.2.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 art_training-0.2.1/art/__init__.py
--rw-r--r--   0        0        0     8816 2020-02-02 00:00:00.000000 art_training-0.2.1/art/checks.py
--rw-r--r--   0        0        0     6920 2020-02-02 00:00:00.000000 art_training-0.2.1/art/core.py
--rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 art_training-0.2.1/art/decorators.py
--rw-r--r--   0        0        0     5791 2020-02-02 00:00:00.000000 art_training-0.2.1/art/loggers.py
--rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 art_training-0.2.1/art/metrics.py
--rw-r--r--   0        0        0     8888 2020-02-02 00:00:00.000000 art_training-0.2.1/art/project.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 art_training-0.2.1/art/py.typed
--rw-r--r--   0        0        0    22817 2020-02-02 00:00:00.000000 art_training-0.2.1/art/steps.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 art_training-0.2.1/art/cli/__init__.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 art_training-0.2.1/art/cli/__main__.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 art_training-0.2.1/art/cli/main.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 art_training-0.2.1/art/cli/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 art_training-0.2.1/art/dashboard/__init__.py
--rw-r--r--   0        0        0     5241 2020-02-02 00:00:00.000000 art_training-0.2.1/art/dashboard/app.py
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 art_training-0.2.1/art/dashboard/backend.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 art_training-0.2.1/art/dashboard/const.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 art_training-0.2.1/art/dashboard/help.py
--rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 art_training-0.2.1/art/dashboard/layout.py
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 art_training-0.2.1/art/dashboard/timeline.py
--rw-r--r--   0        0        0    17733 2020-02-02 00:00:00.000000 art_training-0.2.1/art/dashboard/assets/pallet.jpg
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 art_training-0.2.1/art/dashboard/assets/timeline.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 art_training-0.2.1/art/utils/__init__.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 art_training-0.2.1/art/utils/enums.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 art_training-0.2.1/art/utils/exceptions.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 art_training-0.2.1/art/utils/paths.py
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 art_training-0.2.1/art/utils/savers.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 art_training-0.2.1/docs/Makefile
--rw-r--r--   0        0        0    52666 2020-02-02 00:00:00.000000 art_training-0.2.1/docs/art.png
--rwxr-xr-x   0        0        0      769 2020-02-02 00:00:00.000000 art_training-0.2.1/docs/make.bat
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 art_training-0.2.1/docs/requirements.txt
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 art_training-0.2.1/docs/source/conf.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 art_training-0.2.1/docs/source/index.rst
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 art_training-0.2.1/docs/source/apidocs/art.cli.rst
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 art_training-0.2.1/docs/source/apidocs/art.rst
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 art_training-0.2.1/docs/source/apidocs/art.utils.rst
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 art_training-0.2.1/docs/source/apidocs/modules.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 art_training-0.2.1/stubs/cookiecutter/__init__.pyi
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 art_training-0.2.1/stubs/cookiecutter/main/__init__.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 art_training-0.2.1/stubs/dash/__init__.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 art_training-0.2.1/stubs/dash_bootstrap_components/__init__.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 art_training-0.2.1/stubs/dash_mantine_components/__init__.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 art_training-0.2.1/stubs/datasets/__init__.pyi
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 art_training-0.2.1/stubs/github/__init__.pyi
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 art_training-0.2.1/stubs/lightning/__init__.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 art_training-0.2.1/stubs/lightning/pytorch/__init__.pyi
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 art_training-0.2.1/stubs/lightning/pytorch/accelerators.pyi
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 art_training-0.2.1/stubs/lightning/pytorch/loggers.pyi
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 art_training-0.2.1/stubs/lightning/pytorch/utilities.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 art_training-0.2.1/stubs/lightning/pytorch/core/__init__.pyi
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 art_training-0.2.1/stubs/lightning/pytorch/core/callbacks.pyi
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 art_training-0.2.1/stubs/lightning/pytorch/core/datamodule.pyi
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 art_training-0.2.1/stubs/lightning/pytorch/core/module.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 art_training-0.2.1/stubs/lightning/utilities/__init__.pyi
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 art_training-0.2.1/stubs/lightning/utilities/seed.pyi
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 art_training-0.2.1/stubs/neptune/__init__.pyi
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 art_training-0.2.1/stubs/neptune/exceptions/__init__.pyi
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 art_training-0.2.1/stubs/neptune/utils/__init__.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 art_training-0.2.1/stubs/plotly/__init__.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 art_training-0.2.1/stubs/plotly/express/__init__.pyi
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 art_training-0.2.1/stubs/wandb/__init__.pyi
--rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 art_training-0.2.1/tests/test_jupyter_tutorial.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 art_training-0.2.1/tests/utils/test_files.txt
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 art_training-0.2.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 art_training-0.2.1/LICENCE
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 art_training-0.2.1/README.md
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 art_training-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     5042 2020-02-02 00:00:00.000000 art_training-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 art_training-1.0.0/readthedocs.yml
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 art_training-1.0.0/setup.cfg
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 art_training-1.0.0/tox.ini
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 art_training-1.0.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 art_training-1.0.0/art/__init__.py
+-rw-r--r--   0        0        0     9239 2020-02-02 00:00:00.000000 art_training-1.0.0/art/checks.py
+-rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 art_training-1.0.0/art/core.py
+-rw-r--r--   0        0        0     6365 2020-02-02 00:00:00.000000 art_training-1.0.0/art/decorators.py
+-rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 art_training-1.0.0/art/loggers.py
+-rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 art_training-1.0.0/art/metrics.py
+-rw-r--r--   0        0        0    10307 2020-02-02 00:00:00.000000 art_training-1.0.0/art/project.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 art_training-1.0.0/art/py.typed
+-rw-r--r--   0        0        0    29947 2020-02-02 00:00:00.000000 art_training-1.0.0/art/steps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 art_training-1.0.0/art/cli/__init__.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 art_training-1.0.0/art/cli/__main__.py
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 art_training-1.0.0/art/cli/main.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 art_training-1.0.0/art/cli/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 art_training-1.0.0/art/dashboard/__init__.py
+-rw-r--r--   0        0        0     5241 2020-02-02 00:00:00.000000 art_training-1.0.0/art/dashboard/app.py
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 art_training-1.0.0/art/dashboard/backend.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 art_training-1.0.0/art/dashboard/const.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 art_training-1.0.0/art/dashboard/help.py
+-rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 art_training-1.0.0/art/dashboard/layout.py
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 art_training-1.0.0/art/dashboard/timeline.py
+-rw-r--r--   0        0        0    17733 2020-02-02 00:00:00.000000 art_training-1.0.0/art/dashboard/assets/pallet.jpg
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 art_training-1.0.0/art/dashboard/assets/timeline.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 art_training-1.0.0/art/utils/__init__.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 art_training-1.0.0/art/utils/enums.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 art_training-1.0.0/art/utils/exceptions.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 art_training-1.0.0/art/utils/paths.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 art_training-1.0.0/art/utils/quickstart.py
+-rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 art_training-1.0.0/art/utils/savers.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 art_training-1.0.0/docs/Makefile
+-rw-r--r--   0        0        0    52666 2020-02-02 00:00:00.000000 art_training-1.0.0/docs/art.png
+-rw-r--r--   0        0        0    70964 2020-02-02 00:00:00.000000 art_training-1.0.0/docs/dashboard.png
+-rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 art_training-1.0.0/docs/make.bat
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 art_training-1.0.0/docs/requirements.txt
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 art_training-1.0.0/docs/source/conf.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 art_training-1.0.0/docs/source/index.rst
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 art_training-1.0.0/docs/source/apidocs/art.cli.rst
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 art_training-1.0.0/docs/source/apidocs/art.rst
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 art_training-1.0.0/docs/source/apidocs/art.utils.rst
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 art_training-1.0.0/docs/source/apidocs/modules.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 art_training-1.0.0/stubs/cookiecutter/__init__.pyi
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 art_training-1.0.0/stubs/cookiecutter/main/__init__.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 art_training-1.0.0/stubs/dash/__init__.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 art_training-1.0.0/stubs/dash_bootstrap_components/__init__.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 art_training-1.0.0/stubs/dash_mantine_components/__init__.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 art_training-1.0.0/stubs/datasets/__init__.pyi
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 art_training-1.0.0/stubs/github/__init__.pyi
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 art_training-1.0.0/stubs/lightning/__init__.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 art_training-1.0.0/stubs/lightning/pytorch/__init__.pyi
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 art_training-1.0.0/stubs/lightning/pytorch/accelerators.pyi
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 art_training-1.0.0/stubs/lightning/pytorch/loggers.pyi
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 art_training-1.0.0/stubs/lightning/pytorch/utilities.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 art_training-1.0.0/stubs/lightning/pytorch/core/__init__.pyi
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 art_training-1.0.0/stubs/lightning/pytorch/core/callbacks.pyi
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 art_training-1.0.0/stubs/lightning/pytorch/core/datamodule.pyi
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 art_training-1.0.0/stubs/lightning/pytorch/core/module.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 art_training-1.0.0/stubs/lightning/utilities/__init__.pyi
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 art_training-1.0.0/stubs/lightning/utilities/seed.pyi
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 art_training-1.0.0/stubs/neptune/__init__.pyi
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 art_training-1.0.0/stubs/neptune/exceptions/__init__.pyi
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 art_training-1.0.0/stubs/neptune/utils/__init__.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 art_training-1.0.0/stubs/plotly/__init__.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 art_training-1.0.0/stubs/plotly/express/__init__.pyi
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 art_training-1.0.0/stubs/wandb/__init__.pyi
+-rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 art_training-1.0.0/tests/test_jupyter_tutorial.py
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 art_training-1.0.0/tests/test_quickstart.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 art_training-1.0.0/tests/test_regularize_tutorial.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 art_training-1.0.0/tests/utils.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 art_training-1.0.0/tests/data/test_files.txt
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 art_training-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 art_training-1.0.0/LICENCE
+-rw-r--r--   0        0        0    10921 2020-02-02 00:00:00.000000 art_training-1.0.0/README.md
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 art_training-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    12542 2020-02-02 00:00:00.000000 art_training-1.0.0/PKG-INFO
```

### Comparing `art_training-0.2.1/.github/workflows/tests.yml` & `art_training-1.0.0/.github/workflows/tests.yml`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-name: Tests
-
-on:
-  - push
-
-jobs:
-  test:
-    runs-on: ${{ matrix.os }}
-    strategy:
-      matrix:
-        os: [ubuntu-latest]
-        python-version: ["3.10"]
-
-    steps:
-      - uses: actions/checkout@v2
-      - name: Set up Python $${{ matrix.python-version }}
-        uses: actions/setup-python@v2
-        with:
-          python-version: ${{ matrix.python-version }}
-      - name: Install dependencies
-        run: |
-          python -m pip install --upgrade pip
-          pip install tox tox-gh-actions
-      - name: Test with tox
-        run: tox
+name: Tests
+
+on:
+  - push
+
+jobs:
+  test:
+    runs-on: ${{ matrix.os }}
+    strategy:
+      matrix:
+        os: [ubuntu-latest]
+        python-version: ["3.10"]
+
+    steps:
+      - uses: actions/checkout@v2
+      - name: Set up Python $${{ matrix.python-version }}
+        uses: actions/setup-python@v2
+        with:
+          python-version: ${{ matrix.python-version }}
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          pip install tox tox-gh-actions
+      - name: Test with tox
+        run: tox
```

### Comparing `art_training-0.2.1/art/core.py` & `art_training-1.0.0/art/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 from typing import Any, Dict, Union
 
 import lightning as L
 import torch.nn
 from torch.utils.data import DataLoader
 
 from art.metrics import MetricCalculator
-from art.utils.enums import LOSS, PREDICTION, TARGET
+from art.utils.enums import LOSS, PREDICTION, TARGET, TrainingStage
 
 
 class ArtModule(L.LightningModule, ABC):
     def __init__(
         self,
     ):
         super().__init__()
         self.regularized = True
-        self.reset_pipelines()
+        self.set_pipelines()
+        self.stage: TrainingStage = TrainingStage.TRAIN
 
     """
     A module for managing the training process and application of various model configurations.
     """
 
     def set_metric_calculator(self, metric_calculator: MetricCalculator):
         """
@@ -38,15 +39,15 @@
 
         Raises:
             ValueError: If the metric calculator has not been set.
         """
         if not hasattr(self, "metric_calculator"):
             raise ValueError("You need to set metric calculator first!")
 
-    def reset_pipelines(self):
+    def set_pipelines(self):
         """
         Reset pipelines for training, validation, and testing.
         """
         self.train_step_pipeline = [
             self.parse_data,
             self.predict,
             self.compute_metrics,
@@ -56,48 +57,14 @@
             self.parse_data,
             self.predict,
             self.compute_metrics,
             self.compute_loss,
         ]
         self.ml_train_pipeline = [self.ml_parse_data, self.baseline_train]
 
-    def turn_on_model_regularizations(self):
-        """
-        Turn on model regularizations.
-        """
-        if not self.regularized:
-            for param in self.parameters():
-                name, obj = param
-                if isinstance(obj, torch.nn.Dropout):
-                    obj.p = self.unregularized_params[name]
-
-            self.configure_optimizers = self.original_configure_optimizers
-
-            self.regularized = True
-
-    def turn_off_model_reguralizations(self):
-        """
-        Turn off model regularizations.
-        """
-        if self.regularized:
-            self.unregularized_params = {}
-            for param in self.parameters():
-                name, obj = param
-                if isinstance(obj, torch.nn.Dropout):
-                    self.unregularized_params[name] = obj.p
-                    obj.p = 0
-
-            # Simple Adam, no fancy optimizers at this stage
-            self.original_configure_optimizers = self.configure_optimizers
-            self.configure_optimizers = lambda self: torch.optim.Adam(
-                self.parameters(), lr=3e-4
-            )
-
-            self.regularized = False
-
     def parse_data(self, data: Dict):
         """
         Parse data.
 
         Args:
             data (Dict): Data to parse.
 
@@ -149,14 +116,15 @@
         """
         Validation step.
 
         Args:
             batch (Union[Dict[str, Any], DataLoader, torch.Tensor]): Batch to validate.
             batch_idx (int): Batch index.
         """
+        self.stage = TrainingStage.VALIDATION
         data = {"batch": batch, "batch_idx": batch_idx}
         for func in self.validation_step_pipeline:
             data = func(data)
 
     def training_step(
         self, batch: Union[Dict[str, Any], DataLoader, torch.Tensor], batch_idx: int
     ):
@@ -166,14 +134,15 @@
         Args:
             batch (Union[Dict[str, Any], DataLoader, torch.Tensor]): Batch to train.
             batch_idx (int): Batch index.
 
         Returns:
             Dict: Data with loss.
         """
+        self.stage = TrainingStage.TRAIN
         data = {"batch": batch, "batch_idx": batch_idx}
         for func in self.train_step_pipeline:
             data = func(data)
 
         return data[LOSS]
 
     def test_step(
@@ -182,14 +151,15 @@
         """
         Test step.
 
         Args:
             batch (Union[Dict[str, Any], DataLoader, torch.Tensor]): Batch to test.
             batch_idx (int): Batch index.
         """
+        self.stage = TrainingStage.TEST
         data = {"batch": batch, "batch_idx": batch_idx}
         for func in self.validation_step_pipeline:
             data = func(data)
 
     def ml_parse_data(self, data: Dict):
         """
         Parse data for machine learning training.
```

### Comparing `art_training-0.2.1/art/loggers.py` & `art_training-1.0.0/art/loggers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,36 @@
 import os
 import sys
 import uuid
 from datetime import datetime
+from enum import Enum
 from pathlib import Path
-from typing import List, Optional, Union
+from typing import TYPE_CHECKING, List, Optional, Union
 
 import numpy as np
 from lightning.pytorch.loggers import NeptuneLogger, WandbLogger
 from loguru import logger
 
+if TYPE_CHECKING:
+    from loguru import Logger
+
+
+class LoggerFlags(Enum):
+    SUPRESS_STDOUT = "supress_stdout"
+
+
 logger.remove()
-logger.add(sys.stdout, format="{message}", level="DEBUG")
+logger.add(
+    sys.stdout,
+    format="{message}",
+    level="DEBUG",
+    filter=lambda record: not record["extra"].get(
+        LoggerFlags.SUPRESS_STDOUT.value, False
+    ),
+)
 
 
 def get_run_id() -> str:
     return datetime.now().strftime("%Y-%m-%d_%H-%M-%S") + "_" + str(uuid.uuid4())
 
 
 def get_new_log_file_name(run_id: str) -> str:
@@ -27,17 +43,25 @@
     )
 
 
 def remove_logger(logger_id: int):
     art_logger.remove(logger_id)
 
 
+def supress_stdout(current_logger: "Logger") -> "Logger":
+    return current_logger.bind(**{LoggerFlags.SUPRESS_STDOUT.value: True})
+
+
 art_logger = logger
 
 
+def log_yellow_warning(message: str):
+    art_logger.opt(ansi=True).warning(f"<yellow>{message}</yellow>")
+
+
 class NeptuneLoggerAdapter(NeptuneLogger):
     """
     This is a wrapper for LightningLogger for simplifying basic functionalities between different loggers.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
```

### Comparing `art_training-0.2.1/art/metrics.py` & `art_training-1.0.0/art/metrics.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,125 +1,138 @@
-from typing import TYPE_CHECKING, Any, Dict, List
-
-from art.utils.enums import TrainingStage
-
-if TYPE_CHECKING:
-    from art.core import ArtModule
-    from art.project import ArtProject
-
-
-class DefaultMetric:
-    """Placeholder for a default metric."""
-
-    pass
-
-
-class DefaultModel:
-    """Placeholder for a default model."""
-
-    pass
-
-
-class SkippedMetric:
-    """Represents a metric that should be skipped during certain training stages."""
-
-    def __init__(
-        self,
-        metric,
-        stages: List[str] = [TrainingStage.TRAIN.value, TrainingStage.VALIDATION.value],
-    ):
-        self.metric = metric.__class__.__name__
-        self.stages = stages
-
-
-class MetricCalculator:
-    """
-    Facilitates the management and application of metrics during different stages of training.
-
-    This class makes preparing templates for different kinds of projects easy.
-    """
-
-    def __init__(self, experiment: "ArtProject"):
-        self.metrics: List[Any] = []
-        self.experiment = experiment
-
-    def build_name(self, metric: Any) -> str:
-        """
-        Builds a name for the metric based on its type, current stage.
-
-        Args:
-            metric (Any): The metric being calculated.
-        """
-        stage = self.experiment.state.get_current_stage()
-
-        return f"{metric.__class__.__name__}-{stage}"
-
-    def to(self, device: str):
-        """
-        Move all metrics to a specified device.
-
-        Args:
-            device (str): The device to move the metrics to.
-        """
-        self.metrics = [metric.to(device) for metric in self.metrics]
-
-    def add_metrics(self, metric: Any):
-        """
-        Add metrics to the list.
-
-        Args:
-            metric (Any): The metric to add.
-        """
-        self.metrics.extend(metric)
-
-    def compile(self, skipped_metrics: List[SkippedMetric]):
-        """
-        Organize metrics based on stages, skipping specified ones.
-
-        Args:
-            skipped_metrics (List[SkippedMetric]): A list of SkippedMetric instances.
-        """
-        # Initialize a dictionary to store compiled metrics for each training stage
-        self.compiled_metrics: Dict = {
-            TrainingStage.TRAIN.value: [],
-            TrainingStage.VALIDATION.value: [],
-            TrainingStage.TEST.value: [],
-            TrainingStage.SANITY_CHECK.value: [],
-        }
-
-        # Convert the list of SkippedMetric instances into a dictionary for easier access
-        skipped_metrics_dict = {sm.metric: sm.stages for sm in skipped_metrics}
-
-        # Populate compiled_metrics based on whether a metric should be included or skipped for each stage
-        for metric in self.metrics:
-            if hasattr(metric, "reset"):
-                metric.reset()  # Ensure state is forgotten between steps
-
-            metric_name = metric.__class__.__name__
-            if metric_name not in skipped_metrics_dict.keys():
-                for stage in self.compiled_metrics.keys():
-                    self.compiled_metrics[stage].append(metric)
-            else:
-                for stage in self.compiled_metrics.keys():
-                    if stage not in skipped_metrics_dict[metric_name]:
-                        self.compiled_metrics[stage].append(metric)
-
-    def __call__(self, model: "ArtModule", data_for_metrics: Dict) -> Dict:
-        """
-        Compute and log metrics for the current training stage.
-
-        Args:
-            model (ArtModule): The model for which the metrics are being calculated.
-            data_for_metrics (Dict): The data used for calculating metrics.
-
-        Returns:
-            The data used for calculating metrics.
-        """
-        stage = self.experiment.state.get_current_stage()
-        for metric in self.compiled_metrics[stage]:
-            prepared_data = model.prepare_for_metric(data_for_metrics)
-            metric_val = metric(*prepared_data)
-            metric_name = self.build_name(metric)
-            model.log(metric_name, metric_val, on_step=False, on_epoch=True)
-            data_for_metrics[metric.__class__.__name__] = metric_val
-
-        return data_for_metrics
+from typing import TYPE_CHECKING, Any, Dict, List
+
+from art.utils.enums import TrainingStage
+
+if TYPE_CHECKING:
+    from art.core import ArtModule
+    from art.project import ArtProject
+
+
+class DefaultMetric:
+    """Placeholder for a default metric."""
+
+    pass
+
+
+class DefaultModel:
+    """Placeholder for a default model."""
+
+    pass
+
+
+class SkippedMetric:
+    """Represents a metric that should be skipped during certain training stages."""
+
+    def __init__(
+        self,
+        metric,
+        stages: List[str] = [TrainingStage.TRAIN.value, TrainingStage.VALIDATION.value],
+    ):
+        self.metric = metric.__class__.__name__
+        self.stages = stages
+
+
+def build_metric_name(metric: Any, stage: str) -> str:
+    """
+    Builds a name for the metric based on its type and given training stage.
+
+    Args:
+        metric (Any): The metric being calculated.
+        stage (str): The current stage of training.
+    """
+    return f"{metric.__class__.__name__}-{stage}"
+
+
+class MetricCalculator:
+    """
+    Facilitates the management and application of metrics during different stages of training.
+
+    This class makes preparing templates for different kinds of projects easy.
+    """
+
+    def __init__(self, experiment: "ArtProject"):
+        self.metrics: List[Any] = []
+        self.experiment = experiment
+
+    def build_name(self, metric: Any) -> str:
+        """
+        Builds a name for the metric based on its type, current stage.
+
+        Args:
+            metric (Any): The metric being calculated.
+        """
+        stage = self.experiment.state.get_current_stage()
+
+        return build_metric_name(metric, stage)
+
+    def to(self, device: str):
+        """
+        Move all metrics to a specified device.
+
+        Args:
+            device (str): The device to move the metrics to.
+        """
+        self.metrics = [metric.to(device) for metric in self.metrics]
+
+    def add_metrics(self, metric: Any):
+        """
+        Add metrics to the list.
+
+        Args:
+            metric (Any): The metric to add.
+        """
+        self.metrics.extend(metric)
+
+    def compile(self, skipped_metrics: List[SkippedMetric]):
+        """
+        Organize metrics based on stages, skipping specified ones.
+
+        Args:
+            skipped_metrics (List[SkippedMetric]): A list of SkippedMetric instances.
+        """
+        # Initialize a dictionary to store compiled metrics for each training stage
+        self.compiled_metrics: Dict = {
+            TrainingStage.TRAIN.value: [],
+            TrainingStage.VALIDATION.value: [],
+            TrainingStage.TEST.value: [],
+            TrainingStage.SANITY_CHECK.value: [],
+        }
+
+        # Convert the list of SkippedMetric instances into a dictionary for easier access
+        skipped_metrics_dict = {sm.metric: sm.stages for sm in skipped_metrics}
+
+        # Populate compiled_metrics based on whether a metric should be included or skipped for each stage
+        for metric in self.metrics:
+            if hasattr(metric, "reset"):
+                metric.reset()  # Ensure state is forgotten between steps
+
+            metric_name = metric.__class__.__name__
+            if metric_name not in skipped_metrics_dict.keys():
+                for stage in self.compiled_metrics.keys():
+                    self.compiled_metrics[stage].append(metric)
+            else:
+                for stage in self.compiled_metrics.keys():
+                    if stage not in skipped_metrics_dict[metric_name]:
+                        self.compiled_metrics[stage].append(metric)
+
+    def __call__(self, model: "ArtModule", data_for_metrics: Dict) -> Dict:
+        """
+        Compute and log metrics for the current training stage.
+
+        Args:
+            model (ArtModule): The model for which the metrics are being calculated.
+            data_for_metrics (Dict): The data used for calculating metrics.
+
+        Returns:
+            The data used for calculating metrics.
+        """
+        stage = self.experiment.state.get_current_stage()
+        for metric in self.compiled_metrics[stage]:
+            prepared_data = model.prepare_for_metric(data_for_metrics)
+            metric_val = metric(*prepared_data)
+            metric_name = self.build_name(metric)
+            model.log(
+                metric_name, metric_val, on_step=False, on_epoch=True, prog_bar=True
+            )
+            data_for_metrics[metric.__class__.__name__] = metric_val
+
+        return data_for_metrics
```

### Comparing `art_training-0.2.1/art/project.py` & `art_training-1.0.0/art/project.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from collections import defaultdict
-from typing import Any, Dict, List, Union
+from typing import Any, Dict, List, Optional, Union
 
 import lightning as L
 
 from art.checks import Check
+from art.decorators import ModelDecorator
 from art.loggers import (
     add_logger,
     art_logger,
     get_new_log_file_name,
     get_run_id,
     remove_logger,
+    supress_stdout,
 )
 from art.metrics import MetricCalculator, SkippedMetric
 from art.steps import ModelStep, Step
 from art.utils.enums import TrainingStage
 from art.utils.exceptions import CheckFailedException
 from art.utils.paths import EXPERIMENT_LOG_DIR
 
@@ -46,23 +48,14 @@
         Returns all steps that were run
 
         Returns:
             Dict[str, Dict[str, Dict[str, str]]]: [description]
         """
         return self.step_states
 
-    def add_step(self, step):
-        """
-        Adds step to the state
-
-        Args:
-            step (Step): A step to be add the the project
-        """
-        self.step_states.append(step)
-
     def get_current_step(self):
         """
         Gets current step
 
         Returns:
             Step: Current step
         """
@@ -79,34 +72,43 @@
 
 
 class ArtProject:
     """
     Represents a single Art project, encapsulating steps, state, metrics, and logging.
     """
 
-    def __init__(self, name: str, datamodule: L.LightningDataModule, **kwargs):
+    def __init__(
+        self,
+        name: str,
+        datamodule: L.LightningDataModule,
+        use_metric_calculator: bool = True,
+        **kwargs,
+    ):
         """
         Initialize an Art project.
 
         Args:
             name (str): The name of the project.
             datamodule (L.LightningDataModule): Data module to be used in this project.
+            use_metric_calculator (bool): Whether to use the metric calculator.
             **kwargs: Additional keyword arguments.
         """
         self.name = name
         self.steps: List[Dict] = []
         self.datamodule = datamodule
         self.state = ArtProjectState()
-        self.metric_calculator = MetricCalculator(self)
+        self.metric_calculator = (
+            MetricCalculator(self) if use_metric_calculator else None
+        )
         self.changed_steps: List[str] = []
 
     def add_step(
         self,
         step: "Step",
-        checks: List[Check],
+        checks: Optional[List[Check]] = [],
         skipped_metrics: List[SkippedMetric] = [],
     ):
         """
         Add a step to the project.
 
         Args:
             step (Step): The step to be added.
@@ -159,83 +161,131 @@
             checks (List[Check]): List of checks to validate.
 
         Returns:
             bool: True if the step must be run, False otherwise.
         """
         if not step.was_run():
             return True
+        if step.check_if_already_tried():
+            return False
         else:
             step_current_hash = step.get_hash()
             step_saved_hash = step.get_latest_run()["hash"]
             model_changed = True if step_current_hash != step_saved_hash else False
             if model_changed:
                 self.changed_steps.append(step.get_full_step_name())
             try:
                 self.check_checks(step, checks)
             except CheckFailedException:
                 return True
 
             return False
 
-    def run_all(self, force_rerun=False):
+    def run_step(
+        self,
+        step: "Step",
+        skipped_metrics: List[SkippedMetric],
+        model_decorators: List[ModelDecorator],
+        trainer_kwargs: Dict[str, Any],
+        run_id: str,
+    ):
+        """
+        Run a given step.
+
+        Args:
+            step (Step): The step to run.
+            skipped_metrics (List[SkippedMetric]): List of metrics to skip for this step.
+            model_decorators (List[Tuple(str, Callable)]): List of model decorators to be applied.
+            run_id (str): The ID of the run.
+        """
+        if isinstance(step, ModelStep):
+            step(
+                self.state.step_states,
+                self.datamodule,
+                self.metric_calculator,
+                skipped_metrics,
+                model_decorators,
+                trainer_kwargs,
+                run_id,
+            )
+        else:
+            step(
+                self.state.step_states,
+                self.datamodule,
+                run_id,
+            )
+
+    def run_all(
+        self,
+        force_rerun=False,
+        model_decorators: List[ModelDecorator] = [],
+        trainer_kwargs: Dict[str, Any] = {},
+    ):
         """
         Execute all steps in the project.
 
         Args:
             force_rerun (bool): Whether to force rerun all steps.
+            model_decorators (List[ModelDecorator]): List of model decorators to be applied.
         """
         run_id = get_run_id()
         logger_id = add_logger(EXPERIMENT_LOG_DIR / get_new_log_file_name(run_id))
         self.changed_steps = []
         try:
             for step_dict in self.steps:
-                self.metric_calculator.compile(step_dict["skipped_metrics"])
                 step, checks = step_dict["step"], step_dict["checks"]
                 self.state.current_step = step
 
                 rerun_step = self.check_if_must_be_run(step, checks)
 
                 if not rerun_step and not force_rerun:
                     self.fill_step_states(step)
                     continue
                 try:
-                    step(
-                        self.state.step_states,
-                        self.datamodule,
-                        self.metric_calculator,
+                    self.run_step(
+                        step,
+                        step_dict["skipped_metrics"],
+                        model_decorators,
+                        trainer_kwargs,
                         run_id,
                     )
                     self.check_checks(step, checks)
                 except CheckFailedException as e:
                     art_logger.warning(e)
-                    step.save_to_disk()
-                    break
+                    if not step.continue_on_failure:
+                        step.save_to_disk()
+                        break
 
                 self.fill_step_states(step)
                 step.save_to_disk()
 
             self.print_summary()
         except Exception as e:
+            supress_stdout(art_logger).exception(e)
             raise e
         finally:
             remove_logger(logger_id)
 
     def print_summary(self):
         """
         Prints a summary of the project.
         """
         art_logger.info("Summary: ")
         for step in self.steps:
-            art_logger.info(step["step"])
-            if not step["step"].is_successful():
+            step = step["step"]
+            art_logger.info(step)
+
+            if not step.is_successful() and not step.continue_on_failure:
                 break
+
         if len(self.changed_steps) > 0:
             art_logger.info(
                 f"Code of the following steps was changed: {', '.join(self.changed_steps)}\n Rerun could be needed."
             )
+        art_logger.info("Explore all runs with `python -m art.cli run-dashboard`")
 
     def get_steps(self):
         """
         Retrieve all steps in the project.
 
         Returns:
             List[Dict[str, Any]]: List of steps.
@@ -269,23 +319,14 @@
         Register metrics to the project.
 
         Args:
             metrics (List[Any]): A list of metrics to be registered.
         """
         self.metric_calculator.add_metrics(metrics)
 
-    def to(self, device: str):
-        """
-        Move the metric calculator to a specified device.
-
-        Args:
-            device (str): The device to move the metrics to.
-        """
-        self.metric_calculator.to(device)
-
     def update_datamodule(self, datamodule: L.LightningDataModule):
         """
         Update the data module of the project.
 
         Args:
             datamodule (L.LightningDataModule): New data module to be used in the project.
         """
```

### Comparing `art_training-0.2.1/art/steps.py` & `art_training-1.0.0/art/steps.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 import datetime
 import gc
 import hashlib
 import inspect
 import subprocess
 from abc import ABC, abstractmethod
-from typing import Any, Callable, Dict, Iterable, List, Optional, Union
+from typing import Any, Callable, Dict, List, Optional, Union
 
 import lightning as L
 from lightning import Trainer
 from lightning.pytorch.accelerators import CUDAAccelerator
+from lightning.pytorch.callbacks import ModelCheckpoint
 from lightning.pytorch.loggers import Logger
 
 from art.core import ArtModule
+from art.decorators import ModelDecorator, art_decorate
 from art.loggers import (
     add_logger,
     art_logger,
     get_new_log_file_name,
     get_run_id,
+    log_yellow_warning,
     remove_logger,
 )
-from art.metrics import MetricCalculator
+from art.metrics import MetricCalculator, SkippedMetric
 from art.utils.enums import TrainingStage
-from art.utils.exceptions import MissingLogParamsException
 from art.utils.paths import get_checkpoint_logs_folder_path
 from art.utils.savers import JSONStepSaver
 
 
 class NoModelUsed:
     pass
 
@@ -33,14 +35,15 @@
 class Step(ABC):
     """
     An abstract base class representing a generic step in a project.
     """
 
     name = "Data analysis"
     model = NoModelUsed()
+    continue_on_failure = False
 
     def __init__(self):
         """
         Initialize the step with an empty results dictionary.
         """
         self.results = {
             "scores": {},
@@ -51,15 +54,14 @@
         self.finalized = False
         self.model_name = ""
 
     def __call__(
         self,
         previous_states: Dict,
         datamodule: L.LightningDataModule,
-        metric_calculator: MetricCalculator,
         run_id: Optional[str] = None,
     ):
         """
         Call the step and save its results.
 
         Args:
             previous_states (Dict): Dictionary containing the previous step states.
@@ -90,15 +92,17 @@
         try:
             self.results["commit_id"] = (
                 subprocess.check_output(["git", "rev-parse", "HEAD"])
                 .decode("ascii")
                 .strip()
             )
         except Exception:
-            art_logger.exception("Error while getting commit id!")
+            art_logger.exception(
+                "Error while getting commit id!\nNote: Every art directory should be a git repository"
+            )
 
     def get_full_step_name(self) -> str:
         """
         Retrieve the full name of the step, which is a combination of its ID and name.
 
         Returns:
             str: The full step name.
@@ -161,44 +165,45 @@
     def set_successful(self):
         self.results["successful"] = True
 
     def is_successful(self):
         return self.results["successful"]
 
     @abstractmethod
-    def log_params(
-        self,
-    ):
-        pass
-
-    @abstractmethod
     def do(self, previous_states: Dict):
         """
         Abstract method to execute the step. Must be implemented by child classes.
 
         Args:
             previous_states (Dict): Dictionary containing the previous step states.
         """
         pass
 
     def save_to_disk(self):
         JSONStepSaver().save(self, self.get_full_step_name(), "results.json")
 
+    def check_if_already_tried(self):
+        """The idea of this function is to help the project decide if there is any more reason the step shouldn't be run even though it has failed."""
+        return False
+
 
 class ModelStep(Step):
     """
     A specialized step in the project, representing a model-based step.
     """
 
+    requires_ckpt_callback = True
+
     def __init__(
         self,
         model_class: ArtModule,
         trainer_kwargs: Dict = {},
         model_kwargs: Dict = {},
         model_modifiers: List[Callable] = [],
+        datamodule_modifiers: List[Callable] = [],
         logger: Optional[Logger] = None,
     ):
         """
         Initialize a model-based step.
 
         Args:
             model_class (ArtModule): The model's class associated with this step.
@@ -216,41 +221,57 @@
             raise ValueError(
                 "model_func must be class inhertiting from Art Module or path to the checkpoint. This is to avoid memory leaks. Simplest way of doing this is to use lambda function lambda : ArtModule()"
             )
 
         self.model_class = model_class
         self.model_kwargs = model_kwargs
         self.model_modifiers = model_modifiers
+        self.datamodule_modifiers = datamodule_modifiers
         self.logger = logger
         self.trainer_kwargs = trainer_kwargs
 
         self.model_name = model_class.__name__
 
     def __call__(
         self,
         previous_states: Dict,
         datamodule: L.LightningDataModule,
-        metric_calculator: MetricCalculator,
+        metric_calculator: Union[MetricCalculator, None],
+        skipped_metrics: List[SkippedMetric] = [],
+        model_decorators: List[ModelDecorator] = [],
+        trainer_kwargs: Dict = {},
         run_id: Optional[str] = None,
     ):
         """
         Call the model step, set the metric calculator for the model, and save the results.
 
         Args:
             previous_states (Dict): Dictionary containing the previous step states.
             datamodule (L.LightningDataModule): Data module to be used.
             metric_calculator (MetricCalculator): Metric calculator for this step.
+            skipped_metrics (List[SkippedMetric]): A list of metrics to skip for this step.
+            model_decorators (List[ModelDecorator]): List of model decorators to be applied.
         """
-        self.trainer = Trainer(**self.trainer_kwargs, logger=self.logger)
+        trainer_kwargs = {**self.trainer_kwargs, **trainer_kwargs}
+        self.trainer = Trainer(**trainer_kwargs, logger=self.logger)
         self.metric_calculator = metric_calculator
+        self.model_decorators = model_decorators
         curr_device = (
             "cuda" if isinstance(self.trainer.accelerator, CUDAAccelerator) else "cpu"
         )
-        self.metric_calculator.to(curr_device)
-        super().__call__(previous_states, datamodule, metric_calculator, run_id)
+        if self.metric_calculator is not None:
+            self.metric_calculator.to(curr_device)
+            self.metric_calculator.compile(skipped_metrics)
+
+        for modifier in self.datamodule_modifiers:
+            modifier(datamodule)
+
+        super().__call__(previous_states, datamodule, run_id)
+        self.log_data_params()
+
         del self.trainer
         gc.collect()
 
     def initialize_model(
         self,
     ) -> Optional[ArtModule]:
         """
@@ -258,17 +279,27 @@
         """
         if self.trainer.model is not None:
             return None
 
         model = self.model_class(**self.model_kwargs)
         for modifier in self.model_modifiers:
             modifier(model)
-        model.set_metric_calculator(self.metric_calculator)
 
-        self.log_params(model)
+        for decorator in self.model_decorators:
+            art_decorate(
+                [(model, decorator.funcion_name)],
+                decorator.input_decorator,
+                decorator.output_decorator,
+            )
+
+        if isinstance(model, ArtModule):
+            model.set_metric_calculator(self.metric_calculator)
+            model.set_pipelines()
+
+        self.log_model_params(model)
         return model
 
     def train(self, trainer_kwargs: Dict):
         """
         Train the model using the provided trainer arguments.
 
         Args:
@@ -283,17 +314,20 @@
     def get_hash(self) -> str:
         """
         Compute a hash based on the source code of the step's class.
 
         Returns:
             str: MD5 hash of the step's source code.
         """
-        return hashlib.md5(
-            inspect.getsource(self.model_class).encode("utf-8")
-        ).hexdigest()
+        try:
+            model_code = inspect.getsource(self.model_class).encode("utf-8")
+            return hashlib.md5(model_code).hexdigest()
+        except OSError:
+            art_logger.warning("Could not get source code of the model.")
+            return "Error"
 
     def validate(self, trainer_kwargs: Dict):
         """
         Validate the model using the provided trainer arguments.
 
         Args:
             trainer_kwargs (Dict): Arguments to be passed to the trainer for validating the model.
@@ -336,54 +370,80 @@
         Get the validation stage value from the TrainingStage enum.
 
         Returns:
             str: Validation stage value.
         """
         return TrainingStage.VALIDATION.value
 
-    def log_params(self, model):
+    def log_model_params(self, model):
+        msg = "does not have log_params method. You don't want to regret lack of logs."
+        self.results["parameters"].update(self.trainer_kwargs)
         if hasattr(model, "log_params"):
             model_params = model.log_params()
             self.results["parameters"].update(model_params)
 
         else:
-            raise MissingLogParamsException(
-                "Model does not have log_params method. You don't want to regret lack of logs :)"
-            )
+            log_yellow_warning(f"Art/Lightning Module {msg}")
 
+    def log_data_params(self):
+        msg = "does not have log_params method. You don't want to regret lack of logs."
         if hasattr(self.datamodule, "log_params"):
             data_params = self.datamodule.log_params()
             self.results["parameters"].update(data_params)
+
         else:
-            raise MissingLogParamsException(
-                "Datamodule does not have log_params method. You don't want to regret lack of logs :)"
-            )
+            log_yellow_warning(f"Datamodule {msg}")
 
     def reset_trainer(self, logger: Optional[Logger] = None, trainer_kwargs: Dict = {}):
         """
         Reset the trainer.
         Args:
             trainer_kwargs (Dict): Arguments to be passed to the trainer.
             logger (Optional[Logger], optional): Logger to be used. Defaults to None.
         """
         self.trainer = Trainer(**trainer_kwargs, logger=logger)
 
+    def get_trainloader(self):
+        try:
+            return self.datamodule.train_dataloader()
+        except Exception:
+            self.datamodule.setup(stage=TrainingStage.TRAIN.value)
+            return self.datamodule.train_dataloader()
+
+    def get_valloader(self):
+        try:
+            return self.datamodule.val_dataloader()
+        except Exception:
+            self.datamodule.setup(stage=TrainingStage.VALIDATION.value)
+            return self.datamodule.val_dataloader()
+
+    def check_ckpt_callback(self, trainer_kwargs: Dict):
+        if self.requires_ckpt_callback:
+            except_msg = f"At stage {self.name} it is very likely to train some usefull model. Please provide checkpoint callback. You can check how to do this here https://pytorch-lightning.readthedocs.io/en/1.5.10/extensions/generated/pytorch_lightning.callbacks.ModelCheckpoint.html"
+            if "callbacks" not in trainer_kwargs:
+                log_yellow_warning(except_msg)
+            for callback in trainer_kwargs["callbacks"]:
+                if isinstance(callback, ModelCheckpoint):
+                    return
+                log_yellow_warning(except_msg)
+
 
 class ExploreData(Step):
     """This class checks whether we have some markdown file description of the dataset + we implemented visualizations"""
 
     name = "Data analysis"
     description = "This step allows you to perform data analysis and extract information that is necessery in next steps"
 
 
 class EvaluateBaseline(ModelStep):
     """This class takes a baseline and evaluates/trains it on the dataset"""
 
     name = "Evaluate Baseline"
     description = "Evaluates a baseline on the dataset"
+    requires_ckpt_callback = False
 
     def __init__(
         self,
         baseline: ArtModule,
         device: Optional[str] = "cpu",
     ):
         super().__init__(baseline, {"accelerator": device})
@@ -391,52 +451,57 @@
     def do(self, previous_states: Dict):
         """
         This method evaluates baseline on the dataset
 
         Args:
             previous_states (Dict): previous states
         """
+        # Running setup for ml_train with pure train dataloader
+        self.datamodule.setup(stage=TrainingStage.TRAIN.value)
         art_logger.info("Training baseline")
-        model = self.model_class()
-        model.ml_train({"dataloader": self.datamodule.train_dataloader()})
+        model = self.initialize_model()
+        model.ml_train({"dataloader": self.get_trainloader()})
         art_logger.info("Validating baseline")
-        model.set_metric_calculator(self.metric_calculator)
         result = self.trainer.validate(model=model, datamodule=self.datamodule)
         self.results["scores"].update(result[0])
 
 
 class CheckLossOnInit(ModelStep):
     """This step checks whether the loss on init is as expected"""
 
     name = "Check Loss On Init"
     description = "Checks loss on init"
+    requires_ckpt_callback = False
 
     def __init__(
         self,
         model: ArtModule,
     ):
         super().__init__(model)
 
     def do(self, previous_states: Dict):
         """
         This method checks loss on init. It validates the model on the train dataloader and checks whether the loss is as expected.
 
         Args:
             previous_states (Dict): previous states
         """
-        train_loader = self.datamodule.train_dataloader()
+        # Running setup for train dataloader used in validation
+        self.datamodule.setup(stage=TrainingStage.TRAIN.value)
+        train_loader = self.get_trainloader()
         art_logger.info("Calculating loss on init")
         self.validate(trainer_kwargs={"dataloaders": train_loader})
 
 
 class OverfitOneBatch(ModelStep):
     """This step tries to Overfit one train batch"""
 
     name = "Overfit One Batch"
     description = "Overfits one batch"
+    requires_ckpt_callback = False
 
     def __init__(
         self,
         model: ArtModule,
         number_of_steps: int = 50,
     ):
         self.number_of_steps = number_of_steps
@@ -445,30 +510,32 @@
     def do(self, previous_states: Dict):
         """
         This method overfits one batch
 
         Args:
             previous_states (Dict): previous states
         """
-        train_loader = self.datamodule.train_dataloader()
+        # Running setup for train with pure dataloader
+        self.datamodule.setup(stage=TrainingStage.TRAIN.value)
+        train_loader = self.get_trainloader()
         art_logger.info("Overfitting one batch")
         self.train(trainer_kwargs={"train_dataloaders": train_loader})
         for key, value in self.trainer.logged_metrics.items():
             if hasattr(value, "item"):
                 self.results[key] = value.item()
             else:
                 self.results[key] = value
 
     def get_check_stage(self):
         """Returns check stage"""
         return TrainingStage.TRAIN.value
 
-    def log_params(self, model):
+    def log_model_params(self, model):
         self.results["parameters"]["number_of_steps"] = self.number_of_steps
-        super().log_params(model)
+        super().log_model_params(model)
 
 
 class Overfit(ModelStep):
     """This step tries to overfit the model"""
 
     name = "Overfit"
     description = "Overfits model"
@@ -486,59 +553,151 @@
     def do(self, previous_states: Dict):
         """
         This method overfits the model
 
         Args:
             previous_states (Dict): previous states
         """
-        train_loader = self.datamodule.train_dataloader()
+        # Running setup for train with pure dataloader
+        self.datamodule.setup(stage=TrainingStage.TRAIN.value)
+        train_loader = self.get_trainloader()
         art_logger.info("Overfitting model")
         self.train(trainer_kwargs={"train_dataloaders": train_loader})
         art_logger.info("Validating overfitted model")
         self.validate(trainer_kwargs={"datamodule": self.datamodule})
 
     def get_check_stage(self):
         """Returns check stage"""
         return TrainingStage.TRAIN.value
 
-    def log_params(self, model):
+    def log_model_params(self, model):
         self.results["parameters"]["max_epochs"] = self.max_epochs
-        super().log_params(model)
+        super().log_model_params(model)
 
 
 class Regularize(ModelStep):
     """This step tries applying regularization to the model"""
 
     name = "Regularize"
     description = "Regularizes model"
+    continue_on_failure = True
 
     def __init__(
         self,
         model: ArtModule,
         logger: Optional[Logger] = None,
         trainer_kwargs: Dict = {},
+        model_kwargs: Dict = {},
+        model_modifiers: List[Callable] = [],
+        datamodule_modifiers: List[Callable] = [],
     ):
-        self.trainer_kwargs = trainer_kwargs
-        super().__init__(model, trainer_kwargs, logger=logger)
+        """
+        Args:
+            model (ArtModule): model
+            logger (Logger, optional): logger. Defaults to None.
+            trainer_kwargs (Dict, optional): Kwargs passed to lightning Trainer. Defaults to {}.
+            model_kwargs (Dict, optional): Kwargs passed to model. Defaults to {}.
+            model_modifiers (List[Callable], optional): model modifiers. Defaults to [].
+            datamodule_modifiers (List[Callable], optional): datamodule modifiers. Defaults to [].
+        """
+        super().__init__(
+            model,
+            trainer_kwargs,
+            model_kwargs,
+            model_modifiers,
+            datamodule_modifiers,
+            logger=logger,
+        )
+
+        # Internal structure to store regularization parameters
+        self.parameters = {
+            **model_kwargs,
+            "model_modifiers": self.stringify_modifiers(self.model_modifiers),
+            "datamodule_modifiers": self.stringify_modifiers(self.datamodule_modifiers),
+        }
+        # To decide whether to rerun the step
+        self.was_already_tried = False
+        # Regularize parameters will be saved to JSON
+        self.results["parameters"]["regularize"] = self.parameters
+
+    def stringify_modifiers(self, modifiers: List[Callable]):
+        return "_".join(sorted([modifier.__repr__() for modifier in modifiers]))
 
     def do(self, previous_states: Dict):
         """
         This method regularizes the model
 
         Args:
             previous_states (Dict): previous states
         """
-        art_logger.info("Turning on regularization")
-        self.datamodule.turn_on_regularizations()
         art_logger.info("Training regularized model")
         self.train(trainer_kwargs={"datamodule": self.datamodule})
 
-    def log_params(self, model):
-        self.results["parameters"].update(self.trainer_kwargs)
-        super().log_params(model)
+    def update_was_already_tried(self):
+        """This method verify if such Regularize parameters was already tried and updates self.was_already_tried"""
+        if not self.was_run():
+            return
+
+        # Load all previous runs and check if any of them has the same parameters
+        runs = JSONStepSaver().load(self.get_full_step_name())["runs"]
+        for run in runs:
+            if run["parameters"]["regularize"] == self.parameters:
+                self.was_already_tried = True
+                self.results = run
+
+    def check_if_already_tried(self):
+        """The idea of this function is to help the project decide if there is any more reason the step shouldn't be run even though it has failed."""
+        self.update_was_already_tried()
+        return self.was_already_tried
+
+    def __repr__(self) -> str:
+        # Step suceeded now or previously
+        if self.is_successful():
+            return (
+                f"{super().__repr__()}.\nRegularization Parameters: {self.parameters}"
+            )
+        # Step failed
+        else:
+            # once upon a time
+            if self.was_already_tried:
+                return f"Step: {self.name}, Model: {self.model_name}, Skipped as already tried and failed, Regularization Parameters: {self.parameters}\n"
+            # Now
+            elif self.finalized:
+                return f"{super().__repr__()}.\nRegularization Parameters: {self.parameters}"
+            # Step was not run yet -> not succesfull, not previously tried and not finalized
+            else:
+                return f"Step: {self.name}, Model: {self.model_name}, Skipped as other run has suceeded previously, Regularization Parameters: {self.parameters}\n"
+
+    def save_to_disk(self):
+        # We save only if this was the first time we tried this regularization
+        if not self.was_already_tried:
+            super().save_to_disk()
+
+    def get_latest_run(self) -> Dict:
+        """
+        If step was run returns itself, otherwise returns the latest run from the JSONStepSaver.
+
+        In case of regularization we are interested in the latest successful run.
+
+        Returns:
+            Dict: The latest run.
+        """
+        if self.finalized:
+            return self.results
+        runs = JSONStepSaver().load(self.get_full_step_name())["runs"]
+        for run in runs:
+            if run["successful"]:
+                return run
+        return runs[0]
+
+    def set_successful(self):
+        # In case of regularization each run is like a different step.
+        if not self.finalized:
+            return
+        self.results["successful"] = True
 
 
 class Tune(ModelStep):
     """This step tunes the model"""
 
     name = "Tune"
     description = "Tunes model"
@@ -619,18 +778,14 @@
         if self.fine_tune:
             self.add_unfreezing()
             self.reset_trainer(
                 logger=self.trainer.logger, trainer_kwargs=self.unfreezed_trainer_kwargs
             )
             self.train(trainer_kwargs={"datamodule": self.datamodule})
 
-    def log_params(self, model):
-        self.results["parameters"].update(self.trainer_kwargs)
-        super().log_params(model)
-
     def get_check_stage(self):
         """Returns check stage"""
         return TrainingStage.VALIDATION.value
 
     def add_freezing(self):
         """Adds freezing to the model"""
```

### Comparing `art_training-0.2.1/art/cli/main.py` & `art_training-1.0.0/art/cli/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,16 +74,16 @@
             os.system(f"git push -u origin {current_branch}")
         except Exception as e:
             print("Error while creating GitHub repository:", str(e))
 
 
 @app.command()
 def get_started():
-    """Create a project named 'mnist_tutorial' using the 'mnist_tutorial_cookiecutter' branch."""
-    create_project(project_name="mnist_tutorial", branch="mnist_tutorial_cookiecutter")
+    """Create a project named 'mnist_tutorial' using the 'mnist_tutorial' branch."""
+    create_project(project_name="mnist_tutorial", branch="mnist_tutorial")
 
 
 @app.command()
 def run_dashboard(experiment_folder: str = "."):
     """Run dashboard for a given experiment folder."""
     os.system(f"python -m art.dashboard.app --exp_path {experiment_folder}")
 
@@ -93,9 +93,18 @@
     """Create a project named 'bert_transfer_learning_tutorial' using the 'bert_transfer_learning_tutorial' branch."""
     create_project(
         project_name="bert_transfer_learning_tutorial",
         branch="bert_transfer_learning_tutorial",
     )
 
 
+@app.command()
+def regularization_tutorial():
+    """Creates a regularize tutorial."""
+    create_project(
+        project_name="regularize_tutorial",
+        branch="regularize_tutorial",
+    )
+
+
 if __name__ == "__main__":
     app()
```

### Comparing `art_training-0.2.1/art/cli/utils.py` & `art_training-1.0.0/art/cli/utils.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-import subprocess
-from enum import Enum
-
-
-class ProjectType(Enum):
-    """
-    Enum for project types
-    """
-
-    CLASSIFICATION = 1
-    REGRESSION = 2
-    CLUSTERING = 3
-    TIME_SERIES = 4
-
-
-def get_git_user_info():
-    """
-    Retrieve the git user's username and email.
-
-    Returns:
-        Tuple[str, str]: A tuple containing the git username and email.
-                         Returns (None, None) if retrieval fails.
-
-    Raises:
-        subprocess.CalledProcessError: If the git command fails.
-    """
-    try:
-        username = (
-            subprocess.check_output(["git", "config", "--get", "user.name"])
-            .decode()
-            .strip()
-        )
-        email = (
-            subprocess.check_output(["git", "config", "--get", "user.email"])
-            .decode()
-            .strip()
-        )
-        return username, email
-    except subprocess.CalledProcessError:
-        return None, None
+import subprocess
+from enum import Enum
+
+
+class ProjectType(Enum):
+    """
+    Enum for project types
+    """
+
+    CLASSIFICATION = 1
+    REGRESSION = 2
+    CLUSTERING = 3
+    TIME_SERIES = 4
+
+
+def get_git_user_info():
+    """
+    Retrieve the git user's username and email.
+
+    Returns:
+        Tuple[str, str]: A tuple containing the git username and email.
+                         Returns (None, None) if retrieval fails.
+
+    Raises:
+        subprocess.CalledProcessError: If the git command fails.
+    """
+    try:
+        username = (
+            subprocess.check_output(["git", "config", "--get", "user.name"])
+            .decode()
+            .strip()
+        )
+        email = (
+            subprocess.check_output(["git", "config", "--get", "user.email"])
+            .decode()
+            .strip()
+        )
+        return username, email
+    except subprocess.CalledProcessError:
+        return None, None
```

### Comparing `art_training-0.2.1/art/dashboard/app.py` & `art_training-1.0.0/art/dashboard/app.py`

 * *Files identical despite different names*

### Comparing `art_training-0.2.1/art/dashboard/help.py` & `art_training-1.0.0/art/dashboard/help.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from dash import dcc
-
-HELP = dcc.Markdown(
-    """
-Within this dashboard you can track progress of your Project and visualize/compare results of each step.
-
-On the left you see timeline with all steps that you've defined in your Project. 
-* Next to every step there is a short summary of its results.
-* Green indicates that step is passed and red indicates it failed.
-
-On the right you can see table with all results of selected step.
-* Select step with the dropdown selection. 
-* You can sort and filter results by clicking on column headers. 
-* You can also select single row to make it your `base` run. This will be important for the plot.
-
-Below the table you can see plot with results of selected step.
-* You can select which metrics you want to plot on x and y axis
-* As you hover over the plot you can see logged details of each run
-    * Your base run will be bigger and contain all logged metrics
-    * Other runs will be smaller and contain only metrics that are different from the base run.
-"""
-)
+from dash import dcc
+
+HELP = dcc.Markdown(
+    """
+Within this dashboard you can track progress of your Project and visualize/compare results of each step.
+
+On the left you see timeline with all steps that you've defined in your Project. 
+* Next to every step there is a short summary of its results.
+* Green indicates that step is passed and red indicates it failed.
+
+On the right you can see table with all results of selected step.
+* Select step with the dropdown selection. 
+* You can sort and filter results by clicking on column headers. 
+* You can also select single row to make it your `base` run. This will be important for the plot.
+
+Below the table you can see plot with results of selected step.
+* You can select which metrics you want to plot on x and y axis
+* As you hover over the plot you can see logged details of each run
+    * Your base run will be bigger and contain all logged metrics
+    * Other runs will be smaller and contain only metrics that are different from the base run.
+"""
+)
```

### Comparing `art_training-0.2.1/art/dashboard/timeline.py` & `art_training-1.0.0/art/dashboard/timeline.py`

 * *Files identical despite different names*

### Comparing `art_training-0.2.1/art/dashboard/assets/pallet.jpg` & `art_training-1.0.0/art/dashboard/assets/pallet.jpg`

 * *Files identical despite different names*

### Comparing `art_training-0.2.1/art/utils/paths.py` & `art_training-1.0.0/art/utils/paths.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from pathlib import Path
-
-CHECKPOINTS_PATH = Path("art_checkpoints")
-EXPERIMENT_LOG_DIR = CHECKPOINTS_PATH / "experiment" / "logs"
-
-
-def get_checkpoint_step_dir_path(full_step_name) -> Path:
-    """
-    Get the name of the directory for the given step.
-
-    Args:
-        step_id (str): The ID of the step.
-        step_name (str): The name of the step.
-
-    Returns:
-        str: The name of the directory.
-    """
-    return CHECKPOINTS_PATH / f"{full_step_name}"
-
-
-def get_checkpoint_logs_folder_path(full_step_name) -> Path:
-    return get_checkpoint_step_dir_path(full_step_name) / "logs"
-
-
-#
-EXPERIMENT_LOG_DIR.mkdir(parents=True, exist_ok=True)
+from pathlib import Path
+
+CHECKPOINTS_PATH = Path("art_checkpoints")
+EXPERIMENT_LOG_DIR = CHECKPOINTS_PATH / "experiment" / "logs"
+
+
+def get_checkpoint_step_dir_path(full_step_name) -> Path:
+    """
+    Get the name of the directory for the given step.
+
+    Args:
+        step_id (str): The ID of the step.
+        step_name (str): The name of the step.
+
+    Returns:
+        str: The name of the directory.
+    """
+    return CHECKPOINTS_PATH / f"{full_step_name}"
+
+
+def get_checkpoint_logs_folder_path(full_step_name) -> Path:
+    return get_checkpoint_step_dir_path(full_step_name) / "logs"
+
+
+#
+EXPERIMENT_LOG_DIR.mkdir(parents=True, exist_ok=True)
```

### Comparing `art_training-0.2.1/art/utils/savers.py` & `art_training-1.0.0/art/utils/savers.py`

 * *Files identical despite different names*

### Comparing `art_training-0.2.1/docs/Makefile` & `art_training-1.0.0/docs/Makefile`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Minimal makefile for Sphinx documentation
-#
-
-# You can set these variables from the command line, and also
-# from the environment for the first two.
-SPHINXOPTS    ?=
-SPHINXBUILD   ?= sphinx-build
-SOURCEDIR     = source
-BUILDDIR      = build
-
-# Put it first so that "make" without argument is like "make help".
-help:
-	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
-
-.PHONY: help Makefile
-
-# Catch-all target: route all unknown targets to Sphinx using the new
-# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
-%: Makefile
-	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+# Minimal makefile for Sphinx documentation
+#
+
+# You can set these variables from the command line, and also
+# from the environment for the first two.
+SPHINXOPTS    ?=
+SPHINXBUILD   ?= sphinx-build
+SOURCEDIR     = source
+BUILDDIR      = build
+
+# Put it first so that "make" without argument is like "make help".
+help:
+	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+
+.PHONY: help Makefile
+
+# Catch-all target: route all unknown targets to Sphinx using the new
+# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
+%: Makefile
+	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `art_training-0.2.1/docs/art.png` & `art_training-1.0.0/docs/art.png`

 * *Files identical despite different names*

### Comparing `art_training-0.2.1/docs/make.bat` & `art_training-1.0.0/docs/make.bat`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-@ECHO OFF
-
-pushd %~dp0
-
-REM Command file for Sphinx documentation
-
-if "%SPHINXBUILD%" == "" (
-	set SPHINXBUILD=sphinx-build
-)
-set SOURCEDIR=source
-set BUILDDIR=build
-
-%SPHINXBUILD% >NUL 2>NUL
-if errorlevel 9009 (
-	echo.
-	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
-	echo.installed, then set the SPHINXBUILD environment variable to point
-	echo.to the full path of the 'sphinx-build' executable. Alternatively you
-	echo.may add the Sphinx directory to PATH.
-	echo.
-	echo.If you don't have Sphinx installed, grab it from
-	echo.https://www.sphinx-doc.org/
-	exit /b 1
-)
-
-if "%1" == "" goto help
-
-%SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
-goto end
-
-:help
-%SPHINXBUILD% -M help %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
-
-:end
-popd
+@ECHO OFF
+
+pushd %~dp0
+
+REM Command file for Sphinx documentation
+
+if "%SPHINXBUILD%" == "" (
+	set SPHINXBUILD=sphinx-build
+)
+set SOURCEDIR=source
+set BUILDDIR=build
+
+%SPHINXBUILD% >NUL 2>NUL
+if errorlevel 9009 (
+	echo.
+	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
+	echo.installed, then set the SPHINXBUILD environment variable to point
+	echo.to the full path of the 'sphinx-build' executable. Alternatively you
+	echo.may add the Sphinx directory to PATH.
+	echo.
+	echo.If you don't have Sphinx installed, grab it from
+	echo.https://www.sphinx-doc.org/
+	exit /b 1
+)
+
+if "%1" == "" goto help
+
+%SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
+goto end
+
+:help
+%SPHINXBUILD% -M help %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
+
+:end
+popd
```

### Comparing `art_training-0.2.1/docs/source/conf.py` & `art_training-1.0.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `art_training-0.2.1/docs/source/index.rst` & `art_training-1.0.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `art_training-0.2.1/docs/source/apidocs/art.rst` & `art_training-1.0.0/docs/source/apidocs/art.rst`

 * *Files identical despite different names*

### Comparing `art_training-0.2.1/docs/source/apidocs/art.utils.rst` & `art_training-1.0.0/docs/source/apidocs/art.utils.rst`

 * *Files identical despite different names*

### Comparing `art_training-0.2.1/stubs/lightning/__init__.pyi` & `art_training-1.0.0/stubs/lightning/__init__.pyi`

 * *Files identical despite different names*

### Comparing `art_training-0.2.1/LICENCE` & `art_training-1.0.0/LICENCE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2018 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+Copyright (c) 2018 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `art_training-0.2.1/pyproject.toml` & `art_training-1.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
-requires = ["hatchling"]
+requires = ["hatchling<1.19", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 [project]
 description = "ART - Actually Robust Training framework - a framework that teaches good practices when training deep neural networks. "
 
 
 name = "art-training"
-version = "0.2.1"
+version = "1.0.0"
 authors = [
   { name = "Sebastian Chwilczynski", email = "sebastian.chwilczynski@student.put.poznan.pl" },
   { name = "Kacper Trebacz", email = "kacper.trebacz@student.put.poznan.pl" },
   { name = "Mateusz Malecki", email = "mateusz.malecki.1@student.put.poznan.pl" },
   { name = "Karol Cyganik", email = "karol.cyganik@student.put.poznan.pl" },
 ]
 readme = "README.md"
@@ -27,15 +27,15 @@
   "datasets>=2.11.0",
   "lightning>=1.9",
   "torch>=1.13.1",
   "matplotlib~=3.6",
   "cookiecutter>=2.3.1",
   "typer==0.4.2",
   "loguru==0.7.2",
-  "PyGithub==2.1.1"
+  "PyGithub==2.1.1",
 ]
 
 [project.optional-dependencies]
 dev = [
   "flake8>=6.0.0",
   "tox>=4.4.7",
   "pytest>=7.2.2",
```

