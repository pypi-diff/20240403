# Comparing `tmp/types-aiobotocore-m2-2.9.0.tar.gz` & `tmp/types-aiobotocore-m2-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-m2-2.9.0.tar", last modified: Wed Dec 13 19:59:48 2023, max compression
+gzip compressed data, was "types-aiobotocore-m2-2.9.1.tar", last modified: Thu Jan 18 01:21:10 2024, max compression
```

## Comparing `types-aiobotocore-m2-2.9.0.tar` & `types-aiobotocore-m2-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:48.589503 types-aiobotocore-m2-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:49:33.000000 types-aiobotocore-m2-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14200 2023-12-13 19:59:48.589503 types-aiobotocore-m2-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12637 2023-12-13 19:49:33.000000 types-aiobotocore-m2-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:48.589503 types-aiobotocore-m2-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2023-12-13 19:49:33.000000 types-aiobotocore-m2-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:48.589503 types-aiobotocore-m2-2.9.0/types_aiobotocore_m2/
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2023-12-13 19:49:33.000000 types-aiobotocore-m2-2.9.0/types_aiobotocore_m2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2023-12-13 19:49:33.000000 types-aiobotocore-m2-2.9.0/types_aiobotocore_m2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      941 2023-12-13 19:49:33.000000 types-aiobotocore-m2-2.9.0/types_aiobotocore_m2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30133 2023-12-13 19:49:33.000000 types-aiobotocore-m2-2.9.0/types_aiobotocore_m2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    30129 2023-12-13 19:49:33.000000 types-aiobotocore-m2-2.9.0/types_aiobotocore_m2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10961 2023-12-13 19:49:33.000000 types-aiobotocore-m2-2.9.0/types_aiobotocore_m2/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10959 2023-12-13 19:49:33.000000 types-aiobotocore-m2-2.9.0/types_aiobotocore_m2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11898 2023-12-13 19:49:33.000000 types-aiobotocore-m2-2.9.0/types_aiobotocore_m2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11887 2023-12-13 19:49:33.000000 types-aiobotocore-m2-2.9.0/types_aiobotocore_m2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:49:33.000000 types-aiobotocore-m2-2.9.0/types_aiobotocore_m2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    33885 2023-12-13 19:49:34.000000 types-aiobotocore-m2-2.9.0/types_aiobotocore_m2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    33884 2023-12-13 19:49:34.000000 types-aiobotocore-m2-2.9.0/types_aiobotocore_m2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:49:33.000000 types-aiobotocore-m2-2.9.0/types_aiobotocore_m2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:48.589503 types-aiobotocore-m2-2.9.0/types_aiobotocore_m2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14200 2023-12-13 19:59:48.000000 types-aiobotocore-m2-2.9.0/types_aiobotocore_m2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      718 2023-12-13 19:59:48.000000 types-aiobotocore-m2-2.9.0/types_aiobotocore_m2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:48.000000 types-aiobotocore-m2-2.9.0/types_aiobotocore_m2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:48.000000 types-aiobotocore-m2-2.9.0/types_aiobotocore_m2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:48.000000 types-aiobotocore-m2-2.9.0/types_aiobotocore_m2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-13 19:59:48.000000 types-aiobotocore-m2-2.9.0/types_aiobotocore_m2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:10.857206 types-aiobotocore-m2-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:11:18.000000 types-aiobotocore-m2-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14220 2024-01-18 01:21:10.857206 types-aiobotocore-m2-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12637 2024-01-18 01:11:18.000000 types-aiobotocore-m2-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:10.857206 types-aiobotocore-m2-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-01-18 01:11:18.000000 types-aiobotocore-m2-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:10.857206 types-aiobotocore-m2-2.9.1/types_aiobotocore_m2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-01-18 01:11:18.000000 types-aiobotocore-m2-2.9.1/types_aiobotocore_m2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-01-18 01:11:18.000000 types-aiobotocore-m2-2.9.1/types_aiobotocore_m2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-01-18 01:11:18.000000 types-aiobotocore-m2-2.9.1/types_aiobotocore_m2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30143 2024-01-18 01:11:18.000000 types-aiobotocore-m2-2.9.1/types_aiobotocore_m2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30140 2024-01-18 01:11:18.000000 types-aiobotocore-m2-2.9.1/types_aiobotocore_m2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10959 2024-01-18 01:11:18.000000 types-aiobotocore-m2-2.9.1/types_aiobotocore_m2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10959 2024-01-18 01:11:18.000000 types-aiobotocore-m2-2.9.1/types_aiobotocore_m2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11902 2024-01-18 01:11:18.000000 types-aiobotocore-m2-2.9.1/types_aiobotocore_m2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11892 2024-01-18 01:11:18.000000 types-aiobotocore-m2-2.9.1/types_aiobotocore_m2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:11:18.000000 types-aiobotocore-m2-2.9.1/types_aiobotocore_m2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    33884 2024-01-18 01:11:19.000000 types-aiobotocore-m2-2.9.1/types_aiobotocore_m2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33884 2024-01-18 01:11:19.000000 types-aiobotocore-m2-2.9.1/types_aiobotocore_m2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:11:18.000000 types-aiobotocore-m2-2.9.1/types_aiobotocore_m2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:10.857206 types-aiobotocore-m2-2.9.1/types_aiobotocore_m2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14220 2024-01-18 01:21:10.000000 types-aiobotocore-m2-2.9.1/types_aiobotocore_m2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-01-18 01:21:10.000000 types-aiobotocore-m2-2.9.1/types_aiobotocore_m2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:10.000000 types-aiobotocore-m2-2.9.1/types_aiobotocore_m2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:10.000000 types-aiobotocore-m2-2.9.1/types_aiobotocore_m2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:10.000000 types-aiobotocore-m2-2.9.1/types_aiobotocore_m2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-18 01:21:10.000000 types-aiobotocore-m2-2.9.1/types_aiobotocore_m2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-m2-2.9.0/LICENSE` & `types-aiobotocore-m2-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-m2-2.9.0/PKG-INFO` & `types-aiobotocore-m2-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-m2
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MainframeModernization 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MainframeModernization 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/
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
 
 <a id="types-aiobotocore-m2"></a>
 
 # types-aiobotocore-m2
 
 [![PyPI - types-aiobotocore-m2](https://img.shields.io/pypi/v/types-aiobotocore-m2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-m2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-m2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-m2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-m2)](https://pepy.tech/project/types-aiobotocore-m2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MainframeModernization 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
+[aiobotocore.MainframeModernization 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
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
 [types-aiobotocore-m2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-m2-2.9.0/README.md` & `types-aiobotocore-m2-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-m2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-m2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-m2)](https://pepy.tech/project/types-aiobotocore-m2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MainframeModernization 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
+[aiobotocore.MainframeModernization 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
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
 [types-aiobotocore-m2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-m2-2.9.0/setup.py` & `types-aiobotocore-m2-2.9.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-m2",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_m2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MainframeModernization 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.MainframeModernization 2.9.1 service generated with"
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
     keywords="aiobotocore m2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_m2": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-m2-2.9.0/types_aiobotocore_m2/__init__.py` & `types-aiobotocore-m2-2.9.1/types_aiobotocore_m2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
     ListDeploymentsPaginator,
     ListEngineVersionsPaginator,
     ListEnvironmentsPaginator,
 )
 
 Client = MainframeModernizationClient
 
-
 __all__ = (
     "Client",
     "ListApplicationVersionsPaginator",
     "ListApplicationsPaginator",
     "ListBatchJobDefinitionsPaginator",
     "ListBatchJobExecutionsPaginator",
     "ListDataSetImportHistoryPaginator",
```

### Comparing `types-aiobotocore-m2-2.9.0/types_aiobotocore_m2/__init__.pyi` & `types-aiobotocore-m2-2.9.1/types_aiobotocore_m2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-m2-2.9.0/types_aiobotocore_m2/__main__.py` & `types-aiobotocore-m2-2.9.1/types_aiobotocore_m2/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MainframeModernization 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.MainframeModernization 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization\nOther"
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

### Comparing `types-aiobotocore-m2-2.9.0/types_aiobotocore_m2/client.py` & `types-aiobotocore-m2-2.9.1/types_aiobotocore_m2/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,15 +68,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("MainframeModernizationClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -146,44 +145,44 @@
         definition: DefinitionTypeDef,
         engineType: EngineTypeType,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         kmsKeyId: str = ...,
         roleArn: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates a new application with given parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/client/#create_application)
         """
 
     async def create_data_set_import_task(
         self,
         *,
         applicationId: str,
         importConfig: DataSetImportConfigTypeDef,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateDataSetImportTaskResponseTypeDef:
         """
         Starts a data set import task for a specific application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.create_data_set_import_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/client/#create_data_set_import_task)
         """
 
     async def create_deployment(
         self,
         *,
         applicationId: str,
         applicationVersion: int,
         environmentId: str,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateDeploymentResponseTypeDef:
         """
         Creates and starts a deployment to deploy an application into a runtime
         environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.create_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/client/#create_deployment)
@@ -201,15 +200,15 @@
         highAvailabilityConfig: HighAvailabilityConfigTypeDef = ...,
         kmsKeyId: str = ...,
         preferredMaintenanceWindow: str = ...,
         publiclyAccessible: bool = ...,
         securityGroupIds: Sequence[str] = ...,
         storageConfigurations: Sequence[StorageConfigurationTypeDef] = ...,
         subnetIds: Sequence[str] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateEnvironmentResponseTypeDef:
         """
         Creates a runtime environment for a given runtime engine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.create_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/client/#create_environment)
         """
@@ -344,15 +343,15 @@
 
     async def list_applications(
         self,
         *,
         environmentId: str = ...,
         maxResults: int = ...,
         names: Sequence[str] = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListApplicationsResponseTypeDef:
         """
         Lists the applications associated with a specific Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_applications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/client/#list_applications)
         """
@@ -375,15 +374,15 @@
         applicationId: str,
         executionIds: Sequence[str] = ...,
         jobName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         startedAfter: TimestampTypeDef = ...,
         startedBefore: TimestampTypeDef = ...,
-        status: BatchJobExecutionStatusType = ...
+        status: BatchJobExecutionStatusType = ...,
     ) -> ListBatchJobExecutionsResponseTypeDef:
         """
         Lists historical, current, and scheduled batch job executions for a specific
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_batch_job_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/client/#list_batch_job_executions)
@@ -402,15 +401,15 @@
     async def list_data_sets(
         self,
         *,
         applicationId: str,
         maxResults: int = ...,
         nameFilter: str = ...,
         nextToken: str = ...,
-        prefix: str = ...
+        prefix: str = ...,
     ) -> ListDataSetsResponseTypeDef:
         """
         Lists the data sets imported for a specific application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_data_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/client/#list_data_sets)
         """
@@ -437,15 +436,15 @@
 
     async def list_environments(
         self,
         *,
         engineType: EngineTypeType = ...,
         maxResults: int = ...,
         names: Sequence[str] = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListEnvironmentsResponseTypeDef:
         """
         Lists the runtime environments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_environments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/client/#list_environments)
         """
@@ -469,15 +468,15 @@
         """
 
     async def start_batch_job(
         self,
         *,
         applicationId: str,
         batchJobIdentifier: BatchJobIdentifierTypeDef,
-        jobParams: Mapping[str, str] = ...
+        jobParams: Mapping[str, str] = ...,
     ) -> StartBatchJobResponseTypeDef:
         """
         Starts a batch job and returns the unique identifier of this execution of the
         batch
         job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.start_batch_job)
@@ -512,15 +511,15 @@
 
     async def update_application(
         self,
         *,
         applicationId: str,
         currentApplicationVersion: int,
         definition: DefinitionTypeDef = ...,
-        description: str = ...
+        description: str = ...,
     ) -> UpdateApplicationResponseTypeDef:
         """
         Updates an application and creates a new version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.update_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/client/#update_application)
         """
@@ -530,15 +529,15 @@
         *,
         environmentId: str,
         applyDuringMaintenanceWindow: bool = ...,
         desiredCapacity: int = ...,
         engineVersion: str = ...,
         forceUpdate: bool = ...,
         instanceType: str = ...,
-        preferredMaintenanceWindow: str = ...
+        preferredMaintenanceWindow: str = ...,
     ) -> UpdateEnvironmentResponseTypeDef:
         """
         Updates the configuration details for a specific runtime environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.update_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/client/#update_environment)
         """
```

### Comparing `types-aiobotocore-m2-2.9.0/types_aiobotocore_m2/client.pyi` & `types-aiobotocore-m2-2.9.1/types_aiobotocore_m2/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -142,44 +142,44 @@
         definition: DefinitionTypeDef,
         engineType: EngineTypeType,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         kmsKeyId: str = ...,
         roleArn: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates a new application with given parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/client/#create_application)
         """
 
     async def create_data_set_import_task(
         self,
         *,
         applicationId: str,
         importConfig: DataSetImportConfigTypeDef,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateDataSetImportTaskResponseTypeDef:
         """
         Starts a data set import task for a specific application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.create_data_set_import_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/client/#create_data_set_import_task)
         """
 
     async def create_deployment(
         self,
         *,
         applicationId: str,
         applicationVersion: int,
         environmentId: str,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateDeploymentResponseTypeDef:
         """
         Creates and starts a deployment to deploy an application into a runtime
         environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.create_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/client/#create_deployment)
@@ -197,15 +197,15 @@
         highAvailabilityConfig: HighAvailabilityConfigTypeDef = ...,
         kmsKeyId: str = ...,
         preferredMaintenanceWindow: str = ...,
         publiclyAccessible: bool = ...,
         securityGroupIds: Sequence[str] = ...,
         storageConfigurations: Sequence[StorageConfigurationTypeDef] = ...,
         subnetIds: Sequence[str] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateEnvironmentResponseTypeDef:
         """
         Creates a runtime environment for a given runtime engine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.create_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/client/#create_environment)
         """
@@ -340,15 +340,15 @@
 
     async def list_applications(
         self,
         *,
         environmentId: str = ...,
         maxResults: int = ...,
         names: Sequence[str] = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListApplicationsResponseTypeDef:
         """
         Lists the applications associated with a specific Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_applications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/client/#list_applications)
         """
@@ -371,15 +371,15 @@
         applicationId: str,
         executionIds: Sequence[str] = ...,
         jobName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         startedAfter: TimestampTypeDef = ...,
         startedBefore: TimestampTypeDef = ...,
-        status: BatchJobExecutionStatusType = ...
+        status: BatchJobExecutionStatusType = ...,
     ) -> ListBatchJobExecutionsResponseTypeDef:
         """
         Lists historical, current, and scheduled batch job executions for a specific
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_batch_job_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/client/#list_batch_job_executions)
@@ -398,15 +398,15 @@
     async def list_data_sets(
         self,
         *,
         applicationId: str,
         maxResults: int = ...,
         nameFilter: str = ...,
         nextToken: str = ...,
-        prefix: str = ...
+        prefix: str = ...,
     ) -> ListDataSetsResponseTypeDef:
         """
         Lists the data sets imported for a specific application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_data_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/client/#list_data_sets)
         """
@@ -433,15 +433,15 @@
 
     async def list_environments(
         self,
         *,
         engineType: EngineTypeType = ...,
         maxResults: int = ...,
         names: Sequence[str] = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListEnvironmentsResponseTypeDef:
         """
         Lists the runtime environments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_environments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/client/#list_environments)
         """
@@ -465,15 +465,15 @@
         """
 
     async def start_batch_job(
         self,
         *,
         applicationId: str,
         batchJobIdentifier: BatchJobIdentifierTypeDef,
-        jobParams: Mapping[str, str] = ...
+        jobParams: Mapping[str, str] = ...,
     ) -> StartBatchJobResponseTypeDef:
         """
         Starts a batch job and returns the unique identifier of this execution of the
         batch
         job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.start_batch_job)
@@ -508,15 +508,15 @@
 
     async def update_application(
         self,
         *,
         applicationId: str,
         currentApplicationVersion: int,
         definition: DefinitionTypeDef = ...,
-        description: str = ...
+        description: str = ...,
     ) -> UpdateApplicationResponseTypeDef:
         """
         Updates an application and creates a new version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.update_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/client/#update_application)
         """
@@ -526,15 +526,15 @@
         *,
         environmentId: str,
         applyDuringMaintenanceWindow: bool = ...,
         desiredCapacity: int = ...,
         engineVersion: str = ...,
         forceUpdate: bool = ...,
         instanceType: str = ...,
-        preferredMaintenanceWindow: str = ...
+        preferredMaintenanceWindow: str = ...,
     ) -> UpdateEnvironmentResponseTypeDef:
         """
         Updates the configuration details for a specific runtime environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.update_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/client/#update_environment)
         """
```

### Comparing `types-aiobotocore-m2-2.9.0/types_aiobotocore_m2/literals.py` & `types-aiobotocore-m2-2.9.1/types_aiobotocore_m2/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ApplicationDeploymentLifecycleType",
     "ApplicationLifecycleType",
     "ApplicationVersionLifecycleType",
     "BatchJobExecutionStatusType",
     "BatchJobTypeType",
     "DataSetTaskLifecycleType",
@@ -42,15 +41,14 @@
     "MainframeModernizationServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ApplicationDeploymentLifecycleType = Literal["Deployed", "Deploying"]
 ApplicationLifecycleType = Literal[
     "Available",
     "Created",
     "Creating",
     "Deleting",
     "Deleting From Environment",
```

### Comparing `types-aiobotocore-m2-2.9.0/types_aiobotocore_m2/literals.pyi` & `types-aiobotocore-m2-2.9.1/types_aiobotocore_m2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-m2-2.9.0/types_aiobotocore_m2/paginator.py` & `types-aiobotocore-m2-2.9.1/types_aiobotocore_m2/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,14 @@
     "ListDataSetImportHistoryPaginator",
     "ListDataSetsPaginator",
     "ListDeploymentsPaginator",
     "ListEngineVersionsPaginator",
     "ListEnvironmentsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -102,15 +101,15 @@
     """
 
     def paginate(
         self,
         *,
         environmentId: str = ...,
         names: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listapplicationspaginator)
         """
 
 
@@ -121,15 +120,15 @@
     """
 
     def paginate(
         self,
         *,
         applicationId: str,
         prefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListBatchJobDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListBatchJobDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listbatchjobdefinitionspaginator)
         """
 
 
@@ -144,15 +143,15 @@
         *,
         applicationId: str,
         executionIds: Sequence[str] = ...,
         jobName: str = ...,
         startedAfter: TimestampTypeDef = ...,
         startedBefore: TimestampTypeDef = ...,
         status: BatchJobExecutionStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListBatchJobExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListBatchJobExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listbatchjobexecutionspaginator)
         """
 
 
@@ -179,15 +178,15 @@
 
     def paginate(
         self,
         *,
         applicationId: str,
         nameFilter: str = ...,
         prefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDataSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDataSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listdatasetspaginator)
         """
 
 
@@ -228,13 +227,13 @@
     """
 
     def paginate(
         self,
         *,
         engineType: EngineTypeType = ...,
         names: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListEnvironments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listenvironmentspaginator)
         """
```

### Comparing `types-aiobotocore-m2-2.9.0/types_aiobotocore_m2/paginator.pyi` & `types-aiobotocore-m2-2.9.1/types_aiobotocore_m2/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     """
 
     def paginate(
         self,
         *,
         environmentId: str = ...,
         names: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listapplicationspaginator)
         """
 
 class ListBatchJobDefinitionsPaginator(AioPaginator):
@@ -116,15 +116,15 @@
     """
 
     def paginate(
         self,
         *,
         applicationId: str,
         prefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListBatchJobDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListBatchJobDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listbatchjobdefinitionspaginator)
         """
 
 class ListBatchJobExecutionsPaginator(AioPaginator):
@@ -138,15 +138,15 @@
         *,
         applicationId: str,
         executionIds: Sequence[str] = ...,
         jobName: str = ...,
         startedAfter: TimestampTypeDef = ...,
         startedBefore: TimestampTypeDef = ...,
         status: BatchJobExecutionStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListBatchJobExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListBatchJobExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listbatchjobexecutionspaginator)
         """
 
 class ListDataSetImportHistoryPaginator(AioPaginator):
@@ -171,15 +171,15 @@
 
     def paginate(
         self,
         *,
         applicationId: str,
         nameFilter: str = ...,
         prefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDataSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDataSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listdatasetspaginator)
         """
 
 class ListDeploymentsPaginator(AioPaginator):
@@ -217,13 +217,13 @@
     """
 
     def paginate(
         self,
         *,
         engineType: EngineTypeType = ...,
         names: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListEnvironments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listenvironmentspaginator)
         """
```

### Comparing `types-aiobotocore-m2-2.9.0/types_aiobotocore_m2/type_defs.py` & `types-aiobotocore-m2-2.9.1/types_aiobotocore_m2/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AlternateKeyTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationVersionSummaryTypeDef",
     "FileBatchJobDefinitionTypeDef",
     "ScriptBatchJobDefinitionTypeDef",
     "FileBatchJobIdentifierTypeDef",
```

### Comparing `types-aiobotocore-m2-2.9.0/types_aiobotocore_m2/type_defs.pyi` & `types-aiobotocore-m2-2.9.1/types_aiobotocore_m2/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-m2-2.9.0/types_aiobotocore_m2.egg-info/PKG-INFO` & `types-aiobotocore-m2-2.9.1/types_aiobotocore_m2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-m2
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MainframeModernization 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MainframeModernization 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/
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
 
 <a id="types-aiobotocore-m2"></a>
 
 # types-aiobotocore-m2
 
 [![PyPI - types-aiobotocore-m2](https://img.shields.io/pypi/v/types-aiobotocore-m2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-m2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-m2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-m2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-m2)](https://pepy.tech/project/types-aiobotocore-m2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MainframeModernization 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
+[aiobotocore.MainframeModernization 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
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
 [types-aiobotocore-m2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-m2-2.9.0/types_aiobotocore_m2.egg-info/SOURCES.txt` & `types-aiobotocore-m2-2.9.1/types_aiobotocore_m2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

