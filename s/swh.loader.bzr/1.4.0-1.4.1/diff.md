# Comparing `tmp/swh.loader.bzr-1.4.0.tar.gz` & `tmp/swh.loader.bzr-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swh.loader.bzr-1.4.0.tar", last modified: Tue Dec  5 10:37:04 2023, max compression
+gzip compressed data, was "swh.loader.bzr-1.4.1.tar", last modified: Wed Apr  3 12:16:32 2024, max compression
```

## Comparing `swh.loader.bzr-1.4.0.tar` & `swh.loader.bzr-1.4.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-12-05 10:37:04.884551 swh.loader.bzr-1.4.0/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      366 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/.copier-answers.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       83 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)      943 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/AUTHORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)       26 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/LICENSE
--rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2060 2023-12-05 10:37:04.884551 swh.loader.bzr-1.4.0/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)      291 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/README.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      571 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-12-05 10:37:04.880551 swh.loader.bzr-1.4.0/docs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/docs/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/docs/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)      291 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/docs/README.rst
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-12-05 10:37:04.880551 swh.loader.bzr-1.4.0/docs/_static/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-12-05 10:37:04.880551 swh.loader.bzr-1.4.0/docs/_templates/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/docs/conf.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2044 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/docs/how-bzr-works.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      257 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/docs/index.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      414 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/mypy.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1841 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/pyproject.toml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       97 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/pytest.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)       90 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      115 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/requirements-test.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      277 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/requirements.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      120 2023-12-05 10:37:04.884551 swh.loader.bzr-1.4.0/setup.cfg
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-12-05 10:37:04.872551 swh.loader.bzr-1.4.0/swh/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-12-05 10:37:04.872551 swh.loader.bzr-1.4.0/swh/loader/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-12-05 10:37:04.880551 swh.loader.bzr-1.4.0/swh/loader/bzr/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      470 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/swh/loader/bzr/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    25897 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/swh/loader/bzr/loader.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/swh/loader/bzr/py.typed
--rw-r--r--   0 jenkins    (115) jenkins    (120)      768 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/swh/loader/bzr/tasks.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-12-05 10:37:04.884551 swh.loader.bzr-1.4.0/swh/loader/bzr/tests/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/swh/loader/bzr/tests/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1140 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/swh/loader/bzr/tests/conftest.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/swh/loader/bzr/tests/py.typed
--rw-r--r--   0 jenkins    (115) jenkins    (120)    28720 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/swh/loader/bzr/tests/test_loader.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1477 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/swh/loader/bzr/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-12-05 10:37:04.884551 swh.loader.bzr-1.4.0/swh.loader.bzr.egg-info/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2060 2023-12-05 10:37:04.000000 swh.loader.bzr-1.4.0/swh.loader.bzr.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)      919 2023-12-05 10:37:04.000000 swh.loader.bzr-1.4.0/swh.loader.bzr.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2023-12-05 10:37:04.000000 swh.loader.bzr-1.4.0/swh.loader.bzr.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      118 2023-12-05 10:37:04.000000 swh.loader.bzr-1.4.0/swh.loader.bzr.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      314 2023-12-05 10:37:04.000000 swh.loader.bzr-1.4.0/swh.loader.bzr.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2023-12-05 10:37:04.000000 swh.loader.bzr-1.4.0/swh.loader.bzr.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1343 2023-12-05 10:36:58.000000 swh.loader.bzr-1.4.0/tox.ini
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-03 12:16:32.451561 swh.loader.bzr-1.4.1/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      366 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/.copier-answers.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       83 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1385 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/AUTHORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       26 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/LICENSE
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2085 2024-04-03 12:16:32.451561 swh.loader.bzr-1.4.1/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      291 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/README.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      571 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-03 12:16:32.443561 swh.loader.bzr-1.4.1/docs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/docs/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      291 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/docs/README.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-03 12:16:32.443561 swh.loader.bzr-1.4.1/docs/_static/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-03 12:16:32.443561 swh.loader.bzr-1.4.1/docs/_templates/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/docs/conf.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2044 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/docs/how-bzr-works.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      257 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/docs/index.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      414 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/mypy.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1841 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/pyproject.toml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       96 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/pytest.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       90 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      106 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      306 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/requirements.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      120 2024-04-03 12:16:32.451561 swh.loader.bzr-1.4.1/setup.cfg
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-03 12:16:32.435561 swh.loader.bzr-1.4.1/swh/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-03 12:16:32.435561 swh.loader.bzr-1.4.1/swh/loader/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-03 12:16:32.447561 swh.loader.bzr-1.4.1/swh/loader/bzr/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      470 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/swh/loader/bzr/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    25897 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/swh/loader/bzr/loader.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/swh/loader/bzr/py.typed
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      768 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/swh/loader/bzr/tasks.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-03 12:16:32.447561 swh.loader.bzr-1.4.1/swh/loader/bzr/tests/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/swh/loader/bzr/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1140 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/swh/loader/bzr/tests/conftest.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/swh/loader/bzr/tests/py.typed
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    28720 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/swh/loader/bzr/tests/test_loader.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1477 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/swh/loader/bzr/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-03 12:16:32.447561 swh.loader.bzr-1.4.1/swh.loader.bzr.egg-info/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2085 2024-04-03 12:16:32.000000 swh.loader.bzr-1.4.1/swh.loader.bzr.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      919 2024-04-03 12:16:32.000000 swh.loader.bzr-1.4.1/swh.loader.bzr.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-04-03 12:16:32.000000 swh.loader.bzr-1.4.1/swh.loader.bzr.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      118 2024-04-03 12:16:32.000000 swh.loader.bzr-1.4.1/swh.loader.bzr.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      339 2024-04-03 12:16:32.000000 swh.loader.bzr-1.4.1/swh.loader.bzr.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-04-03 12:16:32.000000 swh.loader.bzr-1.4.1/swh.loader.bzr.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1073 2024-04-03 12:16:27.000000 swh.loader.bzr-1.4.1/tox.ini
```

### Comparing `swh.loader.bzr-1.4.0/CODE_OF_CONDUCT.md` & `swh.loader.bzr-1.4.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.loader.bzr-1.4.0/LICENSE` & `swh.loader.bzr-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.loader.bzr-1.4.0/PKG-INFO` & `swh.loader.bzr-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.loader.bzr
-Version: 1.4.0
+Version: 1.4.1
 Summary: Software Heritage Bazaar/Breezy loader
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-loader-bzr
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-loader-bzr/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-loader-bzr/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-loader-bzr.git
@@ -13,30 +13,30 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: breezy>=3.3.1
+Requires-Dist: breezy!=3.3.6,!=3.3.7,>=3.3.1
 Requires-Dist: swh.model>=2.6.1
 Requires-Dist: swh.storage>=0.41.1
 Requires-Dist: swh.scheduler>=0.23.0
 Requires-Dist: swh.loader.core>=5.7.3
 Provides-Extra: testing
-Requires-Dist: breezy>=3.3.1; extra == "testing"
+Requires-Dist: breezy!=3.3.6,!=3.3.7,>=3.3.1; extra == "testing"
 Requires-Dist: swh.model>=2.6.1; extra == "testing"
 Requires-Dist: swh.storage>=0.41.1; extra == "testing"
 Requires-Dist: swh.scheduler>=0.23.0; extra == "testing"
 Requires-Dist: swh.loader.core>=5.7.3; extra == "testing"
 Requires-Dist: dulwich; extra == "testing"
-Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest>=8.1; extra == "testing"
 Requires-Dist: pytest-mock; extra == "testing"
-Requires-Dist: swh.core[http]>=0.0.61; extra == "testing"
-Requires-Dist: swh.scheduler[testing]>=0.5.0; extra == "testing"
+Requires-Dist: swh.core[testing]; extra == "testing"
+Requires-Dist: swh.scheduler[testing]; extra == "testing"
 Requires-Dist: swh.storage[testing]; extra == "testing"
 Requires-Dist: testtools; extra == "testing"
 
 Software Heritage - Bazaar/Breezy loader
 ========================================
 
 Loader for `Bazaar <http://bazaar.canonical.com/en/>`_ and `Breezy
```

### Comparing `swh.loader.bzr-1.4.0/conftest.py` & `swh.loader.bzr-1.4.1/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.loader.bzr-1.4.0/docs/how-bzr-works.rst` & `swh.loader.bzr-1.4.1/docs/how-bzr-works.rst`

 * *Files identical despite different names*

### Comparing `swh.loader.bzr-1.4.0/pyproject.toml` & `swh.loader.bzr-1.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swh.loader.bzr-1.4.0/swh/loader/bzr/loader.py` & `swh.loader.bzr-1.4.1/swh/loader/bzr/loader.py`

 * *Files identical despite different names*

### Comparing `swh.loader.bzr-1.4.0/swh/loader/bzr/tasks.py` & `swh.loader.bzr-1.4.1/swh/loader/bzr/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.loader.bzr-1.4.0/swh/loader/bzr/tests/conftest.py` & `swh.loader.bzr-1.4.1/swh/loader/bzr/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.loader.bzr-1.4.0/swh/loader/bzr/tests/test_loader.py` & `swh.loader.bzr-1.4.1/swh/loader/bzr/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `swh.loader.bzr-1.4.0/swh/loader/bzr/tests/test_tasks.py` & `swh.loader.bzr-1.4.1/swh/loader/bzr/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.loader.bzr-1.4.0/swh.loader.bzr.egg-info/PKG-INFO` & `swh.loader.bzr-1.4.1/swh.loader.bzr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.loader.bzr
-Version: 1.4.0
+Version: 1.4.1
 Summary: Software Heritage Bazaar/Breezy loader
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-loader-bzr
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-loader-bzr/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-loader-bzr/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-loader-bzr.git
@@ -13,30 +13,30 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: breezy>=3.3.1
+Requires-Dist: breezy!=3.3.6,!=3.3.7,>=3.3.1
 Requires-Dist: swh.model>=2.6.1
 Requires-Dist: swh.storage>=0.41.1
 Requires-Dist: swh.scheduler>=0.23.0
 Requires-Dist: swh.loader.core>=5.7.3
 Provides-Extra: testing
-Requires-Dist: breezy>=3.3.1; extra == "testing"
+Requires-Dist: breezy!=3.3.6,!=3.3.7,>=3.3.1; extra == "testing"
 Requires-Dist: swh.model>=2.6.1; extra == "testing"
 Requires-Dist: swh.storage>=0.41.1; extra == "testing"
 Requires-Dist: swh.scheduler>=0.23.0; extra == "testing"
 Requires-Dist: swh.loader.core>=5.7.3; extra == "testing"
 Requires-Dist: dulwich; extra == "testing"
-Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest>=8.1; extra == "testing"
 Requires-Dist: pytest-mock; extra == "testing"
-Requires-Dist: swh.core[http]>=0.0.61; extra == "testing"
-Requires-Dist: swh.scheduler[testing]>=0.5.0; extra == "testing"
+Requires-Dist: swh.core[testing]; extra == "testing"
+Requires-Dist: swh.scheduler[testing]; extra == "testing"
 Requires-Dist: swh.storage[testing]; extra == "testing"
 Requires-Dist: testtools; extra == "testing"
 
 Software Heritage - Bazaar/Breezy loader
 ========================================
 
 Loader for `Bazaar <http://bazaar.canonical.com/en/>`_ and `Breezy
```

### Comparing `swh.loader.bzr-1.4.0/swh.loader.bzr.egg-info/SOURCES.txt` & `swh.loader.bzr-1.4.1/swh.loader.bzr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

