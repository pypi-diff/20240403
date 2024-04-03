# Comparing `tmp/types-aiobotocore-lakeformation-2.9.0.tar.gz` & `tmp/types-aiobotocore-lakeformation-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-lakeformation-2.9.0.tar", last modified: Wed Dec 13 19:59:42 2023, max compression
+gzip compressed data, was "types-aiobotocore-lakeformation-2.9.1.tar", last modified: Thu Jan 18 01:21:05 2024, max compression
```

## Comparing `types-aiobotocore-lakeformation-2.9.0.tar` & `types-aiobotocore-lakeformation-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:42.577551 types-aiobotocore-lakeformation-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:48:44.000000 types-aiobotocore-lakeformation-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13921 2023-12-13 19:59:42.577551 types-aiobotocore-lakeformation-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12334 2023-12-13 19:48:44.000000 types-aiobotocore-lakeformation-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:42.577551 types-aiobotocore-lakeformation-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2023-12-13 19:48:44.000000 types-aiobotocore-lakeformation-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:42.577551 types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation/
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2023-12-13 19:48:44.000000 types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2023-12-13 19:48:44.000000 types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      956 2023-12-13 19:48:44.000000 types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44827 2023-12-13 19:48:44.000000 types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    44823 2023-12-13 19:48:44.000000 types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11205 2023-12-13 19:48:44.000000 types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11203 2023-12-13 19:48:44.000000 types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2023-12-13 19:48:44.000000 types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7135 2023-12-13 19:48:44.000000 types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:48:44.000000 types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    44198 2023-12-13 19:48:45.000000 types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    44197 2023-12-13 19:48:45.000000 types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:48:44.000000 types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:42.577551 types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13921 2023-12-13 19:59:42.000000 types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      927 2023-12-13 19:59:42.000000 types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:42.000000 types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:42.000000 types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:42.000000 types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-13 19:59:42.000000 types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:05.257231 types-aiobotocore-lakeformation-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:10:31.000000 types-aiobotocore-lakeformation-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13941 2024-01-18 01:21:05.257231 types-aiobotocore-lakeformation-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12334 2024-01-18 01:10:31.000000 types-aiobotocore-lakeformation-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:05.257231 types-aiobotocore-lakeformation-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-01-18 01:10:30.000000 types-aiobotocore-lakeformation-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:05.257231 types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-01-18 01:10:31.000000 types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-01-18 01:10:31.000000 types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-01-18 01:10:31.000000 types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44848 2024-01-18 01:10:31.000000 types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44845 2024-01-18 01:10:31.000000 types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11203 2024-01-18 01:10:31.000000 types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11203 2024-01-18 01:10:31.000000 types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-01-18 01:10:31.000000 types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7138 2024-01-18 01:10:31.000000 types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:10:31.000000 types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    44197 2024-01-18 01:10:32.000000 types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44197 2024-01-18 01:10:32.000000 types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:10:31.000000 types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:05.257231 types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13941 2024-01-18 01:21:05.000000 types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-01-18 01:21:05.000000 types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:05.000000 types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:05.000000 types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:05.000000 types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-18 01:21:05.000000 types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lakeformation-2.9.0/LICENSE` & `types-aiobotocore-lakeformation-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-lakeformation-2.9.0/PKG-INFO` & `types-aiobotocore-lakeformation-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lakeformation
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.LakeFormation 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.LakeFormation 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/
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
 
 <a id="types-aiobotocore-lakeformation"></a>
 
 # types-aiobotocore-lakeformation
 
 [![PyPI - types-aiobotocore-lakeformation](https://img.shields.io/pypi/v/types-aiobotocore-lakeformation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lakeformation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lakeformation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lakeformation)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lakeformation)](https://pepy.tech/project/types-aiobotocore-lakeformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LakeFormation 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
+[aiobotocore.LakeFormation 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
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
 [types-aiobotocore-lakeformation docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-lakeformation-2.9.0/README.md` & `types-aiobotocore-lakeformation-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lakeformation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lakeformation)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lakeformation)](https://pepy.tech/project/types-aiobotocore-lakeformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LakeFormation 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
+[aiobotocore.LakeFormation 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
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
 [types-aiobotocore-lakeformation docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-lakeformation-2.9.0/setup.py` & `types-aiobotocore-lakeformation-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-lakeformation",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_lakeformation"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.LakeFormation 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.LakeFormation 2.9.1 service generated with"
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
     keywords="aiobotocore lakeformation type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_lakeformation": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation/__init__.py` & `types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     ListLFTagsPaginator,
     SearchDatabasesByLFTagsPaginator,
     SearchTablesByLFTagsPaginator,
 )
 
 Client = LakeFormationClient
 
-
 __all__ = (
     "Client",
     "GetWorkUnitsPaginator",
     "LakeFormationClient",
     "ListDataCellsFilterPaginator",
     "ListLFTagsPaginator",
     "SearchDatabasesByLFTagsPaginator",
```

### Comparing `types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation/__init__.pyi` & `types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation/__main__.py` & `types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.LakeFormation 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.LakeFormation 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation\nOther"
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

### Comparing `types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation/client.py` & `types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("LakeFormationClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -234,15 +233,15 @@
         """
 
     async def create_lake_formation_identity_center_configuration(
         self,
         *,
         CatalogId: str = ...,
         InstanceArn: str = ...,
-        ExternalFiltering: ExternalFilteringConfigurationTypeDef = ...
+        ExternalFiltering: ExternalFilteringConfigurationTypeDef = ...,
     ) -> CreateLakeFormationIdentityCenterConfigurationResponseTypeDef:
         """
         Creates an IAM Identity Center connection with Lake Formation to allow IAM
         Identity Center users and groups to access Data Catalog
         resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.create_lake_formation_identity_center_configuration)
@@ -272,15 +271,15 @@
 
     async def delete_data_cells_filter(
         self,
         *,
         TableCatalogId: str = ...,
         DatabaseName: str = ...,
         TableName: str = ...,
-        Name: str = ...
+        Name: str = ...,
     ) -> Dict[str, Any]:
         """
         Deletes a data cell filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.delete_data_cells_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#delete_data_cells_filter)
         """
@@ -318,15 +317,15 @@
     async def delete_objects_on_cancel(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         TransactionId: str,
         Objects: Sequence[VirtualObjectTypeDef],
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> Dict[str, Any]:
         """
         For a specific governed table, provides a list of Amazon S3 objects that will
         be written during the current transaction and that can be automatically deleted
         if the transaction is
         canceled.
 
@@ -470,15 +469,15 @@
         DatabaseName: str,
         TableName: str,
         CatalogId: str = ...,
         TransactionId: str = ...,
         QueryAsOfTime: TimestampTypeDef = ...,
         PartitionPredicate: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetTableObjectsResponseTypeDef:
         """
         Returns the set of Amazon S3 objects that make up the specified governed table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_table_objects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#get_table_objects)
         """
@@ -487,15 +486,15 @@
         self,
         *,
         TableArn: str,
         Partition: PartitionValueListTypeDef,
         Permissions: Sequence[PermissionType] = ...,
         DurationSeconds: int = ...,
         AuditContext: AuditContextTypeDef = ...,
-        SupportedPermissionTypes: Sequence[PermissionTypeType] = ...
+        SupportedPermissionTypes: Sequence[PermissionTypeType] = ...,
     ) -> GetTemporaryGluePartitionCredentialsResponseTypeDef:
         """
         This API is identical to `GetTemporaryTableCredentials` except that this is
         used when the target Data Catalog resource is of type
         Partition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_temporary_glue_partition_credentials)
@@ -505,15 +504,15 @@
     async def get_temporary_glue_table_credentials(
         self,
         *,
         TableArn: str,
         Permissions: Sequence[PermissionType] = ...,
         DurationSeconds: int = ...,
         AuditContext: AuditContextTypeDef = ...,
-        SupportedPermissionTypes: Sequence[PermissionTypeType] = ...
+        SupportedPermissionTypes: Sequence[PermissionTypeType] = ...,
     ) -> GetTemporaryGlueTableCredentialsResponseTypeDef:
         """
         Allows a caller in a secure environment to assume a role with permission to
         access Amazon
         S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_temporary_glue_table_credentials)
@@ -543,15 +542,15 @@
     async def grant_permissions(
         self,
         *,
         Principal: DataLakePrincipalTypeDef,
         Resource: ResourceTypeDef,
         Permissions: Sequence[PermissionType],
         CatalogId: str = ...,
-        PermissionsWithGrantOption: Sequence[PermissionType] = ...
+        PermissionsWithGrantOption: Sequence[PermissionType] = ...,
     ) -> Dict[str, Any]:
         """
         Grants permissions to the principal to access metadata in the Data Catalog and
         data organized in underlying data storage such as Amazon
         S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.grant_permissions)
@@ -570,15 +569,15 @@
 
     async def list_lake_formation_opt_ins(
         self,
         *,
         Principal: DataLakePrincipalTypeDef = ...,
         Resource: ResourceTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListLakeFormationOptInsResponseTypeDef:
         """
         Retrieve the current list of resources and principals that are opt in to
         enforce Lake Formation
         permissions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_lake_formation_opt_ins)
@@ -587,15 +586,15 @@
 
     async def list_lf_tags(
         self,
         *,
         CatalogId: str = ...,
         ResourceShareType: ResourceShareTypeType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListLFTagsResponseTypeDef:
         """
         Lists LF-tags that the requester has permission to view.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_lf_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#list_lf_tags)
         """
@@ -605,15 +604,15 @@
         *,
         CatalogId: str = ...,
         Principal: DataLakePrincipalTypeDef = ...,
         ResourceType: DataLakeResourceTypeType = ...,
         Resource: ResourceTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        IncludeRelated: str = ...
+        IncludeRelated: str = ...,
     ) -> ListPermissionsResponseTypeDef:
         """
         Returns a list of the principal permissions on the resource, filtered by the
         permissions of the
         caller.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_permissions)
@@ -621,15 +620,15 @@
         """
 
     async def list_resources(
         self,
         *,
         FilterConditionList: Sequence[FilterConditionTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListResourcesResponseTypeDef:
         """
         Lists the resources registered to be managed by the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#list_resources)
         """
@@ -638,15 +637,15 @@
         self,
         *,
         DatabaseName: str,
         TableName: str,
         CatalogId: str = ...,
         StorageOptimizerType: OptimizerTypeType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListTableStorageOptimizersResponseTypeDef:
         """
         Returns the configuration of all storage optimizers associated with a specified
         table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_table_storage_optimizers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#list_table_storage_optimizers)
@@ -654,15 +653,15 @@
 
     async def list_transactions(
         self,
         *,
         CatalogId: str = ...,
         StatusFilter: TransactionStatusFilterType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListTransactionsResponseTypeDef:
         """
         Returns metadata about transactions and their status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_transactions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#list_transactions)
         """
@@ -682,15 +681,15 @@
     async def register_resource(
         self,
         *,
         ResourceArn: str,
         UseServiceLinkedRole: bool = ...,
         RoleArn: str = ...,
         WithFederation: bool = ...,
-        HybridAccessEnabled: bool = ...
+        HybridAccessEnabled: bool = ...,
     ) -> Dict[str, Any]:
         """
         Registers the resource as managed by the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.register_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#register_resource)
         """
@@ -708,15 +707,15 @@
     async def revoke_permissions(
         self,
         *,
         Principal: DataLakePrincipalTypeDef,
         Resource: ResourceTypeDef,
         Permissions: Sequence[PermissionType],
         CatalogId: str = ...,
-        PermissionsWithGrantOption: Sequence[PermissionType] = ...
+        PermissionsWithGrantOption: Sequence[PermissionType] = ...,
     ) -> Dict[str, Any]:
         """
         Revokes permissions to the principal to access metadata in the Data Catalog and
         data organized in underlying data storage such as Amazon
         S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.revoke_permissions)
@@ -725,30 +724,30 @@
 
     async def search_databases_by_lf_tags(
         self,
         *,
         Expression: Sequence[LFTagTypeDef],
         NextToken: str = ...,
         MaxResults: int = ...,
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> SearchDatabasesByLFTagsResponseTypeDef:
         """
         This operation allows a search on `DATABASE` resources by `TagCondition`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.search_databases_by_lf_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#search_databases_by_lf_tags)
         """
 
     async def search_tables_by_lf_tags(
         self,
         *,
         Expression: Sequence[LFTagTypeDef],
         NextToken: str = ...,
         MaxResults: int = ...,
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> SearchTablesByLFTagsResponseTypeDef:
         """
         This operation allows a search on `TABLE` resources by `LFTag`s.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.search_tables_by_lf_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#search_tables_by_lf_tags)
         """
@@ -784,45 +783,45 @@
         """
 
     async def update_lake_formation_identity_center_configuration(
         self,
         *,
         CatalogId: str = ...,
         ApplicationStatus: ApplicationStatusType = ...,
-        ExternalFiltering: ExternalFilteringConfigurationTypeDef = ...
+        ExternalFiltering: ExternalFilteringConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the IAM Identity Center connection parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.update_lake_formation_identity_center_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#update_lake_formation_identity_center_configuration)
         """
 
     async def update_lf_tag(
         self,
         *,
         TagKey: str,
         CatalogId: str = ...,
         TagValuesToDelete: Sequence[str] = ...,
-        TagValuesToAdd: Sequence[str] = ...
+        TagValuesToAdd: Sequence[str] = ...,
     ) -> Dict[str, Any]:
         """
         Updates the list of possible values for the specified LF-tag key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.update_lf_tag)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#update_lf_tag)
         """
 
     async def update_resource(
         self,
         *,
         RoleArn: str,
         ResourceArn: str,
         WithFederation: bool = ...,
-        HybridAccessEnabled: bool = ...
+        HybridAccessEnabled: bool = ...,
     ) -> Dict[str, Any]:
         """
         Updates the data access role used for vending access to the given (registered)
         resource in Lake
         Formation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.update_resource)
@@ -832,15 +831,15 @@
     async def update_table_objects(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         WriteOperations: Sequence[WriteOperationTypeDef],
         CatalogId: str = ...,
-        TransactionId: str = ...
+        TransactionId: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the manifest of Amazon S3 objects that make up the specified governed
         table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.update_table_objects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#update_table_objects)
@@ -848,15 +847,15 @@
 
     async def update_table_storage_optimizer(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         StorageOptimizerConfig: Mapping[OptimizerTypeType, Mapping[str, str]],
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> UpdateTableStorageOptimizerResponseTypeDef:
         """
         Updates the configuration of the storage optimizers for a table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.update_table_storage_optimizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#update_table_storage_optimizer)
         """
```

### Comparing `types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation/client.pyi` & `types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -230,15 +230,15 @@
         """
 
     async def create_lake_formation_identity_center_configuration(
         self,
         *,
         CatalogId: str = ...,
         InstanceArn: str = ...,
-        ExternalFiltering: ExternalFilteringConfigurationTypeDef = ...
+        ExternalFiltering: ExternalFilteringConfigurationTypeDef = ...,
     ) -> CreateLakeFormationIdentityCenterConfigurationResponseTypeDef:
         """
         Creates an IAM Identity Center connection with Lake Formation to allow IAM
         Identity Center users and groups to access Data Catalog
         resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.create_lake_formation_identity_center_configuration)
@@ -268,15 +268,15 @@
 
     async def delete_data_cells_filter(
         self,
         *,
         TableCatalogId: str = ...,
         DatabaseName: str = ...,
         TableName: str = ...,
-        Name: str = ...
+        Name: str = ...,
     ) -> Dict[str, Any]:
         """
         Deletes a data cell filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.delete_data_cells_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#delete_data_cells_filter)
         """
@@ -314,15 +314,15 @@
     async def delete_objects_on_cancel(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         TransactionId: str,
         Objects: Sequence[VirtualObjectTypeDef],
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> Dict[str, Any]:
         """
         For a specific governed table, provides a list of Amazon S3 objects that will
         be written during the current transaction and that can be automatically deleted
         if the transaction is
         canceled.
 
@@ -466,15 +466,15 @@
         DatabaseName: str,
         TableName: str,
         CatalogId: str = ...,
         TransactionId: str = ...,
         QueryAsOfTime: TimestampTypeDef = ...,
         PartitionPredicate: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetTableObjectsResponseTypeDef:
         """
         Returns the set of Amazon S3 objects that make up the specified governed table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_table_objects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#get_table_objects)
         """
@@ -483,15 +483,15 @@
         self,
         *,
         TableArn: str,
         Partition: PartitionValueListTypeDef,
         Permissions: Sequence[PermissionType] = ...,
         DurationSeconds: int = ...,
         AuditContext: AuditContextTypeDef = ...,
-        SupportedPermissionTypes: Sequence[PermissionTypeType] = ...
+        SupportedPermissionTypes: Sequence[PermissionTypeType] = ...,
     ) -> GetTemporaryGluePartitionCredentialsResponseTypeDef:
         """
         This API is identical to `GetTemporaryTableCredentials` except that this is
         used when the target Data Catalog resource is of type
         Partition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_temporary_glue_partition_credentials)
@@ -501,15 +501,15 @@
     async def get_temporary_glue_table_credentials(
         self,
         *,
         TableArn: str,
         Permissions: Sequence[PermissionType] = ...,
         DurationSeconds: int = ...,
         AuditContext: AuditContextTypeDef = ...,
-        SupportedPermissionTypes: Sequence[PermissionTypeType] = ...
+        SupportedPermissionTypes: Sequence[PermissionTypeType] = ...,
     ) -> GetTemporaryGlueTableCredentialsResponseTypeDef:
         """
         Allows a caller in a secure environment to assume a role with permission to
         access Amazon
         S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_temporary_glue_table_credentials)
@@ -539,15 +539,15 @@
     async def grant_permissions(
         self,
         *,
         Principal: DataLakePrincipalTypeDef,
         Resource: ResourceTypeDef,
         Permissions: Sequence[PermissionType],
         CatalogId: str = ...,
-        PermissionsWithGrantOption: Sequence[PermissionType] = ...
+        PermissionsWithGrantOption: Sequence[PermissionType] = ...,
     ) -> Dict[str, Any]:
         """
         Grants permissions to the principal to access metadata in the Data Catalog and
         data organized in underlying data storage such as Amazon
         S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.grant_permissions)
@@ -566,15 +566,15 @@
 
     async def list_lake_formation_opt_ins(
         self,
         *,
         Principal: DataLakePrincipalTypeDef = ...,
         Resource: ResourceTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListLakeFormationOptInsResponseTypeDef:
         """
         Retrieve the current list of resources and principals that are opt in to
         enforce Lake Formation
         permissions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_lake_formation_opt_ins)
@@ -583,15 +583,15 @@
 
     async def list_lf_tags(
         self,
         *,
         CatalogId: str = ...,
         ResourceShareType: ResourceShareTypeType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListLFTagsResponseTypeDef:
         """
         Lists LF-tags that the requester has permission to view.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_lf_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#list_lf_tags)
         """
@@ -601,15 +601,15 @@
         *,
         CatalogId: str = ...,
         Principal: DataLakePrincipalTypeDef = ...,
         ResourceType: DataLakeResourceTypeType = ...,
         Resource: ResourceTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        IncludeRelated: str = ...
+        IncludeRelated: str = ...,
     ) -> ListPermissionsResponseTypeDef:
         """
         Returns a list of the principal permissions on the resource, filtered by the
         permissions of the
         caller.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_permissions)
@@ -617,15 +617,15 @@
         """
 
     async def list_resources(
         self,
         *,
         FilterConditionList: Sequence[FilterConditionTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListResourcesResponseTypeDef:
         """
         Lists the resources registered to be managed by the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#list_resources)
         """
@@ -634,15 +634,15 @@
         self,
         *,
         DatabaseName: str,
         TableName: str,
         CatalogId: str = ...,
         StorageOptimizerType: OptimizerTypeType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListTableStorageOptimizersResponseTypeDef:
         """
         Returns the configuration of all storage optimizers associated with a specified
         table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_table_storage_optimizers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#list_table_storage_optimizers)
@@ -650,15 +650,15 @@
 
     async def list_transactions(
         self,
         *,
         CatalogId: str = ...,
         StatusFilter: TransactionStatusFilterType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListTransactionsResponseTypeDef:
         """
         Returns metadata about transactions and their status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_transactions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#list_transactions)
         """
@@ -678,15 +678,15 @@
     async def register_resource(
         self,
         *,
         ResourceArn: str,
         UseServiceLinkedRole: bool = ...,
         RoleArn: str = ...,
         WithFederation: bool = ...,
-        HybridAccessEnabled: bool = ...
+        HybridAccessEnabled: bool = ...,
     ) -> Dict[str, Any]:
         """
         Registers the resource as managed by the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.register_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#register_resource)
         """
@@ -704,15 +704,15 @@
     async def revoke_permissions(
         self,
         *,
         Principal: DataLakePrincipalTypeDef,
         Resource: ResourceTypeDef,
         Permissions: Sequence[PermissionType],
         CatalogId: str = ...,
-        PermissionsWithGrantOption: Sequence[PermissionType] = ...
+        PermissionsWithGrantOption: Sequence[PermissionType] = ...,
     ) -> Dict[str, Any]:
         """
         Revokes permissions to the principal to access metadata in the Data Catalog and
         data organized in underlying data storage such as Amazon
         S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.revoke_permissions)
@@ -721,30 +721,30 @@
 
     async def search_databases_by_lf_tags(
         self,
         *,
         Expression: Sequence[LFTagTypeDef],
         NextToken: str = ...,
         MaxResults: int = ...,
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> SearchDatabasesByLFTagsResponseTypeDef:
         """
         This operation allows a search on `DATABASE` resources by `TagCondition`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.search_databases_by_lf_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#search_databases_by_lf_tags)
         """
 
     async def search_tables_by_lf_tags(
         self,
         *,
         Expression: Sequence[LFTagTypeDef],
         NextToken: str = ...,
         MaxResults: int = ...,
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> SearchTablesByLFTagsResponseTypeDef:
         """
         This operation allows a search on `TABLE` resources by `LFTag`s.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.search_tables_by_lf_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#search_tables_by_lf_tags)
         """
@@ -780,45 +780,45 @@
         """
 
     async def update_lake_formation_identity_center_configuration(
         self,
         *,
         CatalogId: str = ...,
         ApplicationStatus: ApplicationStatusType = ...,
-        ExternalFiltering: ExternalFilteringConfigurationTypeDef = ...
+        ExternalFiltering: ExternalFilteringConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the IAM Identity Center connection parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.update_lake_formation_identity_center_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#update_lake_formation_identity_center_configuration)
         """
 
     async def update_lf_tag(
         self,
         *,
         TagKey: str,
         CatalogId: str = ...,
         TagValuesToDelete: Sequence[str] = ...,
-        TagValuesToAdd: Sequence[str] = ...
+        TagValuesToAdd: Sequence[str] = ...,
     ) -> Dict[str, Any]:
         """
         Updates the list of possible values for the specified LF-tag key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.update_lf_tag)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#update_lf_tag)
         """
 
     async def update_resource(
         self,
         *,
         RoleArn: str,
         ResourceArn: str,
         WithFederation: bool = ...,
-        HybridAccessEnabled: bool = ...
+        HybridAccessEnabled: bool = ...,
     ) -> Dict[str, Any]:
         """
         Updates the data access role used for vending access to the given (registered)
         resource in Lake
         Formation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.update_resource)
@@ -828,15 +828,15 @@
     async def update_table_objects(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         WriteOperations: Sequence[WriteOperationTypeDef],
         CatalogId: str = ...,
-        TransactionId: str = ...
+        TransactionId: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the manifest of Amazon S3 objects that make up the specified governed
         table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.update_table_objects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#update_table_objects)
@@ -844,15 +844,15 @@
 
     async def update_table_storage_optimizer(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         StorageOptimizerConfig: Mapping[OptimizerTypeType, Mapping[str, str]],
-        CatalogId: str = ...
+        CatalogId: str = ...,
     ) -> UpdateTableStorageOptimizerResponseTypeDef:
         """
         Updates the configuration of the storage optimizers for a table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.update_table_storage_optimizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#update_table_storage_optimizer)
         """
```

### Comparing `types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation/literals.py` & `types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation/literals.py`

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
     "ApplicationStatusType",
     "ComparisonOperatorType",
     "DataLakeResourceTypeType",
     "EnableStatusType",
     "FieldNameStringType",
     "GetWorkUnitsPaginatorName",
@@ -43,15 +42,14 @@
     "LakeFormationServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ApplicationStatusType = Literal["DISABLED", "ENABLED"]
 ComparisonOperatorType = Literal[
     "BEGINS_WITH", "BETWEEN", "CONTAINS", "EQ", "GE", "GT", "IN", "LE", "LT", "NE", "NOT_CONTAINS"
 ]
 DataLakeResourceTypeType = Literal[
     "CATALOG",
     "DATABASE",
```

### Comparing `types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation/literals.pyi` & `types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation/paginator.py` & `types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,14 @@
     "GetWorkUnitsPaginator",
     "ListDataCellsFilterPaginator",
     "ListLFTagsPaginator",
     "SearchDatabasesByLFTagsPaginator",
     "SearchTablesByLFTagsPaginator",
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
         CatalogId: str = ...,
         ResourceShareType: ResourceShareTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListLFTagsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListLFTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#listlftagspaginator)
         """
 
 
@@ -121,15 +120,15 @@
     """
 
     def paginate(
         self,
         *,
         Expression: Sequence[LFTagTypeDef],
         CatalogId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchDatabasesByLFTagsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchDatabasesByLFTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#searchdatabasesbylftagspaginator)
         """
 
 
@@ -140,13 +139,13 @@
     """
 
     def paginate(
         self,
         *,
         Expression: Sequence[LFTagTypeDef],
         CatalogId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchTablesByLFTagsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchTablesByLFTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#searchtablesbylftagspaginator)
         """
```

### Comparing `types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation/paginator.pyi` & `types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     """
 
     def paginate(
         self,
         *,
         CatalogId: str = ...,
         ResourceShareType: ResourceShareTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListLFTagsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListLFTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#listlftagspaginator)
         """
 
 class SearchDatabasesByLFTagsPaginator(AioPaginator):
@@ -115,15 +115,15 @@
     """
 
     def paginate(
         self,
         *,
         Expression: Sequence[LFTagTypeDef],
         CatalogId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchDatabasesByLFTagsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchDatabasesByLFTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#searchdatabasesbylftagspaginator)
         """
 
 class SearchTablesByLFTagsPaginator(AioPaginator):
@@ -133,13 +133,13 @@
     """
 
     def paginate(
         self,
         *,
         Expression: Sequence[LFTagTypeDef],
         CatalogId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchTablesByLFTagsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchTablesByLFTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#searchtablesbylftagspaginator)
         """
```

### Comparing `types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation/type_defs.py` & `types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "LFTagPairTypeDef",
     "ResponseMetadataTypeDef",
     "AddObjectInputTypeDef",
     "AssumeDecoratedRoleWithSAMLRequestRequestTypeDef",
     "AuditContextTypeDef",
     "ErrorDetailTypeDef",
```

### Comparing `types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation/type_defs.pyi` & `types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation.egg-info/PKG-INFO` & `types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lakeformation
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.LakeFormation 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.LakeFormation 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/
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
 
 <a id="types-aiobotocore-lakeformation"></a>
 
 # types-aiobotocore-lakeformation
 
 [![PyPI - types-aiobotocore-lakeformation](https://img.shields.io/pypi/v/types-aiobotocore-lakeformation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lakeformation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lakeformation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lakeformation)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lakeformation)](https://pepy.tech/project/types-aiobotocore-lakeformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LakeFormation 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
+[aiobotocore.LakeFormation 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
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
 [types-aiobotocore-lakeformation docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-lakeformation-2.9.0/types_aiobotocore_lakeformation.egg-info/SOURCES.txt` & `types-aiobotocore-lakeformation-2.9.1/types_aiobotocore_lakeformation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

