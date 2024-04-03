# Comparing `tmp/types-aiobotocore-grafana-2.9.0.tar.gz` & `tmp/types-aiobotocore-grafana-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-grafana-2.9.0.tar", last modified: Wed Dec 13 19:59:23 2023, max compression
+gzip compressed data, was "types-aiobotocore-grafana-2.9.1.tar", last modified: Thu Jan 18 01:20:48 2024, max compression
```

## Comparing `types-aiobotocore-grafana-2.9.0.tar` & `types-aiobotocore-grafana-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:23.941724 types-aiobotocore-grafana-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:46:57.000000 types-aiobotocore-grafana-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13290 2023-12-13 19:59:23.941724 types-aiobotocore-grafana-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11720 2023-12-13 19:46:57.000000 types-aiobotocore-grafana-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:23.941724 types-aiobotocore-grafana-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-12-13 19:46:57.000000 types-aiobotocore-grafana-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:23.941724 types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-12-13 19:46:57.000000 types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-12-13 19:46:57.000000 types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-12-13 19:46:57.000000 types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19444 2023-12-13 19:46:57.000000 types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    19440 2023-12-13 19:46:57.000000 types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10041 2023-12-13 19:46:57.000000 types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10039 2023-12-13 19:46:57.000000 types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2023-12-13 19:46:57.000000 types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4333 2023-12-13 19:46:57.000000 types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:46:57.000000 types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    17875 2023-12-13 19:46:57.000000 types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17874 2023-12-13 19:46:57.000000 types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:46:57.000000 types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:23.941724 types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13290 2023-12-13 19:59:23.000000 types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-12-13 19:59:23.000000 types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:23.000000 types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:23.000000 types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:23.000000 types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-13 19:59:23.000000 types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:48.025308 types-aiobotocore-grafana-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:08:51.000000 types-aiobotocore-grafana-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13310 2024-01-18 01:20:48.025308 types-aiobotocore-grafana-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-01-18 01:08:51.000000 types-aiobotocore-grafana-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:48.025308 types-aiobotocore-grafana-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-18 01:08:50.000000 types-aiobotocore-grafana-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:48.025308 types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-01-18 01:08:51.000000 types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-01-18 01:08:51.000000 types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-01-18 01:08:51.000000 types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19447 2024-01-18 01:08:51.000000 types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19444 2024-01-18 01:08:51.000000 types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10039 2024-01-18 01:08:51.000000 types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10039 2024-01-18 01:08:51.000000 types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-01-18 01:08:51.000000 types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-01-18 01:08:51.000000 types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:08:51.000000 types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    17874 2024-01-18 01:08:51.000000 types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17874 2024-01-18 01:08:51.000000 types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:08:51.000000 types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:48.025308 types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13310 2024-01-18 01:20:47.000000 types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-01-18 01:20:47.000000 types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:47.000000 types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:47.000000 types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:47.000000 types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-18 01:20:47.000000 types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-grafana-2.9.0/LICENSE` & `types-aiobotocore-grafana-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-grafana-2.9.0/PKG-INFO` & `types-aiobotocore-grafana-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-grafana
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ManagedGrafana 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ManagedGrafana 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/
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
 
 <a id="types-aiobotocore-grafana"></a>
 
 # types-aiobotocore-grafana
 
 [![PyPI - types-aiobotocore-grafana](https://img.shields.io/pypi/v/types-aiobotocore-grafana.svg?color=blue)](https://pypi.org/project/types-aiobotocore-grafana)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-grafana.svg?color=blue)](https://pypi.org/project/types-aiobotocore-grafana)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-grafana)](https://pepy.tech/project/types-aiobotocore-grafana)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ManagedGrafana 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
+[aiobotocore.ManagedGrafana 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
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
 [types-aiobotocore-grafana docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-grafana-2.9.0/README.md` & `types-aiobotocore-grafana-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-grafana.svg?color=blue)](https://pypi.org/project/types-aiobotocore-grafana)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-grafana)](https://pepy.tech/project/types-aiobotocore-grafana)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ManagedGrafana 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
+[aiobotocore.ManagedGrafana 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
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
 [types-aiobotocore-grafana docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-grafana-2.9.0/setup.py` & `types-aiobotocore-grafana-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-grafana",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_grafana"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ManagedGrafana 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ManagedGrafana 2.9.1 service generated with"
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
     keywords="aiobotocore grafana type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_grafana": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana/__init__.py` & `types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 """
 
 from .client import ManagedGrafanaClient
 from .paginator import ListPermissionsPaginator, ListVersionsPaginator, ListWorkspacesPaginator
 
 Client = ManagedGrafanaClient
 
-
 __all__ = (
     "Client",
     "ListPermissionsPaginator",
     "ListVersionsPaginator",
     "ListWorkspacesPaginator",
     "ManagedGrafanaClient",
 )
```

### Comparing `types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana/__init__.pyi` & `types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana/__main__.py` & `types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ManagedGrafana 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ManagedGrafana 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana\nOther"
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

### Comparing `types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana/client.py` & `types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ManagedGrafanaClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -139,15 +138,15 @@
         tags: Mapping[str, str] = ...,
         vpcConfiguration: VpcConfigurationTypeDef = ...,
         workspaceDataSources: Sequence[DataSourceTypeType] = ...,
         workspaceDescription: str = ...,
         workspaceName: str = ...,
         workspaceNotificationDestinations: Sequence[Literal["SNS"]] = ...,
         workspaceOrganizationalUnits: Sequence[str] = ...,
-        workspaceRoleArn: str = ...
+        workspaceRoleArn: str = ...,
     ) -> CreateWorkspaceResponseTypeDef:
         """
         Creates a *workspace*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.create_workspace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#create_workspace)
         """
@@ -238,15 +237,15 @@
         self,
         *,
         workspaceId: str,
         groupId: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         userId: str = ...,
-        userType: UserTypeType = ...
+        userType: UserTypeType = ...,
     ) -> ListPermissionsResponseTypeDef:
         """
         Lists the users and groups who have the Grafana `Admin` and `Editor` roles in
         this
         workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.list_permissions)
@@ -329,29 +328,29 @@
         stackSetName: str = ...,
         vpcConfiguration: VpcConfigurationTypeDef = ...,
         workspaceDataSources: Sequence[DataSourceTypeType] = ...,
         workspaceDescription: str = ...,
         workspaceName: str = ...,
         workspaceNotificationDestinations: Sequence[Literal["SNS"]] = ...,
         workspaceOrganizationalUnits: Sequence[str] = ...,
-        workspaceRoleArn: str = ...
+        workspaceRoleArn: str = ...,
     ) -> UpdateWorkspaceResponseTypeDef:
         """
         Modifies an existing Amazon Managed Grafana workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.update_workspace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#update_workspace)
         """
 
     async def update_workspace_authentication(
         self,
         *,
         authenticationProviders: Sequence[AuthenticationProviderTypesType],
         workspaceId: str,
-        samlConfiguration: SamlConfigurationTypeDef = ...
+        samlConfiguration: SamlConfigurationTypeDef = ...,
     ) -> UpdateWorkspaceAuthenticationResponseTypeDef:
         """
         Use this operation to define the identity provider (IdP) that this workspace
         authenticates users from, using
         SAML.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.update_workspace_authentication)
```

### Comparing `types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana/client.pyi` & `types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         tags: Mapping[str, str] = ...,
         vpcConfiguration: VpcConfigurationTypeDef = ...,
         workspaceDataSources: Sequence[DataSourceTypeType] = ...,
         workspaceDescription: str = ...,
         workspaceName: str = ...,
         workspaceNotificationDestinations: Sequence[Literal["SNS"]] = ...,
         workspaceOrganizationalUnits: Sequence[str] = ...,
-        workspaceRoleArn: str = ...
+        workspaceRoleArn: str = ...,
     ) -> CreateWorkspaceResponseTypeDef:
         """
         Creates a *workspace*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.create_workspace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#create_workspace)
         """
@@ -234,15 +234,15 @@
         self,
         *,
         workspaceId: str,
         groupId: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         userId: str = ...,
-        userType: UserTypeType = ...
+        userType: UserTypeType = ...,
     ) -> ListPermissionsResponseTypeDef:
         """
         Lists the users and groups who have the Grafana `Admin` and `Editor` roles in
         this
         workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.list_permissions)
@@ -325,29 +325,29 @@
         stackSetName: str = ...,
         vpcConfiguration: VpcConfigurationTypeDef = ...,
         workspaceDataSources: Sequence[DataSourceTypeType] = ...,
         workspaceDescription: str = ...,
         workspaceName: str = ...,
         workspaceNotificationDestinations: Sequence[Literal["SNS"]] = ...,
         workspaceOrganizationalUnits: Sequence[str] = ...,
-        workspaceRoleArn: str = ...
+        workspaceRoleArn: str = ...,
     ) -> UpdateWorkspaceResponseTypeDef:
         """
         Modifies an existing Amazon Managed Grafana workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.update_workspace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#update_workspace)
         """
 
     async def update_workspace_authentication(
         self,
         *,
         authenticationProviders: Sequence[AuthenticationProviderTypesType],
         workspaceId: str,
-        samlConfiguration: SamlConfigurationTypeDef = ...
+        samlConfiguration: SamlConfigurationTypeDef = ...,
     ) -> UpdateWorkspaceAuthenticationResponseTypeDef:
         """
         Use this operation to define the identity provider (IdP) that this workspace
         authenticates users from, using
         SAML.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.update_workspace_authentication)
```

### Comparing `types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana/literals.py` & `types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana/literals.py`

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
     "AccountAccessTypeType",
     "AuthenticationProviderTypesType",
     "DataSourceTypeType",
     "LicenseTypeType",
     "ListPermissionsPaginatorName",
     "ListVersionsPaginatorName",
@@ -38,15 +37,14 @@
     "ManagedGrafanaServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AccountAccessTypeType = Literal["CURRENT_ACCOUNT", "ORGANIZATION"]
 AuthenticationProviderTypesType = Literal["AWS_SSO", "SAML"]
 DataSourceTypeType = Literal[
     "AMAZON_OPENSEARCH_SERVICE",
     "ATHENA",
     "CLOUDWATCH",
     "PROMETHEUS",
```

### Comparing `types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana/literals.pyi` & `types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana/paginator.py` & `types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     ListVersionsResponseTypeDef,
     ListWorkspacesResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListPermissionsPaginator", "ListVersionsPaginator", "ListWorkspacesPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -60,15 +59,15 @@
     def paginate(
         self,
         *,
         workspaceId: str,
         groupId: str = ...,
         userId: str = ...,
         userType: UserTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListPermissions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/paginators/#listpermissionspaginator)
         """
```

### Comparing `types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana/paginator.pyi` & `types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     def paginate(
         self,
         *,
         workspaceId: str,
         groupId: str = ...,
         userId: str = ...,
         userType: UserTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListPermissions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/paginators/#listpermissionspaginator)
         """
 
 class ListVersionsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana/type_defs.py` & `types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssertionAttributesTypeDef",
     "AssociateLicenseRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AwsSsoAuthenticationTypeDef",
     "AuthenticationSummaryTypeDef",
     "CreateWorkspaceApiKeyRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana/type_defs.pyi` & `types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana.egg-info/PKG-INFO` & `types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-grafana
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ManagedGrafana 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ManagedGrafana 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/
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
 
 <a id="types-aiobotocore-grafana"></a>
 
 # types-aiobotocore-grafana
 
 [![PyPI - types-aiobotocore-grafana](https://img.shields.io/pypi/v/types-aiobotocore-grafana.svg?color=blue)](https://pypi.org/project/types-aiobotocore-grafana)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-grafana.svg?color=blue)](https://pypi.org/project/types-aiobotocore-grafana)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-grafana)](https://pepy.tech/project/types-aiobotocore-grafana)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ManagedGrafana 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
+[aiobotocore.ManagedGrafana 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
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
 [types-aiobotocore-grafana docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-grafana-2.9.0/types_aiobotocore_grafana.egg-info/SOURCES.txt` & `types-aiobotocore-grafana-2.9.1/types_aiobotocore_grafana.egg-info/SOURCES.txt`

 * *Files identical despite different names*

