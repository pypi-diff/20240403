# Comparing `tmp/graylint-1.0.1.tar.gz` & `tmp/graylint-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graylint-1.0.1.tar", last modified: Fri Mar 15 15:20:12 2024, max compression
+gzip compressed data, was "graylint-1.1.0.tar", last modified: Wed Apr  3 16:35:39 2024, max compression
```

## Comparing `graylint-1.0.1.tar` & `graylint-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-03-15 15:20:12.761862 graylint-1.0.1/
--rw-r--r--   0 akaihola  (1000) users      (100)     1556 2024-03-13 20:11:01.000000 graylint-1.0.1/LICENSE.rst
--rw-r--r--   0 akaihola  (1000) users      (100)    23158 2024-03-15 15:20:12.761862 graylint-1.0.1/PKG-INFO
--rw-r--r--   0 akaihola  (1000) users      (100)    67690 2024-03-15 15:20:04.000000 graylint-1.0.1/README.rst
--rw-r--r--   0 akaihola  (1000) users      (100)     1713 2024-03-13 20:11:01.000000 graylint-1.0.1/pyproject.toml
--rw-r--r--   0 akaihola  (1000) users      (100)     2147 2024-03-15 15:20:12.761862 graylint-1.0.1/setup.cfg
--rw-r--r--   0 akaihola  (1000) users      (100)     1794 2024-03-13 20:11:01.000000 graylint-1.0.1/setup.py
-drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-03-15 15:20:12.757862 graylint-1.0.1/src/
-drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-03-15 15:20:12.758862 graylint-1.0.1/src/graylint/
--rw-r--r--   0 akaihola  (1000) users      (100)      101 2024-03-10 19:25:37.000000 graylint-1.0.1/src/graylint/__init__.py
--rw-r--r--   0 akaihola  (1000) users      (100)     1882 2024-03-13 20:11:01.000000 graylint-1.0.1/src/graylint/__main__.py
--rw-r--r--   0 akaihola  (1000) users      (100)     1475 2024-03-13 20:11:01.000000 graylint-1.0.1/src/graylint/command_line.py
--rw-r--r--   0 akaihola  (1000) users      (100)      251 2024-03-13 20:11:01.000000 graylint-1.0.1/src/graylint/config.py
--rw-r--r--   0 akaihola  (1000) users      (100)      610 2024-03-13 20:11:01.000000 graylint-1.0.1/src/graylint/help.py
--rw-r--r--   0 akaihola  (1000) users      (100)    21828 2024-03-13 20:11:01.000000 graylint-1.0.1/src/graylint/linting.py
--rw-r--r--   0 akaihola  (1000) users      (100)        0 2024-03-10 20:17:25.000000 graylint-1.0.1/src/graylint/py.typed
-drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-03-15 15:20:12.758862 graylint-1.0.1/src/graylint/tests/
--rw-r--r--   0 akaihola  (1000) users      (100)    20968 2024-03-13 20:11:01.000000 graylint-1.0.1/src/graylint/tests/test_linting.py
--rw-r--r--   0 akaihola  (1000) users      (100)       86 2024-03-15 15:20:04.000000 graylint-1.0.1/src/graylint/version.py
-drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-03-15 15:20:12.759862 graylint-1.0.1/src/graylint.egg-info/
--rw-r--r--   0 akaihola  (1000) users      (100)    23158 2024-03-15 15:20:12.000000 graylint-1.0.1/src/graylint.egg-info/PKG-INFO
--rw-r--r--   0 akaihola  (1000) users      (100)      502 2024-03-15 15:20:12.000000 graylint-1.0.1/src/graylint.egg-info/SOURCES.txt
--rw-r--r--   0 akaihola  (1000) users      (100)        1 2024-03-15 15:20:12.000000 graylint-1.0.1/src/graylint.egg-info/dependency_links.txt
--rw-r--r--   0 akaihola  (1000) users      (100)       72 2024-03-15 15:20:12.000000 graylint-1.0.1/src/graylint.egg-info/entry_points.txt
--rw-r--r--   0 akaihola  (1000) users      (100)      476 2024-03-15 15:20:12.000000 graylint-1.0.1/src/graylint.egg-info/requires.txt
--rw-r--r--   0 akaihola  (1000) users      (100)        9 2024-03-15 15:20:12.000000 graylint-1.0.1/src/graylint.egg-info/top_level.txt
+drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-04-03 16:35:39.445582 graylint-1.1.0/
+-rw-r--r--   0 akaihola  (1000) users      (100)     1556 2024-03-16 14:19:35.000000 graylint-1.1.0/LICENSE.rst
+-rw-r--r--   0 akaihola  (1000) users      (100)    22955 2024-04-03 16:35:39.445582 graylint-1.1.0/PKG-INFO
+-rw-r--r--   0 akaihola  (1000) users      (100)    67637 2024-04-03 16:35:20.000000 graylint-1.1.0/README.rst
+-rw-r--r--   0 akaihola  (1000) users      (100)     1900 2024-04-02 19:44:28.000000 graylint-1.1.0/pyproject.toml
+-rw-r--r--   0 akaihola  (1000) users      (100)     2122 2024-04-03 16:35:39.446582 graylint-1.1.0/setup.cfg
+-rw-r--r--   0 akaihola  (1000) users      (100)     1794 2024-03-16 14:19:35.000000 graylint-1.1.0/setup.py
+drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-04-03 16:35:39.440583 graylint-1.1.0/src/
+drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-04-03 16:35:39.441583 graylint-1.1.0/src/graylint/
+-rw-r--r--   0 akaihola  (1000) users      (100)      101 2024-03-16 14:19:35.000000 graylint-1.1.0/src/graylint/__init__.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     1942 2024-04-02 19:44:28.000000 graylint-1.1.0/src/graylint/__main__.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     1475 2024-03-16 14:19:35.000000 graylint-1.1.0/src/graylint/command_line.py
+-rw-r--r--   0 akaihola  (1000) users      (100)      251 2024-03-16 14:19:35.000000 graylint-1.1.0/src/graylint/config.py
+-rw-r--r--   0 akaihola  (1000) users      (100)      610 2024-03-16 14:19:35.000000 graylint-1.1.0/src/graylint/help.py
+-rw-r--r--   0 akaihola  (1000) users      (100)    21828 2024-03-16 14:19:35.000000 graylint-1.1.0/src/graylint/linting.py
+-rw-r--r--   0 akaihola  (1000) users      (100)        0 2024-03-16 14:19:35.000000 graylint-1.1.0/src/graylint/py.typed
+drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-04-03 16:35:39.442582 graylint-1.1.0/src/graylint/tests/
+-rw-r--r--   0 akaihola  (1000) users      (100)    20968 2024-03-16 14:19:35.000000 graylint-1.1.0/src/graylint/tests/test_linting.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     1056 2024-04-02 19:44:28.000000 graylint-1.1.0/src/graylint/tests/test_main.py
+-rw-r--r--   0 akaihola  (1000) users      (100)       86 2024-04-03 16:35:20.000000 graylint-1.1.0/src/graylint/version.py
+drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-04-03 16:35:39.442582 graylint-1.1.0/src/graylint.egg-info/
+-rw-r--r--   0 akaihola  (1000) users      (100)    22955 2024-04-03 16:35:39.000000 graylint-1.1.0/src/graylint.egg-info/PKG-INFO
+-rw-r--r--   0 akaihola  (1000) users      (100)      534 2024-04-03 16:35:39.000000 graylint-1.1.0/src/graylint.egg-info/SOURCES.txt
+-rw-r--r--   0 akaihola  (1000) users      (100)        1 2024-04-03 16:35:39.000000 graylint-1.1.0/src/graylint.egg-info/dependency_links.txt
+-rw-r--r--   0 akaihola  (1000) users      (100)       72 2024-04-03 16:35:39.000000 graylint-1.1.0/src/graylint.egg-info/entry_points.txt
+-rw-r--r--   0 akaihola  (1000) users      (100)      415 2024-04-03 16:35:39.000000 graylint-1.1.0/src/graylint.egg-info/requires.txt
+-rw-r--r--   0 akaihola  (1000) users      (100)        9 2024-04-03 16:35:39.000000 graylint-1.1.0/src/graylint.egg-info/top_level.txt
```

### Comparing `graylint-1.0.1/LICENSE.rst` & `graylint-1.1.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `graylint-1.0.1/PKG-INFO` & `graylint-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,84 +1,81 @@
 Metadata-Version: 2.1
 Name: graylint
-Version: 1.0.1
+Version: 1.1.0
 Summary: Run linters and show only new errors compared to an older commit
 Home-page: https://github.com/akaihola/graylint
 Author: Antti Kaihola
 Author-email: 13725+akaihola@users.noreply.github.com
 License: BSD
 Project-URL: Source Code, https://github.com/akaihola/graylint
 Project-URL: Change Log, https://github.com/akaihola/graylint/blob/master/CHANGES.rst
 Project-URL: News, https://github.com/akaihola/graylint/discussions/categories/announcements
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
 Requires-Dist: darkgraylib~=1.1.0
 Provides-Extra: color
 Requires-Dist: Pygments>=2.4.0; extra == "color"
 Provides-Extra: test
 Requires-Dist: airium>=0.2.3; extra == "test"
+Requires-Dist: click>=8.0.0; extra == "test"
 Requires-Dist: cryptography>=3.3.2; extra == "test"
 Requires-Dist: defusedxml>=0.7.1; extra == "test"
 Requires-Dist: mypy>=0.990; extra == "test"
 Requires-Dist: pathspec; extra == "test"
 Requires-Dist: pip-requirements-parser; extra == "test"
 Requires-Dist: pydocstyle; extra == "test"
-Requires-Dist: pygments; extra == "test"
+Requires-Dist: Pygments>=2.4.0; extra == "test"
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: pytest>=6.2.0; extra == "test"
 Requires-Dist: pytest-kwparametrize>=0.0.3; extra == "test"
-Requires-Dist: regex>=2021.4.4; extra == "test"
 Requires-Dist: requests_cache>=0.7; extra == "test"
 Requires-Dist: ruamel.yaml>=0.17.21; extra == "test"
 Requires-Dist: ruff>=0.0.292; extra == "test"
 Requires-Dist: twine>=2.0.0; extra == "test"
 Requires-Dist: types-requests>=2.27.9; extra == "test"
 Requires-Dist: types-toml>=0.10.4; extra == "test"
 Requires-Dist: urllib3>=1.25.9; extra == "test"
 Requires-Dist: wheel>=0.21.0; extra == "test"
 Provides-Extra: release
-Requires-Dist: airium>=0.2.3; extra == "release"
-Requires-Dist: click>=8.0.0; extra == "release"
-Requires-Dist: darkgray-dev-tools~=0.0.1; extra == "release"
-Requires-Dist: defusedxml>=0.7.1; extra == "release"
-Requires-Dist: requests_cache>=0.7; extra == "release"
+Requires-Dist: darkgray-dev-tools~=0.0.2; extra == "release"
 
 ==================================================
  Graylint – show new linter errors in Python code
 ==================================================
 
-|build-badge|_ |license-badge|_ |pypi-badge|_ |downloads-badge|_ |black-badge|_ |changelog-badge|_
+|build-badge| |license-badge| |pypi-badge| |downloads-badge| |black-badge| |changelog-badge|
 
 .. |build-badge| image:: https://github.com/akaihola/graylint/actions/workflows/python-package.yml/badge.svg
    :alt: master branch build status
-.. _build-badge: https://github.com/akaihola/graylint/actions/workflows/python-package.yml?query=branch%3Amaster
+   :target: https://github.com/akaihola/graylint/actions/workflows/python-package.yml?query=branch%3Amaster
 .. |license-badge| image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
    :alt: BSD 3 Clause license
-.. _license-badge: https://github.com/akaihola/graylint/blob/master/LICENSE.rst
+   :target: https://github.com/akaihola/graylint/blob/master/LICENSE.rst
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/graylint
    :alt: Latest release on PyPI
-.. _pypi-badge: https://pypi.org/project/graylint/
+   :target: https://pypi.org/project/graylint/
 .. |downloads-badge| image:: https://pepy.tech/badge/graylint
    :alt: Number of downloads
-.. _downloads-badge: https://pepy.tech/project/graylint
+   :target: https://pepy.tech/project/graylint
 .. |black-badge| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :alt: Source code formatted using Black
-.. _black-badge: https://github.com/psf/black
+   :target: https://github.com/psf/black
 .. |changelog-badge| image:: https://img.shields.io/badge/-change%20log-purple
    :alt: Change log
-.. _changelog-badge: https://github.com/akaihola/graylint/blob/master/CHANGES.rst
-.. |next-milestone| image:: https://img.shields.io/github/milestones/progress/akaihola/graylint/2?color=red&label=release%201.1.0
+   :target: https://github.com/akaihola/graylint/blob/master/CHANGES.rst
+.. |next-milestone| image:: https://img.shields.io/github/milestones/progress/akaihola/graylint/2?color=red&label=release%201.1.1
    :alt: Next milestone
-.. _next-milestone: https://github.com/akaihola/graylint/milestone/3
+   :target: https://github.com/akaihola/graylint/milestone/3
 
 
 What?
 =====
 
 This utility runs linters on Python source code files.
 However, when run in a Git repository, it runs the linters both in an old and a newer
@@ -113,15 +110,15 @@
 
 
 How?
 ====
 
 To install or upgrade, use::
 
-  pip install --upgrade graylint~=1.0.1
+  pip install --upgrade graylint~=1.1.0
 
 Or, if you're using Conda_ for package management::
 
   conda install -c conda-forge graylint~=0.0.1
   conda update -c conda-forge graylint
 
 ..
@@ -415,19 +412,19 @@
      lint:
        runs-on: ubuntu-latest
        steps:
          - uses: actions/checkout@v4
            with:
              fetch-depth: 0 
          - uses: actions/setup-python@v5
-         - uses: akaihola/graylint@1.0.1
+         - uses: akaihola/graylint@1.1.0
            with:
              options: "-v"
              src: "./src"
-             version: "~=1.0.1"
+             version: "~=1.1.0"
              lint: "flake8,pylint==2.13.1"
 
 There needs to be a working Python environment, set up using ``actions/setup-python``
 in the above example. Graylint will be installed in an isolated virtualenv to prevent
 conflicts with other workflows.
 
 ``"uses:"`` specifies which Graylint release to get the GitHub Action definition from.
```

### Comparing `graylint-1.0.1/README.rst` & `graylint-1.1.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 ==================================================
  Graylint – show new linter errors in Python code
 ==================================================
 
-|build-badge|_ |license-badge|_ |pypi-badge|_ |downloads-badge|_ |black-badge|_ |changelog-badge|_
+|build-badge| |license-badge| |pypi-badge| |downloads-badge| |black-badge| |changelog-badge|
 
 .. |build-badge| image:: https://github.com/akaihola/graylint/actions/workflows/python-package.yml/badge.svg
    :alt: master branch build status
-.. _build-badge: https://github.com/akaihola/graylint/actions/workflows/python-package.yml?query=branch%3Amaster
+   :target: https://github.com/akaihola/graylint/actions/workflows/python-package.yml?query=branch%3Amaster
 .. |license-badge| image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
    :alt: BSD 3 Clause license
-.. _license-badge: https://github.com/akaihola/graylint/blob/master/LICENSE.rst
+   :target: https://github.com/akaihola/graylint/blob/master/LICENSE.rst
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/graylint
    :alt: Latest release on PyPI
-.. _pypi-badge: https://pypi.org/project/graylint/
+   :target: https://pypi.org/project/graylint/
 .. |downloads-badge| image:: https://pepy.tech/badge/graylint
    :alt: Number of downloads
-.. _downloads-badge: https://pepy.tech/project/graylint
+   :target: https://pepy.tech/project/graylint
 .. |black-badge| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :alt: Source code formatted using Black
-.. _black-badge: https://github.com/psf/black
+   :target: https://github.com/psf/black
 .. |changelog-badge| image:: https://img.shields.io/badge/-change%20log-purple
    :alt: Change log
-.. _changelog-badge: https://github.com/akaihola/graylint/blob/master/CHANGES.rst
-.. |next-milestone| image:: https://img.shields.io/github/milestones/progress/akaihola/graylint/2?color=red&label=release%201.1.0
+   :target: https://github.com/akaihola/graylint/blob/master/CHANGES.rst
+.. |next-milestone| image:: https://img.shields.io/github/milestones/progress/akaihola/graylint/2?color=red&label=release%201.1.1
    :alt: Next milestone
-.. _next-milestone: https://github.com/akaihola/graylint/milestone/3
+   :target: https://github.com/akaihola/graylint/milestone/3
 
 
 What?
 =====
 
 This utility runs linters on Python source code files.
 However, when run in a Git repository, it runs the linters both in an old and a newer
@@ -75,15 +75,15 @@
 
 
 How?
 ====
 
 To install or upgrade, use::
 
-  pip install --upgrade graylint~=1.0.1
+  pip install --upgrade graylint~=1.1.0
 
 Or, if you're using Conda_ for package management::
 
   conda install -c conda-forge graylint~=0.0.1
   conda update -c conda-forge graylint
 
 ..
@@ -377,19 +377,19 @@
      lint:
        runs-on: ubuntu-latest
        steps:
          - uses: actions/checkout@v4
            with:
              fetch-depth: 0 
          - uses: actions/setup-python@v5
-         - uses: akaihola/graylint@1.0.1
+         - uses: akaihola/graylint@1.1.0
            with:
              options: "-v"
              src: "./src"
-             version: "~=1.0.1"
+             version: "~=1.1.0"
              lint: "flake8,pylint==2.13.1"
 
 There needs to be a working Python environment, set up using ``actions/setup-python``
 in the above example. Graylint will be installed in an isolated virtualenv to prevent
 conflicts with other workflows.
 
 ``"uses:"`` specifies which Graylint release to get the GitHub Action definition from.
```

### Comparing `graylint-1.0.1/setup.cfg` & `graylint-1.1.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 long_description_content_type = text/x-rst
 classifiers = 
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 project_urls = 
 	Source Code = https://github.com/akaihola/graylint
 	Change Log = https://github.com/akaihola/graylint/blob/master/CHANGES.rst
 	News = https://github.com/akaihola/graylint/discussions/categories/announcements
 url = https://github.com/akaihola/graylint
 
 [options]
@@ -41,39 +42,35 @@
 	graylint = graylint.__main__:main_with_error_handling
 
 [options.extras_require]
 color = 
 	Pygments>=2.4.0
 test = 
 	airium>=0.2.3
+	click>=8.0.0
 	cryptography>=3.3.2  # through twine, fixes CVE-2020-36242
 	defusedxml>=0.7.1
 	mypy>=0.990
 	pathspec  # to test `gen_python_files` in `test_black_diff.py`
 	pip-requirements-parser
 	pydocstyle
-	pygments
+	Pygments>=2.4.0
 	pylint
 	pytest>=6.2.0
 	pytest-kwparametrize>=0.0.3
-	regex>=2021.4.4
 	requests_cache>=0.7
 	ruamel.yaml>=0.17.21
 	ruff>=0.0.292
 	twine>=2.0.0
 	types-requests>=2.27.9
 	types-toml>=0.10.4
 	urllib3>=1.25.9  # through requests-cache and twine, fixes CVE-2020-26137
 	wheel>=0.21.0
 release = 
-	airium>=0.2.3
-	click>=8.0.0
-	darkgray-dev-tools~=0.0.1
-	defusedxml>=0.7.1
-	requests_cache>=0.7
+	darkgray-dev-tools~=0.0.2
 
 [flake8]
 max-line-length = 88
 ignore = 
 	C408
 	D400
 	D415
```

### Comparing `graylint-1.0.1/setup.py` & `graylint-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `graylint-1.0.1/src/graylint/__main__.py` & `graylint-1.1.0/src/graylint/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 """Graylint - run linters and hide linter errors already present in previous revision"""
 
+from __future__ import annotations
+
 import logging
 import sys
 from argparse import ArgumentError
 
 from darkgraylib.command_line import parse_command_line
 from darkgraylib.config import show_config_if_debug
 from darkgraylib.git import RevisionRange
 from darkgraylib.highlighting import should_use_color
 from darkgraylib.log import setup_logging
 from darkgraylib.main import resolve_paths
-
 from graylint.command_line import make_argument_parser
 from graylint.config import GraylintConfig
 from graylint.linting import run_linters
 
-
 logger = logging.getLogger(__name__)
 
 
 def main_with_error_handling() -> int:
     """Entry point for console script"""
     try:
         return main()
     except ArgumentError as exc_info:
         if logger.root.level < logging.WARNING:
             raise
         sys.exit(str(exc_info))
 
 
-def main() -> int:
+def main(argv: list[str] = None) -> int:
     """Parse the command line and lint each source file
 
     :return: Total number of linting errors found on modified lines
 
     """
     args, config, config_nondefault = parse_command_line(
-        make_argument_parser, sys.argv[1:], "graylint", GraylintConfig
+        make_argument_parser, argv, "graylint", GraylintConfig
     )
     setup_logging(args.log_level)
     show_config_if_debug(config, config_nondefault, args.log_level)
     paths, root = resolve_paths(args.stdin_filename, args.src)
     revrange = RevisionRange.parse_with_common_ancestor(
         args.revision, root, args.stdin_filename is not None
     )
@@ -48,13 +48,13 @@
         args.lint,
         root,
         # paths to lint are not limited to modified files or just Python files:
         {p.resolve().relative_to(root) for p in paths},
         revrange,
         use_color=should_use_color(config["color"]),
     )
-    return linter_failures_on_modified_lines
+    return 1 if linter_failures_on_modified_lines else 0
 
 
 if __name__ == "__main__":
     RETVAL = main_with_error_handling()
     sys.exit(RETVAL)
```

### Comparing `graylint-1.0.1/src/graylint/command_line.py` & `graylint-1.1.0/src/graylint/command_line.py`

 * *Files identical despite different names*

### Comparing `graylint-1.0.1/src/graylint/help.py` & `graylint-1.1.0/src/graylint/help.py`

 * *Files identical despite different names*

### Comparing `graylint-1.0.1/src/graylint/linting.py` & `graylint-1.1.0/src/graylint/linting.py`

 * *Files identical despite different names*

### Comparing `graylint-1.0.1/src/graylint/tests/test_linting.py` & `graylint-1.1.0/src/graylint/tests/test_linting.py`

 * *Files identical despite different names*

### Comparing `graylint-1.0.1/src/graylint.egg-info/PKG-INFO` & `graylint-1.1.0/src/graylint.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,84 +1,81 @@
 Metadata-Version: 2.1
 Name: graylint
-Version: 1.0.1
+Version: 1.1.0
 Summary: Run linters and show only new errors compared to an older commit
 Home-page: https://github.com/akaihola/graylint
 Author: Antti Kaihola
 Author-email: 13725+akaihola@users.noreply.github.com
 License: BSD
 Project-URL: Source Code, https://github.com/akaihola/graylint
 Project-URL: Change Log, https://github.com/akaihola/graylint/blob/master/CHANGES.rst
 Project-URL: News, https://github.com/akaihola/graylint/discussions/categories/announcements
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
 Requires-Dist: darkgraylib~=1.1.0
 Provides-Extra: color
 Requires-Dist: Pygments>=2.4.0; extra == "color"
 Provides-Extra: test
 Requires-Dist: airium>=0.2.3; extra == "test"
+Requires-Dist: click>=8.0.0; extra == "test"
 Requires-Dist: cryptography>=3.3.2; extra == "test"
 Requires-Dist: defusedxml>=0.7.1; extra == "test"
 Requires-Dist: mypy>=0.990; extra == "test"
 Requires-Dist: pathspec; extra == "test"
 Requires-Dist: pip-requirements-parser; extra == "test"
 Requires-Dist: pydocstyle; extra == "test"
-Requires-Dist: pygments; extra == "test"
+Requires-Dist: Pygments>=2.4.0; extra == "test"
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: pytest>=6.2.0; extra == "test"
 Requires-Dist: pytest-kwparametrize>=0.0.3; extra == "test"
-Requires-Dist: regex>=2021.4.4; extra == "test"
 Requires-Dist: requests_cache>=0.7; extra == "test"
 Requires-Dist: ruamel.yaml>=0.17.21; extra == "test"
 Requires-Dist: ruff>=0.0.292; extra == "test"
 Requires-Dist: twine>=2.0.0; extra == "test"
 Requires-Dist: types-requests>=2.27.9; extra == "test"
 Requires-Dist: types-toml>=0.10.4; extra == "test"
 Requires-Dist: urllib3>=1.25.9; extra == "test"
 Requires-Dist: wheel>=0.21.0; extra == "test"
 Provides-Extra: release
-Requires-Dist: airium>=0.2.3; extra == "release"
-Requires-Dist: click>=8.0.0; extra == "release"
-Requires-Dist: darkgray-dev-tools~=0.0.1; extra == "release"
-Requires-Dist: defusedxml>=0.7.1; extra == "release"
-Requires-Dist: requests_cache>=0.7; extra == "release"
+Requires-Dist: darkgray-dev-tools~=0.0.2; extra == "release"
 
 ==================================================
  Graylint – show new linter errors in Python code
 ==================================================
 
-|build-badge|_ |license-badge|_ |pypi-badge|_ |downloads-badge|_ |black-badge|_ |changelog-badge|_
+|build-badge| |license-badge| |pypi-badge| |downloads-badge| |black-badge| |changelog-badge|
 
 .. |build-badge| image:: https://github.com/akaihola/graylint/actions/workflows/python-package.yml/badge.svg
    :alt: master branch build status
-.. _build-badge: https://github.com/akaihola/graylint/actions/workflows/python-package.yml?query=branch%3Amaster
+   :target: https://github.com/akaihola/graylint/actions/workflows/python-package.yml?query=branch%3Amaster
 .. |license-badge| image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
    :alt: BSD 3 Clause license
-.. _license-badge: https://github.com/akaihola/graylint/blob/master/LICENSE.rst
+   :target: https://github.com/akaihola/graylint/blob/master/LICENSE.rst
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/graylint
    :alt: Latest release on PyPI
-.. _pypi-badge: https://pypi.org/project/graylint/
+   :target: https://pypi.org/project/graylint/
 .. |downloads-badge| image:: https://pepy.tech/badge/graylint
    :alt: Number of downloads
-.. _downloads-badge: https://pepy.tech/project/graylint
+   :target: https://pepy.tech/project/graylint
 .. |black-badge| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :alt: Source code formatted using Black
-.. _black-badge: https://github.com/psf/black
+   :target: https://github.com/psf/black
 .. |changelog-badge| image:: https://img.shields.io/badge/-change%20log-purple
    :alt: Change log
-.. _changelog-badge: https://github.com/akaihola/graylint/blob/master/CHANGES.rst
-.. |next-milestone| image:: https://img.shields.io/github/milestones/progress/akaihola/graylint/2?color=red&label=release%201.1.0
+   :target: https://github.com/akaihola/graylint/blob/master/CHANGES.rst
+.. |next-milestone| image:: https://img.shields.io/github/milestones/progress/akaihola/graylint/2?color=red&label=release%201.1.1
    :alt: Next milestone
-.. _next-milestone: https://github.com/akaihola/graylint/milestone/3
+   :target: https://github.com/akaihola/graylint/milestone/3
 
 
 What?
 =====
 
 This utility runs linters on Python source code files.
 However, when run in a Git repository, it runs the linters both in an old and a newer
@@ -113,15 +110,15 @@
 
 
 How?
 ====
 
 To install or upgrade, use::
 
-  pip install --upgrade graylint~=1.0.1
+  pip install --upgrade graylint~=1.1.0
 
 Or, if you're using Conda_ for package management::
 
   conda install -c conda-forge graylint~=0.0.1
   conda update -c conda-forge graylint
 
 ..
@@ -415,19 +412,19 @@
      lint:
        runs-on: ubuntu-latest
        steps:
          - uses: actions/checkout@v4
            with:
              fetch-depth: 0 
          - uses: actions/setup-python@v5
-         - uses: akaihola/graylint@1.0.1
+         - uses: akaihola/graylint@1.1.0
            with:
              options: "-v"
              src: "./src"
-             version: "~=1.0.1"
+             version: "~=1.1.0"
              lint: "flake8,pylint==2.13.1"
 
 There needs to be a working Python environment, set up using ``actions/setup-python``
 in the above example. Graylint will be installed in an isolated virtualenv to prevent
 conflicts with other workflows.
 
 ``"uses:"`` specifies which Graylint release to get the GitHub Action definition from.
```

