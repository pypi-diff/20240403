# Comparing `tmp/types-aiobotocore-amp-2.9.0.tar.gz` & `tmp/types-aiobotocore-amp-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-amp-2.9.0.tar", last modified: Wed Dec 13 19:58:30 2023, max compression
+gzip compressed data, was "types-aiobotocore-amp-2.9.1.tar", last modified: Thu Jan 18 01:19:58 2024, max compression
```

## Comparing `types-aiobotocore-amp-2.9.0.tar` & `types-aiobotocore-amp-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:30.506130 types-aiobotocore-amp-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:40:41.000000 types-aiobotocore-amp-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14279 2023-12-13 19:58:30.506130 types-aiobotocore-amp-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12718 2023-12-13 19:40:41.000000 types-aiobotocore-amp-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:30.506130 types-aiobotocore-amp-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2023-12-13 19:40:41.000000 types-aiobotocore-amp-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:30.506130 types-aiobotocore-amp-2.9.0/types_aiobotocore_amp/
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2023-12-13 19:40:41.000000 types-aiobotocore-amp-2.9.0/types_aiobotocore_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2023-12-13 19:40:41.000000 types-aiobotocore-amp-2.9.0/types_aiobotocore_amp/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      933 2023-12-13 19:40:41.000000 types-aiobotocore-amp-2.9.0/types_aiobotocore_amp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22803 2023-12-13 19:40:41.000000 types-aiobotocore-amp-2.9.0/types_aiobotocore_amp/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    22799 2023-12-13 19:40:41.000000 types-aiobotocore-amp-2.9.0/types_aiobotocore_amp/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10109 2023-12-13 19:40:41.000000 types-aiobotocore-amp-2.9.0/types_aiobotocore_amp/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10107 2023-12-13 19:40:41.000000 types-aiobotocore-amp-2.9.0/types_aiobotocore_amp/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2023-12-13 19:40:41.000000 types-aiobotocore-amp-2.9.0/types_aiobotocore_amp/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2023-12-13 19:40:41.000000 types-aiobotocore-amp-2.9.0/types_aiobotocore_amp/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:40:41.000000 types-aiobotocore-amp-2.9.0/types_aiobotocore_amp/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    22027 2023-12-13 19:40:41.000000 types-aiobotocore-amp-2.9.0/types_aiobotocore_amp/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22026 2023-12-13 19:40:41.000000 types-aiobotocore-amp-2.9.0/types_aiobotocore_amp/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:40:41.000000 types-aiobotocore-amp-2.9.0/types_aiobotocore_amp/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2023-12-13 19:40:41.000000 types-aiobotocore-amp-2.9.0/types_aiobotocore_amp/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4373 2023-12-13 19:40:41.000000 types-aiobotocore-amp-2.9.0/types_aiobotocore_amp/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:30.506130 types-aiobotocore-amp-2.9.0/types_aiobotocore_amp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14279 2023-12-13 19:58:30.000000 types-aiobotocore-amp-2.9.0/types_aiobotocore_amp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      802 2023-12-13 19:58:30.000000 types-aiobotocore-amp-2.9.0/types_aiobotocore_amp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:30.000000 types-aiobotocore-amp-2.9.0/types_aiobotocore_amp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:30.000000 types-aiobotocore-amp-2.9.0/types_aiobotocore_amp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:30.000000 types-aiobotocore-amp-2.9.0/types_aiobotocore_amp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 19:58:30.000000 types-aiobotocore-amp-2.9.0/types_aiobotocore_amp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:58.965534 types-aiobotocore-amp-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:02:40.000000 types-aiobotocore-amp-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14299 2024-01-18 01:19:58.965534 types-aiobotocore-amp-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12718 2024-01-18 01:02:40.000000 types-aiobotocore-amp-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:19:58.965534 types-aiobotocore-amp-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-01-18 01:02:40.000000 types-aiobotocore-amp-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:58.961534 types-aiobotocore-amp-2.9.1/types_aiobotocore_amp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-01-18 01:02:40.000000 types-aiobotocore-amp-2.9.1/types_aiobotocore_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-01-18 01:02:40.000000 types-aiobotocore-amp-2.9.1/types_aiobotocore_amp/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-01-18 01:02:40.000000 types-aiobotocore-amp-2.9.1/types_aiobotocore_amp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22805 2024-01-18 01:02:40.000000 types-aiobotocore-amp-2.9.1/types_aiobotocore_amp/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22802 2024-01-18 01:02:40.000000 types-aiobotocore-amp-2.9.1/types_aiobotocore_amp/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10107 2024-01-18 01:02:41.000000 types-aiobotocore-amp-2.9.1/types_aiobotocore_amp/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10107 2024-01-18 01:02:41.000000 types-aiobotocore-amp-2.9.1/types_aiobotocore_amp/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-01-18 01:02:40.000000 types-aiobotocore-amp-2.9.1/types_aiobotocore_amp/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-01-18 01:02:40.000000 types-aiobotocore-amp-2.9.1/types_aiobotocore_amp/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:02:40.000000 types-aiobotocore-amp-2.9.1/types_aiobotocore_amp/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    22026 2024-01-18 01:02:41.000000 types-aiobotocore-amp-2.9.1/types_aiobotocore_amp/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22026 2024-01-18 01:02:41.000000 types-aiobotocore-amp-2.9.1/types_aiobotocore_amp/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:02:40.000000 types-aiobotocore-amp-2.9.1/types_aiobotocore_amp/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-01-18 01:02:40.000000 types-aiobotocore-amp-2.9.1/types_aiobotocore_amp/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-01-18 01:02:40.000000 types-aiobotocore-amp-2.9.1/types_aiobotocore_amp/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:58.965534 types-aiobotocore-amp-2.9.1/types_aiobotocore_amp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14299 2024-01-18 01:19:58.000000 types-aiobotocore-amp-2.9.1/types_aiobotocore_amp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-01-18 01:19:58.000000 types-aiobotocore-amp-2.9.1/types_aiobotocore_amp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:19:58.000000 types-aiobotocore-amp-2.9.1/types_aiobotocore_amp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:19:58.000000 types-aiobotocore-amp-2.9.1/types_aiobotocore_amp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:19:58.000000 types-aiobotocore-amp-2.9.1/types_aiobotocore_amp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:19:58.000000 types-aiobotocore-amp-2.9.1/types_aiobotocore_amp.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-amp-2.9.0/LICENSE` & `types-aiobotocore-amp-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-amp-2.9.0/PKG-INFO` & `types-aiobotocore-amp-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-amp
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.PrometheusService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.PrometheusService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/
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
 
 <a id="types-aiobotocore-amp"></a>
 
 # types-aiobotocore-amp
 
 [![PyPI - types-aiobotocore-amp](https://img.shields.io/pypi/v/types-aiobotocore-amp.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amp)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-amp.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amp)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-amp)](https://pepy.tech/project/types-aiobotocore-amp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PrometheusService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
+[aiobotocore.PrometheusService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
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
 [types-aiobotocore-amp docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-amp-2.9.0/README.md` & `types-aiobotocore-amp-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-amp.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amp)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-amp)](https://pepy.tech/project/types-aiobotocore-amp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PrometheusService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
+[aiobotocore.PrometheusService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
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
 [types-aiobotocore-amp docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-amp-2.9.0/setup.py` & `types-aiobotocore-amp-2.9.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-amp",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_amp"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.PrometheusService 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.PrometheusService 2.9.1 service generated with"
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
     keywords="aiobotocore amp type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_amp": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-amp-2.9.0/types_aiobotocore_amp/__init__.py` & `types-aiobotocore-amp-2.9.1/types_aiobotocore_amp/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     ScraperDeletedWaiter,
     WorkspaceActiveWaiter,
     WorkspaceDeletedWaiter,
 )
 
 Client = PrometheusServiceClient
 
-
 __all__ = (
     "Client",
     "ListRuleGroupsNamespacesPaginator",
     "ListScrapersPaginator",
     "ListWorkspacesPaginator",
     "PrometheusServiceClient",
     "ScraperActiveWaiter",
```

### Comparing `types-aiobotocore-amp-2.9.0/types_aiobotocore_amp/__init__.pyi` & `types-aiobotocore-amp-2.9.1/types_aiobotocore_amp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.9.0/types_aiobotocore_amp/__main__.py` & `types-aiobotocore-amp-2.9.1/types_aiobotocore_amp/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.PrometheusService 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.PrometheusService 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService\nOther"
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

### Comparing `types-aiobotocore-amp-2.9.0/types_aiobotocore_amp/client.py` & `types-aiobotocore-amp-2.9.1/types_aiobotocore_amp/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("PrometheusServiceClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -143,15 +142,15 @@
     async def create_rule_groups_namespace(
         self,
         *,
         workspaceId: str,
         name: str,
         data: BlobTypeDef,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateRuleGroupsNamespaceResponseTypeDef:
         """
         Create a rule group namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.create_rule_groups_namespace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#create_rule_groups_namespace)
         """
@@ -160,15 +159,15 @@
         self,
         *,
         scrapeConfiguration: ScrapeConfigurationTypeDef,
         source: SourceTypeDef,
         destination: DestinationTypeDef,
         alias: str = ...,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateScraperResponseTypeDef:
         """
         Create a scraper.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.create_scraper)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#create_scraper)
         """
@@ -314,15 +313,15 @@
         """
 
     async def list_scrapers(
         self,
         *,
         filters: Mapping[str, Sequence[str]] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListScrapersResponseTypeDef:
         """
         Lists all scrapers in a customer account, including scrapers being created or
         deleted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.list_scrapers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#list_scrapers)
```

### Comparing `types-aiobotocore-amp-2.9.0/types_aiobotocore_amp/client.pyi` & `types-aiobotocore-amp-2.9.1/types_aiobotocore_amp/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
     async def create_rule_groups_namespace(
         self,
         *,
         workspaceId: str,
         name: str,
         data: BlobTypeDef,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateRuleGroupsNamespaceResponseTypeDef:
         """
         Create a rule group namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.create_rule_groups_namespace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#create_rule_groups_namespace)
         """
@@ -156,15 +156,15 @@
         self,
         *,
         scrapeConfiguration: ScrapeConfigurationTypeDef,
         source: SourceTypeDef,
         destination: DestinationTypeDef,
         alias: str = ...,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateScraperResponseTypeDef:
         """
         Create a scraper.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.create_scraper)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#create_scraper)
         """
@@ -310,15 +310,15 @@
         """
 
     async def list_scrapers(
         self,
         *,
         filters: Mapping[str, Sequence[str]] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListScrapersResponseTypeDef:
         """
         Lists all scrapers in a customer account, including scrapers being created or
         deleted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.list_scrapers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#list_scrapers)
```

### Comparing `types-aiobotocore-amp-2.9.0/types_aiobotocore_amp/literals.py` & `types-aiobotocore-amp-2.9.1/types_aiobotocore_amp/literals.py`

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
     "AlertManagerDefinitionStatusCodeType",
     "ListRuleGroupsNamespacesPaginatorName",
     "ListScrapersPaginatorName",
     "ListWorkspacesPaginatorName",
     "LoggingConfigurationStatusCodeType",
     "RuleGroupsNamespaceStatusCodeType",
@@ -37,15 +36,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AlertManagerDefinitionStatusCodeType = Literal[
     "ACTIVE", "CREATING", "CREATION_FAILED", "DELETING", "UPDATE_FAILED", "UPDATING"
 ]
 ListRuleGroupsNamespacesPaginatorName = Literal["list_rule_groups_namespaces"]
 ListScrapersPaginatorName = Literal["list_scrapers"]
 ListWorkspacesPaginatorName = Literal["list_workspaces"]
 LoggingConfigurationStatusCodeType = Literal[
```

### Comparing `types-aiobotocore-amp-2.9.0/types_aiobotocore_amp/literals.pyi` & `types-aiobotocore-amp-2.9.1/types_aiobotocore_amp/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.9.0/types_aiobotocore_amp/paginator.py` & `types-aiobotocore-amp-2.9.1/types_aiobotocore_amp/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     ListScrapersResponsePaginatorTypeDef,
     ListWorkspacesResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListRuleGroupsNamespacesPaginator", "ListScrapersPaginator", "ListWorkspacesPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -71,15 +70,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/paginators/#listscraperspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Mapping[str, Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListScrapersResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Paginator.ListScrapers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/paginators/#listscraperspaginator)
         """
```

### Comparing `types-aiobotocore-amp-2.9.0/types_aiobotocore_amp/paginator.pyi` & `types-aiobotocore-amp-2.9.1/types_aiobotocore_amp/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/paginators/#listscraperspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Mapping[str, Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListScrapersResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Paginator.ListScrapers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/paginators/#listscraperspaginator)
         """
 
 class ListWorkspacesPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-amp-2.9.0/types_aiobotocore_amp/type_defs.py` & `types-aiobotocore-amp-2.9.1/types_aiobotocore_amp/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AlertManagerDefinitionStatusTypeDef",
     "AmpConfigurationTypeDef",
     "BlobTypeDef",
     "ResponseMetadataTypeDef",
     "CreateLoggingConfigurationRequestRequestTypeDef",
     "LoggingConfigurationStatusTypeDef",
```

### Comparing `types-aiobotocore-amp-2.9.0/types_aiobotocore_amp/type_defs.pyi` & `types-aiobotocore-amp-2.9.1/types_aiobotocore_amp/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.9.0/types_aiobotocore_amp/waiter.py` & `types-aiobotocore-amp-2.9.1/types_aiobotocore_amp/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.9.0/types_aiobotocore_amp/waiter.pyi` & `types-aiobotocore-amp-2.9.1/types_aiobotocore_amp/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.9.0/types_aiobotocore_amp.egg-info/PKG-INFO` & `types-aiobotocore-amp-2.9.1/types_aiobotocore_amp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-amp
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.PrometheusService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.PrometheusService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/
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
 
 <a id="types-aiobotocore-amp"></a>
 
 # types-aiobotocore-amp
 
 [![PyPI - types-aiobotocore-amp](https://img.shields.io/pypi/v/types-aiobotocore-amp.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amp)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-amp.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amp)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-amp)](https://pepy.tech/project/types-aiobotocore-amp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PrometheusService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
+[aiobotocore.PrometheusService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
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
 [types-aiobotocore-amp docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-amp-2.9.0/types_aiobotocore_amp.egg-info/SOURCES.txt` & `types-aiobotocore-amp-2.9.1/types_aiobotocore_amp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

