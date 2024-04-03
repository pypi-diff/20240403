# Comparing `tmp/types-aiobotocore-kendra-ranking-2.9.0.tar.gz` & `tmp/types-aiobotocore-kendra-ranking-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kendra-ranking-2.9.0.tar", last modified: Wed Dec 13 19:59:38 2023, max compression
+gzip compressed data, was "types-aiobotocore-kendra-ranking-2.9.1.tar", last modified: Thu Jan 18 01:21:01 2024, max compression
```

## Comparing `types-aiobotocore-kendra-ranking-2.9.0.tar` & `types-aiobotocore-kendra-ranking-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:38.521584 types-aiobotocore-kendra-ranking-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:48:29.000000 types-aiobotocore-kendra-ranking-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12639 2023-12-13 19:59:38.521584 types-aiobotocore-kendra-ranking-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11049 2023-12-13 19:48:29.000000 types-aiobotocore-kendra-ranking-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:38.521584 types-aiobotocore-kendra-ranking-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2023-12-13 19:48:28.000000 types-aiobotocore-kendra-ranking-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:38.521584 types-aiobotocore-kendra-ranking-2.9.0/types_aiobotocore_kendra_ranking/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2023-12-13 19:48:29.000000 types-aiobotocore-kendra-ranking-2.9.0/types_aiobotocore_kendra_ranking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2023-12-13 19:48:29.000000 types-aiobotocore-kendra-ranking-2.9.0/types_aiobotocore_kendra_ranking/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      958 2023-12-13 19:48:29.000000 types-aiobotocore-kendra-ranking-2.9.0/types_aiobotocore_kendra_ranking/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9959 2023-12-13 19:48:29.000000 types-aiobotocore-kendra-ranking-2.9.0/types_aiobotocore_kendra_ranking/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9956 2023-12-13 19:48:29.000000 types-aiobotocore-kendra-ranking-2.9.0/types_aiobotocore_kendra_ranking/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8824 2023-12-13 19:48:29.000000 types-aiobotocore-kendra-ranking-2.9.0/types_aiobotocore_kendra_ranking/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8822 2023-12-13 19:48:29.000000 types-aiobotocore-kendra-ranking-2.9.0/types_aiobotocore_kendra_ranking/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:48:29.000000 types-aiobotocore-kendra-ranking-2.9.0/types_aiobotocore_kendra_ranking/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6261 2023-12-13 19:48:29.000000 types-aiobotocore-kendra-ranking-2.9.0/types_aiobotocore_kendra_ranking/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6260 2023-12-13 19:48:29.000000 types-aiobotocore-kendra-ranking-2.9.0/types_aiobotocore_kendra_ranking/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:48:29.000000 types-aiobotocore-kendra-ranking-2.9.0/types_aiobotocore_kendra_ranking/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:38.521584 types-aiobotocore-kendra-ranking-2.9.0/types_aiobotocore_kendra_ranking.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12639 2023-12-13 19:59:38.000000 types-aiobotocore-kendra-ranking-2.9.0/types_aiobotocore_kendra_ranking.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      853 2023-12-13 19:59:38.000000 types-aiobotocore-kendra-ranking-2.9.0/types_aiobotocore_kendra_ranking.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:38.000000 types-aiobotocore-kendra-ranking-2.9.0/types_aiobotocore_kendra_ranking.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:38.000000 types-aiobotocore-kendra-ranking-2.9.0/types_aiobotocore_kendra_ranking.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:38.000000 types-aiobotocore-kendra-ranking-2.9.0/types_aiobotocore_kendra_ranking.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-13 19:59:38.000000 types-aiobotocore-kendra-ranking-2.9.0/types_aiobotocore_kendra_ranking.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:01.505247 types-aiobotocore-kendra-ranking-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:10:17.000000 types-aiobotocore-kendra-ranking-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12659 2024-01-18 01:21:01.505247 types-aiobotocore-kendra-ranking-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11049 2024-01-18 01:10:17.000000 types-aiobotocore-kendra-ranking-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:01.505247 types-aiobotocore-kendra-ranking-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-01-18 01:10:17.000000 types-aiobotocore-kendra-ranking-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:01.505247 types-aiobotocore-kendra-ranking-2.9.1/types_aiobotocore_kendra_ranking/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-01-18 01:10:17.000000 types-aiobotocore-kendra-ranking-2.9.1/types_aiobotocore_kendra_ranking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-01-18 01:10:17.000000 types-aiobotocore-kendra-ranking-2.9.1/types_aiobotocore_kendra_ranking/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-01-18 01:10:17.000000 types-aiobotocore-kendra-ranking-2.9.1/types_aiobotocore_kendra_ranking/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-01-18 01:10:17.000000 types-aiobotocore-kendra-ranking-2.9.1/types_aiobotocore_kendra_ranking/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9958 2024-01-18 01:10:17.000000 types-aiobotocore-kendra-ranking-2.9.1/types_aiobotocore_kendra_ranking/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-01-18 01:10:17.000000 types-aiobotocore-kendra-ranking-2.9.1/types_aiobotocore_kendra_ranking/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-01-18 01:10:17.000000 types-aiobotocore-kendra-ranking-2.9.1/types_aiobotocore_kendra_ranking/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:10:17.000000 types-aiobotocore-kendra-ranking-2.9.1/types_aiobotocore_kendra_ranking/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-01-18 01:10:17.000000 types-aiobotocore-kendra-ranking-2.9.1/types_aiobotocore_kendra_ranking/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-01-18 01:10:17.000000 types-aiobotocore-kendra-ranking-2.9.1/types_aiobotocore_kendra_ranking/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:10:17.000000 types-aiobotocore-kendra-ranking-2.9.1/types_aiobotocore_kendra_ranking/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:01.505247 types-aiobotocore-kendra-ranking-2.9.1/types_aiobotocore_kendra_ranking.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12659 2024-01-18 01:21:01.000000 types-aiobotocore-kendra-ranking-2.9.1/types_aiobotocore_kendra_ranking.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-01-18 01:21:01.000000 types-aiobotocore-kendra-ranking-2.9.1/types_aiobotocore_kendra_ranking.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:01.000000 types-aiobotocore-kendra-ranking-2.9.1/types_aiobotocore_kendra_ranking.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:01.000000 types-aiobotocore-kendra-ranking-2.9.1/types_aiobotocore_kendra_ranking.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:01.000000 types-aiobotocore-kendra-ranking-2.9.1/types_aiobotocore_kendra_ranking.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-18 01:21:01.000000 types-aiobotocore-kendra-ranking-2.9.1/types_aiobotocore_kendra_ranking.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kendra-ranking-2.9.0/LICENSE` & `types-aiobotocore-kendra-ranking-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-kendra-ranking-2.9.0/PKG-INFO` & `types-aiobotocore-kendra-ranking-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kendra-ranking
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.KendraRanking 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.KendraRanking 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra_ranking/
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
 
 <a id="types-aiobotocore-kendra-ranking"></a>
 
 # types-aiobotocore-kendra-ranking
 
 [![PyPI - types-aiobotocore-kendra-ranking](https://img.shields.io/pypi/v/types-aiobotocore-kendra-ranking.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kendra-ranking)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kendra-ranking.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kendra-ranking)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra_ranking/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kendra-ranking)](https://pepy.tech/project/types-aiobotocore-kendra-ranking)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KendraRanking 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking)
+[aiobotocore.KendraRanking 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking)
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
 [types-aiobotocore-kendra-ranking docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra_ranking/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-kendra-ranking-2.9.0/README.md` & `types-aiobotocore-kendra-ranking-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kendra-ranking.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kendra-ranking)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra_ranking/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kendra-ranking)](https://pepy.tech/project/types-aiobotocore-kendra-ranking)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KendraRanking 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking)
+[aiobotocore.KendraRanking 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking)
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
 [types-aiobotocore-kendra-ranking docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra_ranking/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-kendra-ranking-2.9.0/setup.py` & `types-aiobotocore-kendra-ranking-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kendra-ranking",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_kendra_ranking"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.KendraRanking 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.KendraRanking 2.9.1 service generated with"
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
     keywords="aiobotocore kendra-ranking type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_kendra_ranking": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra_ranking/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-kendra-ranking-2.9.0/types_aiobotocore_kendra_ranking/__main__.py` & `types-aiobotocore-kendra-ranking-2.9.1/types_aiobotocore_kendra_ranking/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.KendraRanking 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.KendraRanking 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra_ranking//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking\nOther"
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

### Comparing `types-aiobotocore-kendra-ranking-2.9.0/types_aiobotocore_kendra_ranking/client.py` & `types-aiobotocore-kendra-ranking-2.9.1/types_aiobotocore_kendra_ranking/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     async def create_rescore_execution_plan(
         self,
         *,
         Name: str,
         Description: str = ...,
         CapacityUnits: CapacityUnitsConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateRescoreExecutionPlanResponseTypeDef:
         """
         Creates a rescore execution plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking.Client.create_rescore_execution_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra_ranking/client/#create_rescore_execution_plan)
         """
@@ -186,15 +186,15 @@
 
     async def update_rescore_execution_plan(
         self,
         *,
         Id: str,
         Name: str = ...,
         Description: str = ...,
-        CapacityUnits: CapacityUnitsConfigurationTypeDef = ...
+        CapacityUnits: CapacityUnitsConfigurationTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a rescore execution plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking.Client.update_rescore_execution_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra_ranking/client/#update_rescore_execution_plan)
         """
```

### Comparing `types-aiobotocore-kendra-ranking-2.9.0/types_aiobotocore_kendra_ranking/client.pyi` & `types-aiobotocore-kendra-ranking-2.9.1/types_aiobotocore_kendra_ranking/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     async def create_rescore_execution_plan(
         self,
         *,
         Name: str,
         Description: str = ...,
         CapacityUnits: CapacityUnitsConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateRescoreExecutionPlanResponseTypeDef:
         """
         Creates a rescore execution plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking.Client.create_rescore_execution_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra_ranking/client/#create_rescore_execution_plan)
         """
@@ -183,15 +183,15 @@
 
     async def update_rescore_execution_plan(
         self,
         *,
         Id: str,
         Name: str = ...,
         Description: str = ...,
-        CapacityUnits: CapacityUnitsConfigurationTypeDef = ...
+        CapacityUnits: CapacityUnitsConfigurationTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a rescore execution plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking.Client.update_rescore_execution_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra_ranking/client/#update_rescore_execution_plan)
         """
```

### Comparing `types-aiobotocore-kendra-ranking-2.9.0/types_aiobotocore_kendra_ranking/literals.py` & `types-aiobotocore-kendra-ranking-2.9.1/types_aiobotocore_kendra_ranking/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,24 +15,22 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "RescoreExecutionPlanStatusType",
     "KendraRankingServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 RescoreExecutionPlanStatusType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED", "UPDATING"]
 KendraRankingServiceName = Literal["kendra-ranking"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
```

### Comparing `types-aiobotocore-kendra-ranking-2.9.0/types_aiobotocore_kendra_ranking/literals.pyi` & `types-aiobotocore-kendra-ranking-2.9.1/types_aiobotocore_kendra_ranking/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kendra-ranking-2.9.0/types_aiobotocore_kendra_ranking/type_defs.py` & `types-aiobotocore-kendra-ranking-2.9.1/types_aiobotocore_kendra_ranking/type_defs.py`

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
     "CapacityUnitsConfigurationTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteRescoreExecutionPlanRequestRequestTypeDef",
     "DescribeRescoreExecutionPlanRequestRequestTypeDef",
     "DocumentTypeDef",
```

### Comparing `types-aiobotocore-kendra-ranking-2.9.0/types_aiobotocore_kendra_ranking/type_defs.pyi` & `types-aiobotocore-kendra-ranking-2.9.1/types_aiobotocore_kendra_ranking/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kendra-ranking-2.9.0/types_aiobotocore_kendra_ranking.egg-info/PKG-INFO` & `types-aiobotocore-kendra-ranking-2.9.1/types_aiobotocore_kendra_ranking.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kendra-ranking
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.KendraRanking 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.KendraRanking 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra_ranking/
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
 
 <a id="types-aiobotocore-kendra-ranking"></a>
 
 # types-aiobotocore-kendra-ranking
 
 [![PyPI - types-aiobotocore-kendra-ranking](https://img.shields.io/pypi/v/types-aiobotocore-kendra-ranking.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kendra-ranking)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kendra-ranking.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kendra-ranking)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra_ranking/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kendra-ranking)](https://pepy.tech/project/types-aiobotocore-kendra-ranking)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KendraRanking 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking)
+[aiobotocore.KendraRanking 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking)
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
 [types-aiobotocore-kendra-ranking docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra_ranking/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-kendra-ranking-2.9.0/types_aiobotocore_kendra_ranking.egg-info/SOURCES.txt` & `types-aiobotocore-kendra-ranking-2.9.1/types_aiobotocore_kendra_ranking.egg-info/SOURCES.txt`

 * *Files identical despite different names*

