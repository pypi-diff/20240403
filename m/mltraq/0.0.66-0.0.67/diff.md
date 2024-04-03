# Comparing `tmp/mltraq-0.0.66.tar.gz` & `tmp/mltraq-0.0.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mltraq-0.0.66.tar", max compression
+gzip compressed data, was "mltraq-0.0.67.tar", max compression
```

## Comparing `mltraq-0.0.66.tar` & `mltraq-0.0.67.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1558 2023-01-27 08:07:24.086966 mltraq-0.0.66/LICENSE
--rw-r--r--   0        0        0     1862 2023-01-27 08:07:24.087105 mltraq-0.0.66/README.md
--rw-r--r--   0        0        0     1977 2024-01-09 12:13:26.966785 mltraq-0.0.66/pyproject.toml
--rw-r--r--   0        0        0      338 2023-04-03 14:29:49.538194 mltraq-0.0.66/src/mltraq/__init__.py
--rw-r--r--   0        0        0    20717 2024-01-08 15:13:29.160416 mltraq-0.0.66/src/mltraq/experiment.py
--rw-r--r--   0        0        0     2771 2023-01-27 08:07:24.094179 mltraq-0.0.66/src/mltraq/extras/assertions.py
--rw-r--r--   0        0        0     3390 2023-01-27 08:07:24.094262 mltraq-0.0.66/src/mltraq/extras/dask.py
--rw-r--r--   0        0        0     3335 2024-01-09 11:44:08.424180 mltraq-0.0.66/src/mltraq/extras/environment.py
--rw-r--r--   0        0        0      684 2023-01-27 08:07:24.094423 mltraq-0.0.66/src/mltraq/extras/metrics.py
--rw-r--r--   0        0        0      627 2023-01-27 08:07:24.094492 mltraq-0.0.66/src/mltraq/extras/profiling.py
--rw-r--r--   0        0        0      468 2023-01-27 08:07:24.094560 mltraq-0.0.66/src/mltraq/extras/step_code.py
--rw-r--r--   0        0        0      438 2023-04-03 14:29:49.538451 mltraq-0.0.66/src/mltraq/extras/track_params.py
--rw-r--r--   0        0        0     3895 2024-01-08 15:13:29.160682 mltraq-0.0.66/src/mltraq/job.py
--rw-r--r--   0        0        0     2779 2024-01-09 11:02:19.284930 mltraq-0.0.66/src/mltraq/options.py
--rw-r--r--   0        0        0     9792 2024-01-08 15:13:29.161148 mltraq-0.0.66/src/mltraq/run.py
--rw-r--r--   0        0        0     4994 2024-01-08 15:13:29.161348 mltraq-0.0.66/src/mltraq/session.py
--rw-r--r--   0        0        0        0 2023-01-27 08:07:24.094966 mltraq-0.0.66/src/mltraq/storage/__init__.py
--rw-r--r--   0        0        0    10546 2024-01-09 11:44:08.424387 mltraq-0.0.66/src/mltraq/storage/database.py
--rw-r--r--   0        0        0     1164 2024-01-09 11:44:08.424550 mltraq-0.0.66/src/mltraq/storage/models.py
--rw-r--r--   0        0        0    10474 2024-01-08 15:13:29.161947 mltraq-0.0.66/src/mltraq/storage/serialization.py
--rw-r--r--   0        0        0        0 2023-01-27 08:07:24.095322 mltraq-0.0.66/src/mltraq/utils/__init__.py
--rw-r--r--   0        0        0     2089 2023-01-27 08:07:24.095422 mltraq-0.0.66/src/mltraq/utils/dicts.py
--rw-r--r--   0        0        0      632 2024-01-08 15:13:29.162139 mltraq-0.0.66/src/mltraq/utils/enums.py
--rw-r--r--   0        0        0     1107 2023-01-27 08:07:24.095564 mltraq-0.0.66/src/mltraq/utils/frames.py
--rw-r--r--   0        0        0     6469 2024-01-09 11:44:08.424892 mltraq-0.0.66/src/mltraq/utils/log.py
--rw-r--r--   0        0        0      690 2023-04-03 15:50:34.268581 mltraq-0.0.66/src/mltraq/utils/progress.py
--rw-r--r--   0        0        0     1055 2023-01-27 08:07:24.095941 mltraq-0.0.66/src/mltraq/utils/sequence.py
--rw-r--r--   0        0        0     1171 2023-01-27 08:07:24.096020 mltraq-0.0.66/src/mltraq/utils/text.py
--rw-r--r--   0        0        0      505 2023-01-27 08:07:24.096094 mltraq-0.0.66/src/mltraq/utils/uuid.py
--rw-r--r--   0        0        0    87808 2023-04-03 14:29:49.540033 mltraq-0.0.66/src/mltraq/utils/wordlist.py
--rw-r--r--   0        0        0       23 2024-01-09 12:13:26.994189 mltraq-0.0.66/src/mltraq/version.py
--rw-r--r--   0        0        0     3203 1970-01-01 00:00:00.000000 mltraq-0.0.66/setup.py
--rw-r--r--   0        0        0     3239 1970-01-01 00:00:00.000000 mltraq-0.0.66/PKG-INFO
+-rw-r--r--   0        0        0     1558 2023-01-27 08:07:24.086966 mltraq-0.0.67/LICENSE
+-rw-r--r--   0        0        0     1862 2023-01-27 08:07:24.087105 mltraq-0.0.67/README.md
+-rw-r--r--   0        0        0     2063 2024-01-09 11:52:51.555843 mltraq-0.0.67/pyproject.toml
+-rw-r--r--   0        0        0      338 2023-04-03 14:29:49.538194 mltraq-0.0.67/src/mltraq/__init__.py
+-rw-r--r--   0        0        0    20717 2024-01-08 15:13:29.160416 mltraq-0.0.67/src/mltraq/experiment.py
+-rw-r--r--   0        0        0     2771 2023-01-27 08:07:24.094179 mltraq-0.0.67/src/mltraq/extras/assertions.py
+-rw-r--r--   0        0        0     3390 2023-01-27 08:07:24.094262 mltraq-0.0.67/src/mltraq/extras/dask.py
+-rw-r--r--   0        0        0     3335 2024-01-09 11:44:08.424180 mltraq-0.0.67/src/mltraq/extras/environment.py
+-rw-r--r--   0        0        0      684 2023-01-27 08:07:24.094423 mltraq-0.0.67/src/mltraq/extras/metrics.py
+-rw-r--r--   0        0        0      627 2023-01-27 08:07:24.094492 mltraq-0.0.67/src/mltraq/extras/profiling.py
+-rw-r--r--   0        0        0      468 2023-01-27 08:07:24.094560 mltraq-0.0.67/src/mltraq/extras/step_code.py
+-rw-r--r--   0        0        0      438 2023-04-03 14:29:49.538451 mltraq-0.0.67/src/mltraq/extras/track_params.py
+-rw-r--r--   0        0        0     3895 2024-01-08 15:13:29.160682 mltraq-0.0.67/src/mltraq/job.py
+-rw-r--r--   0        0        0     2779 2024-01-09 11:02:19.284930 mltraq-0.0.67/src/mltraq/options.py
+-rw-r--r--   0        0        0     9792 2024-01-08 15:13:29.161148 mltraq-0.0.67/src/mltraq/run.py
+-rw-r--r--   0        0        0     4994 2024-01-08 15:13:29.161348 mltraq-0.0.67/src/mltraq/session.py
+-rw-r--r--   0        0        0        0 2023-01-27 08:07:24.094966 mltraq-0.0.67/src/mltraq/storage/__init__.py
+-rw-r--r--   0        0        0    10546 2024-01-09 11:44:08.424387 mltraq-0.0.67/src/mltraq/storage/database.py
+-rw-r--r--   0        0        0     1164 2024-01-09 11:44:08.424550 mltraq-0.0.67/src/mltraq/storage/models.py
+-rw-r--r--   0        0        0    10474 2024-01-08 15:13:29.161947 mltraq-0.0.67/src/mltraq/storage/serialization.py
+-rw-r--r--   0        0        0        0 2023-01-27 08:07:24.095322 mltraq-0.0.67/src/mltraq/utils/__init__.py
+-rw-r--r--   0        0        0     2089 2023-01-27 08:07:24.095422 mltraq-0.0.67/src/mltraq/utils/dicts.py
+-rw-r--r--   0        0        0      632 2024-01-08 15:13:29.162139 mltraq-0.0.67/src/mltraq/utils/enums.py
+-rw-r--r--   0        0        0     1107 2023-01-27 08:07:24.095564 mltraq-0.0.67/src/mltraq/utils/frames.py
+-rw-r--r--   0        0        0     6469 2024-01-09 11:44:08.424892 mltraq-0.0.67/src/mltraq/utils/log.py
+-rw-r--r--   0        0        0      690 2023-04-03 15:50:34.268581 mltraq-0.0.67/src/mltraq/utils/progress.py
+-rw-r--r--   0        0        0     1055 2023-01-27 08:07:24.095941 mltraq-0.0.67/src/mltraq/utils/sequence.py
+-rw-r--r--   0        0        0     1171 2023-01-27 08:07:24.096020 mltraq-0.0.67/src/mltraq/utils/text.py
+-rw-r--r--   0        0        0      505 2023-01-27 08:07:24.096094 mltraq-0.0.67/src/mltraq/utils/uuid.py
+-rw-r--r--   0        0        0    87808 2023-04-03 14:29:49.540033 mltraq-0.0.67/src/mltraq/utils/wordlist.py
+-rw-r--r--   0        0        0       23 2024-01-09 11:52:51.579314 mltraq-0.0.67/src/mltraq/version.py
+-rw-r--r--   0        0        0     3151 1970-01-01 00:00:00.000000 mltraq-0.0.67/setup.py
+-rw-r--r--   0        0        0     3306 1970-01-01 00:00:00.000000 mltraq-0.0.67/PKG-INFO
```

### Comparing `mltraq-0.0.66/LICENSE` & `mltraq-0.0.67/LICENSE`

 * *Files identical despite different names*

### Comparing `mltraq-0.0.66/README.md` & `mltraq-0.0.67/README.md`

 * *Files identical despite different names*

### Comparing `mltraq-0.0.66/pyproject.toml` & `mltraq-0.0.67/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mltraq"
-version = "0.0.66"
+version = "0.0.67"
 description = "Open source experiment tracking API with ML performance analysis."
 authors = ["Michele Dallachiesa <michele.dallachiesa@sigforge.com>"]
 license = "BSD-3"
 readme = "README.md"
 homepage = "https://mltraq.com/"
 repository = "https://github.com/elehcimd/mltraq"
 classifiers = [
@@ -23,26 +23,27 @@
 sqlalchemy = ">=2.0.0" 
 sqlalchemy-utils = ">=0.38.3"
 ulid-py = "^1.1.0"
 cloudpickle = ">=2.2.0"
 colorama = ">=0.4.6"
 tqdm = ">=4.64.1"
 tabulate = {version="^0.9.0", optional=true}
+jupyterlab = {version="^4.0.10", optional=true}
+ipywidgets = {version="^8.0.2", optional=true}
 scikit-learn = {version="^1.1.3", optional=true}
-dask = {version = "^2022.11.0", extras=["complete"], optional=true}
-psycopg = {version = "^3.1.17", extras = ["binary"], optional=true}
+dask = {version = "^2022.11.0", optional=true, extras = ["complete"]}
+psycopg = {extras = ["binary"], version = "^3.1.17", optional=true}
 
 [tool.poetry.extras]
-pgsql = ["psycopg"]
+pgsql = ["psycopg2-binary"]
 dask = ["dask"]
-complete = ["tabulate", "scikit-learn", "dask", "psycopg"]
+complete = ["tabulate", "ipywidgets", "scikit-learn", "dask"]
 
 [tool.poetry.group.dev.dependencies]
-jupyterlab = "^4.0.10"
-ipywidgets = "^8.0.2"
+jupyterlab = ">=3.5.0"
 flake8 = ">=5.0.4"
 pytest = ">=7.2.0"
 black = {extras = ["jupyter"], version = ">=22.10.0"}
 ruff = ">=0.0.128"
 pytest-cov = ">=4.0.0"
 pylint = ">=2.15.9"
 pytest-xdist = ">=3.1.0"
```

### Comparing `mltraq-0.0.66/src/mltraq/experiment.py` & `mltraq-0.0.67/src/mltraq/experiment.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.0.66/src/mltraq/extras/assertions.py` & `mltraq-0.0.67/src/mltraq/extras/assertions.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.0.66/src/mltraq/extras/dask.py` & `mltraq-0.0.67/src/mltraq/extras/dask.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.0.66/src/mltraq/extras/environment.py` & `mltraq-0.0.67/src/mltraq/extras/environment.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.0.66/src/mltraq/extras/metrics.py` & `mltraq-0.0.67/src/mltraq/extras/metrics.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.0.66/src/mltraq/extras/profiling.py` & `mltraq-0.0.67/src/mltraq/extras/profiling.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.0.66/src/mltraq/job.py` & `mltraq-0.0.67/src/mltraq/job.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.0.66/src/mltraq/options.py` & `mltraq-0.0.67/src/mltraq/options.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.0.66/src/mltraq/run.py` & `mltraq-0.0.67/src/mltraq/run.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.0.66/src/mltraq/session.py` & `mltraq-0.0.67/src/mltraq/session.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.0.66/src/mltraq/storage/database.py` & `mltraq-0.0.67/src/mltraq/storage/database.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.0.66/src/mltraq/storage/models.py` & `mltraq-0.0.67/src/mltraq/storage/models.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.0.66/src/mltraq/storage/serialization.py` & `mltraq-0.0.67/src/mltraq/storage/serialization.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.0.66/src/mltraq/utils/dicts.py` & `mltraq-0.0.67/src/mltraq/utils/dicts.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.0.66/src/mltraq/utils/enums.py` & `mltraq-0.0.67/src/mltraq/utils/enums.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.0.66/src/mltraq/utils/frames.py` & `mltraq-0.0.67/src/mltraq/utils/frames.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.0.66/src/mltraq/utils/log.py` & `mltraq-0.0.67/src/mltraq/utils/log.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.0.66/src/mltraq/utils/progress.py` & `mltraq-0.0.67/src/mltraq/utils/progress.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.0.66/src/mltraq/utils/sequence.py` & `mltraq-0.0.67/src/mltraq/utils/sequence.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.0.66/src/mltraq/utils/text.py` & `mltraq-0.0.67/src/mltraq/utils/text.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.0.66/src/mltraq/utils/wordlist.py` & `mltraq-0.0.67/src/mltraq/utils/wordlist.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.0.66/setup.py` & `mltraq-0.0.67/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,23 +18,22 @@
  'sqlalchemy-utils>=0.38.3',
  'sqlalchemy>=2.0.0',
  'tqdm>=4.64.1',
  'ulid-py>=1.1.0,<2.0.0']
 
 extras_require = \
 {'complete': ['tabulate>=0.9.0,<0.10.0',
+              'ipywidgets>=8.0.2,<9.0.0',
               'scikit-learn>=1.1.3,<2.0.0',
-              'dask[complete]>=2022.11.0,<2023.0.0',
-              'psycopg[binary]>=3.1.17,<4.0.0'],
- 'dask': ['dask[complete]>=2022.11.0,<2023.0.0'],
- 'pgsql': ['psycopg[binary]>=3.1.17,<4.0.0']}
+              'dask[complete]>=2022.11.0,<2023.0.0'],
+ 'dask': ['dask[complete]>=2022.11.0,<2023.0.0']}
 
 setup_kwargs = {
     'name': 'mltraq',
-    'version': '0.0.66',
+    'version': '0.0.67',
     'description': 'Open source experiment tracking API with ML performance analysis.',
     'long_description': '<p align="center">\n<img width="33%" height="33%" src="https://mltraq.com/assets/img/logo-black.svg" alt="MLTRAQ Logo">\n</p>\n\n<p align="center">\n<img src="https://www.mltraq.com/assets/img/badges/test.svg" alt="Test">\n<img src="https://www.mltraq.com/assets/img/badges/coverage.svg" alt="Coverage">\n<img src="https://www.mltraq.com/assets/img/badges/python.svg" alt="Python">\n<img src="https://www.mltraq.com/assets/img/badges/pypi.svg" alt="PyPi">\n<img src="https://www.mltraq.com/assets/img/badges/license.svg" alt="License">\n<img src="https://www.mltraq.com/assets/img/badges/code-style.svg" alt="Code style">\n</p>\n\n---\n\nOpen source **experiment tracking API** with **ML performance analysis** to build better models faster, facilitating collaboration and transparency within the team and with stakeholders.\n\n---\n\n* **Documentation**: [https://www.mltraq.com](https://www.mltraq.com)\n* **Source code**: [https://github.com/elehcimd/mltraq](https://github.com/elehcimd/mltraq)\n\n---\n\n## Key features\n\n* **Fast and efficient**: start tracking experiments with a few lines of code.\n* **Distributed**: work on experiments independently and upstream them for sharing.\n* **Accessible**: Storage on SQL tables accessible with SQL, Pandas and Python API.\n* **Structured types**: track Numpy arrays, Pandas dataframes, and series.\n* **Parallel execution**: define and execute experiment pipelines with parameter grids.\n* **Light checkpointing**: save time by reloading and continuing your experiments anywhere.\n* **Steps library**: enjoy pre-built steps for tracking, testing, analysis and reporting.\n\n## Requirements\n\n* **Python >=3.8**\n* **SQLAlchemy**, **Pandas**, and **Joblib** (installed as dependencies)\n\n## Installation\n\n```\npip install mltraq\n```\n\n## License\n\nThis project is licensed under the terms of the [BSD 3-Clause License](https://mltraq.com/license).\n\n',
     'author': 'Michele Dallachiesa',
     'author_email': 'michele.dallachiesa@sigforge.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://mltraq.com/',
```

### Comparing `mltraq-0.0.66/PKG-INFO` & `mltraq-0.0.67/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mltraq
-Version: 0.0.66
+Version: 0.0.67
 Summary: Open source experiment tracking API with ML performance analysis.
 Home-page: https://mltraq.com/
 License: BSD-3
 Author: Michele Dallachiesa
 Author-email: michele.dallachiesa@sigforge.com
 Requires-Python: >=3.10.0
 Classifier: Development Status :: 3 - Alpha
@@ -16,17 +16,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: complete
 Provides-Extra: dask
 Provides-Extra: pgsql
 Requires-Dist: cloudpickle (>=2.2.0)
 Requires-Dist: colorama (>=0.4.6)
 Requires-Dist: dask[complete] (>=2022.11.0,<2023.0.0); extra == "dask" or extra == "complete"
+Requires-Dist: ipywidgets (>=8.0.2,<9.0.0); extra == "complete"
 Requires-Dist: joblib (>=1.1.1)
+Requires-Dist: jupyterlab (>=4.0.10,<5.0.0)
 Requires-Dist: pandas (>=1.4.4,<2.0.0)
-Requires-Dist: psycopg[binary] (>=3.1.17,<4.0.0); extra == "pgsql" or extra == "complete"
+Requires-Dist: psycopg[binary] (>=3.1.17,<4.0.0)
 Requires-Dist: scikit-learn (>=1.1.3,<2.0.0); extra == "complete"
 Requires-Dist: sqlalchemy (>=2.0.0)
 Requires-Dist: sqlalchemy-utils (>=0.38.3)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0); extra == "complete"
 Requires-Dist: tqdm (>=4.64.1)
 Requires-Dist: ulid-py (>=1.1.0,<2.0.0)
 Project-URL: Repository, https://github.com/elehcimd/mltraq
```

