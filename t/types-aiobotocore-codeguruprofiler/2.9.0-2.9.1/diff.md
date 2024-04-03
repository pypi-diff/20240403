# Comparing `tmp/types-aiobotocore-codeguruprofiler-2.9.0.tar.gz` & `tmp/types-aiobotocore-codeguruprofiler-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codeguruprofiler-2.9.0.tar", last modified: Wed Dec 13 19:58:55 2023, max compression
+gzip compressed data, was "types-aiobotocore-codeguruprofiler-2.9.1.tar", last modified: Thu Jan 18 01:20:21 2024, max compression
```

## Comparing `types-aiobotocore-codeguruprofiler-2.9.0.tar` & `types-aiobotocore-codeguruprofiler-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:55.209927 types-aiobotocore-codeguruprofiler-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:42:56.000000 types-aiobotocore-codeguruprofiler-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13475 2023-12-13 19:58:55.209927 types-aiobotocore-codeguruprofiler-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11876 2023-12-13 19:42:56.000000 types-aiobotocore-codeguruprofiler-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:55.209927 types-aiobotocore-codeguruprofiler-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2023-12-13 19:42:56.000000 types-aiobotocore-codeguruprofiler-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:55.209927 types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2023-12-13 19:42:56.000000 types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2023-12-13 19:42:56.000000 types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      968 2023-12-13 19:42:56.000000 types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21387 2023-12-13 19:42:56.000000 types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    21383 2023-12-13 19:42:56.000000 types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9436 2023-12-13 19:42:56.000000 types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9434 2023-12-13 19:42:56.000000 types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2023-12-13 19:42:56.000000 types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2023-12-13 19:42:56.000000 types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:42:56.000000 types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    18738 2023-12-13 19:42:57.000000 types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18737 2023-12-13 19:42:56.000000 types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:42:56.000000 types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:55.209927 types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13475 2023-12-13 19:58:55.000000 types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      984 2023-12-13 19:58:55.000000 types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:55.000000 types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:55.000000 types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:55.000000 types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-13 19:58:55.000000 types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:21.501438 types-aiobotocore-codeguruprofiler-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:04:52.000000 types-aiobotocore-codeguruprofiler-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13495 2024-01-18 01:20:21.501438 types-aiobotocore-codeguruprofiler-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11876 2024-01-18 01:04:52.000000 types-aiobotocore-codeguruprofiler-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:21.501438 types-aiobotocore-codeguruprofiler-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-01-18 01:04:52.000000 types-aiobotocore-codeguruprofiler-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:21.497438 types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-01-18 01:04:52.000000 types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-01-18 01:04:52.000000 types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-01-18 01:04:52.000000 types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21396 2024-01-18 01:04:52.000000 types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21393 2024-01-18 01:04:52.000000 types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-01-18 01:04:53.000000 types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-01-18 01:04:52.000000 types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-01-18 01:04:52.000000 types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-01-18 01:04:52.000000 types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:04:52.000000 types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    18737 2024-01-18 01:04:53.000000 types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18737 2024-01-18 01:04:53.000000 types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:04:52.000000 types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:21.501438 types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13495 2024-01-18 01:20:21.000000 types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-18 01:20:21.000000 types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:21.000000 types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:21.000000 types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:21.000000 types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-18 01:20:21.000000 types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codeguruprofiler-2.9.0/LICENSE` & `types-aiobotocore-codeguruprofiler-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-codeguruprofiler-2.9.0/PKG-INFO` & `types-aiobotocore-codeguruprofiler-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codeguruprofiler
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CodeGuruProfiler 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CodeGuruProfiler 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/
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
 
 <a id="types-aiobotocore-codeguruprofiler"></a>
 
 # types-aiobotocore-codeguruprofiler
 
 [![PyPI - types-aiobotocore-codeguruprofiler](https://img.shields.io/pypi/v/types-aiobotocore-codeguruprofiler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguruprofiler)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeguruprofiler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguruprofiler)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codeguruprofiler)](https://pepy.tech/project/types-aiobotocore-codeguruprofiler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeGuruProfiler 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
+[aiobotocore.CodeGuruProfiler 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
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
 [types-aiobotocore-codeguruprofiler docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codeguruprofiler-2.9.0/README.md` & `types-aiobotocore-codeguruprofiler-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeguruprofiler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguruprofiler)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codeguruprofiler)](https://pepy.tech/project/types-aiobotocore-codeguruprofiler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeGuruProfiler 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
+[aiobotocore.CodeGuruProfiler 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
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
 [types-aiobotocore-codeguruprofiler docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codeguruprofiler-2.9.0/setup.py` & `types-aiobotocore-codeguruprofiler-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codeguruprofiler",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_codeguruprofiler"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CodeGuruProfiler 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.CodeGuruProfiler 2.9.1 service generated with"
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
     keywords="aiobotocore codeguruprofiler type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_codeguruprofiler": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler/__init__.py` & `types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,9 +22,8 @@
 """
 
 from .client import CodeGuruProfilerClient
 from .paginator import ListProfileTimesPaginator
 
 Client = CodeGuruProfilerClient
 
-
 __all__ = ("Client", "CodeGuruProfilerClient", "ListProfileTimesPaginator")
```

### Comparing `types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler/__init__.pyi` & `types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler/__main__.py` & `types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeGuruProfiler 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CodeGuruProfiler 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler\nOther"
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

### Comparing `types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler/client.py` & `types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CodeGuruProfilerClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -113,15 +112,15 @@
         self,
         *,
         profilingGroupName: str,
         endTime: TimestampTypeDef = ...,
         frameMetrics: Sequence[FrameMetricTypeDef] = ...,
         period: str = ...,
         startTime: TimestampTypeDef = ...,
-        targetResolution: AggregationPeriodType = ...
+        targetResolution: AggregationPeriodType = ...,
     ) -> BatchGetFrameMetricDataResponseTypeDef:
         """
         Returns the time series of values for a requested list of frame metrics from a
         time
         period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.batch_get_frame_metric_data)
@@ -145,15 +144,15 @@
         """
 
     async def configure_agent(
         self,
         *,
         profilingGroupName: str,
         fleetInstanceId: str = ...,
-        metadata: Mapping[MetadataFieldType, str] = ...
+        metadata: Mapping[MetadataFieldType, str] = ...,
     ) -> ConfigureAgentResponseTypeDef:
         """
         Used by profiler agents to report their current state and to receive remote
         configuration
         updates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.configure_agent)
@@ -163,15 +162,15 @@
     async def create_profiling_group(
         self,
         *,
         clientToken: str,
         profilingGroupName: str,
         agentOrchestrationConfig: AgentOrchestrationConfigTypeDef = ...,
         computePlatform: ComputePlatformType = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateProfilingGroupResponseTypeDef:
         """
         Creates a profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.create_profiling_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/client/#create_profiling_group)
         """
@@ -246,30 +245,30 @@
         self,
         *,
         profilingGroupName: str,
         accept: str = ...,
         endTime: TimestampTypeDef = ...,
         maxDepth: int = ...,
         period: str = ...,
-        startTime: TimestampTypeDef = ...
+        startTime: TimestampTypeDef = ...,
     ) -> GetProfileResponseTypeDef:
         """
         Gets the aggregated profile of a profiling group for a specified time range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.get_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/client/#get_profile)
         """
 
     async def get_recommendations(
         self,
         *,
         endTime: TimestampTypeDef,
         profilingGroupName: str,
         startTime: TimestampTypeDef,
-        locale: str = ...
+        locale: str = ...,
     ) -> GetRecommendationsResponseTypeDef:
         """
         Returns a list of
         [Recommendation](https://docs.aws.amazon.com/codeguru/latest/profiler-api/API_Recommendation.html)
         objects that contain recommendations for a profiling group for a given time
         period.
 
@@ -281,15 +280,15 @@
         self,
         *,
         endTime: TimestampTypeDef,
         profilingGroupName: str,
         startTime: TimestampTypeDef,
         dailyReportsOnly: bool = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListFindingsReportsResponseTypeDef:
         """
         List the available reports for a given profiling group and time range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.list_findings_reports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/client/#list_findings_reports)
         """
@@ -299,15 +298,15 @@
         *,
         endTime: TimestampTypeDef,
         period: AggregationPeriodType,
         profilingGroupName: str,
         startTime: TimestampTypeDef,
         maxResults: int = ...,
         nextToken: str = ...,
-        orderBy: OrderByType = ...
+        orderBy: OrderByType = ...,
     ) -> ListProfileTimesResponseTypeDef:
         """
         Lists the start times of the available aggregated profiles of a profiling group
         for an aggregation period within the specified time
         range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.list_profile_times)
@@ -336,30 +335,30 @@
 
     async def post_agent_profile(
         self,
         *,
         agentProfile: BlobTypeDef,
         contentType: str,
         profilingGroupName: str,
-        profileToken: str = ...
+        profileToken: str = ...,
     ) -> Dict[str, Any]:
         """
         Submits profiling data to an aggregated profile of a profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.post_agent_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/client/#post_agent_profile)
         """
 
     async def put_permission(
         self,
         *,
         actionGroup: Literal["agentPermissions"],
         principals: Sequence[str],
         profilingGroupName: str,
-        revisionId: str = ...
+        revisionId: str = ...,
     ) -> PutPermissionResponseTypeDef:
         """
         Adds permissions to a profiling group's resource-based policy that are provided
         using an action
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.put_permission)
@@ -390,15 +389,15 @@
 
     async def submit_feedback(
         self,
         *,
         anomalyInstanceId: str,
         profilingGroupName: str,
         type: FeedbackTypeType,
-        comment: str = ...
+        comment: str = ...,
     ) -> Dict[str, Any]:
         """
         Sends feedback to CodeGuru Profiler about whether the anomaly detected by the
         analysis is useful or
         not.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.submit_feedback)
```

### Comparing `types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler/client.pyi` & `types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         self,
         *,
         profilingGroupName: str,
         endTime: TimestampTypeDef = ...,
         frameMetrics: Sequence[FrameMetricTypeDef] = ...,
         period: str = ...,
         startTime: TimestampTypeDef = ...,
-        targetResolution: AggregationPeriodType = ...
+        targetResolution: AggregationPeriodType = ...,
     ) -> BatchGetFrameMetricDataResponseTypeDef:
         """
         Returns the time series of values for a requested list of frame metrics from a
         time
         period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.batch_get_frame_metric_data)
@@ -141,15 +141,15 @@
         """
 
     async def configure_agent(
         self,
         *,
         profilingGroupName: str,
         fleetInstanceId: str = ...,
-        metadata: Mapping[MetadataFieldType, str] = ...
+        metadata: Mapping[MetadataFieldType, str] = ...,
     ) -> ConfigureAgentResponseTypeDef:
         """
         Used by profiler agents to report their current state and to receive remote
         configuration
         updates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.configure_agent)
@@ -159,15 +159,15 @@
     async def create_profiling_group(
         self,
         *,
         clientToken: str,
         profilingGroupName: str,
         agentOrchestrationConfig: AgentOrchestrationConfigTypeDef = ...,
         computePlatform: ComputePlatformType = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateProfilingGroupResponseTypeDef:
         """
         Creates a profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.create_profiling_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/client/#create_profiling_group)
         """
@@ -242,30 +242,30 @@
         self,
         *,
         profilingGroupName: str,
         accept: str = ...,
         endTime: TimestampTypeDef = ...,
         maxDepth: int = ...,
         period: str = ...,
-        startTime: TimestampTypeDef = ...
+        startTime: TimestampTypeDef = ...,
     ) -> GetProfileResponseTypeDef:
         """
         Gets the aggregated profile of a profiling group for a specified time range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.get_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/client/#get_profile)
         """
 
     async def get_recommendations(
         self,
         *,
         endTime: TimestampTypeDef,
         profilingGroupName: str,
         startTime: TimestampTypeDef,
-        locale: str = ...
+        locale: str = ...,
     ) -> GetRecommendationsResponseTypeDef:
         """
         Returns a list of
         [Recommendation](https://docs.aws.amazon.com/codeguru/latest/profiler-api/API_Recommendation.html)
         objects that contain recommendations for a profiling group for a given time
         period.
 
@@ -277,15 +277,15 @@
         self,
         *,
         endTime: TimestampTypeDef,
         profilingGroupName: str,
         startTime: TimestampTypeDef,
         dailyReportsOnly: bool = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListFindingsReportsResponseTypeDef:
         """
         List the available reports for a given profiling group and time range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.list_findings_reports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/client/#list_findings_reports)
         """
@@ -295,15 +295,15 @@
         *,
         endTime: TimestampTypeDef,
         period: AggregationPeriodType,
         profilingGroupName: str,
         startTime: TimestampTypeDef,
         maxResults: int = ...,
         nextToken: str = ...,
-        orderBy: OrderByType = ...
+        orderBy: OrderByType = ...,
     ) -> ListProfileTimesResponseTypeDef:
         """
         Lists the start times of the available aggregated profiles of a profiling group
         for an aggregation period within the specified time
         range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.list_profile_times)
@@ -332,30 +332,30 @@
 
     async def post_agent_profile(
         self,
         *,
         agentProfile: BlobTypeDef,
         contentType: str,
         profilingGroupName: str,
-        profileToken: str = ...
+        profileToken: str = ...,
     ) -> Dict[str, Any]:
         """
         Submits profiling data to an aggregated profile of a profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.post_agent_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/client/#post_agent_profile)
         """
 
     async def put_permission(
         self,
         *,
         actionGroup: Literal["agentPermissions"],
         principals: Sequence[str],
         profilingGroupName: str,
-        revisionId: str = ...
+        revisionId: str = ...,
     ) -> PutPermissionResponseTypeDef:
         """
         Adds permissions to a profiling group's resource-based policy that are provided
         using an action
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.put_permission)
@@ -386,15 +386,15 @@
 
     async def submit_feedback(
         self,
         *,
         anomalyInstanceId: str,
         profilingGroupName: str,
         type: FeedbackTypeType,
-        comment: str = ...
+        comment: str = ...,
     ) -> Dict[str, Any]:
         """
         Sends feedback to CodeGuru Profiler about whether the anomaly detected by the
         analysis is useful or
         not.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.submit_feedback)
```

### Comparing `types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler/literals.py` & `types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ActionGroupType",
     "AgentParameterFieldType",
     "AggregationPeriodType",
     "ComputePlatformType",
     "EventPublisherType",
     "FeedbackTypeType",
@@ -33,15 +32,14 @@
     "OrderByType",
     "CodeGuruProfilerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 ActionGroupType = Literal["agentPermissions"]
 AgentParameterFieldType = Literal[
     "MaxStackDepth",
     "MemoryUsageLimitPercent",
     "MinimumTimeForReportingInMilliseconds",
     "ReportingIntervalInMilliseconds",
     "SamplingIntervalInMilliseconds",
```

### Comparing `types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler/literals.pyi` & `types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler/paginator.py` & `types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -27,38 +27,35 @@
 from botocore.paginate import PageIterator
 
 from .literals import AggregationPeriodType, OrderByType
 from .type_defs import ListProfileTimesResponseTypeDef, PaginatorConfigTypeDef, TimestampTypeDef
 
 __all__ = ("ListProfileTimesPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListProfileTimesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Paginator.ListProfileTimes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/paginators/#listprofiletimespaginator)
     """
 
     def paginate(
         self,
         *,
         endTime: TimestampTypeDef,
         period: AggregationPeriodType,
         profilingGroupName: str,
         startTime: TimestampTypeDef,
         orderBy: OrderByType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListProfileTimesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Paginator.ListProfileTimes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/paginators/#listprofiletimespaginator)
         """
```

### Comparing `types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler/paginator.pyi` & `types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,33 +29,35 @@
 from .literals import AggregationPeriodType, OrderByType
 from .type_defs import ListProfileTimesResponseTypeDef, PaginatorConfigTypeDef, TimestampTypeDef
 
 __all__ = ("ListProfileTimesPaginator",)
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListProfileTimesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Paginator.ListProfileTimes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/paginators/#listprofiletimespaginator)
     """
 
     def paginate(
         self,
         *,
         endTime: TimestampTypeDef,
         period: AggregationPeriodType,
         profilingGroupName: str,
         startTime: TimestampTypeDef,
         orderBy: OrderByType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListProfileTimesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Paginator.ListProfileTimes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/paginators/#listprofiletimespaginator)
         """
```

### Comparing `types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler/type_defs.py` & `types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ChannelTypeDef",
     "ResponseMetadataTypeDef",
     "AgentConfigurationTypeDef",
     "AgentOrchestrationConfigTypeDef",
     "AggregatedProfileTimeTypeDef",
     "UserFeedbackTypeDef",
```

### Comparing `types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler/type_defs.pyi` & `types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler.egg-info/PKG-INFO` & `types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codeguruprofiler
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CodeGuruProfiler 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CodeGuruProfiler 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/
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
 
 <a id="types-aiobotocore-codeguruprofiler"></a>
 
 # types-aiobotocore-codeguruprofiler
 
 [![PyPI - types-aiobotocore-codeguruprofiler](https://img.shields.io/pypi/v/types-aiobotocore-codeguruprofiler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguruprofiler)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeguruprofiler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguruprofiler)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codeguruprofiler)](https://pepy.tech/project/types-aiobotocore-codeguruprofiler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeGuruProfiler 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
+[aiobotocore.CodeGuruProfiler 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
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
 [types-aiobotocore-codeguruprofiler docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codeguruprofiler-2.9.0/types_aiobotocore_codeguruprofiler.egg-info/SOURCES.txt` & `types-aiobotocore-codeguruprofiler-2.9.1/types_aiobotocore_codeguruprofiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

