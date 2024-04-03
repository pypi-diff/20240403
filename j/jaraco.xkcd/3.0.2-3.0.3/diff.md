# Comparing `tmp/jaraco.xkcd-3.0.2.tar.gz` & `tmp/jaraco.xkcd-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.xkcd-3.0.2.tar", last modified: Mon Mar 15 01:51:29 2021, max compression
+gzip compressed data, was "jaraco.xkcd-3.0.3.tar", last modified: Wed Apr  3 01:27:40 2024, max compression
```

## Comparing `jaraco.xkcd-3.0.2.tar` & `jaraco.xkcd-3.0.3.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 01:51:29.491369 jaraco.xkcd-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)       50 2021-03-15 01:51:05.000000 jaraco.xkcd-3.0.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      195 2021-03-15 01:51:05.000000 jaraco.xkcd-3.0.2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      136 2021-03-15 01:51:05.000000 jaraco.xkcd-3.0.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 01:51:29.487369 jaraco.xkcd-3.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 01:51:29.491369 jaraco.xkcd-3.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      497 2021-03-15 01:51:05.000000 jaraco.xkcd-3.0.2/.github/workflows/automerge.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1163 2021-03-15 01:51:05.000000 jaraco.xkcd-3.0.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)      175 2021-03-15 01:51:05.000000 jaraco.xkcd-3.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-03-15 01:51:05.000000 jaraco.xkcd-3.0.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      641 2021-03-15 01:51:05.000000 jaraco.xkcd-3.0.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2021-03-15 01:51:05.000000 jaraco.xkcd-3.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1427 2021-03-15 01:51:29.491369 jaraco.xkcd-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      694 2021-03-15 01:51:05.000000 jaraco.xkcd-3.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 01:51:29.491369 jaraco.xkcd-3.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      756 2021-03-15 01:51:05.000000 jaraco.xkcd-3.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-03-15 01:51:05.000000 jaraco.xkcd-3.0.2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      295 2021-03-15 01:51:05.000000 jaraco.xkcd-3.0.2/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 01:51:29.491369 jaraco.xkcd-3.0.2/jaraco/
--rw-r--r--   0 runner    (1001) docker     (121)     3839 2021-03-15 01:51:05.000000 jaraco.xkcd-3.0.2/jaraco/xkcd.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 01:51:29.491369 jaraco.xkcd-3.0.2/jaraco.xkcd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1427 2021-03-15 01:51:29.000000 jaraco.xkcd-3.0.2/jaraco.xkcd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      488 2021-03-15 01:51:29.000000 jaraco.xkcd-3.0.2/jaraco.xkcd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-15 01:51:29.000000 jaraco.xkcd-3.0.2/jaraco.xkcd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      360 2021-03-15 01:51:29.000000 jaraco.xkcd-3.0.2/jaraco.xkcd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-03-15 01:51:29.000000 jaraco.xkcd-3.0.2/jaraco.xkcd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-03-15 01:51:05.000000 jaraco.xkcd-3.0.2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      367 2021-03-15 01:51:05.000000 jaraco.xkcd-3.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      198 2021-03-15 01:51:05.000000 jaraco.xkcd-3.0.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1216 2021-03-15 01:51:29.491369 jaraco.xkcd-3.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-03-15 01:51:05.000000 jaraco.xkcd-3.0.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    10139 2021-03-15 01:51:05.000000 jaraco.xkcd-3.0.2/skeleton.md
--rw-r--r--   0 runner    (1001) docker     (121)      801 2021-03-15 01:51:05.000000 jaraco.xkcd-3.0.2/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (121)      707 2021-03-15 01:51:05.000000 jaraco.xkcd-3.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:27:40.310392 jaraco.xkcd-3.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-03 01:27:25.000000 jaraco.xkcd-3.0.3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-03 01:27:25.000000 jaraco.xkcd-3.0.3/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:27:40.306391 jaraco.xkcd-3.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-03 01:27:25.000000 jaraco.xkcd-3.0.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:27:40.306391 jaraco.xkcd-3.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-03 01:27:25.000000 jaraco.xkcd-3.0.3/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-03 01:27:25.000000 jaraco.xkcd-3.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-03 01:27:25.000000 jaraco.xkcd-3.0.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-03 01:27:25.000000 jaraco.xkcd-3.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-03 01:27:25.000000 jaraco.xkcd-3.0.3/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-03 01:27:40.310392 jaraco.xkcd-3.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-03 01:27:25.000000 jaraco.xkcd-3.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:27:40.306391 jaraco.xkcd-3.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-03 01:27:25.000000 jaraco.xkcd-3.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-03 01:27:25.000000 jaraco.xkcd-3.0.3/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-03 01:27:25.000000 jaraco.xkcd-3.0.3/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:27:40.306391 jaraco.xkcd-3.0.3/jaraco/
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-03 01:27:25.000000 jaraco.xkcd-3.0.3/jaraco/xkcd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:27:40.310392 jaraco.xkcd-3.0.3/jaraco.xkcd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-03 01:27:40.000000 jaraco.xkcd-3.0.3/jaraco.xkcd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-03 01:27:40.000000 jaraco.xkcd-3.0.3/jaraco.xkcd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 01:27:40.000000 jaraco.xkcd-3.0.3/jaraco.xkcd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-03 01:27:40.000000 jaraco.xkcd-3.0.3/jaraco.xkcd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 01:27:40.000000 jaraco.xkcd-3.0.3/jaraco.xkcd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-03 01:27:25.000000 jaraco.xkcd-3.0.3/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-03 01:27:25.000000 jaraco.xkcd-3.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-03 01:27:25.000000 jaraco.xkcd-3.0.3/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-03 01:27:25.000000 jaraco.xkcd-3.0.3/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-03 01:27:40.310392 jaraco.xkcd-3.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-03 01:27:25.000000 jaraco.xkcd-3.0.3/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 01:27:25.000000 jaraco.xkcd-3.0.3/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-03 01:27:25.000000 jaraco.xkcd-3.0.3/tox.ini
```

### Comparing `jaraco.xkcd-3.0.2/LICENSE` & `jaraco.xkcd-3.0.3/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-Copyright Jason R. Coombs
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `jaraco.xkcd-3.0.2/README.rst` & `jaraco.xkcd-3.0.3/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 .. image:: https://img.shields.io/pypi/v/jaraco.xkcd.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/jaraco.xkcd
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.xkcd.svg
-   :target: `PyPI link`_
 
-.. _PyPI link: https://pypi.org/project/jaraco.xkcd
-
-.. image:: https://github.com/jaraco/jaraco.xkcd/workflows/tests/badge.svg
+.. image:: https://github.com/jaraco/jaraco.xkcd/actions/workflows/main.yml/badge.svg
    :target: https://github.com/jaraco/jaraco.xkcd/actions?query=workflow%3A%22tests%22
    :alt: tests
 
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-   :alt: Code style: Black
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
+.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
+..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
-.. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
-..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
+.. image:: https://img.shields.io/badge/skeleton-2024-informational
+   :target: https://blog.jaraco.com/skeleton
```

### Comparing `jaraco.xkcd-3.0.2/docs/conf.py` & `jaraco.xkcd-3.0.3/docs/conf.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,42 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-extensions = ['sphinx.ext.autodoc', 'jaraco.packaging.sphinx', 'rst.linker']
+extensions = [
+    'sphinx.ext.autodoc',
+    'jaraco.packaging.sphinx',
+]
 
 master_doc = "index"
+html_theme = "furo"
 
+# Link dates and other references in the changelog
+extensions += ['rst.linker']
 link_files = {
-    '../CHANGES.rst': dict(
+    '../NEWS.rst': dict(
         using=dict(GH='https://github.com'),
         replace=[
             dict(
                 pattern=r'(Issue #|\B#)(?P<issue>\d+)',
                 url='{package_url}/issues/{issue}',
             ),
             dict(
                 pattern=r'(?m:^((?P<scm_version>v?\d+(\.\d+){1,2}))\n[-=]+\n)',
                 with_scm='{text}\n{rev[timestamp]:%d %b %Y}\n',
             ),
             dict(
                 pattern=r'PEP[- ](?P<pep_number>\d+)',
-                url='https://www.python.org/dev/peps/pep-{pep_number:0>4}/',
+                url='https://peps.python.org/pep-{pep_number:0>4}/',
             ),
         ],
     )
 }
+
+# Be strict about any broken references
+nitpicky = True
+
+# Include Python intersphinx mapping to prevent failures
+# jaraco/skeleton#51
+extensions += ['sphinx.ext.intersphinx']
+intersphinx_mapping = {
+    'python': ('https://docs.python.org/3', None),
+}
+
+# Preserve authored syntax for defaults
+autodoc_preserve_defaults = True
```

### Comparing `jaraco.xkcd-3.0.2/jaraco/xkcd.py` & `jaraco.xkcd-3.0.3/jaraco/xkcd.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-import os
-import random
-import importlib
 import contextlib
 import datetime
-import pathlib
+import importlib
 import itertools
+import os
+import pathlib
+import random
 
-import jaraco.text
-from requests_toolbelt import sessions
 import cachecontrol
 from cachecontrol import heuristics
 from cachecontrol.caches import file_cache
-from jaraco.functools import except_
+from requests_toolbelt import sessions
+
+import jaraco.text
 from jaraco.collections import dict_map
+from jaraco.functools import except_
 
 
 def make_cache(path=None):
     default = pathlib.Path('~/.cache/xkcd').expanduser()
     path = os.environ.get('XKCD_CACHE_DIR', path or default)
     return file_cache.FileCache(path)
 
@@ -106,15 +107,15 @@
 
         >>> print(Comic.search('password strength'))
         xkcd 936:Password Strength \
 (https://imgs.xkcd.com/comics/password_strength.png)
         >>> Comic.search('Horse battery')
         Comic(2241)
         >>> Comic.search('ISO 8601')
-        Comic(1179)
+        Comic(2562)
         >>> Comic.search('2013-02-27').title
         'ISO 8601'
         >>> Comic.search('2020-12-25').title
         'Wrapping Paper'
         """
         matches = (comic for comic in cls.all() if text in comic.full_text)
         return next(matches, None)
```

### Comparing `jaraco.xkcd-3.0.2/setup.cfg` & `jaraco.xkcd-3.0.3/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,47 @@
 [metadata]
-license_files = 
-	LICENSE
 name = jaraco.xkcd
 author = Jason R. Coombs
 author_email = jaraco@jaraco.com
 description = Library for requesting XKCD comics from its API
 long_description = file:README.rst
 url = https://github.com/jaraco/jaraco.xkcd
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
-packages = find_namespace:
 include_package_data = true
-python_requires = >=3.6
+python_requires = >=3.8
 install_requires = 
 	jaraco.text
 	cachecontrol[filecache]
 	requests_toolbelt
 	jaraco.functools >= 3.1
 	jaraco.collections
-setup_requires = setuptools_scm[toml] >= 3.4.1
-
-[options.packages.find]
-exclude = 
-	build*
-	dist*
-	docs*
-	tests*
 
 [options.extras_require]
 testing = 
-	pytest >= 4.6
+	pytest >= 6, != 8.1.1
 	pytest-checkdocs >= 2.4
-	pytest-flake8
-	pytest-black >= 0.3.7; python_implementation != "PyPy" and python_version < "3.10"
 	pytest-cov
-	pytest-mypy; python_implementation != "PyPy" and python_version < "3.10"
-	pytest-enabler >= 1.0.1
+	pytest-mypy
+	pytest-enabler >= 2.2
+	pytest-ruff >= 0.2.1
 	
 	tempora
 docs = 
-	sphinx
-	jaraco.packaging >= 8.2
+	sphinx >= 3.5
+	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
+	furo
+	sphinx-lint
 
 [options.entry_points]
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

