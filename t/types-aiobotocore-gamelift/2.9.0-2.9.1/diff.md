# Comparing `tmp/types-aiobotocore-gamelift-2.9.0.tar.gz` & `tmp/types-aiobotocore-gamelift-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-gamelift-2.9.0.tar", last modified: Wed Dec 13 19:59:22 2023, max compression
+gzip compressed data, was "types-aiobotocore-gamelift-2.9.1.tar", last modified: Thu Jan 18 01:20:46 2024, max compression
```

## Comparing `types-aiobotocore-gamelift-2.9.0.tar` & `types-aiobotocore-gamelift-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:22.381737 types-aiobotocore-gamelift-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:46:34.000000 types-aiobotocore-gamelift-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16418 2023-12-13 19:59:22.381737 types-aiobotocore-gamelift-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14851 2023-12-13 19:46:34.000000 types-aiobotocore-gamelift-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:22.381737 types-aiobotocore-gamelift-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-12-13 19:46:34.000000 types-aiobotocore-gamelift-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:22.377737 types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift/
--rw-r--r--   0 runner    (1001) docker     (127)     5418 2023-12-13 19:46:34.000000 types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5417 2023-12-13 19:46:34.000000 types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-12-13 19:46:34.000000 types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    89216 2023-12-13 19:46:36.000000 types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    89212 2023-12-13 19:46:34.000000 types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    22491 2023-12-13 19:46:36.000000 types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    22489 2023-12-13 19:46:36.000000 types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    27652 2023-12-13 19:46:36.000000 types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    27628 2023-12-13 19:46:36.000000 types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:46:34.000000 types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    89649 2023-12-13 19:46:38.000000 types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    89648 2023-12-13 19:46:37.000000 types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:46:34.000000 types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:22.381737 types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16418 2023-12-13 19:59:22.000000 types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-12-13 19:59:22.000000 types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:22.000000 types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:22.000000 types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:22.000000 types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-13 19:59:22.000000 types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:46.589315 types-aiobotocore-gamelift-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:08:28.000000 types-aiobotocore-gamelift-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-01-18 01:20:46.589315 types-aiobotocore-gamelift-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14851 2024-01-18 01:08:28.000000 types-aiobotocore-gamelift-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:46.589315 types-aiobotocore-gamelift-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-18 01:08:28.000000 types-aiobotocore-gamelift-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:46.589315 types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift/
+-rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-01-18 01:08:28.000000 types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-01-18 01:08:28.000000 types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-01-18 01:08:28.000000 types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89254 2024-01-18 01:08:29.000000 types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89251 2024-01-18 01:08:28.000000 types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    22489 2024-01-18 01:08:29.000000 types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22489 2024-01-18 01:08:29.000000 types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    27664 2024-01-18 01:08:29.000000 types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27641 2024-01-18 01:08:29.000000 types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:08:28.000000 types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    89648 2024-01-18 01:08:32.000000 types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89648 2024-01-18 01:08:30.000000 types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:08:28.000000 types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:46.589315 types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-01-18 01:20:46.000000 types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-01-18 01:20:46.000000 types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:46.000000 types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:46.000000 types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:46.000000 types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-18 01:20:46.000000 types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-gamelift-2.9.0/LICENSE` & `types-aiobotocore-gamelift-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-gamelift-2.9.0/PKG-INFO` & `types-aiobotocore-gamelift-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-gamelift
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.GameLift 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.GameLift 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/
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
 
 <a id="types-aiobotocore-gamelift"></a>
 
 # types-aiobotocore-gamelift
 
 [![PyPI - types-aiobotocore-gamelift](https://img.shields.io/pypi/v/types-aiobotocore-gamelift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-gamelift)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-gamelift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-gamelift)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-gamelift)](https://pepy.tech/project/types-aiobotocore-gamelift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GameLift 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
+[aiobotocore.GameLift 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
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
 [types-aiobotocore-gamelift docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-gamelift-2.9.0/README.md` & `types-aiobotocore-gamelift-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-gamelift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-gamelift)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-gamelift)](https://pepy.tech/project/types-aiobotocore-gamelift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GameLift 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
+[aiobotocore.GameLift 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
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
 [types-aiobotocore-gamelift docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-gamelift-2.9.0/setup.py` & `types-aiobotocore-gamelift-2.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-gamelift",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_gamelift"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.GameLift 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.GameLift 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore gamelift type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_gamelift": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift/__init__.py` & `types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,14 @@
     ListLocationsPaginator,
     ListScriptsPaginator,
     SearchGameSessionsPaginator,
 )
 
 Client = GameLiftClient
 
-
 __all__ = (
     "Client",
     "DescribeFleetAttributesPaginator",
     "DescribeFleetCapacityPaginator",
     "DescribeFleetEventsPaginator",
     "DescribeFleetUtilizationPaginator",
     "DescribeGameServerInstancesPaginator",
```

### Comparing `types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift/__init__.pyi` & `types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift/__main__.py` & `types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.GameLift 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.GameLift 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift\nOther"
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

### Comparing `types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift/client.py` & `types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("GameLiftClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -256,15 +255,15 @@
 
     async def claim_game_server(
         self,
         *,
         GameServerGroupName: str,
         GameServerId: str = ...,
         GameServerData: str = ...,
-        FilterOption: ClaimFilterOptionTypeDef = ...
+        FilterOption: ClaimFilterOptionTypeDef = ...,
     ) -> ClaimGameServerOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Locates an available game server and temporarily reserves it
         to host gameplay and
         players.
 
@@ -282,15 +281,15 @@
 
     async def create_alias(
         self,
         *,
         Name: str,
         RoutingStrategy: RoutingStrategyTypeDef,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAliasOutputTypeDef:
         """
         Creates an alias for a fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_alias)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#create_alias)
         """
@@ -299,15 +298,15 @@
         self,
         *,
         Name: str = ...,
         Version: str = ...,
         StorageLocation: S3LocationTypeDef = ...,
         OperatingSystem: OperatingSystemType = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ServerSdkVersion: str = ...
+        ServerSdkVersion: str = ...,
     ) -> CreateBuildOutputTypeDef:
         """
         Creates a new Amazon GameLift build resource for your game server binary files.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_build)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#create_build)
         """
@@ -333,15 +332,15 @@
         FleetType: FleetTypeType = ...,
         InstanceRoleArn: str = ...,
         CertificateConfiguration: CertificateConfigurationTypeDef = ...,
         Locations: Sequence[LocationConfigurationTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ComputeType: ComputeTypeType = ...,
         AnywhereConfiguration: AnywhereConfigurationTypeDef = ...,
-        InstanceRoleCredentialsProvider: Literal["SHARED_CREDENTIAL_FILE"] = ...
+        InstanceRoleCredentialsProvider: Literal["SHARED_CREDENTIAL_FILE"] = ...,
     ) -> CreateFleetOutputTypeDef:
         """
         Creates a fleet of Amazon Elastic Compute Cloud (Amazon EC2) instances to host
         your custom game server or Realtime
         Servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_fleet)
@@ -369,15 +368,15 @@
         MaxSize: int,
         LaunchTemplate: LaunchTemplateSpecificationTypeDef,
         InstanceDefinitions: Sequence[InstanceDefinitionTypeDef],
         AutoScalingPolicy: GameServerGroupAutoScalingPolicyTypeDef = ...,
         BalancingStrategy: BalancingStrategyType = ...,
         GameServerProtectionPolicy: GameServerProtectionPolicyType = ...,
         VpcSubnets: Sequence[str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateGameServerGroupOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Creates a Amazon GameLift FleetIQ game server group for
         managing game hosting on a collection of Amazon Elastic Compute Cloud instances
         for game
         hosting.
@@ -394,15 +393,15 @@
         AliasId: str = ...,
         Name: str = ...,
         GameProperties: Sequence[GamePropertyTypeDef] = ...,
         CreatorId: str = ...,
         GameSessionId: str = ...,
         IdempotencyToken: str = ...,
         GameSessionData: str = ...,
-        Location: str = ...
+        Location: str = ...,
     ) -> CreateGameSessionOutputTypeDef:
         """
         Creates a multiplayer game session for players in a specific fleet location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_game_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#create_game_session)
         """
@@ -414,15 +413,15 @@
         TimeoutInSeconds: int = ...,
         PlayerLatencyPolicies: Sequence[PlayerLatencyPolicyTypeDef] = ...,
         Destinations: Sequence[GameSessionQueueDestinationTypeDef] = ...,
         FilterConfiguration: FilterConfigurationTypeDef = ...,
         PriorityConfiguration: PriorityConfigurationTypeDef = ...,
         CustomEventData: str = ...,
         NotificationTarget: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateGameSessionQueueOutputTypeDef:
         """
         Creates a placement queue that processes requests for new game sessions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_game_session_queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#create_game_session_queue)
         """
@@ -450,15 +449,15 @@
         NotificationTarget: str = ...,
         AdditionalPlayerCount: int = ...,
         CustomEventData: str = ...,
         GameProperties: Sequence[GamePropertyTypeDef] = ...,
         GameSessionData: str = ...,
         BackfillMode: BackfillModeType = ...,
         FlexMatchMode: FlexMatchModeType = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMatchmakingConfigurationOutputTypeDef:
         """
         Defines a new matchmaking configuration for use with FlexMatch.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_matchmaking_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#create_matchmaking_configuration)
         """
@@ -484,15 +483,15 @@
         """
 
     async def create_player_sessions(
         self,
         *,
         GameSessionId: str,
         PlayerIds: Sequence[str],
-        PlayerDataMap: Mapping[str, str] = ...
+        PlayerDataMap: Mapping[str, str] = ...,
     ) -> CreatePlayerSessionsOutputTypeDef:
         """
         Reserves open slots in a game session for a group of players.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_player_sessions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#create_player_sessions)
         """
@@ -500,15 +499,15 @@
     async def create_script(
         self,
         *,
         Name: str = ...,
         Version: str = ...,
         StorageLocation: S3LocationTypeDef = ...,
         ZipFile: BlobTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateScriptOutputTypeDef:
         """
         Creates a new script record for your Realtime Servers script.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_script)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#create_script)
         """
@@ -738,30 +737,30 @@
     async def describe_fleet_events(
         self,
         *,
         FleetId: str,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeFleetEventsOutputTypeDef:
         """
         Retrieves entries from a fleet's event log.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_fleet_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#describe_fleet_events)
         """
 
     async def describe_fleet_location_attributes(
         self,
         *,
         FleetId: str,
         Locations: Sequence[str] = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeFleetLocationAttributesOutputTypeDef:
         """
         Retrieves information on a fleet's remote locations, including life-cycle
         status and any suspended fleet
         activity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_fleet_location_attributes)
@@ -834,15 +833,15 @@
 
     async def describe_game_server_instances(
         self,
         *,
         GameServerGroupName: str,
         InstanceIds: Sequence[str] = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeGameServerInstancesOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Retrieves status information about the Amazon EC2 instances
         associated with a Amazon GameLift FleetIQ game server
         group.
 
@@ -855,15 +854,15 @@
         *,
         FleetId: str = ...,
         GameSessionId: str = ...,
         AliasId: str = ...,
         Location: str = ...,
         StatusFilter: str = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeGameSessionDetailsOutputTypeDef:
         """
         Retrieves additional game session properties, including the game session
         protection policy in force, a set of one or more game sessions in a specific
         fleet
         location.
 
@@ -897,15 +896,15 @@
         *,
         FleetId: str = ...,
         GameSessionId: str = ...,
         AliasId: str = ...,
         Location: str = ...,
         StatusFilter: str = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeGameSessionsOutputTypeDef:
         """
         Retrieves a set of one or more game sessions in a specific fleet location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_game_sessions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#describe_game_sessions)
         """
@@ -913,15 +912,15 @@
     async def describe_instances(
         self,
         *,
         FleetId: str,
         InstanceId: str = ...,
         Limit: int = ...,
         NextToken: str = ...,
-        Location: str = ...
+        Location: str = ...,
     ) -> DescribeInstancesOutputTypeDef:
         """
         Retrieves information about the EC2 instances in an Amazon GameLift managed
         fleet, including instance ID, connection data, and
         status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_instances)
@@ -940,15 +939,15 @@
 
     async def describe_matchmaking_configurations(
         self,
         *,
         Names: Sequence[str] = ...,
         RuleSetName: str = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeMatchmakingConfigurationsOutputTypeDef:
         """
         Retrieves the details of FlexMatch matchmaking configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_matchmaking_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#describe_matchmaking_configurations)
         """
@@ -967,15 +966,15 @@
         self,
         *,
         GameSessionId: str = ...,
         PlayerId: str = ...,
         PlayerSessionId: str = ...,
         PlayerSessionStatusFilter: str = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribePlayerSessionsOutputTypeDef:
         """
         Retrieves properties for one or more player sessions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_player_sessions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#describe_player_sessions)
         """
@@ -993,15 +992,15 @@
     async def describe_scaling_policies(
         self,
         *,
         FleetId: str,
         StatusFilter: ScalingStatusTypeType = ...,
         Limit: int = ...,
         NextToken: str = ...,
-        Location: str = ...
+        Location: str = ...,
     ) -> DescribeScalingPoliciesOutputTypeDef:
         """
         Retrieves all scaling policies applied to a fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_scaling_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#describe_scaling_policies)
         """
@@ -1100,15 +1099,15 @@
 
     async def list_aliases(
         self,
         *,
         RoutingStrategyType: RoutingStrategyTypeType = ...,
         Name: str = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAliasesOutputTypeDef:
         """
         Retrieves all aliases for this Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.list_aliases)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#list_aliases)
         """
@@ -1157,15 +1156,15 @@
 
     async def list_game_servers(
         self,
         *,
         GameServerGroupName: str,
         SortOrder: SortOrderType = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListGameServersOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Retrieves information on all game servers that are currently
         active in a specified game server
         group.
 
@@ -1213,15 +1212,15 @@
         MetricName: MetricNameType,
         ScalingAdjustment: int = ...,
         ScalingAdjustmentType: ScalingAdjustmentTypeType = ...,
         Threshold: float = ...,
         ComparisonOperator: ComparisonOperatorTypeType = ...,
         EvaluationPeriods: int = ...,
         PolicyType: PolicyTypeType = ...,
-        TargetConfiguration: TargetConfigurationTypeDef = ...
+        TargetConfiguration: TargetConfigurationTypeDef = ...,
     ) -> PutScalingPolicyOutputTypeDef:
         """
         Creates or updates a scaling policy for a fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.put_scaling_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#put_scaling_policy)
         """
@@ -1230,15 +1229,15 @@
         self,
         *,
         FleetId: str,
         ComputeName: str,
         CertificatePath: str = ...,
         DnsName: str = ...,
         IpAddress: str = ...,
-        Location: str = ...
+        Location: str = ...,
     ) -> RegisterComputeOutputTypeDef:
         """
         Registers a compute resource to an Amazon GameLift Anywhere fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.register_compute)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#register_compute)
         """
@@ -1246,15 +1245,15 @@
     async def register_game_server(
         self,
         *,
         GameServerGroupName: str,
         GameServerId: str,
         InstanceId: str,
         ConnectionInfo: str = ...,
-        GameServerData: str = ...
+        GameServerData: str = ...,
     ) -> RegisterGameServerOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Creates a new game server resource and notifies Amazon
         GameLift FleetIQ that the game server is ready to host gameplay and
         players.
 
@@ -1282,15 +1281,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#resolve_alias)
         """
 
     async def resume_game_server_group(
         self,
         *,
         GameServerGroupName: str,
-        ResumeActions: Sequence[Literal["REPLACE_INSTANCE_TYPES"]]
+        ResumeActions: Sequence[Literal["REPLACE_INSTANCE_TYPES"]],
     ) -> ResumeGameServerGroupOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Reinstates activity on a game server group after it has been
         suspended.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.resume_game_server_group)
@@ -1302,15 +1301,15 @@
         *,
         FleetId: str = ...,
         AliasId: str = ...,
         Location: str = ...,
         FilterExpression: str = ...,
         SortExpression: str = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> SearchGameSessionsOutputTypeDef:
         """
         Retrieves all active game sessions that match a set of search criteria and
         sorts them into a specified
         order.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.search_game_sessions)
@@ -1334,30 +1333,30 @@
         PlacementId: str,
         GameSessionQueueName: str,
         MaximumPlayerSessionCount: int,
         GameProperties: Sequence[GamePropertyTypeDef] = ...,
         GameSessionName: str = ...,
         PlayerLatencies: Sequence[PlayerLatencyTypeDef] = ...,
         DesiredPlayerSessions: Sequence[DesiredPlayerSessionTypeDef] = ...,
-        GameSessionData: str = ...
+        GameSessionData: str = ...,
     ) -> StartGameSessionPlacementOutputTypeDef:
         """
         Places a request for a new game session in a queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.start_game_session_placement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#start_game_session_placement)
         """
 
     async def start_match_backfill(
         self,
         *,
         ConfigurationName: str,
         Players: Sequence[PlayerTypeDef],
         TicketId: str = ...,
-        GameSessionArn: str = ...
+        GameSessionArn: str = ...,
     ) -> StartMatchBackfillOutputTypeDef:
         """
         Finds new players to fill open slots in currently running game sessions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.start_match_backfill)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#start_match_backfill)
         """
@@ -1403,15 +1402,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#stop_matchmaking)
         """
 
     async def suspend_game_server_group(
         self,
         *,
         GameServerGroupName: str,
-        SuspendActions: Sequence[Literal["REPLACE_INSTANCE_TYPES"]]
+        SuspendActions: Sequence[Literal["REPLACE_INSTANCE_TYPES"]],
     ) -> SuspendGameServerGroupOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Temporarily stops activity on a game server group without
         terminating instances or the game server
         group.
 
@@ -1437,15 +1436,15 @@
 
     async def update_alias(
         self,
         *,
         AliasId: str,
         Name: str = ...,
         Description: str = ...,
-        RoutingStrategy: RoutingStrategyTypeDef = ...
+        RoutingStrategy: RoutingStrategyTypeDef = ...,
     ) -> UpdateAliasOutputTypeDef:
         """
         Updates properties for an alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_alias)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#update_alias)
         """
@@ -1465,15 +1464,15 @@
         *,
         FleetId: str,
         Name: str = ...,
         Description: str = ...,
         NewGameSessionProtectionPolicy: ProtectionPolicyType = ...,
         ResourceCreationLimitPolicy: ResourceCreationLimitPolicyTypeDef = ...,
         MetricGroups: Sequence[str] = ...,
-        AnywhereConfiguration: AnywhereConfigurationTypeDef = ...
+        AnywhereConfiguration: AnywhereConfigurationTypeDef = ...,
     ) -> UpdateFleetAttributesOutputTypeDef:
         """
         Updates a fleet's mutable attributes, including game session protection and
         resource creation
         limits.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_fleet_attributes)
@@ -1483,29 +1482,29 @@
     async def update_fleet_capacity(
         self,
         *,
         FleetId: str,
         DesiredInstances: int = ...,
         MinSize: int = ...,
         MaxSize: int = ...,
-        Location: str = ...
+        Location: str = ...,
     ) -> UpdateFleetCapacityOutputTypeDef:
         """
         Updates capacity settings for a fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_fleet_capacity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#update_fleet_capacity)
         """
 
     async def update_fleet_port_settings(
         self,
         *,
         FleetId: str,
         InboundPermissionAuthorizations: Sequence[IpPermissionTypeDef] = ...,
-        InboundPermissionRevocations: Sequence[IpPermissionTypeDef] = ...
+        InboundPermissionRevocations: Sequence[IpPermissionTypeDef] = ...,
     ) -> UpdateFleetPortSettingsOutputTypeDef:
         """
         Updates permissions that allow inbound traffic to connect to game sessions that
         are being hosted on instances in the
         fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_fleet_port_settings)
@@ -1515,15 +1514,15 @@
     async def update_game_server(
         self,
         *,
         GameServerGroupName: str,
         GameServerId: str,
         GameServerData: str = ...,
         UtilizationStatus: GameServerUtilizationStatusType = ...,
-        HealthCheck: Literal["HEALTHY"] = ...
+        HealthCheck: Literal["HEALTHY"] = ...,
     ) -> UpdateGameServerOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Updates information about a registered game server to help
         Amazon GameLift FleetIQ track game server
         availability.
 
@@ -1534,15 +1533,15 @@
     async def update_game_server_group(
         self,
         *,
         GameServerGroupName: str,
         RoleArn: str = ...,
         InstanceDefinitions: Sequence[InstanceDefinitionTypeDef] = ...,
         GameServerProtectionPolicy: GameServerProtectionPolicyType = ...,
-        BalancingStrategy: BalancingStrategyType = ...
+        BalancingStrategy: BalancingStrategyType = ...,
     ) -> UpdateGameServerGroupOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Updates Amazon GameLift FleetIQ-specific properties for a game
         server
         group.
 
@@ -1553,15 +1552,15 @@
     async def update_game_session(
         self,
         *,
         GameSessionId: str,
         MaximumPlayerSessionCount: int = ...,
         Name: str = ...,
         PlayerSessionCreationPolicy: PlayerSessionCreationPolicyType = ...,
-        ProtectionPolicy: ProtectionPolicyType = ...
+        ProtectionPolicy: ProtectionPolicyType = ...,
     ) -> UpdateGameSessionOutputTypeDef:
         """
         Updates the mutable properties of a game session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_game_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#update_game_session)
         """
@@ -1572,15 +1571,15 @@
         Name: str,
         TimeoutInSeconds: int = ...,
         PlayerLatencyPolicies: Sequence[PlayerLatencyPolicyTypeDef] = ...,
         Destinations: Sequence[GameSessionQueueDestinationTypeDef] = ...,
         FilterConfiguration: FilterConfigurationTypeDef = ...,
         PriorityConfiguration: PriorityConfigurationTypeDef = ...,
         CustomEventData: str = ...,
-        NotificationTarget: str = ...
+        NotificationTarget: str = ...,
     ) -> UpdateGameSessionQueueOutputTypeDef:
         """
         Updates the configuration of a game session queue, which determines how the
         queue processes new game session
         requests.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_game_session_queue)
@@ -1599,15 +1598,15 @@
         RuleSetName: str = ...,
         NotificationTarget: str = ...,
         AdditionalPlayerCount: int = ...,
         CustomEventData: str = ...,
         GameProperties: Sequence[GamePropertyTypeDef] = ...,
         GameSessionData: str = ...,
         BackfillMode: BackfillModeType = ...,
-        FlexMatchMode: FlexMatchModeType = ...
+        FlexMatchMode: FlexMatchModeType = ...,
     ) -> UpdateMatchmakingConfigurationOutputTypeDef:
         """
         Updates settings for a FlexMatch matchmaking configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_matchmaking_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#update_matchmaking_configuration)
         """
@@ -1627,15 +1626,15 @@
     async def update_script(
         self,
         *,
         ScriptId: str,
         Name: str = ...,
         Version: str = ...,
         StorageLocation: S3LocationTypeDef = ...,
-        ZipFile: BlobTypeDef = ...
+        ZipFile: BlobTypeDef = ...,
     ) -> UpdateScriptOutputTypeDef:
         """
         Updates Realtime script metadata and content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_script)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#update_script)
         """
```

### Comparing `types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift/client.pyi` & `types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -252,15 +252,15 @@
 
     async def claim_game_server(
         self,
         *,
         GameServerGroupName: str,
         GameServerId: str = ...,
         GameServerData: str = ...,
-        FilterOption: ClaimFilterOptionTypeDef = ...
+        FilterOption: ClaimFilterOptionTypeDef = ...,
     ) -> ClaimGameServerOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Locates an available game server and temporarily reserves it
         to host gameplay and
         players.
 
@@ -278,15 +278,15 @@
 
     async def create_alias(
         self,
         *,
         Name: str,
         RoutingStrategy: RoutingStrategyTypeDef,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAliasOutputTypeDef:
         """
         Creates an alias for a fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_alias)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#create_alias)
         """
@@ -295,15 +295,15 @@
         self,
         *,
         Name: str = ...,
         Version: str = ...,
         StorageLocation: S3LocationTypeDef = ...,
         OperatingSystem: OperatingSystemType = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ServerSdkVersion: str = ...
+        ServerSdkVersion: str = ...,
     ) -> CreateBuildOutputTypeDef:
         """
         Creates a new Amazon GameLift build resource for your game server binary files.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_build)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#create_build)
         """
@@ -329,15 +329,15 @@
         FleetType: FleetTypeType = ...,
         InstanceRoleArn: str = ...,
         CertificateConfiguration: CertificateConfigurationTypeDef = ...,
         Locations: Sequence[LocationConfigurationTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ComputeType: ComputeTypeType = ...,
         AnywhereConfiguration: AnywhereConfigurationTypeDef = ...,
-        InstanceRoleCredentialsProvider: Literal["SHARED_CREDENTIAL_FILE"] = ...
+        InstanceRoleCredentialsProvider: Literal["SHARED_CREDENTIAL_FILE"] = ...,
     ) -> CreateFleetOutputTypeDef:
         """
         Creates a fleet of Amazon Elastic Compute Cloud (Amazon EC2) instances to host
         your custom game server or Realtime
         Servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_fleet)
@@ -365,15 +365,15 @@
         MaxSize: int,
         LaunchTemplate: LaunchTemplateSpecificationTypeDef,
         InstanceDefinitions: Sequence[InstanceDefinitionTypeDef],
         AutoScalingPolicy: GameServerGroupAutoScalingPolicyTypeDef = ...,
         BalancingStrategy: BalancingStrategyType = ...,
         GameServerProtectionPolicy: GameServerProtectionPolicyType = ...,
         VpcSubnets: Sequence[str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateGameServerGroupOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Creates a Amazon GameLift FleetIQ game server group for
         managing game hosting on a collection of Amazon Elastic Compute Cloud instances
         for game
         hosting.
@@ -390,15 +390,15 @@
         AliasId: str = ...,
         Name: str = ...,
         GameProperties: Sequence[GamePropertyTypeDef] = ...,
         CreatorId: str = ...,
         GameSessionId: str = ...,
         IdempotencyToken: str = ...,
         GameSessionData: str = ...,
-        Location: str = ...
+        Location: str = ...,
     ) -> CreateGameSessionOutputTypeDef:
         """
         Creates a multiplayer game session for players in a specific fleet location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_game_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#create_game_session)
         """
@@ -410,15 +410,15 @@
         TimeoutInSeconds: int = ...,
         PlayerLatencyPolicies: Sequence[PlayerLatencyPolicyTypeDef] = ...,
         Destinations: Sequence[GameSessionQueueDestinationTypeDef] = ...,
         FilterConfiguration: FilterConfigurationTypeDef = ...,
         PriorityConfiguration: PriorityConfigurationTypeDef = ...,
         CustomEventData: str = ...,
         NotificationTarget: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateGameSessionQueueOutputTypeDef:
         """
         Creates a placement queue that processes requests for new game sessions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_game_session_queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#create_game_session_queue)
         """
@@ -446,15 +446,15 @@
         NotificationTarget: str = ...,
         AdditionalPlayerCount: int = ...,
         CustomEventData: str = ...,
         GameProperties: Sequence[GamePropertyTypeDef] = ...,
         GameSessionData: str = ...,
         BackfillMode: BackfillModeType = ...,
         FlexMatchMode: FlexMatchModeType = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMatchmakingConfigurationOutputTypeDef:
         """
         Defines a new matchmaking configuration for use with FlexMatch.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_matchmaking_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#create_matchmaking_configuration)
         """
@@ -480,15 +480,15 @@
         """
 
     async def create_player_sessions(
         self,
         *,
         GameSessionId: str,
         PlayerIds: Sequence[str],
-        PlayerDataMap: Mapping[str, str] = ...
+        PlayerDataMap: Mapping[str, str] = ...,
     ) -> CreatePlayerSessionsOutputTypeDef:
         """
         Reserves open slots in a game session for a group of players.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_player_sessions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#create_player_sessions)
         """
@@ -496,15 +496,15 @@
     async def create_script(
         self,
         *,
         Name: str = ...,
         Version: str = ...,
         StorageLocation: S3LocationTypeDef = ...,
         ZipFile: BlobTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateScriptOutputTypeDef:
         """
         Creates a new script record for your Realtime Servers script.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_script)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#create_script)
         """
@@ -734,30 +734,30 @@
     async def describe_fleet_events(
         self,
         *,
         FleetId: str,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeFleetEventsOutputTypeDef:
         """
         Retrieves entries from a fleet's event log.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_fleet_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#describe_fleet_events)
         """
 
     async def describe_fleet_location_attributes(
         self,
         *,
         FleetId: str,
         Locations: Sequence[str] = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeFleetLocationAttributesOutputTypeDef:
         """
         Retrieves information on a fleet's remote locations, including life-cycle
         status and any suspended fleet
         activity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_fleet_location_attributes)
@@ -830,15 +830,15 @@
 
     async def describe_game_server_instances(
         self,
         *,
         GameServerGroupName: str,
         InstanceIds: Sequence[str] = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeGameServerInstancesOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Retrieves status information about the Amazon EC2 instances
         associated with a Amazon GameLift FleetIQ game server
         group.
 
@@ -851,15 +851,15 @@
         *,
         FleetId: str = ...,
         GameSessionId: str = ...,
         AliasId: str = ...,
         Location: str = ...,
         StatusFilter: str = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeGameSessionDetailsOutputTypeDef:
         """
         Retrieves additional game session properties, including the game session
         protection policy in force, a set of one or more game sessions in a specific
         fleet
         location.
 
@@ -893,15 +893,15 @@
         *,
         FleetId: str = ...,
         GameSessionId: str = ...,
         AliasId: str = ...,
         Location: str = ...,
         StatusFilter: str = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeGameSessionsOutputTypeDef:
         """
         Retrieves a set of one or more game sessions in a specific fleet location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_game_sessions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#describe_game_sessions)
         """
@@ -909,15 +909,15 @@
     async def describe_instances(
         self,
         *,
         FleetId: str,
         InstanceId: str = ...,
         Limit: int = ...,
         NextToken: str = ...,
-        Location: str = ...
+        Location: str = ...,
     ) -> DescribeInstancesOutputTypeDef:
         """
         Retrieves information about the EC2 instances in an Amazon GameLift managed
         fleet, including instance ID, connection data, and
         status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_instances)
@@ -936,15 +936,15 @@
 
     async def describe_matchmaking_configurations(
         self,
         *,
         Names: Sequence[str] = ...,
         RuleSetName: str = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeMatchmakingConfigurationsOutputTypeDef:
         """
         Retrieves the details of FlexMatch matchmaking configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_matchmaking_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#describe_matchmaking_configurations)
         """
@@ -963,15 +963,15 @@
         self,
         *,
         GameSessionId: str = ...,
         PlayerId: str = ...,
         PlayerSessionId: str = ...,
         PlayerSessionStatusFilter: str = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribePlayerSessionsOutputTypeDef:
         """
         Retrieves properties for one or more player sessions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_player_sessions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#describe_player_sessions)
         """
@@ -989,15 +989,15 @@
     async def describe_scaling_policies(
         self,
         *,
         FleetId: str,
         StatusFilter: ScalingStatusTypeType = ...,
         Limit: int = ...,
         NextToken: str = ...,
-        Location: str = ...
+        Location: str = ...,
     ) -> DescribeScalingPoliciesOutputTypeDef:
         """
         Retrieves all scaling policies applied to a fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_scaling_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#describe_scaling_policies)
         """
@@ -1096,15 +1096,15 @@
 
     async def list_aliases(
         self,
         *,
         RoutingStrategyType: RoutingStrategyTypeType = ...,
         Name: str = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAliasesOutputTypeDef:
         """
         Retrieves all aliases for this Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.list_aliases)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#list_aliases)
         """
@@ -1153,15 +1153,15 @@
 
     async def list_game_servers(
         self,
         *,
         GameServerGroupName: str,
         SortOrder: SortOrderType = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListGameServersOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Retrieves information on all game servers that are currently
         active in a specified game server
         group.
 
@@ -1209,15 +1209,15 @@
         MetricName: MetricNameType,
         ScalingAdjustment: int = ...,
         ScalingAdjustmentType: ScalingAdjustmentTypeType = ...,
         Threshold: float = ...,
         ComparisonOperator: ComparisonOperatorTypeType = ...,
         EvaluationPeriods: int = ...,
         PolicyType: PolicyTypeType = ...,
-        TargetConfiguration: TargetConfigurationTypeDef = ...
+        TargetConfiguration: TargetConfigurationTypeDef = ...,
     ) -> PutScalingPolicyOutputTypeDef:
         """
         Creates or updates a scaling policy for a fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.put_scaling_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#put_scaling_policy)
         """
@@ -1226,15 +1226,15 @@
         self,
         *,
         FleetId: str,
         ComputeName: str,
         CertificatePath: str = ...,
         DnsName: str = ...,
         IpAddress: str = ...,
-        Location: str = ...
+        Location: str = ...,
     ) -> RegisterComputeOutputTypeDef:
         """
         Registers a compute resource to an Amazon GameLift Anywhere fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.register_compute)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#register_compute)
         """
@@ -1242,15 +1242,15 @@
     async def register_game_server(
         self,
         *,
         GameServerGroupName: str,
         GameServerId: str,
         InstanceId: str,
         ConnectionInfo: str = ...,
-        GameServerData: str = ...
+        GameServerData: str = ...,
     ) -> RegisterGameServerOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Creates a new game server resource and notifies Amazon
         GameLift FleetIQ that the game server is ready to host gameplay and
         players.
 
@@ -1278,15 +1278,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#resolve_alias)
         """
 
     async def resume_game_server_group(
         self,
         *,
         GameServerGroupName: str,
-        ResumeActions: Sequence[Literal["REPLACE_INSTANCE_TYPES"]]
+        ResumeActions: Sequence[Literal["REPLACE_INSTANCE_TYPES"]],
     ) -> ResumeGameServerGroupOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Reinstates activity on a game server group after it has been
         suspended.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.resume_game_server_group)
@@ -1298,15 +1298,15 @@
         *,
         FleetId: str = ...,
         AliasId: str = ...,
         Location: str = ...,
         FilterExpression: str = ...,
         SortExpression: str = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> SearchGameSessionsOutputTypeDef:
         """
         Retrieves all active game sessions that match a set of search criteria and
         sorts them into a specified
         order.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.search_game_sessions)
@@ -1330,30 +1330,30 @@
         PlacementId: str,
         GameSessionQueueName: str,
         MaximumPlayerSessionCount: int,
         GameProperties: Sequence[GamePropertyTypeDef] = ...,
         GameSessionName: str = ...,
         PlayerLatencies: Sequence[PlayerLatencyTypeDef] = ...,
         DesiredPlayerSessions: Sequence[DesiredPlayerSessionTypeDef] = ...,
-        GameSessionData: str = ...
+        GameSessionData: str = ...,
     ) -> StartGameSessionPlacementOutputTypeDef:
         """
         Places a request for a new game session in a queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.start_game_session_placement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#start_game_session_placement)
         """
 
     async def start_match_backfill(
         self,
         *,
         ConfigurationName: str,
         Players: Sequence[PlayerTypeDef],
         TicketId: str = ...,
-        GameSessionArn: str = ...
+        GameSessionArn: str = ...,
     ) -> StartMatchBackfillOutputTypeDef:
         """
         Finds new players to fill open slots in currently running game sessions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.start_match_backfill)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#start_match_backfill)
         """
@@ -1399,15 +1399,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#stop_matchmaking)
         """
 
     async def suspend_game_server_group(
         self,
         *,
         GameServerGroupName: str,
-        SuspendActions: Sequence[Literal["REPLACE_INSTANCE_TYPES"]]
+        SuspendActions: Sequence[Literal["REPLACE_INSTANCE_TYPES"]],
     ) -> SuspendGameServerGroupOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Temporarily stops activity on a game server group without
         terminating instances or the game server
         group.
 
@@ -1433,15 +1433,15 @@
 
     async def update_alias(
         self,
         *,
         AliasId: str,
         Name: str = ...,
         Description: str = ...,
-        RoutingStrategy: RoutingStrategyTypeDef = ...
+        RoutingStrategy: RoutingStrategyTypeDef = ...,
     ) -> UpdateAliasOutputTypeDef:
         """
         Updates properties for an alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_alias)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#update_alias)
         """
@@ -1461,15 +1461,15 @@
         *,
         FleetId: str,
         Name: str = ...,
         Description: str = ...,
         NewGameSessionProtectionPolicy: ProtectionPolicyType = ...,
         ResourceCreationLimitPolicy: ResourceCreationLimitPolicyTypeDef = ...,
         MetricGroups: Sequence[str] = ...,
-        AnywhereConfiguration: AnywhereConfigurationTypeDef = ...
+        AnywhereConfiguration: AnywhereConfigurationTypeDef = ...,
     ) -> UpdateFleetAttributesOutputTypeDef:
         """
         Updates a fleet's mutable attributes, including game session protection and
         resource creation
         limits.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_fleet_attributes)
@@ -1479,29 +1479,29 @@
     async def update_fleet_capacity(
         self,
         *,
         FleetId: str,
         DesiredInstances: int = ...,
         MinSize: int = ...,
         MaxSize: int = ...,
-        Location: str = ...
+        Location: str = ...,
     ) -> UpdateFleetCapacityOutputTypeDef:
         """
         Updates capacity settings for a fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_fleet_capacity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#update_fleet_capacity)
         """
 
     async def update_fleet_port_settings(
         self,
         *,
         FleetId: str,
         InboundPermissionAuthorizations: Sequence[IpPermissionTypeDef] = ...,
-        InboundPermissionRevocations: Sequence[IpPermissionTypeDef] = ...
+        InboundPermissionRevocations: Sequence[IpPermissionTypeDef] = ...,
     ) -> UpdateFleetPortSettingsOutputTypeDef:
         """
         Updates permissions that allow inbound traffic to connect to game sessions that
         are being hosted on instances in the
         fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_fleet_port_settings)
@@ -1511,15 +1511,15 @@
     async def update_game_server(
         self,
         *,
         GameServerGroupName: str,
         GameServerId: str,
         GameServerData: str = ...,
         UtilizationStatus: GameServerUtilizationStatusType = ...,
-        HealthCheck: Literal["HEALTHY"] = ...
+        HealthCheck: Literal["HEALTHY"] = ...,
     ) -> UpdateGameServerOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Updates information about a registered game server to help
         Amazon GameLift FleetIQ track game server
         availability.
 
@@ -1530,15 +1530,15 @@
     async def update_game_server_group(
         self,
         *,
         GameServerGroupName: str,
         RoleArn: str = ...,
         InstanceDefinitions: Sequence[InstanceDefinitionTypeDef] = ...,
         GameServerProtectionPolicy: GameServerProtectionPolicyType = ...,
-        BalancingStrategy: BalancingStrategyType = ...
+        BalancingStrategy: BalancingStrategyType = ...,
     ) -> UpdateGameServerGroupOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Updates Amazon GameLift FleetIQ-specific properties for a game
         server
         group.
 
@@ -1549,15 +1549,15 @@
     async def update_game_session(
         self,
         *,
         GameSessionId: str,
         MaximumPlayerSessionCount: int = ...,
         Name: str = ...,
         PlayerSessionCreationPolicy: PlayerSessionCreationPolicyType = ...,
-        ProtectionPolicy: ProtectionPolicyType = ...
+        ProtectionPolicy: ProtectionPolicyType = ...,
     ) -> UpdateGameSessionOutputTypeDef:
         """
         Updates the mutable properties of a game session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_game_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#update_game_session)
         """
@@ -1568,15 +1568,15 @@
         Name: str,
         TimeoutInSeconds: int = ...,
         PlayerLatencyPolicies: Sequence[PlayerLatencyPolicyTypeDef] = ...,
         Destinations: Sequence[GameSessionQueueDestinationTypeDef] = ...,
         FilterConfiguration: FilterConfigurationTypeDef = ...,
         PriorityConfiguration: PriorityConfigurationTypeDef = ...,
         CustomEventData: str = ...,
-        NotificationTarget: str = ...
+        NotificationTarget: str = ...,
     ) -> UpdateGameSessionQueueOutputTypeDef:
         """
         Updates the configuration of a game session queue, which determines how the
         queue processes new game session
         requests.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_game_session_queue)
@@ -1595,15 +1595,15 @@
         RuleSetName: str = ...,
         NotificationTarget: str = ...,
         AdditionalPlayerCount: int = ...,
         CustomEventData: str = ...,
         GameProperties: Sequence[GamePropertyTypeDef] = ...,
         GameSessionData: str = ...,
         BackfillMode: BackfillModeType = ...,
-        FlexMatchMode: FlexMatchModeType = ...
+        FlexMatchMode: FlexMatchModeType = ...,
     ) -> UpdateMatchmakingConfigurationOutputTypeDef:
         """
         Updates settings for a FlexMatch matchmaking configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_matchmaking_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#update_matchmaking_configuration)
         """
@@ -1623,15 +1623,15 @@
     async def update_script(
         self,
         *,
         ScriptId: str,
         Name: str = ...,
         Version: str = ...,
         StorageLocation: S3LocationTypeDef = ...,
-        ZipFile: BlobTypeDef = ...
+        ZipFile: BlobTypeDef = ...,
     ) -> UpdateScriptOutputTypeDef:
         """
         Updates Realtime script metadata and content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_script)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#update_script)
         """
```

### Comparing `types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift/literals.py` & `types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift/literals.py`

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
     "AcceptanceTypeType",
     "BackfillModeType",
     "BalancingStrategyType",
     "BuildStatusType",
     "CertificateTypeType",
     "ComparisonOperatorTypeType",
@@ -90,15 +89,14 @@
     "GameLiftServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AcceptanceTypeType = Literal["ACCEPT", "REJECT"]
 BackfillModeType = Literal["AUTOMATIC", "MANUAL"]
 BalancingStrategyType = Literal["ON_DEMAND_ONLY", "SPOT_ONLY", "SPOT_PREFERRED"]
 BuildStatusType = Literal["FAILED", "INITIALIZED", "READY"]
 CertificateTypeType = Literal["DISABLED", "GENERATED"]
 ComparisonOperatorTypeType = Literal[
     "GreaterThanOrEqualToThreshold",
```

### Comparing `types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift/literals.pyi` & `types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift/paginator.py` & `types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,14 @@
     "ListGameServerGroupsPaginator",
     "ListGameServersPaginator",
     "ListLocationsPaginator",
     "ListScriptsPaginator",
     "SearchGameSessionsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -176,15 +175,15 @@
 
     def paginate(
         self,
         *,
         FleetId: str,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeFleetEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeFleetEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/paginators/#describefleeteventspaginator)
         """
 
 
@@ -210,15 +209,15 @@
     """
 
     def paginate(
         self,
         *,
         GameServerGroupName: str,
         InstanceIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeGameServerInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeGameServerInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/paginators/#describegameserverinstancespaginator)
         """
 
 
@@ -232,15 +231,15 @@
         self,
         *,
         FleetId: str = ...,
         GameSessionId: str = ...,
         AliasId: str = ...,
         Location: str = ...,
         StatusFilter: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeGameSessionDetailsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeGameSessionDetails.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/paginators/#describegamesessiondetailspaginator)
         """
 
 
@@ -269,15 +268,15 @@
         self,
         *,
         FleetId: str = ...,
         GameSessionId: str = ...,
         AliasId: str = ...,
         Location: str = ...,
         StatusFilter: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeGameSessionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeGameSessions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/paginators/#describegamesessionspaginator)
         """
 
 
@@ -289,15 +288,15 @@
 
     def paginate(
         self,
         *,
         FleetId: str,
         InstanceId: str = ...,
         Location: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/paginators/#describeinstancespaginator)
         """
 
 
@@ -308,15 +307,15 @@
     """
 
     def paginate(
         self,
         *,
         Names: Sequence[str] = ...,
         RuleSetName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeMatchmakingConfigurationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeMatchmakingConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/paginators/#describematchmakingconfigurationspaginator)
         """
 
 
@@ -344,15 +343,15 @@
     def paginate(
         self,
         *,
         GameSessionId: str = ...,
         PlayerId: str = ...,
         PlayerSessionId: str = ...,
         PlayerSessionStatusFilter: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribePlayerSessionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribePlayerSessions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/paginators/#describeplayersessionspaginator)
         """
 
 
@@ -364,15 +363,15 @@
 
     def paginate(
         self,
         *,
         FleetId: str,
         StatusFilter: ScalingStatusTypeType = ...,
         Location: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeScalingPoliciesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeScalingPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/paginators/#describescalingpoliciespaginator)
         """
 
 
@@ -383,15 +382,15 @@
     """
 
     def paginate(
         self,
         *,
         RoutingStrategyType: RoutingStrategyTypeType = ...,
         Name: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAliasesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListAliases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/paginators/#listaliasespaginator)
         """
 
 
@@ -432,15 +431,15 @@
     """
 
     def paginate(
         self,
         *,
         BuildId: str = ...,
         ScriptId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFleetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListFleets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/paginators/#listfleetspaginator)
         """
 
 
@@ -466,15 +465,15 @@
     """
 
     def paginate(
         self,
         *,
         GameServerGroupName: str,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListGameServersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListGameServers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/paginators/#listgameserverspaginator)
         """
 
 
@@ -484,15 +483,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/paginators/#listlocationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[LocationFilterType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListLocationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListLocations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/paginators/#listlocationspaginator)
         """
 
 
@@ -521,13 +520,13 @@
         self,
         *,
         FleetId: str = ...,
         AliasId: str = ...,
         Location: str = ...,
         FilterExpression: str = ...,
         SortExpression: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchGameSessionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.SearchGameSessions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/paginators/#searchgamesessionspaginator)
         """
```

### Comparing `types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift/paginator.pyi` & `types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -171,15 +171,15 @@
 
     def paginate(
         self,
         *,
         FleetId: str,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeFleetEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeFleetEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/paginators/#describefleeteventspaginator)
         """
 
 class DescribeFleetUtilizationPaginator(AioPaginator):
@@ -203,15 +203,15 @@
     """
 
     def paginate(
         self,
         *,
         GameServerGroupName: str,
         InstanceIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeGameServerInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeGameServerInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/paginators/#describegameserverinstancespaginator)
         """
 
 class DescribeGameSessionDetailsPaginator(AioPaginator):
@@ -224,15 +224,15 @@
         self,
         *,
         FleetId: str = ...,
         GameSessionId: str = ...,
         AliasId: str = ...,
         Location: str = ...,
         StatusFilter: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeGameSessionDetailsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeGameSessionDetails.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/paginators/#describegamesessiondetailspaginator)
         """
 
 class DescribeGameSessionQueuesPaginator(AioPaginator):
@@ -259,15 +259,15 @@
         self,
         *,
         FleetId: str = ...,
         GameSessionId: str = ...,
         AliasId: str = ...,
         Location: str = ...,
         StatusFilter: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeGameSessionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeGameSessions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/paginators/#describegamesessionspaginator)
         """
 
 class DescribeInstancesPaginator(AioPaginator):
@@ -278,15 +278,15 @@
 
     def paginate(
         self,
         *,
         FleetId: str,
         InstanceId: str = ...,
         Location: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/paginators/#describeinstancespaginator)
         """
 
 class DescribeMatchmakingConfigurationsPaginator(AioPaginator):
@@ -296,15 +296,15 @@
     """
 
     def paginate(
         self,
         *,
         Names: Sequence[str] = ...,
         RuleSetName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeMatchmakingConfigurationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeMatchmakingConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/paginators/#describematchmakingconfigurationspaginator)
         """
 
 class DescribeMatchmakingRuleSetsPaginator(AioPaginator):
@@ -330,15 +330,15 @@
     def paginate(
         self,
         *,
         GameSessionId: str = ...,
         PlayerId: str = ...,
         PlayerSessionId: str = ...,
         PlayerSessionStatusFilter: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribePlayerSessionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribePlayerSessions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/paginators/#describeplayersessionspaginator)
         """
 
 class DescribeScalingPoliciesPaginator(AioPaginator):
@@ -349,15 +349,15 @@
 
     def paginate(
         self,
         *,
         FleetId: str,
         StatusFilter: ScalingStatusTypeType = ...,
         Location: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeScalingPoliciesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeScalingPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/paginators/#describescalingpoliciespaginator)
         """
 
 class ListAliasesPaginator(AioPaginator):
@@ -367,15 +367,15 @@
     """
 
     def paginate(
         self,
         *,
         RoutingStrategyType: RoutingStrategyTypeType = ...,
         Name: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAliasesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListAliases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/paginators/#listaliasespaginator)
         """
 
 class ListBuildsPaginator(AioPaginator):
@@ -413,15 +413,15 @@
     """
 
     def paginate(
         self,
         *,
         BuildId: str = ...,
         ScriptId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFleetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListFleets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/paginators/#listfleetspaginator)
         """
 
 class ListGameServerGroupsPaginator(AioPaginator):
@@ -445,15 +445,15 @@
     """
 
     def paginate(
         self,
         *,
         GameServerGroupName: str,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListGameServersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListGameServers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/paginators/#listgameserverspaginator)
         """
 
 class ListLocationsPaginator(AioPaginator):
@@ -462,15 +462,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/paginators/#listlocationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[LocationFilterType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListLocationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListLocations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/paginators/#listlocationspaginator)
         """
 
 class ListScriptsPaginator(AioPaginator):
@@ -497,13 +497,13 @@
         self,
         *,
         FleetId: str = ...,
         AliasId: str = ...,
         Location: str = ...,
         FilterExpression: str = ...,
         SortExpression: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchGameSessionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.SearchGameSessions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/paginators/#searchgamesessionspaginator)
         """
```

### Comparing `types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift/type_defs.py` & `types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceptMatchInputRequestTypeDef",
     "RoutingStrategyTypeDef",
     "AnywhereConfigurationTypeDef",
     "AttributeValueTypeDef",
     "AwsCredentialsTypeDef",
     "BlobTypeDef",
```

### Comparing `types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift/type_defs.pyi` & `types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift.egg-info/PKG-INFO` & `types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-gamelift
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.GameLift 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.GameLift 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/
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
 
 <a id="types-aiobotocore-gamelift"></a>
 
 # types-aiobotocore-gamelift
 
 [![PyPI - types-aiobotocore-gamelift](https://img.shields.io/pypi/v/types-aiobotocore-gamelift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-gamelift)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-gamelift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-gamelift)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-gamelift)](https://pepy.tech/project/types-aiobotocore-gamelift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GameLift 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
+[aiobotocore.GameLift 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
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
 [types-aiobotocore-gamelift docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-gamelift-2.9.0/types_aiobotocore_gamelift.egg-info/SOURCES.txt` & `types-aiobotocore-gamelift-2.9.1/types_aiobotocore_gamelift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

