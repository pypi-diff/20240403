# Comparing `tmp/types-aiobotocore-applicationcostprofiler-2.9.0.tar.gz` & `tmp/types-aiobotocore-applicationcostprofiler-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-applicationcostprofiler-2.9.0.tar", last modified: Wed Dec 13 19:58:35 2023, max compression
+gzip compressed data, was "types-aiobotocore-applicationcostprofiler-2.9.1.tar", last modified: Thu Jan 18 01:20:03 2024, max compression
```

## Comparing `types-aiobotocore-applicationcostprofiler-2.9.0.tar` & `types-aiobotocore-applicationcostprofiler-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:35.714086 types-aiobotocore-applicationcostprofiler-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:41:07.000000 types-aiobotocore-applicationcostprofiler-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13965 2023-12-13 19:58:35.714086 types-aiobotocore-applicationcostprofiler-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12338 2023-12-13 19:41:07.000000 types-aiobotocore-applicationcostprofiler-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:35.714086 types-aiobotocore-applicationcostprofiler-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2023-12-13 19:41:07.000000 types-aiobotocore-applicationcostprofiler-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:35.714086 types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler/
--rw-r--r--   0 runner    (1001) docker     (127)      820 2023-12-13 19:41:07.000000 types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2023-12-13 19:41:07.000000 types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      996 2023-12-13 19:41:07.000000 types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9515 2023-12-13 19:41:07.000000 types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9511 2023-12-13 19:41:07.000000 types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8601 2023-12-13 19:41:07.000000 types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8599 2023-12-13 19:41:07.000000 types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2023-12-13 19:41:07.000000 types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2023-12-13 19:41:07.000000 types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:41:07.000000 types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2023-12-13 19:41:07.000000 types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2023-12-13 19:41:07.000000 types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:41:07.000000 types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:35.714086 types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13965 2023-12-13 19:58:35.000000 types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2023-12-13 19:58:35.000000 types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:35.000000 types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:35.000000 types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:35.000000 types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-13 19:58:35.000000 types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:03.725511 types-aiobotocore-applicationcostprofiler-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:03:06.000000 types-aiobotocore-applicationcostprofiler-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13985 2024-01-18 01:20:03.725511 types-aiobotocore-applicationcostprofiler-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12338 2024-01-18 01:03:06.000000 types-aiobotocore-applicationcostprofiler-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:03.725511 types-aiobotocore-applicationcostprofiler-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-01-18 01:03:06.000000 types-aiobotocore-applicationcostprofiler-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:03.721511 types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-01-18 01:03:06.000000 types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-01-18 01:03:06.000000 types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-01-18 01:03:06.000000 types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-01-18 01:03:06.000000 types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-01-18 01:03:06.000000 types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8599 2024-01-18 01:03:06.000000 types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8599 2024-01-18 01:03:06.000000 types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-01-18 01:03:06.000000 types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-01-18 01:03:06.000000 types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:03:06.000000 types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-01-18 01:03:07.000000 types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-01-18 01:03:06.000000 types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:03:06.000000 types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:03.725511 types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13985 2024-01-18 01:20:03.000000 types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-01-18 01:20:03.000000 types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:03.000000 types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:03.000000 types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:03.000000 types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-18 01:20:03.000000 types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-applicationcostprofiler-2.9.0/LICENSE` & `types-aiobotocore-applicationcostprofiler-2.9.1/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2024 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `types-aiobotocore-applicationcostprofiler-2.9.0/PKG-INFO` & `types-aiobotocore-applicationcostprofiler-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-applicationcostprofiler
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ApplicationCostProfiler 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ApplicationCostProfiler 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="types-aiobotocore-applicationcostprofiler"></a>
 
 # types-aiobotocore-applicationcostprofiler
 
 [![PyPI - types-aiobotocore-applicationcostprofiler](https://img.shields.io/pypi/v/types-aiobotocore-applicationcostprofiler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-applicationcostprofiler)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-applicationcostprofiler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-applicationcostprofiler)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-applicationcostprofiler)](https://pepy.tech/project/types-aiobotocore-applicationcostprofiler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ApplicationCostProfiler 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler)
+[aiobotocore.ApplicationCostProfiler 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-applicationcostprofiler docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-applicationcostprofiler-2.9.0/README.md` & `types-aiobotocore-applicationcostprofiler-2.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-applicationcostprofiler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-applicationcostprofiler)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-applicationcostprofiler)](https://pepy.tech/project/types-aiobotocore-applicationcostprofiler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ApplicationCostProfiler 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler)
+[aiobotocore.ApplicationCostProfiler 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-applicationcostprofiler docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-applicationcostprofiler-2.9.0/setup.py` & `types-aiobotocore-applicationcostprofiler-2.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,50 +7,49 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-applicationcostprofiler",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_applicationcostprofiler"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ApplicationCostProfiler 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ApplicationCostProfiler 2.9.1 service generated with"
+        " mypy-boto3-builder 7.23.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
-        "Typing :: Typed",
+        "Typing :: Stubs Only",
     ],
     keywords=(
         "aiobotocore applicationcostprofiler type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_applicationcostprofiler": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler/__init__.py` & `types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,9 +22,8 @@
 """
 
 from .client import ApplicationCostProfilerClient
 from .paginator import ListReportDefinitionsPaginator
 
 Client = ApplicationCostProfilerClient
 
-
 __all__ = ("ApplicationCostProfilerClient", "Client", "ListReportDefinitionsPaginator")
```

### Comparing `types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler/__init__.pyi` & `types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler/__main__.py` & `types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ApplicationCostProfiler 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ApplicationCostProfiler 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.9.0")
+    print("2.9.1")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler/client.py` & `types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler/client.pyi`

 * *Files identical despite different names*

```diff
@@ -35,35 +35,31 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ApplicationCostProfilerClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class ApplicationCostProfilerClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/client/)
     """
 
     meta: ClientMeta
@@ -149,15 +145,15 @@
     async def put_report_definition(
         self,
         *,
         reportId: str,
         reportDescription: str,
         reportFrequency: ReportFrequencyType,
         format: FormatType,
-        destinationS3Location: S3LocationTypeDef
+        destinationS3Location: S3LocationTypeDef,
     ) -> PutReportDefinitionResultTypeDef:
         """
         Creates the report definition for a report in Application Cost Profiler.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Client.put_report_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/client/#put_report_definition)
         """
@@ -165,15 +161,15 @@
     async def update_report_definition(
         self,
         *,
         reportId: str,
         reportDescription: str,
         reportFrequency: ReportFrequencyType,
         format: FormatType,
-        destinationS3Location: S3LocationTypeDef
+        destinationS3Location: S3LocationTypeDef,
     ) -> UpdateReportDefinitionResultTypeDef:
         """
         Updates existing report in AWS Application Cost Profiler.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Client.update_report_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/client/#update_report_definition)
         """
```

### Comparing `types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler/client.pyi` & `types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,29 +37,32 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("ApplicationCostProfilerClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class ApplicationCostProfilerClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/client/)
     """
 
     meta: ClientMeta
@@ -145,15 +148,15 @@
     async def put_report_definition(
         self,
         *,
         reportId: str,
         reportDescription: str,
         reportFrequency: ReportFrequencyType,
         format: FormatType,
-        destinationS3Location: S3LocationTypeDef
+        destinationS3Location: S3LocationTypeDef,
     ) -> PutReportDefinitionResultTypeDef:
         """
         Creates the report definition for a report in Application Cost Profiler.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Client.put_report_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/client/#put_report_definition)
         """
@@ -161,15 +164,15 @@
     async def update_report_definition(
         self,
         *,
         reportId: str,
         reportDescription: str,
         reportFrequency: ReportFrequencyType,
         format: FormatType,
-        destinationS3Location: S3LocationTypeDef
+        destinationS3Location: S3LocationTypeDef,
     ) -> UpdateReportDefinitionResultTypeDef:
         """
         Updates existing report in AWS Application Cost Profiler.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Client.update_report_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/client/#update_report_definition)
         """
```

### Comparing `types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler/literals.py` & `types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,27 +15,25 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "FormatType",
     "ListReportDefinitionsPaginatorName",
     "ReportFrequencyType",
     "S3BucketRegionType",
     "ApplicationCostProfilerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 FormatType = Literal["CSV", "PARQUET"]
 ListReportDefinitionsPaginatorName = Literal["list_report_definitions"]
 ReportFrequencyType = Literal["ALL", "DAILY", "MONTHLY"]
 S3BucketRegionType = Literal["af-south-1", "ap-east-1", "eu-south-1", "me-south-1"]
 ApplicationCostProfilerServiceName = Literal["applicationcostprofiler"]
 ServiceName = Literal[
     "accessanalyzer",
```

### Comparing `types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler/literals.pyi` & `types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler/paginator.py` & `types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import ListReportDefinitionsResultTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListReportDefinitionsPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler/paginator.pyi` & `types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler/type_defs.py` & `types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "DeleteReportDefinitionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "GetReportDefinitionRequestRequestTypeDef",
     "S3LocationTypeDef",
     "SourceS3LocationTypeDef",
     "PaginatorConfigTypeDef",
```

### Comparing `types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler/type_defs.pyi` & `types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler.egg-info/PKG-INFO` & `types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-applicationcostprofiler
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ApplicationCostProfiler 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ApplicationCostProfiler 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="types-aiobotocore-applicationcostprofiler"></a>
 
 # types-aiobotocore-applicationcostprofiler
 
 [![PyPI - types-aiobotocore-applicationcostprofiler](https://img.shields.io/pypi/v/types-aiobotocore-applicationcostprofiler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-applicationcostprofiler)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-applicationcostprofiler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-applicationcostprofiler)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-applicationcostprofiler)](https://pepy.tech/project/types-aiobotocore-applicationcostprofiler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ApplicationCostProfiler 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler)
+[aiobotocore.ApplicationCostProfiler 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-applicationcostprofiler docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-applicationcostprofiler-2.9.0/types_aiobotocore_applicationcostprofiler.egg-info/SOURCES.txt` & `types-aiobotocore-applicationcostprofiler-2.9.1/types_aiobotocore_applicationcostprofiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

