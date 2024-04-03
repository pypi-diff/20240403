# Comparing `tmp/types-aiobotocore-swf-2.9.0.tar.gz` & `tmp/types-aiobotocore-swf-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-swf-2.9.0.tar", last modified: Wed Dec 13 20:00:39 2023, max compression
+gzip compressed data, was "types-aiobotocore-swf-2.9.1.tar", last modified: Thu Jan 18 01:21:57 2024, max compression
```

## Comparing `types-aiobotocore-swf-2.9.0.tar` & `types-aiobotocore-swf-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:39.637059 types-aiobotocore-swf-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:57:13.000000 types-aiobotocore-swf-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13839 2023-12-13 20:00:39.637059 types-aiobotocore-swf-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12292 2023-12-13 19:57:13.000000 types-aiobotocore-swf-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:39.637059 types-aiobotocore-swf-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-12-13 19:57:13.000000 types-aiobotocore-swf-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:39.637059 types-aiobotocore-swf-2.9.0/types_aiobotocore_swf/
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2023-12-13 19:57:13.000000 types-aiobotocore-swf-2.9.0/types_aiobotocore_swf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2023-12-13 19:57:13.000000 types-aiobotocore-swf-2.9.0/types_aiobotocore_swf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-13 19:57:13.000000 types-aiobotocore-swf-2.9.0/types_aiobotocore_swf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33203 2023-12-13 19:57:13.000000 types-aiobotocore-swf-2.9.0/types_aiobotocore_swf/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    33199 2023-12-13 19:57:13.000000 types-aiobotocore-swf-2.9.0/types_aiobotocore_swf/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16612 2023-12-13 19:57:13.000000 types-aiobotocore-swf-2.9.0/types_aiobotocore_swf/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    16610 2023-12-13 19:57:13.000000 types-aiobotocore-swf-2.9.0/types_aiobotocore_swf/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10149 2023-12-13 19:57:13.000000 types-aiobotocore-swf-2.9.0/types_aiobotocore_swf/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10140 2023-12-13 19:57:13.000000 types-aiobotocore-swf-2.9.0/types_aiobotocore_swf/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:57:13.000000 types-aiobotocore-swf-2.9.0/types_aiobotocore_swf/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    60561 2023-12-13 19:57:14.000000 types-aiobotocore-swf-2.9.0/types_aiobotocore_swf/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    60560 2023-12-13 19:57:14.000000 types-aiobotocore-swf-2.9.0/types_aiobotocore_swf/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:57:13.000000 types-aiobotocore-swf-2.9.0/types_aiobotocore_swf/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:39.637059 types-aiobotocore-swf-2.9.0/types_aiobotocore_swf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13839 2023-12-13 20:00:39.000000 types-aiobotocore-swf-2.9.0/types_aiobotocore_swf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      737 2023-12-13 20:00:39.000000 types-aiobotocore-swf-2.9.0/types_aiobotocore_swf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:39.000000 types-aiobotocore-swf-2.9.0/types_aiobotocore_swf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:39.000000 types-aiobotocore-swf-2.9.0/types_aiobotocore_swf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:39.000000 types-aiobotocore-swf-2.9.0/types_aiobotocore_swf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 20:00:39.000000 types-aiobotocore-swf-2.9.0/types_aiobotocore_swf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:57.164996 types-aiobotocore-swf-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:18:40.000000 types-aiobotocore-swf-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13859 2024-01-18 01:21:57.164996 types-aiobotocore-swf-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12292 2024-01-18 01:18:40.000000 types-aiobotocore-swf-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:57.164996 types-aiobotocore-swf-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-01-18 01:18:40.000000 types-aiobotocore-swf-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:57.164996 types-aiobotocore-swf-2.9.1/types_aiobotocore_swf/
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-18 01:18:40.000000 types-aiobotocore-swf-2.9.1/types_aiobotocore_swf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-18 01:18:40.000000 types-aiobotocore-swf-2.9.1/types_aiobotocore_swf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-18 01:18:40.000000 types-aiobotocore-swf-2.9.1/types_aiobotocore_swf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33217 2024-01-18 01:18:41.000000 types-aiobotocore-swf-2.9.1/types_aiobotocore_swf/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33214 2024-01-18 01:18:41.000000 types-aiobotocore-swf-2.9.1/types_aiobotocore_swf/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16610 2024-01-18 01:18:41.000000 types-aiobotocore-swf-2.9.1/types_aiobotocore_swf/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16610 2024-01-18 01:18:41.000000 types-aiobotocore-swf-2.9.1/types_aiobotocore_swf/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10155 2024-01-18 01:18:41.000000 types-aiobotocore-swf-2.9.1/types_aiobotocore_swf/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10147 2024-01-18 01:18:41.000000 types-aiobotocore-swf-2.9.1/types_aiobotocore_swf/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:18:40.000000 types-aiobotocore-swf-2.9.1/types_aiobotocore_swf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    60560 2024-01-18 01:18:42.000000 types-aiobotocore-swf-2.9.1/types_aiobotocore_swf/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60560 2024-01-18 01:18:42.000000 types-aiobotocore-swf-2.9.1/types_aiobotocore_swf/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:18:40.000000 types-aiobotocore-swf-2.9.1/types_aiobotocore_swf/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:57.164996 types-aiobotocore-swf-2.9.1/types_aiobotocore_swf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13859 2024-01-18 01:21:57.000000 types-aiobotocore-swf-2.9.1/types_aiobotocore_swf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-01-18 01:21:57.000000 types-aiobotocore-swf-2.9.1/types_aiobotocore_swf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:57.000000 types-aiobotocore-swf-2.9.1/types_aiobotocore_swf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:57.000000 types-aiobotocore-swf-2.9.1/types_aiobotocore_swf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:57.000000 types-aiobotocore-swf-2.9.1/types_aiobotocore_swf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:21:57.000000 types-aiobotocore-swf-2.9.1/types_aiobotocore_swf.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-swf-2.9.0/LICENSE` & `types-aiobotocore-swf-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-swf-2.9.0/PKG-INFO` & `types-aiobotocore-swf-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-swf
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SWF 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SWF 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/
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
 
 <a id="types-aiobotocore-swf"></a>
 
 # types-aiobotocore-swf
 
 [![PyPI - types-aiobotocore-swf](https://img.shields.io/pypi/v/types-aiobotocore-swf.svg?color=blue)](https://pypi.org/project/types-aiobotocore-swf)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-swf.svg?color=blue)](https://pypi.org/project/types-aiobotocore-swf)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-swf)](https://pepy.tech/project/types-aiobotocore-swf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SWF 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
+[aiobotocore.SWF 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
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
 [types-aiobotocore-swf docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-swf-2.9.0/README.md` & `types-aiobotocore-swf-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-swf.svg?color=blue)](https://pypi.org/project/types-aiobotocore-swf)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-swf)](https://pepy.tech/project/types-aiobotocore-swf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SWF 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
+[aiobotocore.SWF 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
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
 [types-aiobotocore-swf docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-swf-2.9.0/setup.py` & `types-aiobotocore-swf-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-swf",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_swf"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SWF 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.SWF 2.9.1 service generated with mypy-boto3-builder"
+        " 7.23.1"
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
     keywords="aiobotocore swf type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_swf": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-swf-2.9.0/types_aiobotocore_swf/__init__.py` & `types-aiobotocore-swf-2.9.1/types_aiobotocore_swf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     ListOpenWorkflowExecutionsPaginator,
     ListWorkflowTypesPaginator,
     PollForDecisionTaskPaginator,
 )
 
 Client = SWFClient
 
-
 __all__ = (
     "Client",
     "GetWorkflowExecutionHistoryPaginator",
     "ListActivityTypesPaginator",
     "ListClosedWorkflowExecutionsPaginator",
     "ListDomainsPaginator",
     "ListOpenWorkflowExecutionsPaginator",
```

### Comparing `types-aiobotocore-swf-2.9.0/types_aiobotocore_swf/__init__.pyi` & `types-aiobotocore-swf-2.9.1/types_aiobotocore_swf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-swf-2.9.0/types_aiobotocore_swf/__main__.py` & `types-aiobotocore-swf-2.9.1/types_aiobotocore_swf/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SWF 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.SWF 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF\nOther"
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

### Comparing `types-aiobotocore-swf-2.9.0/types_aiobotocore_swf/client.py` & `types-aiobotocore-swf-2.9.1/types_aiobotocore_swf/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SWFClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -131,15 +130,15 @@
         *,
         domain: str,
         startTimeFilter: ExecutionTimeFilterTypeDef = ...,
         closeTimeFilter: ExecutionTimeFilterTypeDef = ...,
         executionFilter: WorkflowExecutionFilterTypeDef = ...,
         typeFilter: WorkflowTypeFilterTypeDef = ...,
         tagFilter: TagFilterTypeDef = ...,
-        closeStatusFilter: CloseStatusFilterTypeDef = ...
+        closeStatusFilter: CloseStatusFilterTypeDef = ...,
     ) -> WorkflowExecutionCountTypeDef:
         """
         Returns the number of closed workflow executions within the given domain that
         meet the specified filtering
         criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Client.count_closed_workflow_executions)
@@ -149,15 +148,15 @@
     async def count_open_workflow_executions(
         self,
         *,
         domain: str,
         startTimeFilter: ExecutionTimeFilterTypeDef,
         typeFilter: WorkflowTypeFilterTypeDef = ...,
         tagFilter: TagFilterTypeDef = ...,
-        executionFilter: WorkflowExecutionFilterTypeDef = ...
+        executionFilter: WorkflowExecutionFilterTypeDef = ...,
     ) -> WorkflowExecutionCountTypeDef:
         """
         Returns the number of open workflow executions within the given domain that
         meet the specified filtering
         criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Client.count_open_workflow_executions)
@@ -270,15 +269,15 @@
     async def get_workflow_execution_history(
         self,
         *,
         domain: str,
         execution: WorkflowExecutionTypeDef,
         nextPageToken: str = ...,
         maximumPageSize: int = ...,
-        reverseOrder: bool = ...
+        reverseOrder: bool = ...,
     ) -> HistoryTypeDef:
         """
         Returns the history of the specified workflow execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Client.get_workflow_execution_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/client/#get_workflow_execution_history)
         """
@@ -287,15 +286,15 @@
         self,
         *,
         domain: str,
         registrationStatus: RegistrationStatusType,
         name: str = ...,
         nextPageToken: str = ...,
         maximumPageSize: int = ...,
-        reverseOrder: bool = ...
+        reverseOrder: bool = ...,
     ) -> ActivityTypeInfosTypeDef:
         """
         Returns information about all activities registered in the specified domain
         that match the specified name and registration
         status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Client.list_activity_types)
@@ -310,15 +309,15 @@
         closeTimeFilter: ExecutionTimeFilterTypeDef = ...,
         executionFilter: WorkflowExecutionFilterTypeDef = ...,
         closeStatusFilter: CloseStatusFilterTypeDef = ...,
         typeFilter: WorkflowTypeFilterTypeDef = ...,
         tagFilter: TagFilterTypeDef = ...,
         nextPageToken: str = ...,
         maximumPageSize: int = ...,
-        reverseOrder: bool = ...
+        reverseOrder: bool = ...,
     ) -> WorkflowExecutionInfosTypeDef:
         """
         Returns a list of closed workflow executions in the specified domain that meet
         the filtering
         criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Client.list_closed_workflow_executions)
@@ -327,15 +326,15 @@
 
     async def list_domains(
         self,
         *,
         registrationStatus: RegistrationStatusType,
         nextPageToken: str = ...,
         maximumPageSize: int = ...,
-        reverseOrder: bool = ...
+        reverseOrder: bool = ...,
     ) -> DomainInfosTypeDef:
         """
         Returns the list of domains registered in the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Client.list_domains)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/client/#list_domains)
         """
@@ -346,15 +345,15 @@
         domain: str,
         startTimeFilter: ExecutionTimeFilterTypeDef,
         typeFilter: WorkflowTypeFilterTypeDef = ...,
         tagFilter: TagFilterTypeDef = ...,
         nextPageToken: str = ...,
         maximumPageSize: int = ...,
         reverseOrder: bool = ...,
-        executionFilter: WorkflowExecutionFilterTypeDef = ...
+        executionFilter: WorkflowExecutionFilterTypeDef = ...,
     ) -> WorkflowExecutionInfosTypeDef:
         """
         Returns a list of open workflow executions in the specified domain that meet
         the filtering
         criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Client.list_open_workflow_executions)
@@ -373,15 +372,15 @@
         self,
         *,
         domain: str,
         registrationStatus: RegistrationStatusType,
         name: str = ...,
         nextPageToken: str = ...,
         maximumPageSize: int = ...,
-        reverseOrder: bool = ...
+        reverseOrder: bool = ...,
     ) -> WorkflowTypeInfosTypeDef:
         """
         Returns information about workflow types in the specified domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Client.list_workflow_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/client/#list_workflow_types)
         """
@@ -401,15 +400,15 @@
         *,
         domain: str,
         taskList: TaskListTypeDef,
         identity: str = ...,
         nextPageToken: str = ...,
         maximumPageSize: int = ...,
         reverseOrder: bool = ...,
-        startAtPreviousStartedEvent: bool = ...
+        startAtPreviousStartedEvent: bool = ...,
     ) -> DecisionTaskTypeDef:
         """
         Used by deciders to get a  DecisionTask from the specified decision `taskList`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Client.poll_for_decision_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/client/#poll_for_decision_task)
         """
@@ -434,15 +433,15 @@
         version: str,
         description: str = ...,
         defaultTaskStartToCloseTimeout: str = ...,
         defaultTaskHeartbeatTimeout: str = ...,
         defaultTaskList: TaskListTypeDef = ...,
         defaultTaskPriority: str = ...,
         defaultTaskScheduleToStartTimeout: str = ...,
-        defaultTaskScheduleToCloseTimeout: str = ...
+        defaultTaskScheduleToCloseTimeout: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Registers a new *activity type* along with its configuration settings in the
         specified
         domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Client.register_activity_type)
@@ -451,15 +450,15 @@
 
     async def register_domain(
         self,
         *,
         name: str,
         workflowExecutionRetentionPeriodInDays: str,
         description: str = ...,
-        tags: Sequence[ResourceTagTypeDef] = ...
+        tags: Sequence[ResourceTagTypeDef] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Registers a new domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Client.register_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/client/#register_domain)
         """
@@ -472,15 +471,15 @@
         version: str,
         description: str = ...,
         defaultTaskStartToCloseTimeout: str = ...,
         defaultExecutionStartToCloseTimeout: str = ...,
         defaultTaskList: TaskListTypeDef = ...,
         defaultTaskPriority: str = ...,
         defaultChildPolicy: ChildPolicyType = ...,
-        defaultLambdaRole: str = ...
+        defaultLambdaRole: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Registers a new *workflow type* and its configuration settings in the specified
         domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Client.register_workflow_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/client/#register_workflow_type)
@@ -537,15 +536,15 @@
     async def respond_decision_task_completed(
         self,
         *,
         taskToken: str,
         decisions: Sequence[DecisionTypeDef] = ...,
         executionContext: str = ...,
         taskList: TaskListTypeDef = ...,
-        taskListScheduleToStartTimeout: str = ...
+        taskListScheduleToStartTimeout: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Used by deciders to tell the service that the  DecisionTask identified by the
         `taskToken` has successfully
         completed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Client.respond_decision_task_completed)
@@ -574,15 +573,15 @@
         taskList: TaskListTypeDef = ...,
         taskPriority: str = ...,
         input: str = ...,
         executionStartToCloseTimeout: str = ...,
         tagList: Sequence[str] = ...,
         taskStartToCloseTimeout: str = ...,
         childPolicy: ChildPolicyType = ...,
-        lambdaRole: str = ...
+        lambdaRole: str = ...,
     ) -> RunTypeDef:
         """
         Starts an execution of the workflow type in the specified domain using the
         provided `workflowId` and input
         data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Client.start_workflow_execution)
@@ -603,15 +602,15 @@
         self,
         *,
         domain: str,
         workflowId: str,
         runId: str = ...,
         reason: str = ...,
         details: str = ...,
-        childPolicy: ChildPolicyType = ...
+        childPolicy: ChildPolicyType = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Records a `WorkflowExecutionTerminated` event and forces closure of the
         workflow execution identified by the given domain, runId, and
         workflowId.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Client.terminate_workflow_execution)
```

### Comparing `types-aiobotocore-swf-2.9.0/types_aiobotocore_swf/client.pyi` & `types-aiobotocore-swf-2.9.1/types_aiobotocore_swf/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         *,
         domain: str,
         startTimeFilter: ExecutionTimeFilterTypeDef = ...,
         closeTimeFilter: ExecutionTimeFilterTypeDef = ...,
         executionFilter: WorkflowExecutionFilterTypeDef = ...,
         typeFilter: WorkflowTypeFilterTypeDef = ...,
         tagFilter: TagFilterTypeDef = ...,
-        closeStatusFilter: CloseStatusFilterTypeDef = ...
+        closeStatusFilter: CloseStatusFilterTypeDef = ...,
     ) -> WorkflowExecutionCountTypeDef:
         """
         Returns the number of closed workflow executions within the given domain that
         meet the specified filtering
         criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Client.count_closed_workflow_executions)
@@ -145,15 +145,15 @@
     async def count_open_workflow_executions(
         self,
         *,
         domain: str,
         startTimeFilter: ExecutionTimeFilterTypeDef,
         typeFilter: WorkflowTypeFilterTypeDef = ...,
         tagFilter: TagFilterTypeDef = ...,
-        executionFilter: WorkflowExecutionFilterTypeDef = ...
+        executionFilter: WorkflowExecutionFilterTypeDef = ...,
     ) -> WorkflowExecutionCountTypeDef:
         """
         Returns the number of open workflow executions within the given domain that
         meet the specified filtering
         criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Client.count_open_workflow_executions)
@@ -266,15 +266,15 @@
     async def get_workflow_execution_history(
         self,
         *,
         domain: str,
         execution: WorkflowExecutionTypeDef,
         nextPageToken: str = ...,
         maximumPageSize: int = ...,
-        reverseOrder: bool = ...
+        reverseOrder: bool = ...,
     ) -> HistoryTypeDef:
         """
         Returns the history of the specified workflow execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Client.get_workflow_execution_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/client/#get_workflow_execution_history)
         """
@@ -283,15 +283,15 @@
         self,
         *,
         domain: str,
         registrationStatus: RegistrationStatusType,
         name: str = ...,
         nextPageToken: str = ...,
         maximumPageSize: int = ...,
-        reverseOrder: bool = ...
+        reverseOrder: bool = ...,
     ) -> ActivityTypeInfosTypeDef:
         """
         Returns information about all activities registered in the specified domain
         that match the specified name and registration
         status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Client.list_activity_types)
@@ -306,15 +306,15 @@
         closeTimeFilter: ExecutionTimeFilterTypeDef = ...,
         executionFilter: WorkflowExecutionFilterTypeDef = ...,
         closeStatusFilter: CloseStatusFilterTypeDef = ...,
         typeFilter: WorkflowTypeFilterTypeDef = ...,
         tagFilter: TagFilterTypeDef = ...,
         nextPageToken: str = ...,
         maximumPageSize: int = ...,
-        reverseOrder: bool = ...
+        reverseOrder: bool = ...,
     ) -> WorkflowExecutionInfosTypeDef:
         """
         Returns a list of closed workflow executions in the specified domain that meet
         the filtering
         criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Client.list_closed_workflow_executions)
@@ -323,15 +323,15 @@
 
     async def list_domains(
         self,
         *,
         registrationStatus: RegistrationStatusType,
         nextPageToken: str = ...,
         maximumPageSize: int = ...,
-        reverseOrder: bool = ...
+        reverseOrder: bool = ...,
     ) -> DomainInfosTypeDef:
         """
         Returns the list of domains registered in the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Client.list_domains)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/client/#list_domains)
         """
@@ -342,15 +342,15 @@
         domain: str,
         startTimeFilter: ExecutionTimeFilterTypeDef,
         typeFilter: WorkflowTypeFilterTypeDef = ...,
         tagFilter: TagFilterTypeDef = ...,
         nextPageToken: str = ...,
         maximumPageSize: int = ...,
         reverseOrder: bool = ...,
-        executionFilter: WorkflowExecutionFilterTypeDef = ...
+        executionFilter: WorkflowExecutionFilterTypeDef = ...,
     ) -> WorkflowExecutionInfosTypeDef:
         """
         Returns a list of open workflow executions in the specified domain that meet
         the filtering
         criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Client.list_open_workflow_executions)
@@ -369,15 +369,15 @@
         self,
         *,
         domain: str,
         registrationStatus: RegistrationStatusType,
         name: str = ...,
         nextPageToken: str = ...,
         maximumPageSize: int = ...,
-        reverseOrder: bool = ...
+        reverseOrder: bool = ...,
     ) -> WorkflowTypeInfosTypeDef:
         """
         Returns information about workflow types in the specified domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Client.list_workflow_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/client/#list_workflow_types)
         """
@@ -397,15 +397,15 @@
         *,
         domain: str,
         taskList: TaskListTypeDef,
         identity: str = ...,
         nextPageToken: str = ...,
         maximumPageSize: int = ...,
         reverseOrder: bool = ...,
-        startAtPreviousStartedEvent: bool = ...
+        startAtPreviousStartedEvent: bool = ...,
     ) -> DecisionTaskTypeDef:
         """
         Used by deciders to get a  DecisionTask from the specified decision `taskList`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Client.poll_for_decision_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/client/#poll_for_decision_task)
         """
@@ -430,15 +430,15 @@
         version: str,
         description: str = ...,
         defaultTaskStartToCloseTimeout: str = ...,
         defaultTaskHeartbeatTimeout: str = ...,
         defaultTaskList: TaskListTypeDef = ...,
         defaultTaskPriority: str = ...,
         defaultTaskScheduleToStartTimeout: str = ...,
-        defaultTaskScheduleToCloseTimeout: str = ...
+        defaultTaskScheduleToCloseTimeout: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Registers a new *activity type* along with its configuration settings in the
         specified
         domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Client.register_activity_type)
@@ -447,15 +447,15 @@
 
     async def register_domain(
         self,
         *,
         name: str,
         workflowExecutionRetentionPeriodInDays: str,
         description: str = ...,
-        tags: Sequence[ResourceTagTypeDef] = ...
+        tags: Sequence[ResourceTagTypeDef] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Registers a new domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Client.register_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/client/#register_domain)
         """
@@ -468,15 +468,15 @@
         version: str,
         description: str = ...,
         defaultTaskStartToCloseTimeout: str = ...,
         defaultExecutionStartToCloseTimeout: str = ...,
         defaultTaskList: TaskListTypeDef = ...,
         defaultTaskPriority: str = ...,
         defaultChildPolicy: ChildPolicyType = ...,
-        defaultLambdaRole: str = ...
+        defaultLambdaRole: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Registers a new *workflow type* and its configuration settings in the specified
         domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Client.register_workflow_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/client/#register_workflow_type)
@@ -533,15 +533,15 @@
     async def respond_decision_task_completed(
         self,
         *,
         taskToken: str,
         decisions: Sequence[DecisionTypeDef] = ...,
         executionContext: str = ...,
         taskList: TaskListTypeDef = ...,
-        taskListScheduleToStartTimeout: str = ...
+        taskListScheduleToStartTimeout: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Used by deciders to tell the service that the  DecisionTask identified by the
         `taskToken` has successfully
         completed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Client.respond_decision_task_completed)
@@ -570,15 +570,15 @@
         taskList: TaskListTypeDef = ...,
         taskPriority: str = ...,
         input: str = ...,
         executionStartToCloseTimeout: str = ...,
         tagList: Sequence[str] = ...,
         taskStartToCloseTimeout: str = ...,
         childPolicy: ChildPolicyType = ...,
-        lambdaRole: str = ...
+        lambdaRole: str = ...,
     ) -> RunTypeDef:
         """
         Starts an execution of the workflow type in the specified domain using the
         provided `workflowId` and input
         data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Client.start_workflow_execution)
@@ -599,15 +599,15 @@
         self,
         *,
         domain: str,
         workflowId: str,
         runId: str = ...,
         reason: str = ...,
         details: str = ...,
-        childPolicy: ChildPolicyType = ...
+        childPolicy: ChildPolicyType = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Records a `WorkflowExecutionTerminated` event and forces closure of the
         workflow execution identified by the given domain, runId, and
         workflowId.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Client.terminate_workflow_execution)
```

### Comparing `types-aiobotocore-swf-2.9.0/types_aiobotocore_swf/literals.py` & `types-aiobotocore-swf-2.9.1/types_aiobotocore_swf/literals.py`

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
     "ActivityTaskTimeoutTypeType",
     "CancelTimerFailedCauseType",
     "CancelWorkflowExecutionFailedCauseType",
     "ChildPolicyType",
     "CloseStatusType",
     "CompleteWorkflowExecutionFailedCauseType",
@@ -57,15 +56,14 @@
     "SWFServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ActivityTaskTimeoutTypeType = Literal[
     "HEARTBEAT", "SCHEDULE_TO_CLOSE", "SCHEDULE_TO_START", "START_TO_CLOSE"
 ]
 CancelTimerFailedCauseType = Literal["OPERATION_NOT_PERMITTED", "TIMER_ID_UNKNOWN"]
 CancelWorkflowExecutionFailedCauseType = Literal["OPERATION_NOT_PERMITTED", "UNHANDLED_DECISION"]
 ChildPolicyType = Literal["ABANDON", "REQUEST_CANCEL", "TERMINATE"]
 CloseStatusType = Literal[
```

### Comparing `types-aiobotocore-swf-2.9.0/types_aiobotocore_swf/literals.pyi` & `types-aiobotocore-swf-2.9.1/types_aiobotocore_swf/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-swf-2.9.0/types_aiobotocore_swf/paginator.py` & `types-aiobotocore-swf-2.9.1/types_aiobotocore_swf/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,14 @@
     "ListClosedWorkflowExecutionsPaginator",
     "ListDomainsPaginator",
     "ListOpenWorkflowExecutionsPaginator",
     "ListWorkflowTypesPaginator",
     "PollForDecisionTaskPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -85,15 +84,15 @@
 
     def paginate(
         self,
         *,
         domain: str,
         execution: WorkflowExecutionTypeDef,
         reverseOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[HistoryTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.GetWorkflowExecutionHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/paginators/#getworkflowexecutionhistorypaginator)
         """
 
 
@@ -106,15 +105,15 @@
     def paginate(
         self,
         *,
         domain: str,
         registrationStatus: RegistrationStatusType,
         name: str = ...,
         reverseOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ActivityTypeInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListActivityTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/paginators/#listactivitytypespaginator)
         """
 
 
@@ -131,15 +130,15 @@
         startTimeFilter: ExecutionTimeFilterTypeDef = ...,
         closeTimeFilter: ExecutionTimeFilterTypeDef = ...,
         executionFilter: WorkflowExecutionFilterTypeDef = ...,
         closeStatusFilter: CloseStatusFilterTypeDef = ...,
         typeFilter: WorkflowTypeFilterTypeDef = ...,
         tagFilter: TagFilterTypeDef = ...,
         reverseOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[WorkflowExecutionInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListClosedWorkflowExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/paginators/#listclosedworkflowexecutionspaginator)
         """
 
 
@@ -150,15 +149,15 @@
     """
 
     def paginate(
         self,
         *,
         registrationStatus: RegistrationStatusType,
         reverseOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DomainInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListDomains.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/paginators/#listdomainspaginator)
         """
 
 
@@ -173,15 +172,15 @@
         *,
         domain: str,
         startTimeFilter: ExecutionTimeFilterTypeDef,
         typeFilter: WorkflowTypeFilterTypeDef = ...,
         tagFilter: TagFilterTypeDef = ...,
         reverseOrder: bool = ...,
         executionFilter: WorkflowExecutionFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[WorkflowExecutionInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListOpenWorkflowExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/paginators/#listopenworkflowexecutionspaginator)
         """
 
 
@@ -194,15 +193,15 @@
     def paginate(
         self,
         *,
         domain: str,
         registrationStatus: RegistrationStatusType,
         name: str = ...,
         reverseOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[WorkflowTypeInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListWorkflowTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/paginators/#listworkflowtypespaginator)
         """
 
 
@@ -216,13 +215,13 @@
         self,
         *,
         domain: str,
         taskList: TaskListTypeDef,
         identity: str = ...,
         reverseOrder: bool = ...,
         startAtPreviousStartedEvent: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DecisionTaskTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.PollForDecisionTask.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/paginators/#pollfordecisiontaskpaginator)
         """
```

### Comparing `types-aiobotocore-swf-2.9.0/types_aiobotocore_swf/paginator.pyi` & `types-aiobotocore-swf-2.9.1/types_aiobotocore_swf/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
     def paginate(
         self,
         *,
         domain: str,
         execution: WorkflowExecutionTypeDef,
         reverseOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[HistoryTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.GetWorkflowExecutionHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/paginators/#getworkflowexecutionhistorypaginator)
         """
 
 class ListActivityTypesPaginator(AioPaginator):
@@ -102,15 +102,15 @@
     def paginate(
         self,
         *,
         domain: str,
         registrationStatus: RegistrationStatusType,
         name: str = ...,
         reverseOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ActivityTypeInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListActivityTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/paginators/#listactivitytypespaginator)
         """
 
 class ListClosedWorkflowExecutionsPaginator(AioPaginator):
@@ -126,15 +126,15 @@
         startTimeFilter: ExecutionTimeFilterTypeDef = ...,
         closeTimeFilter: ExecutionTimeFilterTypeDef = ...,
         executionFilter: WorkflowExecutionFilterTypeDef = ...,
         closeStatusFilter: CloseStatusFilterTypeDef = ...,
         typeFilter: WorkflowTypeFilterTypeDef = ...,
         tagFilter: TagFilterTypeDef = ...,
         reverseOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[WorkflowExecutionInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListClosedWorkflowExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/paginators/#listclosedworkflowexecutionspaginator)
         """
 
 class ListDomainsPaginator(AioPaginator):
@@ -144,15 +144,15 @@
     """
 
     def paginate(
         self,
         *,
         registrationStatus: RegistrationStatusType,
         reverseOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DomainInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListDomains.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/paginators/#listdomainspaginator)
         """
 
 class ListOpenWorkflowExecutionsPaginator(AioPaginator):
@@ -166,15 +166,15 @@
         *,
         domain: str,
         startTimeFilter: ExecutionTimeFilterTypeDef,
         typeFilter: WorkflowTypeFilterTypeDef = ...,
         tagFilter: TagFilterTypeDef = ...,
         reverseOrder: bool = ...,
         executionFilter: WorkflowExecutionFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[WorkflowExecutionInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListOpenWorkflowExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/paginators/#listopenworkflowexecutionspaginator)
         """
 
 class ListWorkflowTypesPaginator(AioPaginator):
@@ -186,15 +186,15 @@
     def paginate(
         self,
         *,
         domain: str,
         registrationStatus: RegistrationStatusType,
         name: str = ...,
         reverseOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[WorkflowTypeInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListWorkflowTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/paginators/#listworkflowtypespaginator)
         """
 
 class PollForDecisionTaskPaginator(AioPaginator):
@@ -207,13 +207,13 @@
         self,
         *,
         domain: str,
         taskList: TaskListTypeDef,
         identity: str = ...,
         reverseOrder: bool = ...,
         startAtPreviousStartedEvent: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DecisionTaskTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.PollForDecisionTask.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/paginators/#pollfordecisiontaskpaginator)
         """
```

### Comparing `types-aiobotocore-swf-2.9.0/types_aiobotocore_swf/type_defs.py` & `types-aiobotocore-swf-2.9.1/types_aiobotocore_swf/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActivityTaskCancelRequestedEventAttributesTypeDef",
     "ActivityTaskCanceledEventAttributesTypeDef",
     "ActivityTaskCompletedEventAttributesTypeDef",
     "ActivityTaskFailedEventAttributesTypeDef",
     "ActivityTypeTypeDef",
     "TaskListTypeDef",
```

### Comparing `types-aiobotocore-swf-2.9.0/types_aiobotocore_swf/type_defs.pyi` & `types-aiobotocore-swf-2.9.1/types_aiobotocore_swf/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-swf-2.9.0/types_aiobotocore_swf.egg-info/PKG-INFO` & `types-aiobotocore-swf-2.9.1/types_aiobotocore_swf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-swf
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SWF 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SWF 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/
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
 
 <a id="types-aiobotocore-swf"></a>
 
 # types-aiobotocore-swf
 
 [![PyPI - types-aiobotocore-swf](https://img.shields.io/pypi/v/types-aiobotocore-swf.svg?color=blue)](https://pypi.org/project/types-aiobotocore-swf)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-swf.svg?color=blue)](https://pypi.org/project/types-aiobotocore-swf)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-swf)](https://pepy.tech/project/types-aiobotocore-swf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SWF 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
+[aiobotocore.SWF 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
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
 [types-aiobotocore-swf docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-swf-2.9.0/types_aiobotocore_swf.egg-info/SOURCES.txt` & `types-aiobotocore-swf-2.9.1/types_aiobotocore_swf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

