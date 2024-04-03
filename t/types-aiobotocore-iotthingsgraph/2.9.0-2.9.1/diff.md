# Comparing `tmp/types-aiobotocore-iotthingsgraph-2.9.0.tar.gz` & `tmp/types-aiobotocore-iotthingsgraph-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotthingsgraph-2.9.0.tar", last modified: Wed Dec 13 19:59:35 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotthingsgraph-2.9.1.tar", last modified: Thu Jan 18 01:20:58 2024, max compression
```

## Comparing `types-aiobotocore-iotthingsgraph-2.9.0.tar` & `types-aiobotocore-iotthingsgraph-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:35.129613 types-aiobotocore-iotthingsgraph-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:48:07.000000 types-aiobotocore-iotthingsgraph-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14932 2023-12-13 19:59:35.129613 types-aiobotocore-iotthingsgraph-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13341 2023-12-13 19:48:07.000000 types-aiobotocore-iotthingsgraph-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:35.129613 types-aiobotocore-iotthingsgraph-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2023-12-13 19:48:07.000000 types-aiobotocore-iotthingsgraph-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:35.129613 types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph/
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2023-12-13 19:48:07.000000 types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2023-12-13 19:48:07.000000 types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      960 2023-12-13 19:48:07.000000 types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31324 2023-12-13 19:48:08.000000 types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    31320 2023-12-13 19:48:08.000000 types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11763 2023-12-13 19:48:08.000000 types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11761 2023-12-13 19:48:08.000000 types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13624 2023-12-13 19:48:08.000000 types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13612 2023-12-13 19:48:08.000000 types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:48:07.000000 types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    26362 2023-12-13 19:48:08.000000 types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    26361 2023-12-13 19:48:08.000000 types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:48:07.000000 types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:35.129613 types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14932 2023-12-13 19:59:35.000000 types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-12-13 19:59:35.000000 types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:35.000000 types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:35.000000 types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:35.000000 types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-13 19:59:35.000000 types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:58.445261 types-aiobotocore-iotthingsgraph-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:09:57.000000 types-aiobotocore-iotthingsgraph-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14952 2024-01-18 01:20:58.445261 types-aiobotocore-iotthingsgraph-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13341 2024-01-18 01:09:57.000000 types-aiobotocore-iotthingsgraph-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:58.445261 types-aiobotocore-iotthingsgraph-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-01-18 01:09:57.000000 types-aiobotocore-iotthingsgraph-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:58.441261 types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph/
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-01-18 01:09:57.000000 types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-01-18 01:09:57.000000 types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-01-18 01:09:57.000000 types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31333 2024-01-18 01:09:57.000000 types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31330 2024-01-18 01:09:57.000000 types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11761 2024-01-18 01:09:57.000000 types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11761 2024-01-18 01:09:57.000000 types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13629 2024-01-18 01:09:57.000000 types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13618 2024-01-18 01:09:57.000000 types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:09:57.000000 types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    26361 2024-01-18 01:09:58.000000 types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26361 2024-01-18 01:09:58.000000 types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:09:57.000000 types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:58.445261 types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14952 2024-01-18 01:20:58.000000 types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-01-18 01:20:58.000000 types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:58.000000 types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:58.000000 types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:58.000000 types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-18 01:20:58.000000 types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotthingsgraph-2.9.0/LICENSE` & `types-aiobotocore-iotthingsgraph-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-iotthingsgraph-2.9.0/PKG-INFO` & `types-aiobotocore-iotthingsgraph-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotthingsgraph
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IoTThingsGraph 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IoTThingsGraph 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/
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
 
 <a id="types-aiobotocore-iotthingsgraph"></a>
 
 # types-aiobotocore-iotthingsgraph
 
 [![PyPI - types-aiobotocore-iotthingsgraph](https://img.shields.io/pypi/v/types-aiobotocore-iotthingsgraph.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotthingsgraph)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotthingsgraph.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotthingsgraph)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotthingsgraph)](https://pepy.tech/project/types-aiobotocore-iotthingsgraph)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTThingsGraph 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
+[aiobotocore.IoTThingsGraph 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
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
 [types-aiobotocore-iotthingsgraph docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iotthingsgraph-2.9.0/README.md` & `types-aiobotocore-iotthingsgraph-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotthingsgraph.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotthingsgraph)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotthingsgraph)](https://pepy.tech/project/types-aiobotocore-iotthingsgraph)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTThingsGraph 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
+[aiobotocore.IoTThingsGraph 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
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
 [types-aiobotocore-iotthingsgraph docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iotthingsgraph-2.9.0/setup.py` & `types-aiobotocore-iotthingsgraph-2.9.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotthingsgraph",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_iotthingsgraph"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.IoTThingsGraph 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.IoTThingsGraph 2.9.1 service generated with"
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
     keywords="aiobotocore iotthingsgraph type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_iotthingsgraph": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph/__init__.py` & `types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     SearchSystemInstancesPaginator,
     SearchSystemTemplatesPaginator,
     SearchThingsPaginator,
 )
 
 Client = IoTThingsGraphClient
 
-
 __all__ = (
     "Client",
     "GetFlowTemplateRevisionsPaginator",
     "GetSystemTemplateRevisionsPaginator",
     "IoTThingsGraphClient",
     "ListFlowExecutionMessagesPaginator",
     "ListTagsForResourcePaginator",
```

### Comparing `types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph/__init__.pyi` & `types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph/__main__.py` & `types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTThingsGraph 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.IoTThingsGraph 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph\nOther"
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

### Comparing `types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph/client.py` & `types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("IoTThingsGraphClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -157,15 +156,15 @@
         *,
         definition: DefinitionDocumentTypeDef,
         target: DeploymentTargetType,
         tags: Sequence[TagTypeDef] = ...,
         greengrassGroupName: str = ...,
         s3BucketName: str = ...,
         metricsConfiguration: MetricsConfigurationTypeDef = ...,
-        flowActionsRoleArn: str = ...
+        flowActionsRoleArn: str = ...,
     ) -> CreateSystemInstanceResponseTypeDef:
         """
         Creates a system instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Client.create_system_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/client/#create_system_instance)
         """
@@ -374,15 +373,15 @@
     async def search_entities(
         self,
         *,
         entityTypes: Sequence[EntityTypeType],
         filters: Sequence[EntityFilterTypeDef] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        namespaceVersion: int = ...
+        namespaceVersion: int = ...,
     ) -> SearchEntitiesResponseTypeDef:
         """
         Searches for entities of the specified type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Client.search_entities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/client/#search_entities)
         """
@@ -391,72 +390,72 @@
         self,
         *,
         systemInstanceId: str,
         flowExecutionId: str = ...,
         startTime: TimestampTypeDef = ...,
         endTime: TimestampTypeDef = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> SearchFlowExecutionsResponseTypeDef:
         """
         Searches for AWS IoT Things Graph workflow execution instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Client.search_flow_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/client/#search_flow_executions)
         """
 
     async def search_flow_templates(
         self,
         *,
         filters: Sequence[FlowTemplateFilterTypeDef] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> SearchFlowTemplatesResponseTypeDef:
         """
         Searches for summary information about workflows.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Client.search_flow_templates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/client/#search_flow_templates)
         """
 
     async def search_system_instances(
         self,
         *,
         filters: Sequence[SystemInstanceFilterTypeDef] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> SearchSystemInstancesResponseTypeDef:
         """
         Searches for system instances in the user's account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Client.search_system_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/client/#search_system_instances)
         """
 
     async def search_system_templates(
         self,
         *,
         filters: Sequence[SystemTemplateFilterTypeDef] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> SearchSystemTemplatesResponseTypeDef:
         """
         Searches for summary information about systems in the user's account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Client.search_system_templates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/client/#search_system_templates)
         """
 
     async def search_things(
         self,
         *,
         entityId: str,
         nextToken: str = ...,
         maxResults: int = ...,
-        namespaceVersion: int = ...
+        namespaceVersion: int = ...,
     ) -> SearchThingsResponseTypeDef:
         """
         Searches for things associated with the specified entity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Client.search_things)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/client/#search_things)
         """
@@ -488,43 +487,43 @@
         """
 
     async def update_flow_template(
         self,
         *,
         id: str,
         definition: DefinitionDocumentTypeDef,
-        compatibleNamespaceVersion: int = ...
+        compatibleNamespaceVersion: int = ...,
     ) -> UpdateFlowTemplateResponseTypeDef:
         """
         Updates the specified workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Client.update_flow_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/client/#update_flow_template)
         """
 
     async def update_system_template(
         self,
         *,
         id: str,
         definition: DefinitionDocumentTypeDef,
-        compatibleNamespaceVersion: int = ...
+        compatibleNamespaceVersion: int = ...,
     ) -> UpdateSystemTemplateResponseTypeDef:
         """
         Updates the specified system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Client.update_system_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/client/#update_system_template)
         """
 
     async def upload_entity_definitions(
         self,
         *,
         document: DefinitionDocumentTypeDef = ...,
         syncWithPublicNamespace: bool = ...,
-        deprecateExistingEntities: bool = ...
+        deprecateExistingEntities: bool = ...,
     ) -> UploadEntityDefinitionsResponseTypeDef:
         """
         Asynchronously uploads one or more entity definitions to the user's namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Client.upload_entity_definitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/client/#upload_entity_definitions)
         """
```

### Comparing `types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph/client.pyi` & `types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
         *,
         definition: DefinitionDocumentTypeDef,
         target: DeploymentTargetType,
         tags: Sequence[TagTypeDef] = ...,
         greengrassGroupName: str = ...,
         s3BucketName: str = ...,
         metricsConfiguration: MetricsConfigurationTypeDef = ...,
-        flowActionsRoleArn: str = ...
+        flowActionsRoleArn: str = ...,
     ) -> CreateSystemInstanceResponseTypeDef:
         """
         Creates a system instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Client.create_system_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/client/#create_system_instance)
         """
@@ -370,15 +370,15 @@
     async def search_entities(
         self,
         *,
         entityTypes: Sequence[EntityTypeType],
         filters: Sequence[EntityFilterTypeDef] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        namespaceVersion: int = ...
+        namespaceVersion: int = ...,
     ) -> SearchEntitiesResponseTypeDef:
         """
         Searches for entities of the specified type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Client.search_entities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/client/#search_entities)
         """
@@ -387,72 +387,72 @@
         self,
         *,
         systemInstanceId: str,
         flowExecutionId: str = ...,
         startTime: TimestampTypeDef = ...,
         endTime: TimestampTypeDef = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> SearchFlowExecutionsResponseTypeDef:
         """
         Searches for AWS IoT Things Graph workflow execution instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Client.search_flow_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/client/#search_flow_executions)
         """
 
     async def search_flow_templates(
         self,
         *,
         filters: Sequence[FlowTemplateFilterTypeDef] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> SearchFlowTemplatesResponseTypeDef:
         """
         Searches for summary information about workflows.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Client.search_flow_templates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/client/#search_flow_templates)
         """
 
     async def search_system_instances(
         self,
         *,
         filters: Sequence[SystemInstanceFilterTypeDef] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> SearchSystemInstancesResponseTypeDef:
         """
         Searches for system instances in the user's account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Client.search_system_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/client/#search_system_instances)
         """
 
     async def search_system_templates(
         self,
         *,
         filters: Sequence[SystemTemplateFilterTypeDef] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> SearchSystemTemplatesResponseTypeDef:
         """
         Searches for summary information about systems in the user's account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Client.search_system_templates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/client/#search_system_templates)
         """
 
     async def search_things(
         self,
         *,
         entityId: str,
         nextToken: str = ...,
         maxResults: int = ...,
-        namespaceVersion: int = ...
+        namespaceVersion: int = ...,
     ) -> SearchThingsResponseTypeDef:
         """
         Searches for things associated with the specified entity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Client.search_things)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/client/#search_things)
         """
@@ -484,43 +484,43 @@
         """
 
     async def update_flow_template(
         self,
         *,
         id: str,
         definition: DefinitionDocumentTypeDef,
-        compatibleNamespaceVersion: int = ...
+        compatibleNamespaceVersion: int = ...,
     ) -> UpdateFlowTemplateResponseTypeDef:
         """
         Updates the specified workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Client.update_flow_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/client/#update_flow_template)
         """
 
     async def update_system_template(
         self,
         *,
         id: str,
         definition: DefinitionDocumentTypeDef,
-        compatibleNamespaceVersion: int = ...
+        compatibleNamespaceVersion: int = ...,
     ) -> UpdateSystemTemplateResponseTypeDef:
         """
         Updates the specified system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Client.update_system_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/client/#update_system_template)
         """
 
     async def upload_entity_definitions(
         self,
         *,
         document: DefinitionDocumentTypeDef = ...,
         syncWithPublicNamespace: bool = ...,
-        deprecateExistingEntities: bool = ...
+        deprecateExistingEntities: bool = ...,
     ) -> UploadEntityDefinitionsResponseTypeDef:
         """
         Asynchronously uploads one or more entity definitions to the user's namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Client.upload_entity_definitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/client/#upload_entity_definitions)
         """
```

### Comparing `types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph/literals.py` & `types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph/literals.py`

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
     "DefinitionLanguageType",
     "DeploymentTargetType",
     "EntityFilterNameType",
     "EntityTypeType",
     "FlowExecutionEventTypeType",
     "FlowExecutionStatusType",
@@ -47,15 +46,14 @@
     "IoTThingsGraphServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DefinitionLanguageType = Literal["GRAPHQL"]
 DeploymentTargetType = Literal["CLOUD", "GREENGRASS"]
 EntityFilterNameType = Literal["NAME", "NAMESPACE", "REFERENCED_ENTITY_ID", "SEMANTIC_TYPE_PATH"]
 EntityTypeType = Literal[
     "ACTION",
     "CAPABILITY",
     "DEVICE",
```

### Comparing `types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph/literals.pyi` & `types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph/paginator.py` & `types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,14 @@
     "SearchFlowExecutionsPaginator",
     "SearchFlowTemplatesPaginator",
     "SearchSystemInstancesPaginator",
     "SearchSystemTemplatesPaginator",
     "SearchThingsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -156,15 +155,15 @@
 
     def paginate(
         self,
         *,
         entityTypes: Sequence[EntityTypeType],
         filters: Sequence[EntityFilterTypeDef] = ...,
         namespaceVersion: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchEntitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchEntities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchentitiespaginator)
         """
 
 
@@ -177,15 +176,15 @@
     def paginate(
         self,
         *,
         systemInstanceId: str,
         flowExecutionId: str = ...,
         startTime: TimestampTypeDef = ...,
         endTime: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchFlowExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchFlowExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchflowexecutionspaginator)
         """
 
 
@@ -195,15 +194,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchflowtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FlowTemplateFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchFlowTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchFlowTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchflowtemplatespaginator)
         """
 
 
@@ -213,15 +212,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchsysteminstancespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SystemInstanceFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchSystemInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchSystemInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchsysteminstancespaginator)
         """
 
 
@@ -231,15 +230,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchsystemtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SystemTemplateFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchSystemTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchSystemTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchsystemtemplatespaginator)
         """
 
 
@@ -250,13 +249,13 @@
     """
 
     def paginate(
         self,
         *,
         entityId: str,
         namespaceVersion: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchThingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchThings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchthingspaginator)
         """
```

### Comparing `types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph/paginator.pyi` & `types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 
     def paginate(
         self,
         *,
         entityTypes: Sequence[EntityTypeType],
         filters: Sequence[EntityFilterTypeDef] = ...,
         namespaceVersion: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchEntitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchEntities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchentitiespaginator)
         """
 
 class SearchFlowExecutionsPaginator(AioPaginator):
@@ -169,15 +169,15 @@
     def paginate(
         self,
         *,
         systemInstanceId: str,
         flowExecutionId: str = ...,
         startTime: TimestampTypeDef = ...,
         endTime: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchFlowExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchFlowExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchflowexecutionspaginator)
         """
 
 class SearchFlowTemplatesPaginator(AioPaginator):
@@ -186,15 +186,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchflowtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FlowTemplateFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchFlowTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchFlowTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchflowtemplatespaginator)
         """
 
 class SearchSystemInstancesPaginator(AioPaginator):
@@ -203,15 +203,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchsysteminstancespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SystemInstanceFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchSystemInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchSystemInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchsysteminstancespaginator)
         """
 
 class SearchSystemTemplatesPaginator(AioPaginator):
@@ -220,15 +220,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchsystemtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SystemTemplateFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchSystemTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchSystemTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchsystemtemplatespaginator)
         """
 
 class SearchThingsPaginator(AioPaginator):
@@ -238,13 +238,13 @@
     """
 
     def paginate(
         self,
         *,
         entityId: str,
         namespaceVersion: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchThingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchThings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchthingspaginator)
         """
```

### Comparing `types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph/type_defs.py` & `types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssociateEntityToThingRequestRequestTypeDef",
     "DefinitionDocumentTypeDef",
     "FlowTemplateSummaryTypeDef",
     "ResponseMetadataTypeDef",
     "MetricsConfigurationTypeDef",
     "TagTypeDef",
```

### Comparing `types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph/type_defs.pyi` & `types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph.egg-info/PKG-INFO` & `types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotthingsgraph
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IoTThingsGraph 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IoTThingsGraph 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/
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
 
 <a id="types-aiobotocore-iotthingsgraph"></a>
 
 # types-aiobotocore-iotthingsgraph
 
 [![PyPI - types-aiobotocore-iotthingsgraph](https://img.shields.io/pypi/v/types-aiobotocore-iotthingsgraph.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotthingsgraph)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotthingsgraph.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotthingsgraph)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotthingsgraph)](https://pepy.tech/project/types-aiobotocore-iotthingsgraph)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTThingsGraph 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
+[aiobotocore.IoTThingsGraph 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
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
 [types-aiobotocore-iotthingsgraph docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iotthingsgraph-2.9.0/types_aiobotocore_iotthingsgraph.egg-info/SOURCES.txt` & `types-aiobotocore-iotthingsgraph-2.9.1/types_aiobotocore_iotthingsgraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

