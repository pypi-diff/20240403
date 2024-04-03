# Comparing `tmp/smadi-0.2.6.tar.gz` & `tmp/smadi-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smadi-0.2.6.tar", last modified: Wed Apr  3 02:38:35 2024, max compression
+gzip compressed data, was "smadi-0.2.7.tar", last modified: Wed Apr  3 19:59:57 2024, max compression
```

## Comparing `smadi-0.2.6.tar` & `smadi-0.2.7.tar`

### file list

```diff
@@ -1,54 +1,53 @@
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-03 02:38:35.956905 smadi-0.2.6/
--rw-rw-r--   0 m294      (1000) m294      (1000)      588 2024-03-30 14:53:43.000000 smadi-0.2.6/.coveragerc
--rw-rw-r--   0 m294      (1000) m294      (1000)      566 2024-03-30 14:53:43.000000 smadi-0.2.6/.gitignore
--rw-rw-r--   0 m294      (1000) m294      (1000)      530 2024-03-30 14:53:43.000000 smadi-0.2.6/.readthedocs.yml
--rw-rw-r--   0 m294      (1000) m294      (1000)       85 2024-03-30 14:53:43.000000 smadi-0.2.6/AUTHORS.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)      128 2024-03-30 14:53:43.000000 smadi-0.2.6/CHANGELOG.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)    13788 2024-03-30 14:53:43.000000 smadi-0.2.6/CONTRIBUTING.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)     1079 2024-03-30 14:53:43.000000 smadi-0.2.6/LICENSE.txt
--rw-r--r--   0 m294      (1000) m294      (1000)     3009 2024-04-03 02:38:35.956905 smadi-0.2.6/PKG-INFO
--rw-rw-r--   0 m294      (1000) m294      (1000)     1591 2024-03-30 14:53:43.000000 smadi-0.2.6/README.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)  1710114 2024-04-03 02:37:06.000000 smadi-0.2.6/Tutorial.ipynb
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-03 02:38:35.860905 smadi-0.2.6/docs/
--rw-rw-r--   0 m294      (1000) m294      (1000)     1154 2024-03-30 14:53:43.000000 smadi-0.2.6/docs/Makefile
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-03 02:38:35.860905 smadi-0.2.6/docs/_static/
--rw-rw-r--   0 m294      (1000) m294      (1000)       18 2024-03-30 14:53:43.000000 smadi-0.2.6/docs/_static/.gitignore
--rw-rw-r--   0 m294      (1000) m294      (1000)       41 2024-03-30 14:53:43.000000 smadi-0.2.6/docs/authors.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)       43 2024-03-30 14:53:43.000000 smadi-0.2.6/docs/changelog.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)     9724 2024-03-30 14:53:43.000000 smadi-0.2.6/docs/conf.py
--rw-rw-r--   0 m294      (1000) m294      (1000)       33 2024-03-30 14:53:43.000000 smadi-0.2.6/docs/contributing.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)     2305 2024-03-30 14:53:43.000000 smadi-0.2.6/docs/index.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)       67 2024-03-30 14:53:43.000000 smadi-0.2.6/docs/license.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)       39 2024-03-30 14:53:43.000000 smadi-0.2.6/docs/readme.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)      233 2024-03-30 14:53:43.000000 smadi-0.2.6/docs/requirements.txt
--rw-rw-r--   0 m294      (1000) m294      (1000)      346 2024-03-30 14:53:43.000000 smadi-0.2.6/pyproject.toml
--rw-rw-r--   0 m294      (1000) m294      (1000)      301 2024-04-03 02:37:06.000000 smadi-0.2.6/requirements.txt
--rw-rw-r--   0 m294      (1000) m294      (1000)     1492 2024-04-03 02:38:35.956905 smadi-0.2.6/setup.cfg
--rw-rw-r--   0 m294      (1000) m294      (1000)      836 2024-04-03 02:38:11.000000 smadi-0.2.6/setup.py
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-03 02:38:35.760904 smadi-0.2.6/src/
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-03 02:38:35.864904 smadi-0.2.6/src/smadi/
--rw-rw-r--   0 m294      (1000) m294      (1000)      577 2024-03-30 14:53:43.000000 smadi-0.2.6/src/smadi/__init__.py
--rw-rw-r--   0 m294      (1000) m294      (1000)    19649 2024-04-01 23:41:33.000000 smadi-0.2.6/src/smadi/anomaly_detectors.py
--rw-rw-r--   0 m294      (1000) m294      (1000)    15611 2024-04-03 02:37:06.000000 smadi-0.2.6/src/smadi/climatology.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     3482 2024-04-02 14:59:26.000000 smadi-0.2.6/src/smadi/data_reader.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     8775 2024-03-29 20:29:06.000000 smadi-0.2.6/src/smadi/indicators.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     5213 2024-04-03 02:37:06.000000 smadi-0.2.6/src/smadi/map.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     1813 2024-04-01 23:41:33.000000 smadi-0.2.6/src/smadi/metadata.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     7719 2024-04-03 02:37:06.000000 smadi-0.2.6/src/smadi/plot.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     8623 2024-03-29 20:28:21.000000 smadi-0.2.6/src/smadi/preprocess.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     4522 2024-04-01 23:09:32.000000 smadi-0.2.6/src/smadi/utils.py
--rw-rw-r--   0 m294      (1000) m294      (1000)    14908 2024-04-03 02:37:06.000000 smadi-0.2.6/src/smadi/workflow.py
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-03 02:38:35.952905 smadi-0.2.6/src/smadi.egg-info/
--rw-r--r--   0 m294      (1000) m294      (1000)     3009 2024-04-03 02:38:35.000000 smadi-0.2.6/src/smadi.egg-info/PKG-INFO
--rw-rw-r--   0 m294      (1000) m294      (1000)      930 2024-04-03 02:38:35.000000 smadi-0.2.6/src/smadi.egg-info/SOURCES.txt
--rw-rw-r--   0 m294      (1000) m294      (1000)        1 2024-04-03 02:38:35.000000 smadi-0.2.6/src/smadi.egg-info/dependency_links.txt
--rw-rw-r--   0 m294      (1000) m294      (1000)       44 2024-04-03 02:38:35.000000 smadi-0.2.6/src/smadi.egg-info/entry_points.txt
--rw-rw-r--   0 m294      (1000) m294      (1000)        1 2024-03-30 15:01:49.000000 smadi-0.2.6/src/smadi.egg-info/not-zip-safe
--rw-rw-r--   0 m294      (1000) m294      (1000)      327 2024-04-03 02:38:35.000000 smadi-0.2.6/src/smadi.egg-info/requires.txt
--rw-rw-r--   0 m294      (1000) m294      (1000)        6 2024-04-03 02:38:35.000000 smadi-0.2.6/src/smadi.egg-info/top_level.txt
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-03 02:38:35.952905 smadi-0.2.6/tests/
--rw-rw-r--   0 m294      (1000) m294      (1000)     1117 2024-03-30 15:11:41.000000 smadi-0.2.6/tests/conftest.py
--rw-rw-r--   0 m294      (1000) m294      (1000)   360610 2024-03-25 13:18:42.000000 smadi-0.2.6/tests/data_sample.csv
--rw-rw-r--   0 m294      (1000) m294      (1000)    20031 2024-03-30 14:58:36.000000 smadi-0.2.6/tests/test_climatology.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     2211 2024-03-30 14:58:43.000000 smadi-0.2.6/tests/test_indicators.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     2851 2024-03-30 14:53:43.000000 smadi-0.2.6/tox.ini
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-03 19:59:57.561693 smadi-0.2.7/
+-rw-rw-r--   0 m294      (1000) m294      (1000)      588 2024-03-30 14:53:43.000000 smadi-0.2.7/.coveragerc
+-rw-rw-r--   0 m294      (1000) m294      (1000)      566 2024-03-30 14:53:43.000000 smadi-0.2.7/.gitignore
+-rw-rw-r--   0 m294      (1000) m294      (1000)      530 2024-03-30 14:53:43.000000 smadi-0.2.7/.readthedocs.yml
+-rw-rw-r--   0 m294      (1000) m294      (1000)       85 2024-03-30 14:53:43.000000 smadi-0.2.7/AUTHORS.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)      128 2024-03-30 14:53:43.000000 smadi-0.2.7/CHANGELOG.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)    13788 2024-03-30 14:53:43.000000 smadi-0.2.7/CONTRIBUTING.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)     1079 2024-03-30 14:53:43.000000 smadi-0.2.7/LICENSE.txt
+-rw-r--r--   0 m294      (1000) m294      (1000)     2224 2024-04-03 19:59:57.561693 smadi-0.2.7/PKG-INFO
+-rw-rw-r--   0 m294      (1000) m294      (1000)      806 2024-04-03 19:20:09.000000 smadi-0.2.7/README.rst
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-03 19:59:57.557692 smadi-0.2.7/docs/
+-rw-rw-r--   0 m294      (1000) m294      (1000)     1154 2024-03-30 14:53:43.000000 smadi-0.2.7/docs/Makefile
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-03 19:59:57.557692 smadi-0.2.7/docs/_static/
+-rw-rw-r--   0 m294      (1000) m294      (1000)       18 2024-03-30 14:53:43.000000 smadi-0.2.7/docs/_static/.gitignore
+-rw-rw-r--   0 m294      (1000) m294      (1000)       41 2024-03-30 14:53:43.000000 smadi-0.2.7/docs/authors.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)       43 2024-03-30 14:53:43.000000 smadi-0.2.7/docs/changelog.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)     9748 2024-04-03 19:56:03.000000 smadi-0.2.7/docs/conf.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)       33 2024-03-30 14:53:43.000000 smadi-0.2.7/docs/contributing.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)     2305 2024-03-30 14:53:43.000000 smadi-0.2.7/docs/index.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)       67 2024-03-30 14:53:43.000000 smadi-0.2.7/docs/license.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)       39 2024-03-30 14:53:43.000000 smadi-0.2.7/docs/readme.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)      233 2024-03-30 14:53:43.000000 smadi-0.2.7/docs/requirements.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)      346 2024-03-30 14:53:43.000000 smadi-0.2.7/pyproject.toml
+-rw-rw-r--   0 m294      (1000) m294      (1000)      301 2024-04-03 02:37:06.000000 smadi-0.2.7/requirements.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)     1492 2024-04-03 19:59:57.561693 smadi-0.2.7/setup.cfg
+-rw-rw-r--   0 m294      (1000) m294      (1000)      836 2024-04-03 19:59:48.000000 smadi-0.2.7/setup.py
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-03 19:59:57.549692 smadi-0.2.7/src/
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-03 19:59:57.557692 smadi-0.2.7/src/smadi/
+-rw-rw-r--   0 m294      (1000) m294      (1000)      577 2024-03-30 14:53:43.000000 smadi-0.2.7/src/smadi/__init__.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)    19649 2024-04-01 23:41:33.000000 smadi-0.2.7/src/smadi/anomaly_detectors.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)    15629 2024-04-03 14:11:17.000000 smadi-0.2.7/src/smadi/climatology.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     3482 2024-04-02 14:59:26.000000 smadi-0.2.7/src/smadi/data_reader.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     8740 2024-04-03 14:10:41.000000 smadi-0.2.7/src/smadi/indicators.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     5213 2024-04-03 02:37:06.000000 smadi-0.2.7/src/smadi/map.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     1813 2024-04-01 23:41:33.000000 smadi-0.2.7/src/smadi/metadata.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     7713 2024-04-03 14:17:09.000000 smadi-0.2.7/src/smadi/plot.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     8624 2024-04-03 14:16:38.000000 smadi-0.2.7/src/smadi/preprocess.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     4882 2024-04-03 14:50:02.000000 smadi-0.2.7/src/smadi/utils.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)    16724 2024-04-03 19:54:00.000000 smadi-0.2.7/src/smadi/workflow.py
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-03 19:59:57.561693 smadi-0.2.7/src/smadi.egg-info/
+-rw-r--r--   0 m294      (1000) m294      (1000)     2224 2024-04-03 19:59:57.000000 smadi-0.2.7/src/smadi.egg-info/PKG-INFO
+-rw-rw-r--   0 m294      (1000) m294      (1000)      915 2024-04-03 19:59:57.000000 smadi-0.2.7/src/smadi.egg-info/SOURCES.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)        1 2024-04-03 19:59:57.000000 smadi-0.2.7/src/smadi.egg-info/dependency_links.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)       44 2024-04-03 19:59:57.000000 smadi-0.2.7/src/smadi.egg-info/entry_points.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)        1 2024-04-03 19:59:57.000000 smadi-0.2.7/src/smadi.egg-info/not-zip-safe
+-rw-rw-r--   0 m294      (1000) m294      (1000)      327 2024-04-03 19:59:57.000000 smadi-0.2.7/src/smadi.egg-info/requires.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)        6 2024-04-03 19:59:57.000000 smadi-0.2.7/src/smadi.egg-info/top_level.txt
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-03 19:59:57.561693 smadi-0.2.7/tests/
+-rw-rw-r--   0 m294      (1000) m294      (1000)     1117 2024-03-30 15:11:41.000000 smadi-0.2.7/tests/conftest.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)   360610 2024-03-25 13:18:42.000000 smadi-0.2.7/tests/data_sample.csv
+-rw-rw-r--   0 m294      (1000) m294      (1000)    20031 2024-03-30 14:58:36.000000 smadi-0.2.7/tests/test_climatology.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     2211 2024-03-30 14:58:43.000000 smadi-0.2.7/tests/test_indicators.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     2851 2024-03-30 14:53:43.000000 smadi-0.2.7/tox.ini
```

### Comparing `smadi-0.2.6/.coveragerc` & `smadi-0.2.7/.coveragerc`

 * *Files identical despite different names*

### Comparing `smadi-0.2.6/.gitignore` & `smadi-0.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `smadi-0.2.6/.readthedocs.yml` & `smadi-0.2.7/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `smadi-0.2.6/CONTRIBUTING.rst` & `smadi-0.2.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `smadi-0.2.6/LICENSE.txt` & `smadi-0.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smadi-0.2.6/README.rst` & `smadi-0.2.7/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,17 @@
 .. These are examples of badges you might want to add to your README:
    please update the URLs accordingly
 
-    .. image:: https://api.cirrus-ci.com/github/<USER>/smadi.svg?branch=main
-        :alt: Built Status
-        :target: https://cirrus-ci.com/github/<USER>/smadi
-    .. image:: https://readthedocs.org/projects/smadi/badge/?version=latest
-        :alt: ReadTheDocs
-        :target: https://smadi.readthedocs.io/en/stable/
-    .. image:: https://img.shields.io/coveralls/github/<USER>/smadi/main.svg
-        :alt: Coveralls
-        :target: https://coveralls.io/r/<USER>/smadi
-    .. image:: https://img.shields.io/pypi/v/smadi.svg
-        :alt: PyPI-Server
-        :target: https://pypi.org/project/smadi/
-    .. image:: https://img.shields.io/conda/vn/conda-forge/smadi.svg
-        :alt: Conda-Forge
-        :target: https://anaconda.org/conda-forge/smadi
-    .. image:: https://pepy.tech/badge/smadi/month
-        :alt: Monthly Downloads
-        :target: https://pepy.tech/project/smadi
-    .. image:: https://img.shields.io/twitter/url/http/shields.io.svg?style=social&label=Twitter
-        :alt: Twitter
-        :target: https://twitter.com/smadi
+.. image:: https://readthedocs.org/projects/smadi/badge/?version=latest
+    :alt: ReadTheDocs
+    :target: https://smadi.readthedocs.io/en/stable/
+
+.. image:: https://img.shields.io/pypi/v/smadi.svg
+    :alt: PyPI-Server
+    :target: https://pypi.org/project/smadi/
 
 .. image:: https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold
     :alt: Project generated with PyScaffold
     :target: https://pyscaffold.org/
 
 |
```

### Comparing `smadi-0.2.6/docs/Makefile` & `smadi-0.2.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `smadi-0.2.6/docs/conf.py` & `smadi-0.2.7/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 # The encoding of source files.
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
-project = "smadi"
+project = "SMADI"
 copyright = "2024, MuhammedM294"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # version: The short X.Y version.
@@ -149,23 +149,21 @@
 todo_emit_warnings = True
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = "alabaster"
+# html_theme = "alabaster"
+html_theme = "sphinx_rtd_theme"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-html_theme_options = {
-    "sidebar_width": "300px",
-    "page_width": "1200px"
-}
+html_theme_options = {"sidebar_width": "300px", "page_width": "1200px"}
 
 # Add any paths that contain custom themes here, relative to this directory.
 # html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
 # html_title = None
```

### Comparing `smadi-0.2.6/docs/index.rst` & `smadi-0.2.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `smadi-0.2.6/setup.cfg` & `smadi-0.2.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `smadi-0.2.6/setup.py` & `smadi-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 from setuptools import setup
 
 if __name__ == "__main__":
     try:
         setup(
-            version="0.2.6",
+            version="0.2.7",
             entry_points={
                 "console_scripts": [
                     "run = smadi.workflow:main",
                 ]
             },
         )
```

### Comparing `smadi-0.2.6/src/smadi/__init__.py` & `smadi-0.2.7/src/smadi/__init__.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.6/src/smadi/anomaly_detectors.py` & `smadi-0.2.7/src/smadi/anomaly_detectors.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.6/src/smadi/climatology.py` & `smadi-0.2.7/src/smadi/climatology.py`

 * *Files 2% similar despite different names*

```diff
@@ -380,15 +380,15 @@
 
 
 class Climatology(Aggregator):
     """
     A class for calculating climatology(climate normal) for time series data.
 
     Attributes:
-    ----------
+    -----------
     df_original: pd.DataFrame
         The original input DataFrame before resampling and removing NaN values.
 
     df: pd.DataFrame
         The input DataFrame containing the preprocessed data to be aggregated.
 
     variable: str
@@ -415,15 +415,15 @@
     normal_metrics: List[str]
         The metrics to be used in the climatology computation. Supported values: 'mean', 'median', 'min', 'max', etc.
 
     clima_df: pd.DataFrame
         The DataFrame containing climatology information.
 
     Methods:
-    -------
+    --------
     aggregate:
         Aggregates the data based on the time step and metrics provided.
 
     _validate_time_step:
         Validates the time step.
 
     _validate_metrics:
@@ -481,14 +481,15 @@
             )
 
     def _validate_metrics(self):
         """
         Validates the metrics to be used in the climatology computation.
 
         Raises:
+        -------
             ValueError: If the metric is not one of the supported values.
 
         """
         for metric in self.normal_metrics:
             if metric not in self.valid_metrics:
                 raise ValueError(
                     f"Invalid metric '{metric}'. Supported values: {self.valid_metrics}."
```

### Comparing `smadi-0.2.6/src/smadi/data_reader.py` & `smadi-0.2.7/src/smadi/data_reader.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.6/src/smadi/indicators.py` & `smadi-0.2.7/src/smadi/indicators.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 
 
 def zscore(obs, mean=None, std=None):
     """
     Computes the standardized z-score of the time series data.
 
     Parameters:
-    ----------
+    -----------
     obs: pd.Series or np.ndarray or sequence-like object
-        The time series data.
+        The observed time series data.
 
     mean: float, pd.Series or np.ndarray or sequence-like object, optional
         The mean of the distribution of the time series data. If None, it will be computed from `obs`.
 
     std:  float, pd.Series or np.ndarray or sequence-like object, optional
         The standard deviation of the distribution of the time series data. If None, it will be computed from `obs`.
 
     Returns:
-    -------
+    --------
     pd.Series or np.ndarray
         The z-score of the time series data.
     """
     # Convert to numpy array if not already a numpy array or a pandas Series
     obs = np.asarray(obs)
     mean = np.asarray(mean) if mean is not None else np.mean(obs)
     std = np.asarray(std) if std is not None else np.std(obs)
@@ -32,15 +32,15 @@
 
 
 def smapi(obs, ref=None, metric="mean"):
     """
     Computes anomalies in time series data based on the Soil Moisture Anomaly Percent Index(SMAPI) method.
 
     parameters:
-    ----------
+    -----------
 
     obs: pd.Series or np.ndarray or sequence-like object
         The observed time series data.
 
     ref: float, pd.Series or np.ndarray or sequence-like object, optional
         The long-term mean (μ​) or median (η) of the variable(the climate normal)
 
@@ -59,15 +59,15 @@
 
 
 def smd(obs, median=None, minimum=None, maximum=None):
     """
     Computes the Soil Moisture Deficit (SD) based on observed value and long-term median, minimum, and maximum values.
 
     parameters:
-    ----------
+    -----------
 
     obs: pd.Series or np.ndarray or sequence-like object
         The observed time series data.
 
     median: float, pd.Series or np.ndarray or sequence-like object, optional
         The long-term median of the variable. if None, it will be computed from `obs`.
 
@@ -110,15 +110,15 @@
 
 
 def smad(obs, median=None, iqr=None):
     """
     Computes the anomalies in time series data based on the Standardized Median Absolute Deviation(SMAD) method.
 
     parameters:
-    ----------
+    -----------
 
     obs: pd.Series or np.ndarray or sequence-like object
         The observed time series data.
 
     median: float, pd.Series or np.ndarray or sequence-like object, optional
         The long-term median of the variable. if None, it will be computed from `obs`.
 
@@ -143,15 +143,15 @@
 
 
 def smca(obs, metric="mean", ref=None, minimum=None, maximum=None):
     """
     Computes the anomalies in time series data based on the Soil Moisture Content Anomaly(SMCA) method.
 
     parameters:
-    ----------
+    -----------
 
     obs: pd.Series or np.ndarray or sequence-like object
         The observed time series data.
 
     metric: str, optional
         The metric to be used for computing the anomalies. Supported values: 'mean', 'median'
 
@@ -183,15 +183,15 @@
 
 
 def smci(obs, minimum=None, maximum=None):
     """
     Computes the anomalies in time series data based on the Soil Moisture Condition Index(SMCI) method.
 
     parameters:
-    ----------
+    -----------
 
     obs: pd.Series or np.ndarray or sequence-like object
         The observed time series data.
 
     minimum: float, pd.Series or np.ndarray or sequence-like object
         The long-term minimum of the variable. if None, it will be computed from `obs`.
 
@@ -214,15 +214,15 @@
 def smds(obs):
     """
     Computes anomalies in time series data based on the Soil Moisture Drought Severity(SMDS) method.
     SMDS = 1 - SMP
     SMP = (rank(x) / (n+1))
 
     parameters:
-    ----------
+    -----------
 
     obs: pd.Series or np.ndarray or sequence-like object
         The observed time series data.
 
     Returns:
     --------
     numpy.ndarray
@@ -235,17 +235,17 @@
 
 
 def essmi(obs):
     """
     Compute the anomalies in time series data based on the Empirical Standardized Soil Moisture Index(ESSMI) method.
 
     parameters:
-    ----------
+    -----------
 
-    obs: pd.Series or np.ndarray or sequence-like object
+    obs: sequence-like object
         The observed time series data.
 
     returns:
     --------
 
     numpy.ndarray
         The Empirical Standardized Soil Moisture Index computed based on the given observed value(s).
@@ -259,17 +259,17 @@
 
 
 def para_dis(obs, dist="beta"):
     """
     Compute the anomalies in time series data based on fitting the observed data to a parametric distribution.
 
     parameters:
-    ----------
+    -----------
 
-    obs: pd.Series or np.ndarray or sequence-like object
+    obs: sequence-like object
         The observed time series data.
 
     dist: str, optional
         The distribution to fit the observed data to. Supported values: 'beta', 'gamma'
     """
 
     obs = np.asarray(obs)
```

### Comparing `smadi-0.2.6/src/smadi/map.py` & `smadi-0.2.7/src/smadi/map.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.6/src/smadi/metadata.py` & `smadi-0.2.7/src/smadi/metadata.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.6/src/smadi/plot.py` & `smadi-0.2.7/src/smadi/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def get_plot_options(**kwargs):
     """
     Set the basic plot options based on the provided kwargs for the plot.
 
     parameters:
     -----------
 
-    **kwargs: dict
+    kwargs: dict
         The keyword arguments for the matplotlib plot.
 
     returns:
     --------
 
     plot_options: dict
         The plot options for the figure.
@@ -208,15 +208,15 @@
 
     plot_hbars: bool
         Whether to plot the horizontal bars on the plot according to the thresholds of the anomaly method used.
 
     plot_categories: bool
         Whether to plot the number of values in each category of the anomaly method that fall within the thresholds.
 
-    **kwargs: dict
+    kwargs: dict
         The keyword arguments for the matplotlib plot for the figure such as title, xlabel, ylabel, legend, figsize, and grid.
 
     """
 
     # Set values for kwargs based on provided values
     plot_params = get_plot_options(**kwargs)
     plt.figure(figsize=plot_params["figsize"])
@@ -264,15 +264,15 @@
 
     raw_var: str
         The name of the raw variable to plot.
 
     raw_kwargs: dict
         The dictionary containing the matplotlib plot options for the raw data.
 
-    **kwargs: dict
+    kwargs: dict
         The keyword arguments for the matplotlib plot for the figure such as title, xlabel, ylabel, legend, figsize, and grid.
 
     """
     # Set values for kwargs based on provided values
     plot_params = get_plot_options(**kwargs)
     if plot_params["figsize"] is not None:
         plt.figure(figsize=plot_params["figsize"])
```

### Comparing `smadi-0.2.6/src/smadi/preprocess.py` & `smadi-0.2.7/src/smadi/preprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,15 +245,15 @@
 
 
 def clim_groupping(df: pd.DataFrame, time_step: str) -> list:
     """
     Groups the DataFrame based on the provided time step for climatology computation.
 
     parameters:
-    ----------
+    -----------
 
     df: pd.DataFrame
         The DataFrame to be grouped.
 
     returns:
     --------
     list
```

### Comparing `smadi-0.2.6/src/smadi/utils.py` & `smadi-0.2.7/src/smadi/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,33 +10,33 @@
 
 
 def create_logger(name, level=logging.DEBUG):
     """
     Create a logger with the given name and level
 
     parameters:
-    ----------
+    -----------
 
     name: str
         name of the logger
     level: logging.LEVEL
         level of the logger
 
     returns:
-    -------
+    --------
     logger: logging.logger
         a logger object
     """
 
     # create logger
     logger = logging.getLogger(name)
     logger.setLevel(level)
 
     # create a file to store all the logs exceptions
-    logfile = logging.FileHandler("run_logger.log")
+    logfile = logging.FileHandler(f"{name}.log")
 
     # create a formatter and set the formatter for the handler
     formatter = logging.Formatter(
         "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
     )
     logfile.setFormatter(formatter)
     logger.addHandler(logfile)
@@ -45,20 +45,20 @@
 
 
 def log_exception(logger):
     """
     A decorator to log exceptions in a function
 
     parameters:
-    ----------
+    -----------
     logger: logging.logger
         a logger object
 
     returns:
-    -------
+    --------
     decorator: function
         a decorator function
 
     """
 
     def decorator(func):
         @wraps(func)
@@ -76,21 +76,21 @@
 
 
 def log_time(logger):
     """
     A decorator to log the time taken by a function
 
     parameters:
-    ----------
+    -----------
 
     logger: logging.logger
         a logger object
 
     returns:
-    -------
+    --------
 
     decorator: function
         a decorator function
 
     """
 
     def decorator(func):
@@ -108,21 +108,21 @@
 
 
 def get_country_code(country_name):
     """
     Get the ISO 3166-1 alpha-3 country code for a given country name.
 
     parameters:
-    ----------
+    -----------
 
     country_name: str
         name of the country
 
     returns:
-    -------
+    --------
 
     country_code: str
         ISO 3166-1 alpha-3 country code
     """
     try:
         # Get ISO alpha-3 code for the provided country name
         country = pycountry.countries.lookup(country_name)
@@ -134,15 +134,15 @@
 
 def load_gpis_by_country(country, res=6.25, format="csv"):
     """
     Load the GPIS based on the country name from the DGG API
     Source: https://dgg.geo.tuwien.ac.at/
 
     parameters:
-    ----------
+    -----------
     country: str
         name of the country
 
     grid: str
         name of the grid to be used. Default is "fibgrid_n6600000". Supported grids are:
         - fibgrid_n6600000 (Fibonacci 6.5 km)
         - fibgrid_n1650000 (Fibonacci 12.5 km)
@@ -179,14 +179,32 @@
             return None
     except Exception as e:
         print(f"An error occurred: {str(e)}")
         return None
 
 
 def get_gpis_from_bbox(bbox, res=6.25):
+    """
+    Get the GPIS based on the bounding box
+
+    parameters:
+    -----------
+
+    bbox: tuple
+        bounding box in the format (lonmin, lonmax, latmin, latmax)
+
+    res: float
+        resolution of the grid. Default is 6.25 km
+
+    returns:
+    --------
+
+    pd.DataFrame
+        a dataframe containing the GPIS, longitude, and latitude
+    """
 
     lonmin, lonmax, latmin, latmax = bbox
     grid = FibLandGrid(res)
     gpis = grid.get_bbox_grid_points(
         lonmin=lonmin, lonmax=lonmax, latmin=latmin, latmax=latmax, both=True
     )
```

### Comparing `smadi-0.2.6/src/smadi/workflow.py` & `smadi-0.2.7/src/smadi/workflow.py`

 * *Files 12% similar despite different names*

```diff
@@ -160,47 +160,55 @@
         default=None,
         help="Save the output to a file to the given path",
     )
 
     return parser
 
 
-parser = setup_argument_parser()
-args: Namespace = parser.parse_args()
+def parse_arguments(parser):
+    """
+    Parse the arguments and return the parsed arguments as a dictionary.
 
-# Required parameters
-data_path = args.data_path
-aoi = args.aoi
-if "," in aoi:
-    aoi = tuple(map(float, aoi.split(",")))
-variable = args.variable
-time_step = args.time_step
-
-# Optional parameters
-data_read_bulk = args.data_read_bulk
-methods = args.methods
-workers = args.workers
-fillna = args.fillna
-fillna_window_size = args.fillna_size
-smoothing = args.smoothing
-smooth_window_size = args.smooth_size
-timespan = args.timespan
-year = args.year
-month = args.month
-dekad = args.dekad
-week = args.week
-bimonth = args.bimonth
-day = args.day
-save_to = args.save_to
+    returns:
+    --------
+    parsed_args: dict
+        The parsed arguments as a dictionary
+    """
+    args: Namespace = parser.parse_args()
+
+    aoi = args.aoi
+    if "," in aoi:
+        aoi = tuple(map(float, aoi.split(",")))
+
+    parsed_args = {
+        "data_path": args.data_path,
+        "aoi": aoi,
+        "variable": args.variable,
+        "time_step": args.time_step,
+        "data_read_bulk": args.data_read_bulk,
+        "methods": args.methods,
+        "workers": args.workers,
+        "fillna": args.fillna,
+        "fillna_size": args.fillna_size,
+        "smoothing": args.smoothing,
+        "smooth_size": args.smooth_size,
+        "timespan": args.timespan,
+        "year": args.year,
+        "month": args.month,
+        "dekad": args.dekad,
+        "week": args.week,
+        "bimonth": args.bimonth,
+        "day": args.day,
+        "save_to": args.save_to,
+    }
+    return parsed_args
 
-# Create an instance of the AscatData class
-ascat_obj = AscatData(data_path, data_read_bulk)
 
 # Create a logger
-logger = create_logger("run_logger")
+logger = create_logger("workflow-logger")
 
 
 @log_exception(logger)
 def load_ts(gpi, variable="sm"):
     """
     Load ASCAT time series for a given gpi
     """
@@ -208,26 +216,65 @@
     valid = ascat_ts["num_sigma"] >= 2
     ascat_ts.loc[~valid, ["sm", "sigma40", "slope40", "curvature40"]] = np.nan
     df = pd.DataFrame(ascat_ts.get(variable))
     return df
 
 
 def _validate_param(param_name: str, param_value: List[int]) -> None:
+    """
+    Validate the date parameters (year, month, dekad, week, bimonth, day) for the anomaly detection workflow.
+
+    Parameters:
+    -----------
+    param_name: str
+        The name of the parameter to validate
+
+    param_value: List[int]
+        The value of the parameter to validate
+
+    Raises:
+    -------
+    ValueError:
+        If the parameter value is None
+        If the parameter value is not a list of integers
+
+    """
 
     if param_value is None:
         raise ValueError(f"The '{param_name}' parameter must be provided")
     if not (isinstance(param_value, (list, int))):
         raise ValueError(f"The '{param_name}' parameter must be an int of list of ints")
 
 
 def _validate_required_params(
     time_step: str,
     required_params: Dict[str, List[str]],
     local_vars: Dict[str, List[int]],
 ) -> None:
+    """
+    Check if the required parameters are provided for the given time_step.
+
+    Parameters:
+    -----------
+
+    time_step: str
+        The time step for the anomaly detection workflow
+
+    required_params: Dict[str, List[str]]
+        A dictionary containing the required parameters for each time step
+
+    local_vars: Dict[str, List[int]]
+        A dictionary containing the local variables
+
+    Raises:
+    -------
+    ValueError:
+        If any of the required parameters are missing
+
+    """
 
     missing_params = [
         param for param in required_params[time_step] if local_vars.get(param) is None
     ]
     if missing_params:
         raise ValueError(
             f"For time_step '{time_step}', the following parameters must be provided: "
@@ -301,15 +348,27 @@
     _validate_required_params(time_step, required_params, local_vars)
 
     return date_param
 
 
 def validate_anomaly_method(methods):
     """
-    Validate the anomaly detection method
+    Validate the names of the anomaly detection methods.
+
+    Parameters:
+    -----------
+
+    methods: List[str]
+        A list of anomaly detection methods names to validate
+
+    Raises:
+    -------
+    ValueError:
+        If any of the methods is not supported
+
     """
 
     for method in methods:
         if method not in _Detectors.keys():
             raise ValueError(
                 f"Anomaly method '{method}' is not supported."
                 f"Supported methods are one of the following: {tuple(_Detectors.keys())}"
@@ -419,26 +478,25 @@
     bimonth: List[int] = None,
     day: List[int] = None,
     workers: int = None,
 ) -> pd.DataFrame:
     """
     Run the anomaly detection workflow for multiple grid point indices with multiprocessing support.
     """
-    # Print workflow start message
-    print("\nWorkflow started....\n")
-    print(f"Loading grid points for {aoi}....")
+    logger.info("\nWorkflow started....\n")
+    logger.info(f"Loading grid points for {aoi}....")
 
     if isinstance(aoi, str):
         pointlist = load_gpis_by_country(aoi)
     else:
         pointlist = get_gpis_from_bbox(aoi)
 
-    print(f"Grid points loaded successfully for {aoi}\n")
-    print(pointlist.head())
-    print("\n")
+    logger.info(f"Grid points loaded successfully for {aoi}\n")
+    logger.info(f"\n\n{pointlist.head()}")
+    pointlist = pointlist[:10]
     pre_compute = partial(
         single_po_run,
         methods=methods,
         variable=variable,
         time_step=time_step,
         fillna=fillna,
         fillna_window_size=fillna_window_size,
@@ -449,82 +507,90 @@
         dekad=dekad,
         week=week,
         bimonth=bimonth,
         day=day,
         timespan=timespan,
     )
 
-    # Print the workflow initiation message
-    print(f"Running the anomaly detection workflow for {aoi}....\n")
+    logger.info(f"Running the anomaly detection workflow for {aoi}....\n")
 
-    # Print workflow parameters
-    print("Workflow parameters:\n")
-    print(f"    Anomaly detection methods: {', '.join(methods)}")
-    print(f"    Variable: {variable}")
-    print(f"    Time step for Climatology: {time_step}")
-    print(f"    Date parameters:\n")
+    logger.info("Workflow parameters:\n")
+    logger.info(f"    Anomaly detection methods: {', '.join(methods)}")
+    logger.info(f"    Variable: {variable}")
+    logger.info(f"    Time step for Climatology: {time_step}")
+    logger.info(f"    Date parameters:\n")
 
-    # Print date parameters if available
     date_parameters = {
         "Year": year,
         "Month": month,
         "Dekad": dekad,
         "Week": week,
         "Bimonth": bimonth,
         "Day": day,
     }
     for param, value in date_parameters.items():
         if value:
-            print(f"     {param}: {value}")
+            logger.info(f"     {param}: {value}")
 
     with ProcessPoolExecutor(workers) as executor:
         results = executor.map(pre_compute, pointlist["point"])
         for result in results:
             pointlist = _finalize(result, pointlist)
 
         return pointlist
 
 
 def main():
 
+    parser = setup_argument_parser()
+    args = parse_arguments(parser)
+
+    # Create an instance of the AscatData class
+    global ascat_obj
+    ascat_obj = AscatData(args["data_path"], args["data_read_bulk"])
+
     try:
-        validate_anomaly_method(methods)
-        validate_date_params(time_step, year, month, dekad, week, bimonth, day)
+        validate_anomaly_method(args["methods"])
+        validate_date_params(
+            args["time_step"],
+            args["year"],
+            args["month"],
+            args["dekad"],
+            args["week"],
+            args["bimonth"],
+            args["day"],
+        )
     except ArgumentError as e:
         parser.error(str(e))
 
-    from time import time
-
-    start = time()
     df = run(
-        aoi=aoi,
-        methods=methods,
-        variable=variable,
-        time_step=time_step,
-        year=year,
-        month=month,
-        week=week,
-        day=day,
-        bimonth=bimonth,
-        dekad=dekad,
-        timespan=timespan,
-        fillna=fillna,
-        fillna_window_size=fillna_window_size,
-        smoothing=smoothing,
-        smooth_window_size=smooth_window_size,
-        workers=workers,
+        aoi=args["aoi"],
+        methods=args["methods"],
+        variable=args["variable"],
+        time_step=args["time_step"],
+        year=args["year"],
+        month=args["month"],
+        week=args["week"],
+        day=args["day"],
+        bimonth=args["bimonth"],
+        dekad=args["dekad"],
+        timespan=args["timespan"],
+        fillna=args["fillna"],
+        fillna_window_size=args["fillna_size"],
+        smoothing=args["smoothing"],
+        smooth_window_size=args["smooth_size"],
+        workers=args["workers"],
     )
 
-    print(f"\nWorkflow completed in {time() - start} seconds\n")
-    print(df)
+    logger.info(f"\n\n {df}")
 
-    if save_to:
+    if args["save_to"]:
         try:
-            df.to_csv(save_to)
-            print(f"Saving the output data frame to {save_to}....")
+            df.to_csv(args["save_to"])
+            print(f"Saving the output data frame to {args['save_to']}....")
             print("Output saved successfully")
 
         except ArgumentError as e:
             parser.error(str(e))
 
 
 if __name__ == "__main__":
```

### Comparing `smadi-0.2.6/src/smadi.egg-info/SOURCES.txt` & `smadi-0.2.7/src/smadi.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 .gitignore
 .readthedocs.yml
 AUTHORS.rst
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE.txt
 README.rst
-Tutorial.ipynb
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
 docs/Makefile
 docs/authors.rst
```

### Comparing `smadi-0.2.6/tests/conftest.py` & `smadi-0.2.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.6/tests/data_sample.csv` & `smadi-0.2.7/tests/data_sample.csv`

 * *Files identical despite different names*

### Comparing `smadi-0.2.6/tests/test_climatology.py` & `smadi-0.2.7/tests/test_climatology.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.6/tests/test_indicators.py` & `smadi-0.2.7/tests/test_indicators.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.6/tox.ini` & `smadi-0.2.7/tox.ini`

 * *Files identical despite different names*

