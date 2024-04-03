# Comparing `tmp/types-aiobotocore-inspector2-2.9.0.tar.gz` & `tmp/types-aiobotocore-inspector2-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-inspector2-2.9.0.tar", last modified: Wed Dec 13 19:59:28 2023, max compression
+gzip compressed data, was "types-aiobotocore-inspector2-2.9.1.tar", last modified: Thu Jan 18 01:20:52 2024, max compression
```

## Comparing `types-aiobotocore-inspector2-2.9.0.tar` & `types-aiobotocore-inspector2-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:28.445686 types-aiobotocore-inspector2-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:47:31.000000 types-aiobotocore-inspector2-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14496 2023-12-13 19:59:28.441686 types-aiobotocore-inspector2-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12921 2023-12-13 19:47:31.000000 types-aiobotocore-inspector2-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:28.445686 types-aiobotocore-inspector2-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2023-12-13 19:47:31.000000 types-aiobotocore-inspector2-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:28.441686 types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2/
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2023-12-13 19:47:31.000000 types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2023-12-13 19:47:31.000000 types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      944 2023-12-13 19:47:31.000000 types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38669 2023-12-13 19:47:31.000000 types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    38665 2023-12-13 19:47:31.000000 types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18394 2023-12-13 19:47:33.000000 types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    18392 2023-12-13 19:47:31.000000 types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13231 2023-12-13 19:47:31.000000 types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13219 2023-12-13 19:47:31.000000 types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:47:31.000000 types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    70245 2023-12-13 19:47:34.000000 types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    70244 2023-12-13 19:47:33.000000 types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:47:31.000000 types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:28.441686 types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14496 2023-12-13 19:59:28.000000 types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      870 2023-12-13 19:59:28.000000 types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:28.000000 types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:28.000000 types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:28.000000 types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-13 19:59:28.000000 types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:52.241289 types-aiobotocore-inspector2-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:09:22.000000 types-aiobotocore-inspector2-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14516 2024-01-18 01:20:52.241289 types-aiobotocore-inspector2-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12921 2024-01-18 01:09:22.000000 types-aiobotocore-inspector2-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:52.241289 types-aiobotocore-inspector2-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-01-18 01:09:22.000000 types-aiobotocore-inspector2-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:52.237289 types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-01-18 01:09:22.000000 types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-01-18 01:09:22.000000 types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-01-18 01:09:22.000000 types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38679 2024-01-18 01:09:22.000000 types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38676 2024-01-18 01:09:22.000000 types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18392 2024-01-18 01:09:22.000000 types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18392 2024-01-18 01:09:22.000000 types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13236 2024-01-18 01:09:22.000000 types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13225 2024-01-18 01:09:22.000000 types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:09:22.000000 types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    70244 2024-01-18 01:09:25.000000 types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70244 2024-01-18 01:09:25.000000 types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:09:22.000000 types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:52.237289 types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14516 2024-01-18 01:20:52.000000 types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-01-18 01:20:52.000000 types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:52.000000 types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:52.000000 types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:52.000000 types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-18 01:20:52.000000 types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-inspector2-2.9.0/LICENSE` & `types-aiobotocore-inspector2-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-inspector2-2.9.0/PKG-INFO` & `types-aiobotocore-inspector2-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-inspector2
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Inspector2 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Inspector2 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/
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
 
 <a id="types-aiobotocore-inspector2"></a>
 
 # types-aiobotocore-inspector2
 
 [![PyPI - types-aiobotocore-inspector2](https://img.shields.io/pypi/v/types-aiobotocore-inspector2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-inspector2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-inspector2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-inspector2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-inspector2)](https://pepy.tech/project/types-aiobotocore-inspector2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Inspector2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
+[aiobotocore.Inspector2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
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
 [types-aiobotocore-inspector2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-inspector2-2.9.0/README.md` & `types-aiobotocore-inspector2-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-inspector2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-inspector2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-inspector2)](https://pepy.tech/project/types-aiobotocore-inspector2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Inspector2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
+[aiobotocore.Inspector2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
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
 [types-aiobotocore-inspector2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-inspector2-2.9.0/setup.py` & `types-aiobotocore-inspector2-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-inspector2",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_inspector2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Inspector2 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.Inspector2 2.9.1 service generated with"
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
     keywords="aiobotocore inspector2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_inspector2": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2/__init__.py` & `types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     ListMembersPaginator,
     ListUsageTotalsPaginator,
     SearchVulnerabilitiesPaginator,
 )
 
 Client = Inspector2Client
 
-
 __all__ = (
     "Client",
     "Inspector2Client",
     "ListAccountPermissionsPaginator",
     "ListCoveragePaginator",
     "ListCoverageStatisticsPaginator",
     "ListDelegatedAdminAccountsPaginator",
```

### Comparing `types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2/__init__.pyi` & `types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2/__main__.py` & `types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Inspector2 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Inspector2 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2\nOther"
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

### Comparing `types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2/client.py` & `types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("Inspector2Client",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -257,43 +256,43 @@
         self,
         *,
         action: FilterActionType,
         filterCriteria: FilterCriteriaTypeDef,
         name: str,
         description: str = ...,
         reason: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateFilterResponseTypeDef:
         """
         Creates a filter resource using specified filter criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#create_filter)
         """
 
     async def create_findings_report(
         self,
         *,
         reportFormat: ReportFormatType,
         s3Destination: DestinationTypeDef,
-        filterCriteria: FilterCriteriaTypeDef = ...
+        filterCriteria: FilterCriteriaTypeDef = ...,
     ) -> CreateFindingsReportResponseTypeDef:
         """
         Creates a finding report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_findings_report)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#create_findings_report)
         """
 
     async def create_sbom_export(
         self,
         *,
         reportFormat: SbomReportFormatType,
         s3Destination: DestinationTypeDef,
-        resourceFilterCriteria: ResourceFilterCriteriaTypeDef = ...
+        resourceFilterCriteria: ResourceFilterCriteriaTypeDef = ...,
     ) -> CreateSbomExportResponseTypeDef:
         """
         Creates a software bill of materials (SBOM) report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_sbom_export)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#create_sbom_export)
         """
@@ -317,15 +316,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#describe_organization_configuration)
         """
 
     async def disable(
         self,
         *,
         accountIds: Sequence[str] = ...,
-        resourceTypes: Sequence[ResourceScanTypeType] = ...
+        resourceTypes: Sequence[ResourceScanTypeType] = ...,
     ) -> DisableResponseTypeDef:
         """
         Disables Amazon Inspector scans for one or more Amazon Web Services accounts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.disable)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#disable)
         """
@@ -349,15 +348,15 @@
         """
 
     async def enable(
         self,
         *,
         resourceTypes: Sequence[ResourceScanTypeType],
         accountIds: Sequence[str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> EnableResponseTypeDef:
         """
         Enables Amazon Inspector scans for one or more Amazon Web Services accounts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.enable)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#enable)
         """
@@ -464,29 +463,29 @@
         """
 
     async def list_coverage(
         self,
         *,
         filterCriteria: CoverageFilterCriteriaTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListCoverageResponseTypeDef:
         """
         Lists coverage details for you environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_coverage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#list_coverage)
         """
 
     async def list_coverage_statistics(
         self,
         *,
         filterCriteria: CoverageFilterCriteriaTypeDef = ...,
         groupBy: GroupKeyType = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListCoverageStatisticsResponseTypeDef:
         """
         Lists Amazon Inspector coverage statistics for your environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_coverage_statistics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#list_coverage_statistics)
         """
@@ -504,15 +503,15 @@
 
     async def list_filters(
         self,
         *,
         action: FilterActionType = ...,
         arns: Sequence[str] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListFiltersResponseTypeDef:
         """
         Lists the filters associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_filters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#list_filters)
         """
@@ -520,30 +519,30 @@
     async def list_finding_aggregations(
         self,
         *,
         aggregationType: AggregationTypeType,
         accountIds: Sequence[StringFilterTypeDef] = ...,
         aggregationRequest: AggregationRequestTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListFindingAggregationsResponseTypeDef:
         """
         Lists aggregated finding data for your environment based on specific criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_finding_aggregations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#list_finding_aggregations)
         """
 
     async def list_findings(
         self,
         *,
         filterCriteria: FilterCriteriaTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        sortCriteria: SortCriteriaTypeDef = ...
+        sortCriteria: SortCriteriaTypeDef = ...,
     ) -> ListFindingsResponseTypeDef:
         """
         Lists findings for your environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_findings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#list_findings)
         """
@@ -652,15 +651,15 @@
         self,
         *,
         filterArn: str,
         action: FilterActionType = ...,
         description: str = ...,
         filterCriteria: FilterCriteriaTypeDef = ...,
         name: str = ...,
-        reason: str = ...
+        reason: str = ...,
     ) -> UpdateFilterResponseTypeDef:
         """
         Specifies the action that is to be applied to the findings that match the
         filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#update_filter)
```

### Comparing `types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2/client.pyi` & `types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -253,43 +253,43 @@
         self,
         *,
         action: FilterActionType,
         filterCriteria: FilterCriteriaTypeDef,
         name: str,
         description: str = ...,
         reason: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateFilterResponseTypeDef:
         """
         Creates a filter resource using specified filter criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#create_filter)
         """
 
     async def create_findings_report(
         self,
         *,
         reportFormat: ReportFormatType,
         s3Destination: DestinationTypeDef,
-        filterCriteria: FilterCriteriaTypeDef = ...
+        filterCriteria: FilterCriteriaTypeDef = ...,
     ) -> CreateFindingsReportResponseTypeDef:
         """
         Creates a finding report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_findings_report)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#create_findings_report)
         """
 
     async def create_sbom_export(
         self,
         *,
         reportFormat: SbomReportFormatType,
         s3Destination: DestinationTypeDef,
-        resourceFilterCriteria: ResourceFilterCriteriaTypeDef = ...
+        resourceFilterCriteria: ResourceFilterCriteriaTypeDef = ...,
     ) -> CreateSbomExportResponseTypeDef:
         """
         Creates a software bill of materials (SBOM) report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_sbom_export)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#create_sbom_export)
         """
@@ -313,15 +313,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#describe_organization_configuration)
         """
 
     async def disable(
         self,
         *,
         accountIds: Sequence[str] = ...,
-        resourceTypes: Sequence[ResourceScanTypeType] = ...
+        resourceTypes: Sequence[ResourceScanTypeType] = ...,
     ) -> DisableResponseTypeDef:
         """
         Disables Amazon Inspector scans for one or more Amazon Web Services accounts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.disable)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#disable)
         """
@@ -345,15 +345,15 @@
         """
 
     async def enable(
         self,
         *,
         resourceTypes: Sequence[ResourceScanTypeType],
         accountIds: Sequence[str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> EnableResponseTypeDef:
         """
         Enables Amazon Inspector scans for one or more Amazon Web Services accounts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.enable)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#enable)
         """
@@ -460,29 +460,29 @@
         """
 
     async def list_coverage(
         self,
         *,
         filterCriteria: CoverageFilterCriteriaTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListCoverageResponseTypeDef:
         """
         Lists coverage details for you environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_coverage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#list_coverage)
         """
 
     async def list_coverage_statistics(
         self,
         *,
         filterCriteria: CoverageFilterCriteriaTypeDef = ...,
         groupBy: GroupKeyType = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListCoverageStatisticsResponseTypeDef:
         """
         Lists Amazon Inspector coverage statistics for your environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_coverage_statistics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#list_coverage_statistics)
         """
@@ -500,15 +500,15 @@
 
     async def list_filters(
         self,
         *,
         action: FilterActionType = ...,
         arns: Sequence[str] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListFiltersResponseTypeDef:
         """
         Lists the filters associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_filters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#list_filters)
         """
@@ -516,30 +516,30 @@
     async def list_finding_aggregations(
         self,
         *,
         aggregationType: AggregationTypeType,
         accountIds: Sequence[StringFilterTypeDef] = ...,
         aggregationRequest: AggregationRequestTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListFindingAggregationsResponseTypeDef:
         """
         Lists aggregated finding data for your environment based on specific criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_finding_aggregations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#list_finding_aggregations)
         """
 
     async def list_findings(
         self,
         *,
         filterCriteria: FilterCriteriaTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        sortCriteria: SortCriteriaTypeDef = ...
+        sortCriteria: SortCriteriaTypeDef = ...,
     ) -> ListFindingsResponseTypeDef:
         """
         Lists findings for your environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_findings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#list_findings)
         """
@@ -648,15 +648,15 @@
         self,
         *,
         filterArn: str,
         action: FilterActionType = ...,
         description: str = ...,
         filterCriteria: FilterCriteriaTypeDef = ...,
         name: str = ...,
-        reason: str = ...
+        reason: str = ...,
     ) -> UpdateFilterResponseTypeDef:
         """
         Specifies the action that is to be applied to the findings that match the
         filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#update_filter)
```

### Comparing `types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2/literals.py` & `types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2/literals.py`

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
     "AccountSortByType",
     "AggregationFindingTypeType",
     "AggregationResourceTypeType",
     "AggregationTypeType",
     "AmiSortByType",
     "ArchitectureType",
@@ -97,15 +96,14 @@
     "Inspector2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AccountSortByType = Literal["ALL", "CRITICAL", "HIGH"]
 AggregationFindingTypeType = Literal[
     "CODE_VULNERABILITY", "NETWORK_REACHABILITY", "PACKAGE_VULNERABILITY"
 ]
 AggregationResourceTypeType = Literal[
     "AWS_EC2_INSTANCE", "AWS_ECR_CONTAINER_IMAGE", "AWS_LAMBDA_FUNCTION"
 ]
```

### Comparing `types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2/literals.pyi` & `types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2/paginator.py` & `types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,14 @@
     "ListFindingAggregationsPaginator",
     "ListFindingsPaginator",
     "ListMembersPaginator",
     "ListUsageTotalsPaginator",
     "SearchVulnerabilitiesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -110,15 +109,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listcoveragepaginator)
     """
 
     def paginate(
         self,
         *,
         filterCriteria: CoverageFilterCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCoverageResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListCoverage.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listcoveragepaginator)
         """
 
 
@@ -129,15 +128,15 @@
     """
 
     def paginate(
         self,
         *,
         filterCriteria: CoverageFilterCriteriaTypeDef = ...,
         groupBy: GroupKeyType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCoverageStatisticsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListCoverageStatistics.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listcoveragestatisticspaginator)
         """
 
 
@@ -163,15 +162,15 @@
     """
 
     def paginate(
         self,
         *,
         action: FilterActionType = ...,
         arns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFiltersResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFilters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listfilterspaginator)
         """
 
 
@@ -183,15 +182,15 @@
 
     def paginate(
         self,
         *,
         aggregationType: AggregationTypeType,
         accountIds: Sequence[StringFilterTypeDef] = ...,
         aggregationRequest: AggregationRequestTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFindingAggregationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindingAggregations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listfindingaggregationspaginator)
         """
 
 
@@ -202,15 +201,15 @@
     """
 
     def paginate(
         self,
         *,
         filterCriteria: FilterCriteriaPaginatorTypeDef = ...,
         sortCriteria: SortCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listfindingspaginator)
         """
 
 
@@ -250,13 +249,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#searchvulnerabilitiespaginator)
     """
 
     def paginate(
         self,
         *,
         filterCriteria: SearchVulnerabilitiesFilterCriteriaTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchVulnerabilitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.SearchVulnerabilities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#searchvulnerabilitiespaginator)
         """
```

### Comparing `types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2/paginator.pyi` & `types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listcoveragepaginator)
     """
 
     def paginate(
         self,
         *,
         filterCriteria: CoverageFilterCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCoverageResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListCoverage.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listcoveragepaginator)
         """
 
 class ListCoverageStatisticsPaginator(AioPaginator):
@@ -124,15 +124,15 @@
     """
 
     def paginate(
         self,
         *,
         filterCriteria: CoverageFilterCriteriaTypeDef = ...,
         groupBy: GroupKeyType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCoverageStatisticsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListCoverageStatistics.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listcoveragestatisticspaginator)
         """
 
 class ListDelegatedAdminAccountsPaginator(AioPaginator):
@@ -156,15 +156,15 @@
     """
 
     def paginate(
         self,
         *,
         action: FilterActionType = ...,
         arns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFiltersResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFilters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listfilterspaginator)
         """
 
 class ListFindingAggregationsPaginator(AioPaginator):
@@ -175,15 +175,15 @@
 
     def paginate(
         self,
         *,
         aggregationType: AggregationTypeType,
         accountIds: Sequence[StringFilterTypeDef] = ...,
         aggregationRequest: AggregationRequestTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFindingAggregationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindingAggregations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listfindingaggregationspaginator)
         """
 
 class ListFindingsPaginator(AioPaginator):
@@ -193,15 +193,15 @@
     """
 
     def paginate(
         self,
         *,
         filterCriteria: FilterCriteriaPaginatorTypeDef = ...,
         sortCriteria: SortCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listfindingspaginator)
         """
 
 class ListMembersPaginator(AioPaginator):
@@ -238,13 +238,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#searchvulnerabilitiespaginator)
     """
 
     def paginate(
         self,
         *,
         filterCriteria: SearchVulnerabilitiesFilterCriteriaTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchVulnerabilitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.SearchVulnerabilities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#searchvulnerabilitiespaginator)
         """
```

### Comparing `types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2/type_defs.py` & `types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "SeverityCountsTypeDef",
     "AccountAggregationTypeDef",
     "StateTypeDef",
     "ResourceStatusTypeDef",
     "FindingTypeAggregationTypeDef",
     "StringFilterTypeDef",
```

### Comparing `types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2/type_defs.pyi` & `types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2.egg-info/PKG-INFO` & `types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-inspector2
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Inspector2 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Inspector2 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/
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
 
 <a id="types-aiobotocore-inspector2"></a>
 
 # types-aiobotocore-inspector2
 
 [![PyPI - types-aiobotocore-inspector2](https://img.shields.io/pypi/v/types-aiobotocore-inspector2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-inspector2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-inspector2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-inspector2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-inspector2)](https://pepy.tech/project/types-aiobotocore-inspector2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Inspector2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
+[aiobotocore.Inspector2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
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
 [types-aiobotocore-inspector2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-inspector2-2.9.0/types_aiobotocore_inspector2.egg-info/SOURCES.txt` & `types-aiobotocore-inspector2-2.9.1/types_aiobotocore_inspector2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

