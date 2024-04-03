# Comparing `tmp/types-aiobotocore-mgh-2.9.0.tar.gz` & `tmp/types-aiobotocore-mgh-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mgh-2.9.0.tar", last modified: Wed Dec 13 19:59:56 2023, max compression
+gzip compressed data, was "types-aiobotocore-mgh-2.9.1.tar", last modified: Thu Jan 18 01:21:18 2024, max compression
```

## Comparing `types-aiobotocore-mgh-2.9.0.tar` & `types-aiobotocore-mgh-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:56.845429 types-aiobotocore-mgh-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:50:27.000000 types-aiobotocore-mgh-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13556 2023-12-13 19:59:56.845429 types-aiobotocore-mgh-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12000 2023-12-13 19:50:27.000000 types-aiobotocore-mgh-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:56.845429 types-aiobotocore-mgh-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2023-12-13 19:50:27.000000 types-aiobotocore-mgh-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:56.845429 types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh/
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2023-12-13 19:50:27.000000 types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2023-12-13 19:50:27.000000 types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-12-13 19:50:27.000000 types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18712 2023-12-13 19:50:27.000000 types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    18708 2023-12-13 19:50:27.000000 types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9520 2023-12-13 19:50:27.000000 types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9518 2023-12-13 19:50:27.000000 types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6865 2023-12-13 19:50:27.000000 types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6858 2023-12-13 19:50:27.000000 types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:50:27.000000 types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12261 2023-12-13 19:50:27.000000 types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12260 2023-12-13 19:50:27.000000 types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:50:27.000000 types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:56.845429 types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13556 2023-12-13 19:59:56.000000 types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      737 2023-12-13 19:59:56.000000 types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:56.000000 types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:56.000000 types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:56.000000 types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 19:59:56.000000 types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:18.441171 types-aiobotocore-mgh-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:12:08.000000 types-aiobotocore-mgh-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13576 2024-01-18 01:21:18.441171 types-aiobotocore-mgh-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12000 2024-01-18 01:12:08.000000 types-aiobotocore-mgh-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:18.441171 types-aiobotocore-mgh-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-01-18 01:12:08.000000 types-aiobotocore-mgh-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:18.441171 types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh/
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-01-18 01:12:08.000000 types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-01-18 01:12:08.000000 types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-01-18 01:12:08.000000 types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18720 2024-01-18 01:12:08.000000 types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18717 2024-01-18 01:12:08.000000 types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9518 2024-01-18 01:12:11.000000 types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9518 2024-01-18 01:12:08.000000 types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-01-18 01:12:08.000000 types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-01-18 01:12:08.000000 types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:12:08.000000 types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12260 2024-01-18 01:12:11.000000 types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12260 2024-01-18 01:12:11.000000 types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:12:08.000000 types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:18.441171 types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13576 2024-01-18 01:21:18.000000 types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-01-18 01:21:18.000000 types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:18.000000 types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:18.000000 types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:18.000000 types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:21:18.000000 types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mgh-2.9.0/LICENSE` & `types-aiobotocore-mgh-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-mgh-2.9.0/PKG-INFO` & `types-aiobotocore-mgh-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mgh
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MigrationHub 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MigrationHub 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/
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
 
 <a id="types-aiobotocore-mgh"></a>
 
 # types-aiobotocore-mgh
 
 [![PyPI - types-aiobotocore-mgh](https://img.shields.io/pypi/v/types-aiobotocore-mgh.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mgh)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mgh.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mgh)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mgh)](https://pepy.tech/project/types-aiobotocore-mgh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MigrationHub 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
+[aiobotocore.MigrationHub 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
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
 [types-aiobotocore-mgh docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mgh-2.9.0/README.md` & `types-aiobotocore-mgh-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mgh.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mgh)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mgh)](https://pepy.tech/project/types-aiobotocore-mgh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MigrationHub 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
+[aiobotocore.MigrationHub 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
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
 [types-aiobotocore-mgh docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mgh-2.9.0/setup.py` & `types-aiobotocore-mgh-2.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mgh",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_mgh"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MigrationHub 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.MigrationHub 2.9.1 service generated with"
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
     keywords="aiobotocore mgh type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_mgh": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh/__init__.py` & `types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     ListDiscoveredResourcesPaginator,
     ListMigrationTasksPaginator,
     ListProgressUpdateStreamsPaginator,
 )
 
 Client = MigrationHubClient
 
-
 __all__ = (
     "Client",
     "ListApplicationStatesPaginator",
     "ListCreatedArtifactsPaginator",
     "ListDiscoveredResourcesPaginator",
     "ListMigrationTasksPaginator",
     "ListProgressUpdateStreamsPaginator",
```

### Comparing `types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh/__init__.pyi` & `types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh/__main__.py` & `types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MigrationHub 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.MigrationHub 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub\nOther"
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

### Comparing `types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh/client.py` & `types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("MigrationHubClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -94,15 +93,15 @@
 
     async def associate_created_artifact(
         self,
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
         CreatedArtifact: CreatedArtifactTypeDef,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> Dict[str, Any]:
         """
         Associates a created artifact of an AWS cloud resource, the target receiving
         the migration, with the migration task performed by a migration
         tool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.associate_created_artifact)
@@ -111,15 +110,15 @@
 
     async def associate_discovered_resource(
         self,
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
         DiscoveredResource: DiscoveredResourceTypeDef,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> Dict[str, Any]:
         """
         Associates a discovered resource ID from Application Discovery Service with a
         migration
         task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.associate_discovered_resource)
@@ -189,15 +188,15 @@
 
     async def disassociate_created_artifact(
         self,
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
         CreatedArtifactName: str,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> Dict[str, Any]:
         """
         Disassociates a created artifact of an AWS resource with a migration task
         performed by a migration tool that was previously
         associated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.disassociate_created_artifact)
@@ -206,15 +205,15 @@
 
     async def disassociate_discovered_resource(
         self,
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
         ConfigurationId: str,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> Dict[str, Any]:
         """
         Disassociate an Application Discovery Service discovered resource from a
         migration
         task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.disassociate_discovered_resource)
@@ -259,15 +258,15 @@
 
     async def list_created_artifacts(
         self,
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListCreatedArtifactsResultTypeDef:
         """
         Lists the created artifacts attached to a given migration task in an update
         stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.list_created_artifacts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/client/#list_created_artifacts)
@@ -275,15 +274,15 @@
 
     async def list_discovered_resources(
         self,
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListDiscoveredResourcesResultTypeDef:
         """
         Lists discovered resources associated with the given `MigrationTask`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.list_discovered_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/client/#list_discovered_resources)
         """
@@ -312,15 +311,15 @@
 
     async def notify_application_state(
         self,
         *,
         ApplicationId: str,
         Status: ApplicationStatusType,
         UpdateDateTime: TimestampTypeDef = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> Dict[str, Any]:
         """
         Sets the migration state of an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.notify_application_state)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/client/#notify_application_state)
         """
@@ -329,15 +328,15 @@
         self,
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
         Task: TaskTypeDef,
         UpdateDateTime: TimestampTypeDef,
         NextUpdateSeconds: int,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> Dict[str, Any]:
         """
         Notifies Migration Hub of the current status, progress, or other detail
         regarding a migration
         task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.notify_migration_task_state)
@@ -346,15 +345,15 @@
 
     async def put_resource_attributes(
         self,
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
         ResourceAttributeList: Sequence[ResourceAttributeTypeDef],
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> Dict[str, Any]:
         """
         Provides identifying details of the resource being migrated so that it can be
         associated in the Application Discovery Service
         repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.put_resource_attributes)
```

### Comparing `types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh/client.pyi` & `types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
     async def associate_created_artifact(
         self,
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
         CreatedArtifact: CreatedArtifactTypeDef,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> Dict[str, Any]:
         """
         Associates a created artifact of an AWS cloud resource, the target receiving
         the migration, with the migration task performed by a migration
         tool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.associate_created_artifact)
@@ -107,15 +107,15 @@
 
     async def associate_discovered_resource(
         self,
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
         DiscoveredResource: DiscoveredResourceTypeDef,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> Dict[str, Any]:
         """
         Associates a discovered resource ID from Application Discovery Service with a
         migration
         task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.associate_discovered_resource)
@@ -185,15 +185,15 @@
 
     async def disassociate_created_artifact(
         self,
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
         CreatedArtifactName: str,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> Dict[str, Any]:
         """
         Disassociates a created artifact of an AWS resource with a migration task
         performed by a migration tool that was previously
         associated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.disassociate_created_artifact)
@@ -202,15 +202,15 @@
 
     async def disassociate_discovered_resource(
         self,
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
         ConfigurationId: str,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> Dict[str, Any]:
         """
         Disassociate an Application Discovery Service discovered resource from a
         migration
         task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.disassociate_discovered_resource)
@@ -255,15 +255,15 @@
 
     async def list_created_artifacts(
         self,
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListCreatedArtifactsResultTypeDef:
         """
         Lists the created artifacts attached to a given migration task in an update
         stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.list_created_artifacts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/client/#list_created_artifacts)
@@ -271,15 +271,15 @@
 
     async def list_discovered_resources(
         self,
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListDiscoveredResourcesResultTypeDef:
         """
         Lists discovered resources associated with the given `MigrationTask`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.list_discovered_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/client/#list_discovered_resources)
         """
@@ -308,15 +308,15 @@
 
     async def notify_application_state(
         self,
         *,
         ApplicationId: str,
         Status: ApplicationStatusType,
         UpdateDateTime: TimestampTypeDef = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> Dict[str, Any]:
         """
         Sets the migration state of an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.notify_application_state)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/client/#notify_application_state)
         """
@@ -325,15 +325,15 @@
         self,
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
         Task: TaskTypeDef,
         UpdateDateTime: TimestampTypeDef,
         NextUpdateSeconds: int,
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> Dict[str, Any]:
         """
         Notifies Migration Hub of the current status, progress, or other detail
         regarding a migration
         task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.notify_migration_task_state)
@@ -342,15 +342,15 @@
 
     async def put_resource_attributes(
         self,
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
         ResourceAttributeList: Sequence[ResourceAttributeTypeDef],
-        DryRun: bool = ...
+        DryRun: bool = ...,
     ) -> Dict[str, Any]:
         """
         Provides identifying details of the resource being migrated so that it can be
         associated in the Application Discovery Service
         repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.put_resource_attributes)
```

### Comparing `types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh/literals.py` & `types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh/literals.py`

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
     "ApplicationStatusType",
     "ListApplicationStatesPaginatorName",
     "ListCreatedArtifactsPaginatorName",
     "ListDiscoveredResourcesPaginatorName",
     "ListMigrationTasksPaginatorName",
     "ListProgressUpdateStreamsPaginatorName",
@@ -32,15 +31,14 @@
     "MigrationHubServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ApplicationStatusType = Literal["COMPLETED", "IN_PROGRESS", "NOT_STARTED"]
 ListApplicationStatesPaginatorName = Literal["list_application_states"]
 ListCreatedArtifactsPaginatorName = Literal["list_created_artifacts"]
 ListDiscoveredResourcesPaginatorName = Literal["list_discovered_resources"]
 ListMigrationTasksPaginatorName = Literal["list_migration_tasks"]
 ListProgressUpdateStreamsPaginatorName = Literal["list_progress_update_streams"]
 ResourceAttributeTypeType = Literal[
```

### Comparing `types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh/literals.pyi` & `types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh/paginator.py` & `types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     "ListApplicationStatesPaginator",
     "ListCreatedArtifactsPaginator",
     "ListDiscoveredResourcesPaginator",
     "ListMigrationTasksPaginator",
     "ListProgressUpdateStreamsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -84,15 +83,15 @@
     """
 
     def paginate(
         self,
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCreatedArtifactsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListCreatedArtifacts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/paginators/#listcreatedartifactspaginator)
         """
 
 
@@ -103,15 +102,15 @@
     """
 
     def paginate(
         self,
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDiscoveredResourcesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListDiscoveredResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/paginators/#listdiscoveredresourcespaginator)
         """
```

### Comparing `types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh/paginator.pyi` & `types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     """
 
     def paginate(
         self,
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCreatedArtifactsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListCreatedArtifacts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/paginators/#listcreatedartifactspaginator)
         """
 
 class ListDiscoveredResourcesPaginator(AioPaginator):
@@ -98,15 +98,15 @@
     """
 
     def paginate(
         self,
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDiscoveredResourcesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListDiscoveredResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/paginators/#listdiscoveredresourcespaginator)
         """
 
 class ListMigrationTasksPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh/type_defs.py` & `types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh/type_defs.py`

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
     "ApplicationStateTypeDef",
     "CreatedArtifactTypeDef",
     "DiscoveredResourceTypeDef",
     "CreateProgressUpdateStreamRequestRequestTypeDef",
     "DeleteProgressUpdateStreamRequestRequestTypeDef",
     "DescribeApplicationStateRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh/type_defs.pyi` & `types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh.egg-info/PKG-INFO` & `types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mgh
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MigrationHub 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MigrationHub 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/
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
 
 <a id="types-aiobotocore-mgh"></a>
 
 # types-aiobotocore-mgh
 
 [![PyPI - types-aiobotocore-mgh](https://img.shields.io/pypi/v/types-aiobotocore-mgh.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mgh)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mgh.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mgh)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mgh)](https://pepy.tech/project/types-aiobotocore-mgh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MigrationHub 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
+[aiobotocore.MigrationHub 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
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
 [types-aiobotocore-mgh docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mgh-2.9.0/types_aiobotocore_mgh.egg-info/SOURCES.txt` & `types-aiobotocore-mgh-2.9.1/types_aiobotocore_mgh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

