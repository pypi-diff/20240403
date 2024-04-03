# Comparing `tmp/anl-0.1.8.tar.gz` & `tmp/anl-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anl-0.1.8.tar", last modified: Sun Dec 31 13:22:53 2023, max compression
+gzip compressed data, was "anl-0.1.9.tar", last modified: Wed Feb 14 07:03:04 2024, max compression
```

## Comparing `anl-0.1.8.tar` & `anl-0.1.9.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-12-31 13:22:53.910807 anl-0.1.8/
--rw-r--r--   0 yasser     (501) staff       (20)      288 2023-12-31 12:16:11.000000 anl-0.1.8/.bumpversion.cfg
--rw-r--r--   0 yasser     (501) staff       (20)      171 2023-12-24 12:42:29.000000 anl-0.1.8/.coveragerc
--rw-r--r--   0 yasser     (501) staff       (20)      217 2023-12-24 12:42:29.000000 anl-0.1.8/.editorconfig
--rw-r--r--   0 yasser     (501) staff       (20)       78 2023-12-24 12:42:29.000000 anl-0.1.8/AUTHORS.rst
--rw-r--r--   0 yasser     (501) staff       (20)     2812 2023-12-31 12:16:42.000000 anl-0.1.8/CHANGELOG.rst
--rw-r--r--   0 yasser     (501) staff       (20)     2629 2023-12-24 12:42:29.000000 anl-0.1.8/CONTRIBUTING.rst
--rw-r--r--   0 yasser     (501) staff       (20)      739 2023-12-24 12:42:29.000000 anl-0.1.8/LICENSE
--rw-r--r--   0 yasser     (501) staff       (20)      522 2023-12-24 12:42:29.000000 anl-0.1.8/MANIFEST.in
--rw-r--r--   0 yasser     (501) staff       (20)     4542 2023-12-31 13:22:53.910923 anl-0.1.8/PKG-INFO
--rw-r--r--   0 yasser     (501) staff       (20)     3729 2023-12-24 12:42:29.000000 anl-0.1.8/README.rst
--rw-r--r--   0 yasser     (501) staff       (20)      570 2023-12-31 13:22:53.912105 anl-0.1.8/setup.cfg
--rw-r--r--   0 yasser     (501) staff       (20)     2689 2023-12-31 12:16:11.000000 anl-0.1.8/setup.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-12-31 13:22:53.835716 anl-0.1.8/src/
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-12-31 13:22:53.869629 anl-0.1.8/src/anl/
--rw-r--r--   0 yasser     (501) staff       (20)      145 2023-12-31 12:16:11.000000 anl-0.1.8/src/anl/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)      354 2023-12-24 12:42:29.000000 anl-0.1.8/src/anl/__main__.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-12-31 13:22:53.879694 anl-0.1.8/src/anl/anl2024/
--rwxr-xr-x   0 yasser     (501) staff       (20)      228 2023-12-24 12:42:29.000000 anl-0.1.8/src/anl/anl2024/__init__.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-12-31 13:22:53.881491 anl-0.1.8/src/anl/anl2024/negotiators/
--rw-r--r--   0 yasser     (501) staff       (20)       52 2023-12-24 12:42:29.000000 anl-0.1.8/src/anl/anl2024/negotiators/__init__.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-12-31 13:22:53.891883 anl-0.1.8/src/anl/anl2024/negotiators/builtins/
--rw-r--r--   0 yasser     (501) staff       (20)      183 2023-12-25 07:17:37.000000 anl-0.1.8/src/anl/anl2024/negotiators/builtins/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)     4206 2023-12-31 07:28:08.000000 anl-0.1.8/src/anl/anl2024/negotiators/builtins/micro.py
--rw-r--r--   0 yasser     (501) staff       (20)     3525 2023-12-25 06:33:38.000000 anl-0.1.8/src/anl/anl2024/negotiators/builtins/nash_seeker.py
--rw-r--r--   0 yasser     (501) staff       (20)     9211 2023-12-31 02:36:25.000000 anl-0.1.8/src/anl/anl2024/negotiators/builtins/rv_fitter.py
--rw-r--r--   0 yasser     (501) staff       (20)     1950 2023-12-24 12:42:29.000000 anl-0.1.8/src/anl/anl2024/negotiators/builtins/wrappers.py
--rw-r--r--   0 yasser     (501) staff       (20)    24686 2023-12-25 07:32:18.000000 anl-0.1.8/src/anl/anl2024/runner.py
--rw-r--r--   0 yasser     (501) staff       (20)    24732 2023-12-27 12:32:58.000000 anl-0.1.8/src/anl/cli.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-12-31 13:22:53.892815 anl-0.1.8/src/anl/visualizer/
--rw-r--r--   0 yasser     (501) staff       (20)    22630 2023-12-31 12:15:22.000000 anl-0.1.8/src/anl/visualizer/app.py
--rwxr-xr-x   0 yasser     (501) staff       (20)     1395 2023-12-31 12:14:32.000000 anl-0.1.8/src/anl/visualizer/cli.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-12-31 13:22:53.873180 anl-0.1.8/src/anl.egg-info/
--rw-r--r--   0 yasser     (501) staff       (20)     4542 2023-12-31 13:22:53.000000 anl-0.1.8/src/anl.egg-info/PKG-INFO
--rw-r--r--   0 yasser     (501) staff       (20)      960 2023-12-31 13:22:53.000000 anl-0.1.8/src/anl.egg-info/SOURCES.txt
--rw-r--r--   0 yasser     (501) staff       (20)        1 2023-12-31 13:22:53.000000 anl-0.1.8/src/anl.egg-info/dependency_links.txt
--rw-r--r--   0 yasser     (501) staff       (20)      135 2023-12-31 13:22:53.000000 anl-0.1.8/src/anl.egg-info/entry_points.txt
--rw-r--r--   0 yasser     (501) staff       (20)        1 2023-11-30 20:07:32.000000 anl-0.1.8/src/anl.egg-info/not-zip-safe
--rw-r--r--   0 yasser     (501) staff       (20)       86 2023-12-31 13:22:53.000000 anl-0.1.8/src/anl.egg-info/requires.txt
--rw-r--r--   0 yasser     (501) staff       (20)        4 2023-12-31 13:22:53.000000 anl-0.1.8/src/anl.egg-info/top_level.txt
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-12-31 13:22:53.906586 anl-0.1.8/tests/
--rw-r--r--   0 yasser     (501) staff       (20)        0 2023-12-24 12:42:29.000000 anl-0.1.8/tests/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)      827 2023-12-25 01:10:03.000000 anl-0.1.8/tests/switches.py
--rw-r--r--   0 yasser     (501) staff       (20)      212 2023-12-25 01:01:04.000000 anl-0.1.8/tests/test_cli.py
--rw-r--r--   0 yasser     (501) staff       (20)      745 2023-12-25 01:02:05.000000 anl-0.1.8/tests/test_jupyter.py
--rw-r--r--   0 yasser     (501) staff       (20)     1678 2023-12-25 01:13:01.000000 anl-0.1.8/tests/test_micro.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-12-31 13:22:53.842533 anl-0.1.8/tests/tmp_notebooks/
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-12-31 13:22:53.910406 anl-0.1.8/tests/tmp_notebooks/tutorials/
--rw-r--r--   0 yasser     (501) staff       (20)    21978 2023-12-25 05:53:14.000000 anl-0.1.8/tests/tmp_notebooks/tutorials/01.develop_an_agent.ipynb
--rw-r--r--   0 yasser     (501) staff       (20)     1828 2023-12-24 12:42:29.000000 anl-0.1.8/tox.ini
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-02-14 07:03:04.066638 anl-0.1.9/
+-rw-r--r--   0 yasser     (501) staff       (20)      288 2024-02-14 06:56:30.000000 anl-0.1.9/.bumpversion.cfg
+-rw-r--r--   0 yasser     (501) staff       (20)      171 2023-12-24 12:42:29.000000 anl-0.1.9/.coveragerc
+-rw-r--r--   0 yasser     (501) staff       (20)      217 2023-12-24 12:42:29.000000 anl-0.1.9/.editorconfig
+-rw-r--r--   0 yasser     (501) staff       (20)       78 2023-12-24 12:42:29.000000 anl-0.1.9/AUTHORS.rst
+-rw-r--r--   0 yasser     (501) staff       (20)     2970 2024-02-14 06:56:44.000000 anl-0.1.9/CHANGELOG.rst
+-rw-r--r--   0 yasser     (501) staff       (20)     2629 2023-12-24 12:42:29.000000 anl-0.1.9/CONTRIBUTING.rst
+-rw-r--r--   0 yasser     (501) staff       (20)      739 2023-12-24 12:42:29.000000 anl-0.1.9/LICENSE
+-rw-r--r--   0 yasser     (501) staff       (20)      522 2023-12-24 12:42:29.000000 anl-0.1.9/MANIFEST.in
+-rw-r--r--   0 yasser     (501) staff       (20)     4700 2024-02-14 07:03:04.066893 anl-0.1.9/PKG-INFO
+-rw-r--r--   0 yasser     (501) staff       (20)     3729 2023-12-24 12:42:29.000000 anl-0.1.9/README.rst
+-rw-r--r--   0 yasser     (501) staff       (20)      570 2024-02-14 07:03:04.067796 anl-0.1.9/setup.cfg
+-rw-r--r--   0 yasser     (501) staff       (20)     2689 2024-02-14 07:00:38.000000 anl-0.1.9/setup.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-02-14 07:03:03.988405 anl-0.1.9/src/
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-02-14 07:03:04.004543 anl-0.1.9/src/anl/
+-rw-r--r--   0 yasser     (501) staff       (20)      145 2024-02-14 06:56:30.000000 anl-0.1.9/src/anl/__init__.py
+-rw-r--r--   0 yasser     (501) staff       (20)      354 2023-12-24 12:42:29.000000 anl-0.1.9/src/anl/__main__.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-02-14 07:03:04.007915 anl-0.1.9/src/anl/anl2024/
+-rwxr-xr-x   0 yasser     (501) staff       (20)      228 2023-12-24 12:42:29.000000 anl-0.1.9/src/anl/anl2024/__init__.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-02-14 07:03:04.009811 anl-0.1.9/src/anl/anl2024/negotiators/
+-rw-r--r--   0 yasser     (501) staff       (20)       52 2023-12-24 12:42:29.000000 anl-0.1.9/src/anl/anl2024/negotiators/__init__.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-02-14 07:03:04.017943 anl-0.1.9/src/anl/anl2024/negotiators/builtins/
+-rw-r--r--   0 yasser     (501) staff       (20)      183 2023-12-25 07:17:37.000000 anl-0.1.9/src/anl/anl2024/negotiators/builtins/__init__.py
+-rw-r--r--   0 yasser     (501) staff       (20)     4206 2023-12-31 07:28:08.000000 anl-0.1.9/src/anl/anl2024/negotiators/builtins/micro.py
+-rw-r--r--   0 yasser     (501) staff       (20)     3525 2023-12-25 06:33:38.000000 anl-0.1.9/src/anl/anl2024/negotiators/builtins/nash_seeker.py
+-rw-r--r--   0 yasser     (501) staff       (20)     9211 2023-12-31 02:36:25.000000 anl-0.1.9/src/anl/anl2024/negotiators/builtins/rv_fitter.py
+-rw-r--r--   0 yasser     (501) staff       (20)     1950 2023-12-24 12:42:29.000000 anl-0.1.9/src/anl/anl2024/negotiators/builtins/wrappers.py
+-rw-r--r--   0 yasser     (501) staff       (20)     5706 2024-01-30 23:53:39.000000 anl-0.1.9/src/anl/anl2024/negotiators/builtins.py
+-rw-r--r--   0 yasser     (501) staff       (20)    32171 2024-01-09 12:32:47.000000 anl-0.1.9/src/anl/anl2024/runner.py
+-rw-r--r--   0 yasser     (501) staff       (20)    25084 2024-01-09 12:29:28.000000 anl-0.1.9/src/anl/cli.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-02-14 07:03:04.045001 anl-0.1.9/src/anl/visualizer/
+-rw-r--r--   0 yasser     (501) staff       (20)    22630 2023-12-31 12:15:22.000000 anl-0.1.9/src/anl/visualizer/app.py
+-rwxr-xr-x   0 yasser     (501) staff       (20)     1395 2023-12-31 12:14:32.000000 anl-0.1.9/src/anl/visualizer/cli.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-02-14 07:03:04.006540 anl-0.1.9/src/anl.egg-info/
+-rw-r--r--   0 yasser     (501) staff       (20)     4700 2024-02-14 07:03:03.000000 anl-0.1.9/src/anl.egg-info/PKG-INFO
+-rw-r--r--   0 yasser     (501) staff       (20)     1000 2024-02-14 07:03:03.000000 anl-0.1.9/src/anl.egg-info/SOURCES.txt
+-rw-r--r--   0 yasser     (501) staff       (20)        1 2024-02-14 07:03:03.000000 anl-0.1.9/src/anl.egg-info/dependency_links.txt
+-rw-r--r--   0 yasser     (501) staff       (20)      135 2024-02-14 07:03:03.000000 anl-0.1.9/src/anl.egg-info/entry_points.txt
+-rw-r--r--   0 yasser     (501) staff       (20)        1 2023-11-30 20:07:32.000000 anl-0.1.9/src/anl.egg-info/not-zip-safe
+-rw-r--r--   0 yasser     (501) staff       (20)       86 2024-02-14 07:03:03.000000 anl-0.1.9/src/anl.egg-info/requires.txt
+-rw-r--r--   0 yasser     (501) staff       (20)        4 2024-02-14 07:03:03.000000 anl-0.1.9/src/anl.egg-info/top_level.txt
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-02-14 07:03:04.059133 anl-0.1.9/tests/
+-rw-r--r--   0 yasser     (501) staff       (20)        0 2023-12-24 12:42:29.000000 anl-0.1.9/tests/__init__.py
+-rw-r--r--   0 yasser     (501) staff       (20)      827 2023-12-25 01:10:03.000000 anl-0.1.9/tests/switches.py
+-rw-r--r--   0 yasser     (501) staff       (20)      212 2023-12-25 01:01:04.000000 anl-0.1.9/tests/test_cli.py
+-rw-r--r--   0 yasser     (501) staff       (20)      745 2023-12-25 01:02:05.000000 anl-0.1.9/tests/test_jupyter.py
+-rw-r--r--   0 yasser     (501) staff       (20)     1612 2024-01-30 23:50:51.000000 anl-0.1.9/tests/test_micro.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-02-14 07:03:03.989829 anl-0.1.9/tests/tmp_notebooks/
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-02-14 07:03:04.065459 anl-0.1.9/tests/tmp_notebooks/tutorials/
+-rw-r--r--   0 yasser     (501) staff       (20)    21978 2023-12-25 05:53:14.000000 anl-0.1.9/tests/tmp_notebooks/tutorials/01.develop_an_agent.ipynb
+-rw-r--r--   0 yasser     (501) staff       (20)     1828 2023-12-24 12:42:29.000000 anl-0.1.9/tox.ini
```

### Comparing `anl-0.1.8/CHANGELOG.rst` & `anl-0.1.9/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+0.1.9 (2024.02.14)
+------------------
+
+- Adding divide-the-pies scenarios
+- Adding workflow to test on negmas master
+- Tutorial and docs update
+- Update faq
+
 0.1.8 (2023.12.31)
 ------------------
 
 * bugfix in visualizer initial tournament list
 * Correcting auto pushing to PyPi
 
 0.1.7 (2023.12.31)
```

### Comparing `anl-0.1.8/CONTRIBUTING.rst` & `anl-0.1.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `anl-0.1.8/LICENSE` & `anl-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `anl-0.1.8/MANIFEST.in` & `anl-0.1.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `anl-0.1.8/PKG-INFO` & `anl-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anl
-Version: 0.1.8
+Version: 0.1.9
 Summary: ANAC Automated Negotiations League Platform
 Home-page: https://github.com/autoneg/anl
 Author: Yasser Mohammad
 Author-email: yasserfarouk@gmail.com
 Project-URL: Documentation, https://anl.readthedocs.io/
 Project-URL: Changelog, https://anl.readthedocs.io/en/latest/changelog.html
 Project-URL: Issue Tracker, https://github.com/autoneg/anl/issues
@@ -57,14 +57,22 @@
 
 
 https://yasserfarouk.github.io/anl/
 
 Changelog
 =========
 
+0.1.9 (2024.02.14)
+------------------
+
+- Adding divide-the-pies scenarios
+- Adding workflow to test on negmas master
+- Tutorial and docs update
+- Update faq
+
 0.1.8 (2023.12.31)
 ------------------
 
 * bugfix in visualizer initial tournament list
 * Correcting auto pushing to PyPi
 
 0.1.7 (2023.12.31)
```

### Comparing `anl-0.1.8/README.rst` & `anl-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `anl-0.1.8/setup.cfg` & `anl-0.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `anl-0.1.8/setup.py` & `anl-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")
     ) as fh:
         return fh.read()
 
 
 setup(
     name="anl",
-    version="0.1.8",
+    version="0.1.9",
     description="ANAC Automated Negotiations League Platform",
     long_description="%s\n%s"
     % (
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub(
             "", read("README.rst")
         ),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
@@ -60,15 +60,15 @@
     python_requires=">=3.10",
     install_requires=[
         # 'dataclasses; python_version < "3.7"',
         "click",
         "pytest",
         "hypothesis",
         "prettytable",
-        "negmas>=0.10.12",
+        "negmas>=0.10.13",
         "tqdm",
         "joblib",
         "jupyter",
         "gif",
         "streamlit",
     ],
     extras_require={},
```

### Comparing `anl-0.1.8/src/anl/anl2024/negotiators/builtins/micro.py` & `anl-0.1.9/src/anl/anl2024/negotiators/builtins/micro.py`

 * *Files identical despite different names*

### Comparing `anl-0.1.8/src/anl/anl2024/negotiators/builtins/nash_seeker.py` & `anl-0.1.9/src/anl/anl2024/negotiators/builtins/nash_seeker.py`

 * *Files identical despite different names*

### Comparing `anl-0.1.8/src/anl/anl2024/negotiators/builtins/rv_fitter.py` & `anl-0.1.9/src/anl/anl2024/negotiators/builtins/rv_fitter.py`

 * *Files identical despite different names*

### Comparing `anl-0.1.8/src/anl/anl2024/negotiators/builtins/wrappers.py` & `anl-0.1.9/src/anl/anl2024/negotiators/builtins/wrappers.py`

 * *Files identical despite different names*

### Comparing `anl-0.1.8/src/anl/anl2024/runner.py` & `anl-0.1.9/src/anl/anl2024/runner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,26 @@
+import itertools
 import random
 from pathlib import Path
 from typing import Any, Callable, Iterable, Sequence
 
 import numpy as np
 from negmas.helpers.misc import intin
 from negmas.helpers.strings import unique_name
 from negmas.inout import Scenario, UtilityFunction, pareto_frontier
 from negmas.negotiators import Negotiator
 from negmas.outcomes import make_issue, make_os
 from negmas.preferences import LinearAdditiveUtilityFunction as U
-from negmas.preferences.generators import generate_utility_values
+from negmas.preferences.generators import GENERATOR_MAP, generate_multi_issue_ufuns, generate_utility_values
 from negmas.preferences.ops import nash_points
 from negmas.preferences.value_fun import TableFun
 from negmas.sao.mechanism import SAOMechanism
 from negmas.tournaments.neg.simple import SimpleTournamentResults, cartesian_tournament
 
-from anl.anl2024.negotiators.builtins import (
-    Boulware,
-    Conceder,
-    Linear,
-    MiCRO,
-    NashSeeker,
-    RVFitter,
-)
+from anl.anl2024.negotiators.builtins import Boulware, Conceder, Linear, MiCRO, NashSeeker, RVFitter
 
 # from anl.anl2024.negotiators.builtin import (
 #     StochasticBoulware,
 #     StochasticConceder,
 #     StochasticLinear,
 # NaiveTitForTat,
 # )
@@ -85,26 +79,128 @@
     scenario_generator="mix",
     outcomes_log_uniform=True,
     generator_params=dict(
         reserved_ranges=((0.0, 1.0), (0.0, 1.0)),
         log_uniform=False,
         zerosum_fraction=0.05,
         monotonic_fraction=0.25,
-        curve_fraction=0.5,
+        curve_fraction=0.25,
+        pies_fraction=0.2,
         pareto_first=False,
         n_pareto=(0.005, 0.25),
     ),
 )
 """Default settings for ANL 2024"""
 
 
 ScenarioGenerator = Callable[[int, int | tuple[int, int] | list[int]], list[Scenario]]
 """Type of callable that can be used for generating scenarios. It must receive the number of scenarios and number of outcomes (as int, tuple or list) and return a list of `Scenario` s"""
 
 
+def pies_scenarios(
+    n_scenarios: int = 20,
+    n_outcomes: int | tuple[int, int] | list[int] = 100,
+    *,
+    reserved_ranges: ReservedRanges = ((0.0, 0.999999), (0.0, 0.999999)),
+    log_uniform: bool = True,
+    monotonic=True,
+) -> list[Scenario]:
+    """Creates multi-issue scenarios with arbitrary/monotonically increasing value functions
+
+    Args:
+        n_scenarios: Number of scenarios to create
+        n_outcomes: Number of outcomes per scenario. If a tuple it will be interpreted as a min/max range to sample n. outcomes from.
+                    If a list, samples from this list will be used (with replacement).
+        reserved_ranges: Ranges of reserved values for first and second negotiators
+        log_uniform: If given, the distribution used will be uniform on the logarithm of n. outcomes (only used when n_outcomes is a 2-valued tuple).
+        monotonic: If true all ufuns are monotonically increasing in the portion of the pie
+
+    Remarks:
+        - When n_outcomes is a tuple, the number of outcomes for each scenario will be sampled independently.
+    """
+    ufun_sets = []
+    base_name = "DivideTyePies" if monotonic else "S"
+
+    def normalize(x):
+        mn, mx = x.min(), x.max()
+        return ((x - mn) / (mx - mn)).tolist()
+
+    def make_monotonic(x, i):
+        x = np.sort(np.asarray(x), axis=None)
+
+        if i:
+            x = x[::-1]
+        r = random.random()
+        if r < 0.33:
+            x = np.exp(x)
+        elif r < 0.67:
+            x = np.log(x)
+        else:
+            pass
+        return normalize(x)
+
+    max_jitter_level = 0.8
+    for i in range(n_scenarios):
+        n = intin(n_outcomes, log_uniform)
+        issues = (
+            make_issue(
+                [f"{i}_{n-1 - i}" for i in range(n)],
+                "portions" if not monotonic else "i1",
+            ),
+        )
+        # funs = [
+        #     dict(
+        #         zip(
+        #             issues[0].all,
+        #             # adjust(np.asarray([random.random() for _ in range(n)])),
+        #             generate(n, i),
+        #         )
+        #     )
+        #     for i in range(2)
+        # ]
+        os = make_os(issues, name=f"{base_name}{i}")
+        outcomes = list(os.enumerate_or_sample())
+        ufuns = U.generate_bilateral(
+            outcomes,
+            conflict_level=0.5 + 0.5 * random.random(),
+            conflict_delta=random.random(),
+        )
+        jitter_level = random.random() * max_jitter_level
+        funs = [
+            np.asarray([float(u(_)) for _ in outcomes])
+            + np.random.random() * jitter_level
+            for u in ufuns
+        ]
+
+        if monotonic:
+            funs = [make_monotonic(x, i) for i, x in enumerate(funs)]
+        else:
+            funs = [normalize(x) for x in funs]
+        ufuns = tuple(
+            U(
+                values=(TableFun(dict(zip(issues[0].all, vals))),),
+                name=f"{uname}{i}",
+                outcome_space=os,
+                # reserved_value=(r[0] + random.random() * (r[1] - r[0] - 1e-8)),
+            )
+            for (uname, vals) in zip(("First", "Second"), funs)
+            # for (uname, r, vals) in zip(("First", "Second"), reserved_ranges, funs)
+        )
+        sample_reserved_values(ufuns, reserved_ranges=reserved_ranges)
+        ufun_sets.append(ufuns)
+
+    return [
+        Scenario(
+            outcome_space=ufuns[0].outcome_space,  # type: ignore We are sure this is not None
+            ufuns=ufuns,
+        )
+        for ufuns in ufun_sets
+    ]
+
+
 def pie_scenarios(
     n_scenarios: int = 20,
     n_outcomes: int | tuple[int, int] | list[int] = 100,
     *,
     reserved_ranges: ReservedRanges = ((0.0, 0.999999), (0.0, 0.999999)),
     log_uniform: bool = True,
     monotonic=False,
@@ -214,14 +310,121 @@
         n_outcomes,
         reserved_ranges=reserved_ranges,
         log_uniform=log_uniform,
         monotonic=False,
     )
 
 
+def product(generator):
+    """
+    Calculates the product of all elements in a generator.
+
+    Args:
+        generator: A generator of numbers.
+
+    Returns:
+        The product of all elements in the generator.
+    """
+    total = 1
+    for num in generator:
+        total *= num
+    return total
+
+
+def find_three_integers(x):
+    """Finds three integers that multiply to a number, considering numbers around x."""
+
+    for offset in itertools.count(0):
+        current_number = x + (-1) ** offset * offset
+
+        # Stop searching downwards at 8
+        if current_number < 8:
+            break
+
+        result = find_three_integers_for_number(current_number)
+        if result:
+            return result
+
+    return None  # No solution found within the search range
+
+
+def find_three_integers_for_number(x, fraction=0.1):
+    """Helper function to find three integers for a given number."""
+
+    # Check for perfect cubes
+    cube_root = int(x ** (1 / 3))
+    if cube_root**3 >= x * (1 - fraction):
+        return (
+            cube_root,
+            cube_root + random.randint(-1, 1),
+            cube_root,
+        )
+
+    # Factor x into primes
+    prime_factors = []
+    divisor = 2
+    while x > 1:
+        while x % divisor == 0:
+            prime_factors.append(divisor)
+            x //= divisor
+        divisor += 1
+
+    # Try to group prime factors into threes
+    for combination in itertools.combinations(prime_factors, 3):
+        if product(combination) == x:
+            return combination
+
+    # Try combining factors to create three integers
+    if len(prime_factors) >= 4:
+        for i in range(1, len(prime_factors) - 2):
+            if (
+                prime_factors[0] * prime_factors[i] * product(prime_factors[i + 1 :])
+                == x
+            ):
+                return (
+                    prime_factors[0],
+                    prime_factors[i],
+                    product(prime_factors[i + 1 :]),
+                )
+
+    return None
+
+
+def monotonic_pies_scenarios(
+    n_scenarios: int = 20,
+    n_outcomes: int | tuple[int, int] | list[int] = 100,
+    *,
+    reserved_ranges: ReservedRanges = ((0.0, 0.999999), (0.0, 0.999999)),
+    log_uniform: bool = False,
+) -> list[Scenario]:
+    ufun_sets = []
+    for s in range(n_scenarios):
+        ufuns = generate_multi_issue_ufuns(
+            3,
+            sizes=find_three_integers_for_number(n_outcomes),
+            os_name=f"DivideThePies{s}",
+        )
+        os = ufuns[0].outcome_space
+        assert os is not None
+        sample_reserved_values(
+            ufuns,
+            pareto=tuple(tuple(u(_) for u in ufuns) for _ in os.enumerate_or_sample()),
+            reserved_ranges=reserved_ranges,
+        )
+        ufun_sets.append(ufuns)
+
+    return [
+        Scenario(
+            outcome_space=ufuns[0].outcome_space,  # type: ignore We are sure this is not None
+            ufuns=ufuns,
+        )
+        for ufuns in ufun_sets
+    ]
+
+
 def monotonic_pie_scenarios(
     n_scenarios: int = 20,
     n_outcomes: int | tuple[int, int] | list[int] = 100,
     *,
     reserved_ranges: ReservedRanges = ((0.0, 0.999999), (0.0, 0.999999)),
     log_uniform: bool = True,
 ) -> list[Scenario]:
@@ -229,14 +432,22 @@
         n_scenarios,
         n_outcomes,
         reserved_ranges=reserved_ranges,
         log_uniform=log_uniform,
         monotonic=True,
     )
 
+    return [
+        Scenario(
+            outcome_space=ufuns[0].outcome_space,  # type: ignore We are sure this is not None
+            ufuns=ufuns,
+        )
+        for ufuns in ufun_sets
+    ]
+
 
 def sample_reserved_values(
     ufuns: tuple[UtilityFunction, ...],
     pareto: tuple[tuple[float, ...], ...] | None = None,
     reserved_ranges: ReservedRanges = ((0.0, 1.0), (0.0, 1.0)),
     eps: float = 1e-3,
 ) -> tuple[float, ...]:
@@ -340,14 +551,15 @@
     | list[int] = DEFAULT2024SETTINGS["n_outcomes"],  # type: ignore
     *,
     reserved_ranges: ReservedRanges = DEFAULT2024SETTINGS["reserved_ranges"],  # type: ignore
     log_uniform: bool = DEFAULT2024SETTINGS["outcomes_log_uniform"],  # type: ignore
     zerosum_fraction: float = DEFAULT2024SETTINGS["generator_params"]["zerosum_fraction"],  # type: ignore
     monotonic_fraction: float = DEFAULT2024SETTINGS["generator_params"]["monotonic_fraction"],  # type: ignore
     curve_fraction: float = DEFAULT2024SETTINGS["generator_params"]["curve_fraction"],  # type: ignore
+    pies_fraction: float = DEFAULT2024SETTINGS["generator_params"]["pies_fraction"],  # type: ignore
     pareto_first: bool = DEFAULT2024SETTINGS["generator_params"]["pareto_first"],  # type: ignore
     n_ufuns: int = DEFAULT2024SETTINGS["n_ufuns"],  # type: ignore
     n_pareto: int | float | tuple[float | int, float | int] | list[int | float] = DEFAULT2024SETTINGS["generator_params"]["n_pareto"],  # type: ignore
     pareto_log_uniform: bool = False,
     n_trials=10,
 ) -> list[Scenario]:
     """Generates a mix of zero-sum, monotonic and general scenarios
@@ -359,14 +571,15 @@
                          Note that the upper limit will be overridden to guarantee
                          the existence of at least one rational outcome
         log_uniform: Use log-uniform instead of uniform sampling if n_outcomes is a tuple giving a range.
         zerosum_fraction: Fraction of zero-sum scenarios. These are original DivideThePie scenarios
         monotonic_fraction: Fraction of scenarios where each ufun is a monotonic function of the received pie.
         curve_fraction: Fraction of general and monotonic scenarios that use a curve for Pareto generation instead of
                         a piecewise linear Pareto frontier.
+        pies_fraction: Fraction of divide-the-pies multi-issue scenarios
         pareto_first: If given, the Pareto frontier will always be in the first set of outcomes
         n_ufuns: Number of ufuns to generate per scenario
         n_pareto: Number of outcomes on the Pareto frontier in general scenarios.
                 Can be specified as a number, a tuple of a min and max to sample within, a list of possibilities.
                 Each value can either be an integer > 1 or a fraction of the number of outcomes in the scenario.
         pareto_log_uniform: Use log-uniform instead of uniform sampling if n_pareto is a tuple
         n_trials: Number of times to retry generating each scenario if failures occures
@@ -388,25 +601,35 @@
             if isinstance(n_pareto, Iterable):
                 n_pareto = type(n_pareto)(
                     int(_ * n + 0.5) if _ < 1 else int(_) for _ in n_pareto  # type: ignore
                 )
             else:
                 n_pareto = int(0.5 + n_pareto * n) if n_pareto < 1 else int(n_pareto)
             n_pareto_selected = intin(n_pareto, log_uniform=pareto_log_uniform)  # type: ignore
+        ufuns, vals = None, None
         for _ in range(n_trials):
             try:
                 if r < zerosum_fraction:
+                    name = "DivideThePie"
                     vals = generate_utility_values(
                         n_pareto=n_pareto_selected,
                         n_outcomes=n,
                         n_ufuns=n_ufuns,
                         pareto_first=pareto_first,
                         pareto_generator="zero_sum",
                     )
-                    name = "DivideThePie"
+                elif r < zerosum_fraction + pies_fraction:
+                    name = "DivideThePies"
+                    ufuns = generate_multi_issue_ufuns(
+                        n_issues=3,
+                        n_values=(9, 11),
+                        pareto_generators=tuple(GENERATOR_MAP.keys()),
+                        ufun_names=("First0", "Second1"),
+                        os_name=f"{name}{i}",
+                    )
                 else:
                     if n_pareto_selected < 2:
                         n_pareto_selected = 2
                     vals = generate_utility_values(
                         n_pareto=n_pareto_selected,
                         n_outcomes=n,
                         n_ufuns=n_ufuns,
@@ -417,45 +640,47 @@
                     )
                 break
             except:
                 continue
         else:
             continue
 
-        issues = (make_issue([f"{i}_{n-1 - i}" for i in range(n)], "portions"),)
-        ufuns = tuple(
-            U(
-                values=(
-                    TableFun(
-                        {_: float(vals[i][k]) for i, _ in enumerate(issues[0].all)}
+        if ufuns is None:
+            issues = (make_issue([f"{i}_{n-1 - i}" for i in range(n)], "portions"),)
+            ufuns = tuple(
+                U(
+                    values=(
+                        TableFun(
+                            {_: float(vals[i][k]) for i, _ in enumerate(issues[0].all)}  # type: ignore
+                        ),
                     ),
-                ),
-                name=f"{uname}{i}",
-                # reserved_value=(r[0] + random.random() * (r[1] - r[0] - 1e-8)),
-                outcome_space=make_os(issues, name=f"{name}{i}"),
+                    name=f"{uname}{i}",
+                    # reserved_value=(r[0] + random.random() * (r[1] - r[0] - 1e-8)),
+                    outcome_space=make_os(issues, name=f"{name}{i}"),
+                )
+                for k, uname in enumerate(("First", "Second"))
+                # for k, (uname, r) in enumerate(zip(("First", "Second"), reserved_ranges))
             )
-            for k, uname in enumerate(("First", "Second"))
-            # for k, (uname, r) in enumerate(zip(("First", "Second"), reserved_ranges))
-        )
         sample_reserved_values(ufuns, reserved_ranges=reserved_ranges)
         ufun_sets.append(ufuns)
 
     return [
         Scenario(
             outcome_space=ufuns[0].outcome_space,  # type: ignore We are sure this is not None
             ufuns=ufuns,
         )
         for ufuns in ufun_sets
     ]
 
 
-GENERAROR_MAP = dict(
+GENMAP = dict(
     monotonic=monotonic_pie_scenarios,
     arbitrary=arbitrary_pie_scenarios,
     zerosum=zerosum_pie_scenarios,
+    pies=monotonic_pies_scenarios,
     default=mixed_scenarios,
     mix=mixed_scenarios,
 )
 
 DEFAULT2024GENERATOR = mixed_scenarios
 """Default generator type for ANL 2024"""
 
@@ -532,15 +757,15 @@
 
     Returns:
         Tournament results as a `SimpleTournamentResults` object.
     """
     if generator_params is None:
         generator_params = dict()
     if isinstance(scenario_generator, str):
-        scenario_generator = GENERAROR_MAP[scenario_generator]
+        scenario_generator = GENMAP[scenario_generator]
     all_outcomes = not scenario_generator == zerosum_pie_scenarios
     if nologs:
         path = None
     elif base_path is not None:
         path = Path(base_path) / (name if name else unique_name("anl"))
     else:
         path = DEFAULT_TOURNAMENT_PATH / (name if name else unique_name("anl"))
```

### Comparing `anl-0.1.8/src/anl/cli.py` & `anl-0.1.9/src/anl/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,15 @@
 from negmas.helpers.types import get_class
 from negmas.inout import Scenario
 from negmas.plots.util import plot_offline_run
 from rich import print
 
 import anl
 from anl import DEFAULT_AN2024_COMPETITORS
-from anl.anl2024.runner import (
-    DEFAULT2024SETTINGS,
-    DEFAULT_TOURNAMENT_PATH,
-    GENERAROR_MAP,
-    anl2024_tournament,
-)
+from anl.anl2024.runner import DEFAULT2024SETTINGS, DEFAULT_TOURNAMENT_PATH, GENMAP, anl2024_tournament
 
 n_completed = 0
 n_total = 0
 
 
 def default_log_path():
     """Default location for all logs"""
@@ -315,15 +310,15 @@
     type=int,
     help="Number of negotiations after which to save stats",
 )
 @click.option(
     "--generator",
     default=DEFAULT2024SETTINGS["scenario_generator"],  # type: ignore
     type=str,
-    help="The method to generate scenarios. Default is mix which generates a mix of scenario types containing zero-sum, monotonic and general scenarios",
+    help="The method to generate scenarios. Default is mix which generates a mix of scenario types containing zero-sum, monotonic and general scenarios. Other possibilities are monotonic, pie, zerosom, arbitrary",
 )
 @click.option(
     "--zerosum",
     "-z",
     default=DEFAULT2024SETTINGS["generator_params"].get("zerosum_fraction", 0.05),  # type: ignore
     type=float,
     help="Fraction of zero-sum scenarios (used when generator=mix)",
@@ -334,15 +329,21 @@
     default=DEFAULT2024SETTINGS["generator_params"].get("monotonic_fraction", 0.25),  # type: ignore
     type=float,
     help="Fraction of monotonic scenarios (used when generator=mix)",
 )
 @click.option(
     "--curve",
     "-c",
-    default=DEFAULT2024SETTINGS["generator_params"].get("curve_fraction", 0.5),  # type: ignore
+    default=DEFAULT2024SETTINGS["generator_params"].get("curve_fraction", 0.25),  # type: ignore
+    type=float,
+    help="Fraction of monotonic and general scenarios generated using a Pareto curve not piecewise linear Pareto (used when generator=mix)",
+)
+@click.option(
+    "--pies",
+    default=DEFAULT2024SETTINGS["generator_params"].get("pies_fraction", 0.25),  # type: ignore
     type=float,
     help="Fraction of monotonic and general scenarios generated using a Pareto curve not piecewise linear Pareto (used when generator=mix)",
 )
 @click.option(
     "--rotate/--no-rotate",
     default=DEFAULT2024SETTINGS["rotate_ufuns"],  # type: ignore
     help="Rotate utility functions when creating scenarios for the tournament",
@@ -416,14 +417,15 @@
     max_outcomes,
     scenarios,
     small,
     settings_file,
     zerosum,
     monotonic,
     curve,
+    pies,
     two,
     scenarios_path,
 ):
     if two:
         competitorslst = competitors.split(";")
         scenarios = 1
         rotate = False
@@ -442,14 +444,15 @@
         generator_params = load(settings_file)
     # override settings with the appropriate ones based on the generator
     if generator == "mix":
         generator_params.update(
             zerosum_fraction=zerosum,
             monotonic_fraction=monotonic,
             curve_fraction=curve,
+            pies_fraction=pies,
         )
     if small:
         scenarios = min(scenarios, 2)
         steps = -1
         min_steps, max_steps = (10, 1000)
         outcomes = 100
         repetitions = 1
@@ -703,15 +706,15 @@
             monotonic_fraction=monotonic,
             curve_fraction=curve,
         )
 
     outcomes = read_range(outcomes, min_outcomes, max_outcomes)
 
     print(f"Will generate {scenarios} scenarios of {outcomes} outcomes each.")
-    scenario_generator = GENERAROR_MAP[generator]
+    scenario_generator = GENMAP[generator]
     scenarios = scenario_generator(
         n_scenarios=scenarios, n_outcomes=outcomes, **generator_params
     )
     path = Path(path)
     for s in scenarios:
         mypath = path / s.outcome_space.name  # type: ignore
         s.dumpas(mypath)  # type: ignore
```

### Comparing `anl-0.1.8/src/anl/visualizer/app.py` & `anl-0.1.9/src/anl/visualizer/app.py`

 * *Files identical despite different names*

### Comparing `anl-0.1.8/src/anl/visualizer/cli.py` & `anl-0.1.9/src/anl/visualizer/cli.py`

 * *Files identical despite different names*

### Comparing `anl-0.1.8/src/anl.egg-info/PKG-INFO` & `anl-0.1.9/src/anl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anl
-Version: 0.1.8
+Version: 0.1.9
 Summary: ANAC Automated Negotiations League Platform
 Home-page: https://github.com/autoneg/anl
 Author: Yasser Mohammad
 Author-email: yasserfarouk@gmail.com
 Project-URL: Documentation, https://anl.readthedocs.io/
 Project-URL: Changelog, https://anl.readthedocs.io/en/latest/changelog.html
 Project-URL: Issue Tracker, https://github.com/autoneg/anl/issues
@@ -57,14 +57,22 @@
 
 
 https://yasserfarouk.github.io/anl/
 
 Changelog
 =========
 
+0.1.9 (2024.02.14)
+------------------
+
+- Adding divide-the-pies scenarios
+- Adding workflow to test on negmas master
+- Tutorial and docs update
+- Update faq
+
 0.1.8 (2023.12.31)
 ------------------
 
 * bugfix in visualizer initial tournament list
 * Correcting auto pushing to PyPi
 
 0.1.7 (2023.12.31)
```

### Comparing `anl-0.1.8/src/anl.egg-info/SOURCES.txt` & `anl-0.1.9/src/anl.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 src/anl.egg-info/entry_points.txt
 src/anl.egg-info/not-zip-safe
 src/anl.egg-info/requires.txt
 src/anl.egg-info/top_level.txt
 src/anl/anl2024/__init__.py
 src/anl/anl2024/runner.py
 src/anl/anl2024/negotiators/__init__.py
+src/anl/anl2024/negotiators/builtins.py
 src/anl/anl2024/negotiators/builtins/__init__.py
 src/anl/anl2024/negotiators/builtins/micro.py
 src/anl/anl2024/negotiators/builtins/nash_seeker.py
 src/anl/anl2024/negotiators/builtins/rv_fitter.py
 src/anl/anl2024/negotiators/builtins/wrappers.py
 src/anl/visualizer/app.py
 src/anl/visualizer/cli.py
```

### Comparing `anl-0.1.8/tests/switches.py` & `anl-0.1.9/tests/switches.py`

 * *Files identical despite different names*

### Comparing `anl-0.1.8/tests/test_jupyter.py` & `anl-0.1.9/tests/test_jupyter.py`

 * *Files identical despite different names*

### Comparing `anl-0.1.8/tests/test_micro.py` & `anl-0.1.9/tests/test_micro.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from negmas import MappingUtilityFunction
 from negmas.inout import SAOMechanism
 from negmas.outcomes import make_issue, make_os
 from negmas.preferences.generators import make_zero_sum_pareto
-from negmas.tournaments.neg.simple import SimpleTournamentResults
 
 from anl.anl2024.negotiators.builtins import MiCRO
 from anl.anl2024.runner import anl2024_tournament
 
 
 def test_micro_agrees_with_itself():
     n_outcomes = 1000
```

### Comparing `anl-0.1.8/tests/tmp_notebooks/tutorials/01.develop_an_agent.ipynb` & `anl-0.1.9/tests/tmp_notebooks/tutorials/01.develop_an_agent.ipynb`

 * *Files identical despite different names*

### Comparing `anl-0.1.8/tox.ini` & `anl-0.1.9/tox.ini`

 * *Files identical despite different names*

