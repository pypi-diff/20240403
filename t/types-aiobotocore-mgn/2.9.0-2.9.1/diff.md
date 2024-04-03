# Comparing `tmp/types-aiobotocore-mgn-2.9.0.tar.gz` & `tmp/types-aiobotocore-mgn-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mgn-2.9.0.tar", last modified: Wed Dec 13 19:59:57 2023, max compression
+gzip compressed data, was "types-aiobotocore-mgn-2.9.1.tar", last modified: Thu Jan 18 01:21:18 2024, max compression
```

## Comparing `types-aiobotocore-mgn-2.9.0.tar` & `types-aiobotocore-mgn-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:57.213426 types-aiobotocore-mgn-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:50:28.000000 types-aiobotocore-mgn-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15137 2023-12-13 19:59:57.213426 types-aiobotocore-mgn-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13590 2023-12-13 19:50:28.000000 types-aiobotocore-mgn-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:57.213426 types-aiobotocore-mgn-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-12-13 19:50:28.000000 types-aiobotocore-mgn-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:57.213426 types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn/
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2023-12-13 19:50:28.000000 types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2023-12-13 19:50:28.000000 types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-13 19:50:28.000000 types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    57950 2023-12-13 19:50:28.000000 types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    57946 2023-12-13 19:50:28.000000 types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16230 2023-12-13 19:50:31.000000 types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    16228 2023-12-13 19:50:29.000000 types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    20006 2023-12-13 19:50:29.000000 types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    19988 2023-12-13 19:50:28.000000 types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:50:28.000000 types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    73341 2023-12-13 19:50:32.000000 types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    73340 2023-12-13 19:50:31.000000 types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:50:28.000000 types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:57.213426 types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15137 2023-12-13 19:59:57.000000 types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      737 2023-12-13 19:59:57.000000 types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:57.000000 types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:57.000000 types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:57.000000 types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 19:59:57.000000 types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:18.777169 types-aiobotocore-mgn-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:12:12.000000 types-aiobotocore-mgn-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15157 2024-01-18 01:21:18.777169 types-aiobotocore-mgn-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13590 2024-01-18 01:12:12.000000 types-aiobotocore-mgn-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:18.777169 types-aiobotocore-mgn-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-01-18 01:12:12.000000 types-aiobotocore-mgn-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:18.777169 types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn/
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-01-18 01:12:12.000000 types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-01-18 01:12:12.000000 types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-18 01:12:12.000000 types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57974 2024-01-18 01:12:12.000000 types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57971 2024-01-18 01:12:12.000000 types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16228 2024-01-18 01:12:13.000000 types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16228 2024-01-18 01:12:12.000000 types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    20016 2024-01-18 01:12:12.000000 types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19999 2024-01-18 01:12:12.000000 types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:12:12.000000 types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    73340 2024-01-18 01:12:14.000000 types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73340 2024-01-18 01:12:13.000000 types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:12:12.000000 types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:18.777169 types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15157 2024-01-18 01:21:18.000000 types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-01-18 01:21:18.000000 types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:18.000000 types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:18.000000 types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:18.000000 types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:21:18.000000 types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mgn-2.9.0/LICENSE` & `types-aiobotocore-mgn-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-mgn-2.9.0/PKG-INFO` & `types-aiobotocore-mgn-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mgn
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.mgn 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.mgn 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/
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
 
 <a id="types-aiobotocore-mgn"></a>
 
 # types-aiobotocore-mgn
 
 [![PyPI - types-aiobotocore-mgn](https://img.shields.io/pypi/v/types-aiobotocore-mgn.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mgn)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mgn.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mgn)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mgn)](https://pepy.tech/project/types-aiobotocore-mgn)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.mgn 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
+[aiobotocore.mgn 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
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
 [types-aiobotocore-mgn docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mgn-2.9.0/README.md` & `types-aiobotocore-mgn-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mgn.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mgn)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mgn)](https://pepy.tech/project/types-aiobotocore-mgn)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.mgn 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
+[aiobotocore.mgn 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
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
 [types-aiobotocore-mgn docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mgn-2.9.0/setup.py` & `types-aiobotocore-mgn-2.9.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mgn",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_mgn"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.mgn 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.mgn 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore mgn type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_mgn": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn/__init__.py` & `types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,14 @@
     ListSourceServerActionsPaginator,
     ListTemplateActionsPaginator,
     ListWavesPaginator,
 )
 
 Client = mgnClient
 
-
 __all__ = (
     "Client",
     "DescribeJobLogItemsPaginator",
     "DescribeJobsPaginator",
     "DescribeLaunchConfigurationTemplatesPaginator",
     "DescribeReplicationConfigurationTemplatesPaginator",
     "DescribeSourceServersPaginator",
```

### Comparing `types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn/__init__.pyi` & `types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn/__main__.py` & `types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.mgn 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.mgn 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn\nOther"
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

### Comparing `types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn/client.py` & `types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,15 +105,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("mgnClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -197,15 +196,15 @@
         """
 
     async def change_server_life_cycle_state(
         self,
         *,
         lifeCycle: ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,
         sourceServerID: str,
-        accountID: str = ...
+        accountID: str = ...,
     ) -> SourceServerResponseTypeDef:
         """
         Allows the user to set the SourceServer.LifeCycle.state property for specific
         Source Server IDs to one of the following: READY_FOR_TEST or
         READY_FOR_CUTOVER.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.change_server_life_cycle_state)
@@ -222,30 +221,30 @@
 
     async def create_application(
         self,
         *,
         name: str,
         accountID: str = ...,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> ApplicationResponseTypeDef:
         """
         Create application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#create_application)
         """
 
     async def create_connector(
         self,
         *,
         name: str,
         ssmInstanceID: str,
         ssmCommandConfig: ConnectorSsmCommandConfigTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> ConnectorResponseTypeDef:
         """
         Create Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_connector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#create_connector)
         """
@@ -262,15 +261,15 @@
         launchDisposition: LaunchDispositionType = ...,
         licensing: LicensingTypeDef = ...,
         mapAutoTaggingMpeID: str = ...,
         postLaunchActions: PostLaunchActionsTypeDef = ...,
         smallVolumeConf: LaunchTemplateDiskConfTypeDef = ...,
         smallVolumeMaxSize: int = ...,
         tags: Mapping[str, str] = ...,
-        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
+        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...,
     ) -> LaunchConfigurationTemplateResponseTypeDef:
         """
         Creates a new Launch Configuration Template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_launch_configuration_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#create_launch_configuration_template)
         """
@@ -287,30 +286,30 @@
         replicationServerInstanceType: str,
         replicationServersSecurityGroupsIDs: Sequence[str],
         stagingAreaSubnetId: str,
         stagingAreaTags: Mapping[str, str],
         useDedicatedReplicationServer: bool,
         ebsEncryptionKeyArn: str = ...,
         tags: Mapping[str, str] = ...,
-        useFipsEndpoint: bool = ...
+        useFipsEndpoint: bool = ...,
     ) -> ReplicationConfigurationTemplateResponseTypeDef:
         """
         Creates a new ReplicationConfigurationTemplate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_replication_configuration_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#create_replication_configuration_template)
         """
 
     async def create_wave(
         self,
         *,
         name: str,
         accountID: str = ...,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> WaveResponseTypeDef:
         """
         Create wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_wave)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#create_wave)
         """
@@ -400,29 +399,29 @@
 
     async def describe_jobs(
         self,
         *,
         accountID: str = ...,
         filters: DescribeJobsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeJobsResponseTypeDef:
         """
         Returns a list of Jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#describe_jobs)
         """
 
     async def describe_launch_configuration_templates(
         self,
         *,
         launchConfigurationTemplateIDs: Sequence[str] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeLaunchConfigurationTemplatesResponseTypeDef:
         """
         Lists all Launch Configuration Templates, filtered by Launch Configuration
         Template IDs See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/mgn-2020-02-26/DescribeLaunchConfigurationTemplates).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_launch_configuration_templates)
@@ -430,30 +429,30 @@
         """
 
     async def describe_replication_configuration_templates(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
-        replicationConfigurationTemplateIDs: Sequence[str] = ...
+        replicationConfigurationTemplateIDs: Sequence[str] = ...,
     ) -> DescribeReplicationConfigurationTemplatesResponseTypeDef:
         """
         Lists all ReplicationConfigurationTemplates, filtered by Source Server IDs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_replication_configuration_templates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#describe_replication_configuration_templates)
         """
 
     async def describe_source_servers(
         self,
         *,
         accountID: str = ...,
         filters: DescribeSourceServersRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeSourceServersResponseTypeDef:
         """
         Retrieves all SourceServers or multiple SourceServers by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_source_servers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#describe_source_servers)
         """
@@ -552,29 +551,29 @@
 
     async def list_applications(
         self,
         *,
         accountID: str = ...,
         filters: ListApplicationsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListApplicationsResponseTypeDef:
         """
         Retrieves all applications or multiple applications by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_applications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#list_applications)
         """
 
     async def list_connectors(
         self,
         *,
         filters: ListConnectorsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListConnectorsResponseTypeDef:
         """
         List Connectors.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_connectors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#list_connectors)
         """
@@ -590,15 +589,15 @@
         """
 
     async def list_exports(
         self,
         *,
         filters: ListExportsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListExportsResponseTypeDef:
         """
         List exports.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_exports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#list_exports)
         """
@@ -614,15 +613,15 @@
         """
 
     async def list_imports(
         self,
         *,
         filters: ListImportsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListImportsResponseTypeDef:
         """
         List imports.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_imports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#list_imports)
         """
@@ -640,15 +639,15 @@
     async def list_source_server_actions(
         self,
         *,
         sourceServerID: str,
         accountID: str = ...,
         filters: SourceServerActionsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListSourceServerActionsResponseTypeDef:
         """
         List source server post migration custom actions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_source_server_actions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#list_source_server_actions)
         """
@@ -665,30 +664,30 @@
 
     async def list_template_actions(
         self,
         *,
         launchConfigurationTemplateID: str,
         filters: TemplateActionsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListTemplateActionsResponseTypeDef:
         """
         List template post migration custom actions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_template_actions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#list_template_actions)
         """
 
     async def list_waves(
         self,
         *,
         accountID: str = ...,
         filters: ListWavesRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListWavesResponseTypeDef:
         """
         Retrieves all waves or multiple waves by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_waves)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#list_waves)
         """
@@ -727,15 +726,15 @@
         active: bool = ...,
         category: ActionCategoryType = ...,
         description: str = ...,
         documentVersion: str = ...,
         externalParameters: Mapping[str, SsmExternalParameterTypeDef] = ...,
         mustSucceedForCutover: bool = ...,
         parameters: Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]] = ...,
-        timeoutSeconds: int = ...
+        timeoutSeconds: int = ...,
     ) -> SourceServerActionDocumentResponseTypeDef:
         """
         Put source server post migration custom action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.put_source_server_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#put_source_server_action)
         """
@@ -752,15 +751,15 @@
         category: ActionCategoryType = ...,
         description: str = ...,
         documentVersion: str = ...,
         externalParameters: Mapping[str, SsmExternalParameterTypeDef] = ...,
         mustSucceedForCutover: bool = ...,
         operatingSystem: str = ...,
         parameters: Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]] = ...,
-        timeoutSeconds: int = ...
+        timeoutSeconds: int = ...,
     ) -> TemplateActionDocumentResponseTypeDef:
         """
         Put template post migration custom action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.put_template_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#put_template_action)
         """
@@ -931,15 +930,15 @@
         """
 
     async def update_connector(
         self,
         *,
         connectorID: str,
         name: str = ...,
-        ssmCommandConfig: ConnectorSsmCommandConfigTypeDef = ...
+        ssmCommandConfig: ConnectorSsmCommandConfigTypeDef = ...,
     ) -> ConnectorResponseTypeDef:
         """
         Update Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_connector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#update_connector)
         """
@@ -954,15 +953,15 @@
         copyTags: bool = ...,
         enableMapAutoTagging: bool = ...,
         launchDisposition: LaunchDispositionType = ...,
         licensing: LicensingTypeDef = ...,
         mapAutoTaggingMpeID: str = ...,
         name: str = ...,
         postLaunchActions: PostLaunchActionsTypeDef = ...,
-        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
+        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...,
     ) -> LaunchConfigurationTypeDef:
         """
         Updates multiple LaunchConfigurations by Source Server ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_launch_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#update_launch_configuration)
         """
@@ -979,15 +978,15 @@
         largeVolumeConf: LaunchTemplateDiskConfTypeDef = ...,
         launchDisposition: LaunchDispositionType = ...,
         licensing: LicensingTypeDef = ...,
         mapAutoTaggingMpeID: str = ...,
         postLaunchActions: PostLaunchActionsTypeDef = ...,
         smallVolumeConf: LaunchTemplateDiskConfTypeDef = ...,
         smallVolumeMaxSize: int = ...,
-        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
+        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...,
     ) -> LaunchConfigurationTemplateResponseTypeDef:
         """
         Updates an existing Launch Configuration Template by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_launch_configuration_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#update_launch_configuration_template)
         """
@@ -1007,15 +1006,15 @@
         name: str = ...,
         replicatedDisks: Sequence[ReplicationConfigurationReplicatedDiskTypeDef] = ...,
         replicationServerInstanceType: str = ...,
         replicationServersSecurityGroupsIDs: Sequence[str] = ...,
         stagingAreaSubnetId: str = ...,
         stagingAreaTags: Mapping[str, str] = ...,
         useDedicatedReplicationServer: bool = ...,
-        useFipsEndpoint: bool = ...
+        useFipsEndpoint: bool = ...,
     ) -> ReplicationConfigurationTypeDef:
         """
         Allows you to update multiple ReplicationConfigurations by Source Server ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_replication_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#update_replication_configuration)
         """
@@ -1033,29 +1032,29 @@
         ebsEncryption: ReplicationConfigurationEbsEncryptionType = ...,
         ebsEncryptionKeyArn: str = ...,
         replicationServerInstanceType: str = ...,
         replicationServersSecurityGroupsIDs: Sequence[str] = ...,
         stagingAreaSubnetId: str = ...,
         stagingAreaTags: Mapping[str, str] = ...,
         useDedicatedReplicationServer: bool = ...,
-        useFipsEndpoint: bool = ...
+        useFipsEndpoint: bool = ...,
     ) -> ReplicationConfigurationTemplateResponseTypeDef:
         """
         Updates multiple ReplicationConfigurationTemplates by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_replication_configuration_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#update_replication_configuration_template)
         """
 
     async def update_source_server(
         self,
         *,
         sourceServerID: str,
         accountID: str = ...,
-        connectorAction: SourceServerConnectorActionTypeDef = ...
+        connectorAction: SourceServerConnectorActionTypeDef = ...,
     ) -> SourceServerResponseTypeDef:
         """
         Update Source Server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_source_server)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#update_source_server)
         """
```

### Comparing `types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn/client.pyi` & `types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -193,15 +193,15 @@
         """
 
     async def change_server_life_cycle_state(
         self,
         *,
         lifeCycle: ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,
         sourceServerID: str,
-        accountID: str = ...
+        accountID: str = ...,
     ) -> SourceServerResponseTypeDef:
         """
         Allows the user to set the SourceServer.LifeCycle.state property for specific
         Source Server IDs to one of the following: READY_FOR_TEST or
         READY_FOR_CUTOVER.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.change_server_life_cycle_state)
@@ -218,30 +218,30 @@
 
     async def create_application(
         self,
         *,
         name: str,
         accountID: str = ...,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> ApplicationResponseTypeDef:
         """
         Create application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#create_application)
         """
 
     async def create_connector(
         self,
         *,
         name: str,
         ssmInstanceID: str,
         ssmCommandConfig: ConnectorSsmCommandConfigTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> ConnectorResponseTypeDef:
         """
         Create Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_connector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#create_connector)
         """
@@ -258,15 +258,15 @@
         launchDisposition: LaunchDispositionType = ...,
         licensing: LicensingTypeDef = ...,
         mapAutoTaggingMpeID: str = ...,
         postLaunchActions: PostLaunchActionsTypeDef = ...,
         smallVolumeConf: LaunchTemplateDiskConfTypeDef = ...,
         smallVolumeMaxSize: int = ...,
         tags: Mapping[str, str] = ...,
-        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
+        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...,
     ) -> LaunchConfigurationTemplateResponseTypeDef:
         """
         Creates a new Launch Configuration Template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_launch_configuration_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#create_launch_configuration_template)
         """
@@ -283,30 +283,30 @@
         replicationServerInstanceType: str,
         replicationServersSecurityGroupsIDs: Sequence[str],
         stagingAreaSubnetId: str,
         stagingAreaTags: Mapping[str, str],
         useDedicatedReplicationServer: bool,
         ebsEncryptionKeyArn: str = ...,
         tags: Mapping[str, str] = ...,
-        useFipsEndpoint: bool = ...
+        useFipsEndpoint: bool = ...,
     ) -> ReplicationConfigurationTemplateResponseTypeDef:
         """
         Creates a new ReplicationConfigurationTemplate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_replication_configuration_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#create_replication_configuration_template)
         """
 
     async def create_wave(
         self,
         *,
         name: str,
         accountID: str = ...,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> WaveResponseTypeDef:
         """
         Create wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_wave)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#create_wave)
         """
@@ -396,29 +396,29 @@
 
     async def describe_jobs(
         self,
         *,
         accountID: str = ...,
         filters: DescribeJobsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeJobsResponseTypeDef:
         """
         Returns a list of Jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#describe_jobs)
         """
 
     async def describe_launch_configuration_templates(
         self,
         *,
         launchConfigurationTemplateIDs: Sequence[str] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeLaunchConfigurationTemplatesResponseTypeDef:
         """
         Lists all Launch Configuration Templates, filtered by Launch Configuration
         Template IDs See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/mgn-2020-02-26/DescribeLaunchConfigurationTemplates).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_launch_configuration_templates)
@@ -426,30 +426,30 @@
         """
 
     async def describe_replication_configuration_templates(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
-        replicationConfigurationTemplateIDs: Sequence[str] = ...
+        replicationConfigurationTemplateIDs: Sequence[str] = ...,
     ) -> DescribeReplicationConfigurationTemplatesResponseTypeDef:
         """
         Lists all ReplicationConfigurationTemplates, filtered by Source Server IDs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_replication_configuration_templates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#describe_replication_configuration_templates)
         """
 
     async def describe_source_servers(
         self,
         *,
         accountID: str = ...,
         filters: DescribeSourceServersRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeSourceServersResponseTypeDef:
         """
         Retrieves all SourceServers or multiple SourceServers by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_source_servers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#describe_source_servers)
         """
@@ -548,29 +548,29 @@
 
     async def list_applications(
         self,
         *,
         accountID: str = ...,
         filters: ListApplicationsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListApplicationsResponseTypeDef:
         """
         Retrieves all applications or multiple applications by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_applications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#list_applications)
         """
 
     async def list_connectors(
         self,
         *,
         filters: ListConnectorsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListConnectorsResponseTypeDef:
         """
         List Connectors.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_connectors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#list_connectors)
         """
@@ -586,15 +586,15 @@
         """
 
     async def list_exports(
         self,
         *,
         filters: ListExportsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListExportsResponseTypeDef:
         """
         List exports.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_exports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#list_exports)
         """
@@ -610,15 +610,15 @@
         """
 
     async def list_imports(
         self,
         *,
         filters: ListImportsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListImportsResponseTypeDef:
         """
         List imports.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_imports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#list_imports)
         """
@@ -636,15 +636,15 @@
     async def list_source_server_actions(
         self,
         *,
         sourceServerID: str,
         accountID: str = ...,
         filters: SourceServerActionsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListSourceServerActionsResponseTypeDef:
         """
         List source server post migration custom actions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_source_server_actions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#list_source_server_actions)
         """
@@ -661,30 +661,30 @@
 
     async def list_template_actions(
         self,
         *,
         launchConfigurationTemplateID: str,
         filters: TemplateActionsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListTemplateActionsResponseTypeDef:
         """
         List template post migration custom actions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_template_actions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#list_template_actions)
         """
 
     async def list_waves(
         self,
         *,
         accountID: str = ...,
         filters: ListWavesRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListWavesResponseTypeDef:
         """
         Retrieves all waves or multiple waves by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_waves)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#list_waves)
         """
@@ -723,15 +723,15 @@
         active: bool = ...,
         category: ActionCategoryType = ...,
         description: str = ...,
         documentVersion: str = ...,
         externalParameters: Mapping[str, SsmExternalParameterTypeDef] = ...,
         mustSucceedForCutover: bool = ...,
         parameters: Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]] = ...,
-        timeoutSeconds: int = ...
+        timeoutSeconds: int = ...,
     ) -> SourceServerActionDocumentResponseTypeDef:
         """
         Put source server post migration custom action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.put_source_server_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#put_source_server_action)
         """
@@ -748,15 +748,15 @@
         category: ActionCategoryType = ...,
         description: str = ...,
         documentVersion: str = ...,
         externalParameters: Mapping[str, SsmExternalParameterTypeDef] = ...,
         mustSucceedForCutover: bool = ...,
         operatingSystem: str = ...,
         parameters: Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]] = ...,
-        timeoutSeconds: int = ...
+        timeoutSeconds: int = ...,
     ) -> TemplateActionDocumentResponseTypeDef:
         """
         Put template post migration custom action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.put_template_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#put_template_action)
         """
@@ -927,15 +927,15 @@
         """
 
     async def update_connector(
         self,
         *,
         connectorID: str,
         name: str = ...,
-        ssmCommandConfig: ConnectorSsmCommandConfigTypeDef = ...
+        ssmCommandConfig: ConnectorSsmCommandConfigTypeDef = ...,
     ) -> ConnectorResponseTypeDef:
         """
         Update Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_connector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#update_connector)
         """
@@ -950,15 +950,15 @@
         copyTags: bool = ...,
         enableMapAutoTagging: bool = ...,
         launchDisposition: LaunchDispositionType = ...,
         licensing: LicensingTypeDef = ...,
         mapAutoTaggingMpeID: str = ...,
         name: str = ...,
         postLaunchActions: PostLaunchActionsTypeDef = ...,
-        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
+        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...,
     ) -> LaunchConfigurationTypeDef:
         """
         Updates multiple LaunchConfigurations by Source Server ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_launch_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#update_launch_configuration)
         """
@@ -975,15 +975,15 @@
         largeVolumeConf: LaunchTemplateDiskConfTypeDef = ...,
         launchDisposition: LaunchDispositionType = ...,
         licensing: LicensingTypeDef = ...,
         mapAutoTaggingMpeID: str = ...,
         postLaunchActions: PostLaunchActionsTypeDef = ...,
         smallVolumeConf: LaunchTemplateDiskConfTypeDef = ...,
         smallVolumeMaxSize: int = ...,
-        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
+        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...,
     ) -> LaunchConfigurationTemplateResponseTypeDef:
         """
         Updates an existing Launch Configuration Template by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_launch_configuration_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#update_launch_configuration_template)
         """
@@ -1003,15 +1003,15 @@
         name: str = ...,
         replicatedDisks: Sequence[ReplicationConfigurationReplicatedDiskTypeDef] = ...,
         replicationServerInstanceType: str = ...,
         replicationServersSecurityGroupsIDs: Sequence[str] = ...,
         stagingAreaSubnetId: str = ...,
         stagingAreaTags: Mapping[str, str] = ...,
         useDedicatedReplicationServer: bool = ...,
-        useFipsEndpoint: bool = ...
+        useFipsEndpoint: bool = ...,
     ) -> ReplicationConfigurationTypeDef:
         """
         Allows you to update multiple ReplicationConfigurations by Source Server ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_replication_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#update_replication_configuration)
         """
@@ -1029,29 +1029,29 @@
         ebsEncryption: ReplicationConfigurationEbsEncryptionType = ...,
         ebsEncryptionKeyArn: str = ...,
         replicationServerInstanceType: str = ...,
         replicationServersSecurityGroupsIDs: Sequence[str] = ...,
         stagingAreaSubnetId: str = ...,
         stagingAreaTags: Mapping[str, str] = ...,
         useDedicatedReplicationServer: bool = ...,
-        useFipsEndpoint: bool = ...
+        useFipsEndpoint: bool = ...,
     ) -> ReplicationConfigurationTemplateResponseTypeDef:
         """
         Updates multiple ReplicationConfigurationTemplates by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_replication_configuration_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#update_replication_configuration_template)
         """
 
     async def update_source_server(
         self,
         *,
         sourceServerID: str,
         accountID: str = ...,
-        connectorAction: SourceServerConnectorActionTypeDef = ...
+        connectorAction: SourceServerConnectorActionTypeDef = ...,
     ) -> SourceServerResponseTypeDef:
         """
         Update Source Server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_source_server)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#update_source_server)
         """
```

### Comparing `types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn/literals.py` & `types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn/literals.py`

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
     "ActionCategoryType",
     "ApplicationHealthStatusType",
     "ApplicationProgressStatusType",
     "BootModeType",
     "ChangeServerLifeCycleStateSourceServerLifecycleStateType",
     "DataReplicationErrorStringType",
@@ -73,15 +72,14 @@
     "mgnServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ActionCategoryType = Literal[
     "BACKUP",
     "CONFIGURATION",
     "DISASTER_RECOVERY",
     "LICENSE_AND_SUBSCRIPTION",
     "NETWORKING",
     "OBSERVABILITY",
```

### Comparing `types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn/literals.pyi` & `types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn/paginator.py` & `types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,14 @@
     "ListImportsPaginator",
     "ListManagedAccountsPaginator",
     "ListSourceServerActionsPaginator",
     "ListTemplateActionsPaginator",
     "ListWavesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -137,15 +136,15 @@
     """
 
     def paginate(
         self,
         *,
         accountID: str = ...,
         filters: DescribeJobsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeJobsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#describejobspaginator)
         """
 
 
@@ -155,15 +154,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#describelaunchconfigurationtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         launchConfigurationTemplateIDs: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeLaunchConfigurationTemplatesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeLaunchConfigurationTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#describelaunchconfigurationtemplatespaginator)
         """
 
 
@@ -173,15 +172,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#describereplicationconfigurationtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         replicationConfigurationTemplateIDs: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeReplicationConfigurationTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeReplicationConfigurationTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#describereplicationconfigurationtemplatespaginator)
         """
 
 
@@ -192,15 +191,15 @@
     """
 
     def paginate(
         self,
         *,
         accountID: str = ...,
         filters: DescribeSourceServersRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeSourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeSourceServers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#describesourceserverspaginator)
         """
 
 
@@ -226,15 +225,15 @@
     """
 
     def paginate(
         self,
         *,
         accountID: str = ...,
         filters: ListApplicationsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listapplicationspaginator)
         """
 
 
@@ -244,15 +243,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listconnectorspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: ListConnectorsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListConnectorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListConnectors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listconnectorspaginator)
         """
 
 
@@ -277,15 +276,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listexportspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: ListExportsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListExportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListExports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listexportspaginator)
         """
 
 
@@ -310,15 +309,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listimportspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: ListImportsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListImportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListImports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listimportspaginator)
         """
 
 
@@ -345,15 +344,15 @@
 
     def paginate(
         self,
         *,
         sourceServerID: str,
         accountID: str = ...,
         filters: SourceServerActionsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSourceServerActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListSourceServerActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listsourceserveractionspaginator)
         """
 
 
@@ -364,15 +363,15 @@
     """
 
     def paginate(
         self,
         *,
         launchConfigurationTemplateID: str,
         filters: TemplateActionsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTemplateActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListTemplateActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listtemplateactionspaginator)
         """
 
 
@@ -383,13 +382,13 @@
     """
 
     def paginate(
         self,
         *,
         accountID: str = ...,
         filters: ListWavesRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListWavesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListWaves.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listwavespaginator)
         """
```

### Comparing `types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn/paginator.pyi` & `types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
     """
 
     def paginate(
         self,
         *,
         accountID: str = ...,
         filters: DescribeJobsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeJobsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#describejobspaginator)
         """
 
 class DescribeLaunchConfigurationTemplatesPaginator(AioPaginator):
@@ -150,15 +150,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#describelaunchconfigurationtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         launchConfigurationTemplateIDs: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeLaunchConfigurationTemplatesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeLaunchConfigurationTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#describelaunchconfigurationtemplatespaginator)
         """
 
 class DescribeReplicationConfigurationTemplatesPaginator(AioPaginator):
@@ -167,15 +167,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#describereplicationconfigurationtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         replicationConfigurationTemplateIDs: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeReplicationConfigurationTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeReplicationConfigurationTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#describereplicationconfigurationtemplatespaginator)
         """
 
 class DescribeSourceServersPaginator(AioPaginator):
@@ -185,15 +185,15 @@
     """
 
     def paginate(
         self,
         *,
         accountID: str = ...,
         filters: DescribeSourceServersRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeSourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeSourceServers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#describesourceserverspaginator)
         """
 
 class DescribeVcenterClientsPaginator(AioPaginator):
@@ -217,15 +217,15 @@
     """
 
     def paginate(
         self,
         *,
         accountID: str = ...,
         filters: ListApplicationsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listapplicationspaginator)
         """
 
 class ListConnectorsPaginator(AioPaginator):
@@ -234,15 +234,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listconnectorspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: ListConnectorsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListConnectorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListConnectors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listconnectorspaginator)
         """
 
 class ListExportErrorsPaginator(AioPaginator):
@@ -265,15 +265,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listexportspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: ListExportsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListExportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListExports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listexportspaginator)
         """
 
 class ListImportErrorsPaginator(AioPaginator):
@@ -296,15 +296,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listimportspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: ListImportsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListImportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListImports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listimportspaginator)
         """
 
 class ListManagedAccountsPaginator(AioPaginator):
@@ -329,15 +329,15 @@
 
     def paginate(
         self,
         *,
         sourceServerID: str,
         accountID: str = ...,
         filters: SourceServerActionsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSourceServerActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListSourceServerActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listsourceserveractionspaginator)
         """
 
 class ListTemplateActionsPaginator(AioPaginator):
@@ -347,15 +347,15 @@
     """
 
     def paginate(
         self,
         *,
         launchConfigurationTemplateID: str,
         filters: TemplateActionsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTemplateActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListTemplateActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listtemplateactionspaginator)
         """
 
 class ListWavesPaginator(AioPaginator):
@@ -365,13 +365,13 @@
     """
 
     def paginate(
         self,
         *,
         accountID: str = ...,
         filters: ListWavesRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListWavesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListWaves.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listwavespaginator)
         """
```

### Comparing `types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn/type_defs.py` & `types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ApplicationAggregatedStatusTypeDef",
     "ResponseMetadataTypeDef",
     "ArchiveApplicationRequestRequestTypeDef",
     "ArchiveWaveRequestRequestTypeDef",
     "AssociateApplicationsRequestRequestTypeDef",
     "AssociateSourceServersRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn/type_defs.pyi` & `types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn.egg-info/PKG-INFO` & `types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mgn
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.mgn 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.mgn 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/
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
 
 <a id="types-aiobotocore-mgn"></a>
 
 # types-aiobotocore-mgn
 
 [![PyPI - types-aiobotocore-mgn](https://img.shields.io/pypi/v/types-aiobotocore-mgn.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mgn)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mgn.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mgn)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mgn)](https://pepy.tech/project/types-aiobotocore-mgn)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.mgn 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
+[aiobotocore.mgn 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
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
 [types-aiobotocore-mgn docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mgn-2.9.0/types_aiobotocore_mgn.egg-info/SOURCES.txt` & `types-aiobotocore-mgn-2.9.1/types_aiobotocore_mgn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

