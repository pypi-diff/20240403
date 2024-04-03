# Comparing `tmp/types-aiobotocore-amplify-2.9.0.tar.gz` & `tmp/types-aiobotocore-amplify-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-amplify-2.9.0.tar", last modified: Wed Dec 13 19:58:30 2023, max compression
+gzip compressed data, was "types-aiobotocore-amplify-2.9.1.tar", last modified: Thu Jan 18 01:19:59 2024, max compression
```

## Comparing `types-aiobotocore-amplify-2.9.0.tar` & `types-aiobotocore-amplify-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:30.874127 types-aiobotocore-amplify-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:40:42.000000 types-aiobotocore-amplify-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13353 2023-12-13 19:58:30.874127 types-aiobotocore-amplify-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11790 2023-12-13 19:40:42.000000 types-aiobotocore-amplify-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:30.874127 types-aiobotocore-amplify-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2023-12-13 19:40:42.000000 types-aiobotocore-amplify-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:30.874127 types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify/
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2023-12-13 19:40:42.000000 types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2023-12-13 19:40:42.000000 types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      932 2023-12-13 19:40:42.000000 types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30007 2023-12-13 19:40:43.000000 types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    30003 2023-12-13 19:40:42.000000 types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9668 2023-12-13 19:40:43.000000 types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9666 2023-12-13 19:40:43.000000 types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2023-12-13 19:40:43.000000 types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2023-12-13 19:40:43.000000 types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:40:42.000000 types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    30972 2023-12-13 19:40:43.000000 types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    30971 2023-12-13 19:40:43.000000 types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:40:42.000000 types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:30.874127 types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13353 2023-12-13 19:58:30.000000 types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-12-13 19:58:30.000000 types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:30.000000 types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:30.000000 types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:30.000000 types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-13 19:58:30.000000 types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:59.297532 types-aiobotocore-amplify-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:02:41.000000 types-aiobotocore-amplify-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13373 2024-01-18 01:19:59.297532 types-aiobotocore-amplify-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11790 2024-01-18 01:02:41.000000 types-aiobotocore-amplify-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:19:59.301532 types-aiobotocore-amplify-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-01-18 01:02:41.000000 types-aiobotocore-amplify-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:59.297532 types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-01-18 01:02:41.000000 types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-01-18 01:02:41.000000 types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-01-18 01:02:41.000000 types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30016 2024-01-18 01:02:42.000000 types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30013 2024-01-18 01:02:42.000000 types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-01-18 01:02:42.000000 types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-01-18 01:02:42.000000 types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-01-18 01:02:42.000000 types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-01-18 01:02:42.000000 types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:02:41.000000 types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    30971 2024-01-18 01:02:43.000000 types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30971 2024-01-18 01:02:43.000000 types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:02:41.000000 types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:59.297532 types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13373 2024-01-18 01:19:59.000000 types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-01-18 01:19:59.000000 types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:19:59.000000 types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:19:59.000000 types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:19:59.000000 types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-18 01:19:59.000000 types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-amplify-2.9.0/LICENSE` & `types-aiobotocore-amplify-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-amplify-2.9.0/PKG-INFO` & `types-aiobotocore-amplify-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-amplify
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Amplify 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Amplify 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/
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
 
 <a id="types-aiobotocore-amplify"></a>
 
 # types-aiobotocore-amplify
 
 [![PyPI - types-aiobotocore-amplify](https://img.shields.io/pypi/v/types-aiobotocore-amplify.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amplify)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-amplify.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amplify)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-amplify)](https://pepy.tech/project/types-aiobotocore-amplify)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Amplify 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
+[aiobotocore.Amplify 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
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
 [types-aiobotocore-amplify docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-amplify-2.9.0/README.md` & `types-aiobotocore-amplify-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-amplify.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amplify)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-amplify)](https://pepy.tech/project/types-aiobotocore-amplify)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Amplify 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
+[aiobotocore.Amplify 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
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
 [types-aiobotocore-amplify docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-amplify-2.9.0/setup.py` & `types-aiobotocore-amplify-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-amplify",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_amplify"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Amplify 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Amplify 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore amplify type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_amplify": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify/__init__.py` & `types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     ListBranchesPaginator,
     ListDomainAssociationsPaginator,
     ListJobsPaginator,
 )
 
 Client = AmplifyClient
 
-
 __all__ = (
     "AmplifyClient",
     "Client",
     "ListAppsPaginator",
     "ListBranchesPaginator",
     "ListDomainAssociationsPaginator",
     "ListJobsPaginator",
```

### Comparing `types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify/__init__.pyi` & `types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify/__main__.py` & `types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Amplify 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Amplify 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify\nOther"
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

### Comparing `types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify/client.py` & `types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("AmplifyClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -149,30 +148,30 @@
         basicAuthCredentials: str = ...,
         customRules: Sequence[CustomRuleTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         buildSpec: str = ...,
         customHeaders: str = ...,
         enableAutoBranchCreation: bool = ...,
         autoBranchCreationPatterns: Sequence[str] = ...,
-        autoBranchCreationConfig: AutoBranchCreationConfigTypeDef = ...
+        autoBranchCreationConfig: AutoBranchCreationConfigTypeDef = ...,
     ) -> CreateAppResultTypeDef:
         """
         Creates a new Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.create_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/client/#create_app)
         """
 
     async def create_backend_environment(
         self,
         *,
         appId: str,
         environmentName: str,
         stackName: str = ...,
-        deploymentArtifacts: str = ...
+        deploymentArtifacts: str = ...,
     ) -> CreateBackendEnvironmentResultTypeDef:
         """
         Creates a new backend environment for an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.create_backend_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/client/#create_backend_environment)
         """
@@ -194,15 +193,15 @@
         tags: Mapping[str, str] = ...,
         buildSpec: str = ...,
         ttl: str = ...,
         displayName: str = ...,
         enablePullRequestPreview: bool = ...,
         pullRequestEnvironmentName: str = ...,
         backendEnvironmentArn: str = ...,
-        backend: BackendTypeDef = ...
+        backend: BackendTypeDef = ...,
     ) -> CreateBranchResultTypeDef:
         """
         Creates a new branch for an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.create_branch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/client/#create_branch)
         """
@@ -221,15 +220,15 @@
         self,
         *,
         appId: str,
         domainName: str,
         subDomainSettings: Sequence[SubDomainSettingTypeDef],
         enableAutoSubDomain: bool = ...,
         autoSubDomainCreationPatterns: Sequence[str] = ...,
-        autoSubDomainIAMRole: str = ...
+        autoSubDomainIAMRole: str = ...,
     ) -> CreateDomainAssociationResultTypeDef:
         """
         Creates a new domain association for an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.create_domain_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/client/#create_domain_association)
         """
@@ -300,15 +299,15 @@
 
     async def generate_access_logs(
         self,
         *,
         domainName: str,
         appId: str,
         startTime: TimestampTypeDef = ...,
-        endTime: TimestampTypeDef = ...
+        endTime: TimestampTypeDef = ...,
     ) -> GenerateAccessLogsResultTypeDef:
         """
         Returns the website access logs for a specific time range using a presigned URL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.generate_access_logs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/client/#generate_access_logs)
         """
@@ -400,15 +399,15 @@
     async def list_artifacts(
         self,
         *,
         appId: str,
         branchName: str,
         jobId: str,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListArtifactsResultTypeDef:
         """
         Returns a list of artifacts for a specified app, branch, and job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.list_artifacts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/client/#list_artifacts)
         """
@@ -489,15 +488,15 @@
         appId: str,
         branchName: str,
         jobType: JobTypeType,
         jobId: str = ...,
         jobReason: str = ...,
         commitId: str = ...,
         commitMessage: str = ...,
-        commitTime: TimestampTypeDef = ...
+        commitTime: TimestampTypeDef = ...,
     ) -> StartJobResultTypeDef:
         """
         Starts a new job for a branch of an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.start_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/client/#start_job)
         """
@@ -543,15 +542,15 @@
         buildSpec: str = ...,
         customHeaders: str = ...,
         enableAutoBranchCreation: bool = ...,
         autoBranchCreationPatterns: Sequence[str] = ...,
         autoBranchCreationConfig: AutoBranchCreationConfigTypeDef = ...,
         repository: str = ...,
         oauthToken: str = ...,
-        accessToken: str = ...
+        accessToken: str = ...,
     ) -> UpdateAppResultTypeDef:
         """
         Updates an existing Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.update_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/client/#update_app)
         """
@@ -572,15 +571,15 @@
         enablePerformanceMode: bool = ...,
         buildSpec: str = ...,
         ttl: str = ...,
         displayName: str = ...,
         enablePullRequestPreview: bool = ...,
         pullRequestEnvironmentName: str = ...,
         backendEnvironmentArn: str = ...,
-        backend: BackendTypeDef = ...
+        backend: BackendTypeDef = ...,
     ) -> UpdateBranchResultTypeDef:
         """
         Updates a branch for an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.update_branch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/client/#update_branch)
         """
@@ -589,15 +588,15 @@
         self,
         *,
         appId: str,
         domainName: str,
         enableAutoSubDomain: bool = ...,
         subDomainSettings: Sequence[SubDomainSettingTypeDef] = ...,
         autoSubDomainCreationPatterns: Sequence[str] = ...,
-        autoSubDomainIAMRole: str = ...
+        autoSubDomainIAMRole: str = ...,
     ) -> UpdateDomainAssociationResultTypeDef:
         """
         Creates a new domain association for an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.update_domain_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/client/#update_domain_association)
         """
```

### Comparing `types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify/client.pyi` & `types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -145,30 +145,30 @@
         basicAuthCredentials: str = ...,
         customRules: Sequence[CustomRuleTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         buildSpec: str = ...,
         customHeaders: str = ...,
         enableAutoBranchCreation: bool = ...,
         autoBranchCreationPatterns: Sequence[str] = ...,
-        autoBranchCreationConfig: AutoBranchCreationConfigTypeDef = ...
+        autoBranchCreationConfig: AutoBranchCreationConfigTypeDef = ...,
     ) -> CreateAppResultTypeDef:
         """
         Creates a new Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.create_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/client/#create_app)
         """
 
     async def create_backend_environment(
         self,
         *,
         appId: str,
         environmentName: str,
         stackName: str = ...,
-        deploymentArtifacts: str = ...
+        deploymentArtifacts: str = ...,
     ) -> CreateBackendEnvironmentResultTypeDef:
         """
         Creates a new backend environment for an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.create_backend_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/client/#create_backend_environment)
         """
@@ -190,15 +190,15 @@
         tags: Mapping[str, str] = ...,
         buildSpec: str = ...,
         ttl: str = ...,
         displayName: str = ...,
         enablePullRequestPreview: bool = ...,
         pullRequestEnvironmentName: str = ...,
         backendEnvironmentArn: str = ...,
-        backend: BackendTypeDef = ...
+        backend: BackendTypeDef = ...,
     ) -> CreateBranchResultTypeDef:
         """
         Creates a new branch for an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.create_branch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/client/#create_branch)
         """
@@ -217,15 +217,15 @@
         self,
         *,
         appId: str,
         domainName: str,
         subDomainSettings: Sequence[SubDomainSettingTypeDef],
         enableAutoSubDomain: bool = ...,
         autoSubDomainCreationPatterns: Sequence[str] = ...,
-        autoSubDomainIAMRole: str = ...
+        autoSubDomainIAMRole: str = ...,
     ) -> CreateDomainAssociationResultTypeDef:
         """
         Creates a new domain association for an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.create_domain_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/client/#create_domain_association)
         """
@@ -296,15 +296,15 @@
 
     async def generate_access_logs(
         self,
         *,
         domainName: str,
         appId: str,
         startTime: TimestampTypeDef = ...,
-        endTime: TimestampTypeDef = ...
+        endTime: TimestampTypeDef = ...,
     ) -> GenerateAccessLogsResultTypeDef:
         """
         Returns the website access logs for a specific time range using a presigned URL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.generate_access_logs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/client/#generate_access_logs)
         """
@@ -396,15 +396,15 @@
     async def list_artifacts(
         self,
         *,
         appId: str,
         branchName: str,
         jobId: str,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListArtifactsResultTypeDef:
         """
         Returns a list of artifacts for a specified app, branch, and job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.list_artifacts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/client/#list_artifacts)
         """
@@ -485,15 +485,15 @@
         appId: str,
         branchName: str,
         jobType: JobTypeType,
         jobId: str = ...,
         jobReason: str = ...,
         commitId: str = ...,
         commitMessage: str = ...,
-        commitTime: TimestampTypeDef = ...
+        commitTime: TimestampTypeDef = ...,
     ) -> StartJobResultTypeDef:
         """
         Starts a new job for a branch of an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.start_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/client/#start_job)
         """
@@ -539,15 +539,15 @@
         buildSpec: str = ...,
         customHeaders: str = ...,
         enableAutoBranchCreation: bool = ...,
         autoBranchCreationPatterns: Sequence[str] = ...,
         autoBranchCreationConfig: AutoBranchCreationConfigTypeDef = ...,
         repository: str = ...,
         oauthToken: str = ...,
-        accessToken: str = ...
+        accessToken: str = ...,
     ) -> UpdateAppResultTypeDef:
         """
         Updates an existing Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.update_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/client/#update_app)
         """
@@ -568,15 +568,15 @@
         enablePerformanceMode: bool = ...,
         buildSpec: str = ...,
         ttl: str = ...,
         displayName: str = ...,
         enablePullRequestPreview: bool = ...,
         pullRequestEnvironmentName: str = ...,
         backendEnvironmentArn: str = ...,
-        backend: BackendTypeDef = ...
+        backend: BackendTypeDef = ...,
     ) -> UpdateBranchResultTypeDef:
         """
         Updates a branch for an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.update_branch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/client/#update_branch)
         """
@@ -585,15 +585,15 @@
         self,
         *,
         appId: str,
         domainName: str,
         enableAutoSubDomain: bool = ...,
         subDomainSettings: Sequence[SubDomainSettingTypeDef] = ...,
         autoSubDomainCreationPatterns: Sequence[str] = ...,
-        autoSubDomainIAMRole: str = ...
+        autoSubDomainIAMRole: str = ...,
     ) -> UpdateDomainAssociationResultTypeDef:
         """
         Creates a new domain association for an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.update_domain_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/client/#update_domain_association)
         """
```

### Comparing `types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify/literals.py` & `types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify/literals.py`

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
     "DomainStatusType",
     "JobStatusType",
     "JobTypeType",
     "ListAppsPaginatorName",
     "ListBranchesPaginatorName",
     "ListDomainAssociationsPaginatorName",
@@ -34,15 +33,14 @@
     "AmplifyServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DomainStatusType = Literal[
     "AVAILABLE",
     "CREATING",
     "FAILED",
     "IN_PROGRESS",
     "PENDING_DEPLOYMENT",
     "PENDING_VERIFICATION",
```

### Comparing `types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify/literals.pyi` & `types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify/paginator.py` & `types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 __all__ = (
     "ListAppsPaginator",
     "ListBranchesPaginator",
     "ListDomainAssociationsPaginator",
     "ListJobsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify/paginator.pyi` & `types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify/type_defs.py` & `types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AutoBranchCreationConfigPaginatorTypeDef",
     "CustomRuleTypeDef",
     "ProductionBranchTypeDef",
     "AutoBranchCreationConfigTypeDef",
     "ArtifactTypeDef",
     "BackendEnvironmentTypeDef",
```

### Comparing `types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify/type_defs.pyi` & `types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify.egg-info/PKG-INFO` & `types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-amplify
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Amplify 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Amplify 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/
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
 
 <a id="types-aiobotocore-amplify"></a>
 
 # types-aiobotocore-amplify
 
 [![PyPI - types-aiobotocore-amplify](https://img.shields.io/pypi/v/types-aiobotocore-amplify.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amplify)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-amplify.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amplify)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-amplify)](https://pepy.tech/project/types-aiobotocore-amplify)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Amplify 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
+[aiobotocore.Amplify 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
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
 [types-aiobotocore-amplify docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-amplify-2.9.0/types_aiobotocore_amplify.egg-info/SOURCES.txt` & `types-aiobotocore-amplify-2.9.1/types_aiobotocore_amplify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

