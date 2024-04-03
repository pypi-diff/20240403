# Comparing `tmp/types-aiobotocore-datasync-2.9.0.tar.gz` & `tmp/types-aiobotocore-datasync-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-datasync-2.9.0.tar", last modified: Wed Dec 13 19:59:04 2023, max compression
+gzip compressed data, was "types-aiobotocore-datasync-2.9.1.tar", last modified: Thu Jan 18 01:20:29 2024, max compression
```

## Comparing `types-aiobotocore-datasync-2.9.0.tar` & `types-aiobotocore-datasync-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:04.197854 types-aiobotocore-datasync-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:43:48.000000 types-aiobotocore-datasync-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14078 2023-12-13 19:59:04.197854 types-aiobotocore-datasync-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12511 2023-12-13 19:43:48.000000 types-aiobotocore-datasync-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:04.197854 types-aiobotocore-datasync-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-12-13 19:43:48.000000 types-aiobotocore-datasync-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:04.193854 types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync/
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2023-12-13 19:43:48.000000 types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2023-12-13 19:43:48.000000 types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-12-13 19:43:48.000000 types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51025 2023-12-13 19:43:49.000000 types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    51021 2023-12-13 19:43:48.000000 types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13908 2023-12-13 19:43:50.000000 types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13906 2023-12-13 19:43:50.000000 types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10353 2023-12-13 19:43:49.000000 types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10343 2023-12-13 19:43:49.000000 types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:43:48.000000 types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    52519 2023-12-13 19:43:51.000000 types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    52518 2023-12-13 19:43:50.000000 types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:43:48.000000 types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:04.197854 types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14078 2023-12-13 19:59:04.000000 types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-12-13 19:59:04.000000 types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:04.000000 types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:04.000000 types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:04.000000 types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-13 19:59:04.000000 types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:29.765398 types-aiobotocore-datasync-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:05:44.000000 types-aiobotocore-datasync-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14098 2024-01-18 01:20:29.765398 types-aiobotocore-datasync-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12511 2024-01-18 01:05:44.000000 types-aiobotocore-datasync-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:29.765398 types-aiobotocore-datasync-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-18 01:05:44.000000 types-aiobotocore-datasync-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:29.765398 types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync/
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-01-18 01:05:44.000000 types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-01-18 01:05:44.000000 types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-01-18 01:05:44.000000 types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51052 2024-01-18 01:05:44.000000 types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51049 2024-01-18 01:05:44.000000 types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13906 2024-01-18 01:05:45.000000 types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13906 2024-01-18 01:05:45.000000 types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-01-18 01:05:44.000000 types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10346 2024-01-18 01:05:44.000000 types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:05:44.000000 types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    52518 2024-01-18 01:05:46.000000 types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52518 2024-01-18 01:05:45.000000 types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:05:44.000000 types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:29.765398 types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14098 2024-01-18 01:20:29.000000 types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-01-18 01:20:29.000000 types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:29.000000 types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:29.000000 types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:29.000000 types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-18 01:20:29.000000 types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-datasync-2.9.0/LICENSE` & `types-aiobotocore-datasync-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-datasync-2.9.0/PKG-INFO` & `types-aiobotocore-datasync-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-datasync
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.DataSync 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.DataSync 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/
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
 
 <a id="types-aiobotocore-datasync"></a>
 
 # types-aiobotocore-datasync
 
 [![PyPI - types-aiobotocore-datasync](https://img.shields.io/pypi/v/types-aiobotocore-datasync.svg?color=blue)](https://pypi.org/project/types-aiobotocore-datasync)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-datasync.svg?color=blue)](https://pypi.org/project/types-aiobotocore-datasync)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-datasync)](https://pepy.tech/project/types-aiobotocore-datasync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DataSync 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
+[aiobotocore.DataSync 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
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
 [types-aiobotocore-datasync docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-datasync-2.9.0/README.md` & `types-aiobotocore-datasync-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-datasync.svg?color=blue)](https://pypi.org/project/types-aiobotocore-datasync)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-datasync)](https://pepy.tech/project/types-aiobotocore-datasync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DataSync 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
+[aiobotocore.DataSync 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
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
 [types-aiobotocore-datasync docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-datasync-2.9.0/setup.py` & `types-aiobotocore-datasync-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-datasync",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_datasync"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.DataSync 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.DataSync 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore datasync type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_datasync": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync/__init__.py` & `types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     ListTagsForResourcePaginator,
     ListTaskExecutionsPaginator,
     ListTasksPaginator,
 )
 
 Client = DataSyncClient
 
-
 __all__ = (
     "Client",
     "DataSyncClient",
     "DescribeStorageSystemResourceMetricsPaginator",
     "ListAgentsPaginator",
     "ListDiscoveryJobsPaginator",
     "ListLocationsPaginator",
```

### Comparing `types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync/__init__.pyi` & `types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync/__main__.py` & `types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DataSync 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.DataSync 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync\nOther"
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

### Comparing `types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync/client.py` & `types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("DataSyncClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -149,15 +148,15 @@
         ServerConfiguration: DiscoveryServerConfigurationTypeDef,
         SystemType: Literal["NetAppONTAP"],
         AgentArns: Sequence[str],
         ClientToken: str,
         Credentials: CredentialsTypeDef,
         CloudWatchLogGroupArn: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
-        Name: str = ...
+        Name: str = ...,
     ) -> AddStorageSystemResponseTypeDef:
         """
         Creates an Amazon Web Services resource for an on-premises storage system that
         you want DataSync Discovery to collect information
         about.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.add_storage_system)
@@ -192,15 +191,15 @@
         self,
         *,
         ActivationKey: str,
         AgentName: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         VpcEndpointId: str = ...,
         SubnetArns: Sequence[str] = ...,
-        SecurityGroupArns: Sequence[str] = ...
+        SecurityGroupArns: Sequence[str] = ...,
     ) -> CreateAgentResponseTypeDef:
         """
         Activates an DataSync agent that you've deployed in your storage environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_agent)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#create_agent)
         """
@@ -211,15 +210,15 @@
         ContainerUrl: str,
         AuthenticationType: Literal["SAS"],
         AgentArns: Sequence[str],
         SasConfiguration: AzureBlobSasConfigurationTypeDef = ...,
         BlobType: Literal["BLOCK"] = ...,
         AccessTier: AzureAccessTierType = ...,
         Subdirectory: str = ...,
-        Tags: Sequence[TagListEntryTypeDef] = ...
+        Tags: Sequence[TagListEntryTypeDef] = ...,
     ) -> CreateLocationAzureBlobResponseTypeDef:
         """
         Creates an endpoint for a Microsoft Azure Blob Storage container that DataSync
         can use as a transfer source or
         destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_azure_blob)
@@ -231,15 +230,15 @@
         *,
         EfsFilesystemArn: str,
         Ec2Config: Ec2ConfigTypeDef,
         Subdirectory: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         AccessPointArn: str = ...,
         FileSystemAccessRoleArn: str = ...,
-        InTransitEncryption: EfsInTransitEncryptionType = ...
+        InTransitEncryption: EfsInTransitEncryptionType = ...,
     ) -> CreateLocationEfsResponseTypeDef:
         """
         Creates an endpoint for an Amazon EFS file system that DataSync can access for
         a
         transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_efs)
@@ -248,15 +247,15 @@
 
     async def create_location_fsx_lustre(
         self,
         *,
         FsxFilesystemArn: str,
         SecurityGroupArns: Sequence[str],
         Subdirectory: str = ...,
-        Tags: Sequence[TagListEntryTypeDef] = ...
+        Tags: Sequence[TagListEntryTypeDef] = ...,
     ) -> CreateLocationFsxLustreResponseTypeDef:
         """
         Creates an endpoint for an Amazon FSx for Lustre file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_fsx_lustre)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#create_location_fsx_lustre)
         """
@@ -264,15 +263,15 @@
     async def create_location_fsx_ontap(
         self,
         *,
         Protocol: FsxProtocolTypeDef,
         SecurityGroupArns: Sequence[str],
         StorageVirtualMachineArn: str,
         Subdirectory: str = ...,
-        Tags: Sequence[TagListEntryTypeDef] = ...
+        Tags: Sequence[TagListEntryTypeDef] = ...,
     ) -> CreateLocationFsxOntapResponseTypeDef:
         """
         Creates an endpoint for an Amazon FSx for NetApp ONTAP file system that
         DataSync can use for a data
         transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_fsx_ontap)
@@ -282,15 +281,15 @@
     async def create_location_fsx_open_zfs(
         self,
         *,
         FsxFilesystemArn: str,
         Protocol: FsxProtocolTypeDef,
         SecurityGroupArns: Sequence[str],
         Subdirectory: str = ...,
-        Tags: Sequence[TagListEntryTypeDef] = ...
+        Tags: Sequence[TagListEntryTypeDef] = ...,
     ) -> CreateLocationFsxOpenZfsResponseTypeDef:
         """
         Creates an endpoint for an Amazon FSx for OpenZFS file system that DataSync can
         access for a
         transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_fsx_open_zfs)
@@ -302,15 +301,15 @@
         *,
         FsxFilesystemArn: str,
         SecurityGroupArns: Sequence[str],
         User: str,
         Password: str,
         Subdirectory: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
-        Domain: str = ...
+        Domain: str = ...,
     ) -> CreateLocationFsxWindowsResponseTypeDef:
         """
         Creates an endpoint for an Amazon FSx for Windows File Server file system that
         DataSync can use for a data
         transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_fsx_windows)
@@ -328,15 +327,15 @@
         ReplicationFactor: int = ...,
         KmsKeyProviderUri: str = ...,
         QopConfiguration: QopConfigurationTypeDef = ...,
         SimpleUser: str = ...,
         KerberosPrincipal: str = ...,
         KerberosKeytab: BlobTypeDef = ...,
         KerberosKrb5Conf: BlobTypeDef = ...,
-        Tags: Sequence[TagListEntryTypeDef] = ...
+        Tags: Sequence[TagListEntryTypeDef] = ...,
     ) -> CreateLocationHdfsResponseTypeDef:
         """
         Creates an endpoint for a Hadoop Distributed File System (HDFS).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_hdfs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#create_location_hdfs)
         """
@@ -344,15 +343,15 @@
     async def create_location_nfs(
         self,
         *,
         Subdirectory: str,
         ServerHostname: str,
         OnPremConfig: OnPremConfigTypeDef,
         MountOptions: NfsMountOptionsTypeDef = ...,
-        Tags: Sequence[TagListEntryTypeDef] = ...
+        Tags: Sequence[TagListEntryTypeDef] = ...,
     ) -> CreateLocationNfsResponseTypeDef:
         """
         Creates an endpoint for a Network File System (NFS) file server that DataSync
         can use for a data
         transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_nfs)
@@ -367,15 +366,15 @@
         AgentArns: Sequence[str],
         ServerPort: int = ...,
         ServerProtocol: ObjectStorageServerProtocolType = ...,
         Subdirectory: str = ...,
         AccessKey: str = ...,
         SecretKey: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
-        ServerCertificate: BlobTypeDef = ...
+        ServerCertificate: BlobTypeDef = ...,
     ) -> CreateLocationObjectStorageResponseTypeDef:
         """
         Creates an endpoint for an object storage system that DataSync can access for a
         transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_object_storage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#create_location_object_storage)
@@ -385,15 +384,15 @@
         self,
         *,
         S3BucketArn: str,
         S3Config: S3ConfigTypeDef,
         Subdirectory: str = ...,
         S3StorageClass: S3StorageClassType = ...,
         AgentArns: Sequence[str] = ...,
-        Tags: Sequence[TagListEntryTypeDef] = ...
+        Tags: Sequence[TagListEntryTypeDef] = ...,
     ) -> CreateLocationS3ResponseTypeDef:
         """
         A *location* is an endpoint for an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_s3)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#create_location_s3)
         """
@@ -404,15 +403,15 @@
         Subdirectory: str,
         ServerHostname: str,
         User: str,
         Password: str,
         AgentArns: Sequence[str],
         Domain: str = ...,
         MountOptions: SmbMountOptionsTypeDef = ...,
-        Tags: Sequence[TagListEntryTypeDef] = ...
+        Tags: Sequence[TagListEntryTypeDef] = ...,
     ) -> CreateLocationSmbResponseTypeDef:
         """
         Creates an endpoint for a Server Message Block (SMB) file server that DataSync
         can use for a data
         transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_smb)
@@ -427,15 +426,15 @@
         CloudWatchLogGroupArn: str = ...,
         Name: str = ...,
         Options: OptionsTypeDef = ...,
         Excludes: Sequence[FilterRuleTypeDef] = ...,
         Schedule: TaskScheduleTypeDef = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         Includes: Sequence[FilterRuleTypeDef] = ...,
-        TaskReportConfig: TaskReportConfigTypeDef = ...
+        TaskReportConfig: TaskReportConfigTypeDef = ...,
     ) -> CreateTaskResponseTypeDef:
         """
         Configures a transfer task, which defines where and how DataSync moves your
         data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#create_task)
@@ -624,15 +623,15 @@
         *,
         DiscoveryJobArn: str,
         ResourceType: DiscoveryResourceTypeType,
         ResourceId: str,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeStorageSystemResourceMetricsResponseTypeDef:
         """
         Returns information, including performance data and capacity usage, which
         DataSync Discovery collects about a specific resource in your-premises storage
         system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_storage_system_resource_metrics)
@@ -643,15 +642,15 @@
         self,
         *,
         DiscoveryJobArn: str,
         ResourceType: DiscoveryResourceTypeType,
         ResourceIds: Sequence[str] = ...,
         Filter: Mapping[Literal["SVM"], Sequence[str]] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeStorageSystemResourcesResponseTypeDef:
         """
         Returns information that DataSync Discovery collects about resources in your
         on-premises storage
         system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_storage_system_resources)
@@ -691,15 +690,15 @@
         """
 
     async def generate_recommendations(
         self,
         *,
         DiscoveryJobArn: str,
         ResourceIds: Sequence[str],
-        ResourceType: DiscoveryResourceTypeType
+        ResourceType: DiscoveryResourceTypeType,
     ) -> Dict[str, Any]:
         """
         Creates recommendations about where to migrate your data to in Amazon Web
         Services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.generate_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#generate_recommendations)
@@ -730,15 +729,15 @@
         """
 
     async def list_locations(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Filters: Sequence[LocationFilterTypeDef] = ...
+        Filters: Sequence[LocationFilterTypeDef] = ...,
     ) -> ListLocationsResponseTypeDef:
         """
         Returns a list of source and destination locations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_locations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#list_locations)
         """
@@ -774,15 +773,15 @@
         """
 
     async def list_tasks(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Filters: Sequence[TaskFilterTypeDef] = ...
+        Filters: Sequence[TaskFilterTypeDef] = ...,
     ) -> ListTasksResponseTypeDef:
         """
         Returns a list of the DataSync tasks you created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#list_tasks)
         """
@@ -799,15 +798,15 @@
 
     async def start_discovery_job(
         self,
         *,
         StorageSystemArn: str,
         CollectionDurationMinutes: int,
         ClientToken: str,
-        Tags: Sequence[TagListEntryTypeDef] = ...
+        Tags: Sequence[TagListEntryTypeDef] = ...,
     ) -> StartDiscoveryJobResponseTypeDef:
         """
         Runs a DataSync discovery job on your on-premises storage system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.start_discovery_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#start_discovery_job)
         """
@@ -816,15 +815,15 @@
         self,
         *,
         TaskArn: str,
         OverrideOptions: OptionsTypeDef = ...,
         Includes: Sequence[FilterRuleTypeDef] = ...,
         Excludes: Sequence[FilterRuleTypeDef] = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
-        TaskReportConfig: TaskReportConfigTypeDef = ...
+        TaskReportConfig: TaskReportConfigTypeDef = ...,
     ) -> StartTaskExecutionResponseTypeDef:
         """
         Starts an DataSync transfer task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.start_task_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#start_task_execution)
         """
@@ -878,15 +877,15 @@
         *,
         LocationArn: str,
         Subdirectory: str = ...,
         AuthenticationType: Literal["SAS"] = ...,
         SasConfiguration: AzureBlobSasConfigurationTypeDef = ...,
         BlobType: Literal["BLOCK"] = ...,
         AccessTier: AzureAccessTierType = ...,
-        AgentArns: Sequence[str] = ...
+        AgentArns: Sequence[str] = ...,
     ) -> Dict[str, Any]:
         """
         Modifies some configurations of the Microsoft Azure Blob Storage transfer
         location that you're using with
         DataSync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_location_azure_blob)
@@ -904,15 +903,15 @@
         KmsKeyProviderUri: str = ...,
         QopConfiguration: QopConfigurationTypeDef = ...,
         AuthenticationType: HdfsAuthenticationTypeType = ...,
         SimpleUser: str = ...,
         KerberosPrincipal: str = ...,
         KerberosKeytab: BlobTypeDef = ...,
         KerberosKrb5Conf: BlobTypeDef = ...,
-        AgentArns: Sequence[str] = ...
+        AgentArns: Sequence[str] = ...,
     ) -> Dict[str, Any]:
         """
         Updates some parameters of a previously created location for a Hadoop
         Distributed File System
         cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_location_hdfs)
@@ -921,15 +920,15 @@
 
     async def update_location_nfs(
         self,
         *,
         LocationArn: str,
         Subdirectory: str = ...,
         OnPremConfig: OnPremConfigTypeDef = ...,
-        MountOptions: NfsMountOptionsTypeDef = ...
+        MountOptions: NfsMountOptionsTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Modifies some configurations of the Network File System (NFS) transfer location
         that you're using with
         DataSync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_location_nfs)
@@ -942,15 +941,15 @@
         LocationArn: str,
         ServerPort: int = ...,
         ServerProtocol: ObjectStorageServerProtocolType = ...,
         Subdirectory: str = ...,
         AccessKey: str = ...,
         SecretKey: str = ...,
         AgentArns: Sequence[str] = ...,
-        ServerCertificate: BlobTypeDef = ...
+        ServerCertificate: BlobTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates some parameters of an existing object storage location that DataSync
         accesses for a
         transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_location_object_storage)
@@ -962,15 +961,15 @@
         *,
         LocationArn: str,
         Subdirectory: str = ...,
         User: str = ...,
         Domain: str = ...,
         Password: str = ...,
         AgentArns: Sequence[str] = ...,
-        MountOptions: SmbMountOptionsTypeDef = ...
+        MountOptions: SmbMountOptionsTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates some of the parameters of a Server Message Block (SMB) file server
         location that you can use for DataSync
         transfers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_location_smb)
@@ -981,15 +980,15 @@
         self,
         *,
         StorageSystemArn: str,
         ServerConfiguration: DiscoveryServerConfigurationTypeDef = ...,
         AgentArns: Sequence[str] = ...,
         Name: str = ...,
         CloudWatchLogGroupArn: str = ...,
-        Credentials: CredentialsTypeDef = ...
+        Credentials: CredentialsTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Modifies some configurations of an on-premises storage system resource that
         you're using with DataSync
         Discovery.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_storage_system)
@@ -1002,15 +1001,15 @@
         TaskArn: str,
         Options: OptionsTypeDef = ...,
         Excludes: Sequence[FilterRuleTypeDef] = ...,
         Schedule: TaskScheduleTypeDef = ...,
         Name: str = ...,
         CloudWatchLogGroupArn: str = ...,
         Includes: Sequence[FilterRuleTypeDef] = ...,
-        TaskReportConfig: TaskReportConfigTypeDef = ...
+        TaskReportConfig: TaskReportConfigTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the configuration of a DataSync transfer task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#update_task)
         """
```

### Comparing `types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync/client.pyi` & `types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         ServerConfiguration: DiscoveryServerConfigurationTypeDef,
         SystemType: Literal["NetAppONTAP"],
         AgentArns: Sequence[str],
         ClientToken: str,
         Credentials: CredentialsTypeDef,
         CloudWatchLogGroupArn: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
-        Name: str = ...
+        Name: str = ...,
     ) -> AddStorageSystemResponseTypeDef:
         """
         Creates an Amazon Web Services resource for an on-premises storage system that
         you want DataSync Discovery to collect information
         about.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.add_storage_system)
@@ -188,15 +188,15 @@
         self,
         *,
         ActivationKey: str,
         AgentName: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         VpcEndpointId: str = ...,
         SubnetArns: Sequence[str] = ...,
-        SecurityGroupArns: Sequence[str] = ...
+        SecurityGroupArns: Sequence[str] = ...,
     ) -> CreateAgentResponseTypeDef:
         """
         Activates an DataSync agent that you've deployed in your storage environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_agent)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#create_agent)
         """
@@ -207,15 +207,15 @@
         ContainerUrl: str,
         AuthenticationType: Literal["SAS"],
         AgentArns: Sequence[str],
         SasConfiguration: AzureBlobSasConfigurationTypeDef = ...,
         BlobType: Literal["BLOCK"] = ...,
         AccessTier: AzureAccessTierType = ...,
         Subdirectory: str = ...,
-        Tags: Sequence[TagListEntryTypeDef] = ...
+        Tags: Sequence[TagListEntryTypeDef] = ...,
     ) -> CreateLocationAzureBlobResponseTypeDef:
         """
         Creates an endpoint for a Microsoft Azure Blob Storage container that DataSync
         can use as a transfer source or
         destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_azure_blob)
@@ -227,15 +227,15 @@
         *,
         EfsFilesystemArn: str,
         Ec2Config: Ec2ConfigTypeDef,
         Subdirectory: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         AccessPointArn: str = ...,
         FileSystemAccessRoleArn: str = ...,
-        InTransitEncryption: EfsInTransitEncryptionType = ...
+        InTransitEncryption: EfsInTransitEncryptionType = ...,
     ) -> CreateLocationEfsResponseTypeDef:
         """
         Creates an endpoint for an Amazon EFS file system that DataSync can access for
         a
         transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_efs)
@@ -244,15 +244,15 @@
 
     async def create_location_fsx_lustre(
         self,
         *,
         FsxFilesystemArn: str,
         SecurityGroupArns: Sequence[str],
         Subdirectory: str = ...,
-        Tags: Sequence[TagListEntryTypeDef] = ...
+        Tags: Sequence[TagListEntryTypeDef] = ...,
     ) -> CreateLocationFsxLustreResponseTypeDef:
         """
         Creates an endpoint for an Amazon FSx for Lustre file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_fsx_lustre)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#create_location_fsx_lustre)
         """
@@ -260,15 +260,15 @@
     async def create_location_fsx_ontap(
         self,
         *,
         Protocol: FsxProtocolTypeDef,
         SecurityGroupArns: Sequence[str],
         StorageVirtualMachineArn: str,
         Subdirectory: str = ...,
-        Tags: Sequence[TagListEntryTypeDef] = ...
+        Tags: Sequence[TagListEntryTypeDef] = ...,
     ) -> CreateLocationFsxOntapResponseTypeDef:
         """
         Creates an endpoint for an Amazon FSx for NetApp ONTAP file system that
         DataSync can use for a data
         transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_fsx_ontap)
@@ -278,15 +278,15 @@
     async def create_location_fsx_open_zfs(
         self,
         *,
         FsxFilesystemArn: str,
         Protocol: FsxProtocolTypeDef,
         SecurityGroupArns: Sequence[str],
         Subdirectory: str = ...,
-        Tags: Sequence[TagListEntryTypeDef] = ...
+        Tags: Sequence[TagListEntryTypeDef] = ...,
     ) -> CreateLocationFsxOpenZfsResponseTypeDef:
         """
         Creates an endpoint for an Amazon FSx for OpenZFS file system that DataSync can
         access for a
         transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_fsx_open_zfs)
@@ -298,15 +298,15 @@
         *,
         FsxFilesystemArn: str,
         SecurityGroupArns: Sequence[str],
         User: str,
         Password: str,
         Subdirectory: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
-        Domain: str = ...
+        Domain: str = ...,
     ) -> CreateLocationFsxWindowsResponseTypeDef:
         """
         Creates an endpoint for an Amazon FSx for Windows File Server file system that
         DataSync can use for a data
         transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_fsx_windows)
@@ -324,15 +324,15 @@
         ReplicationFactor: int = ...,
         KmsKeyProviderUri: str = ...,
         QopConfiguration: QopConfigurationTypeDef = ...,
         SimpleUser: str = ...,
         KerberosPrincipal: str = ...,
         KerberosKeytab: BlobTypeDef = ...,
         KerberosKrb5Conf: BlobTypeDef = ...,
-        Tags: Sequence[TagListEntryTypeDef] = ...
+        Tags: Sequence[TagListEntryTypeDef] = ...,
     ) -> CreateLocationHdfsResponseTypeDef:
         """
         Creates an endpoint for a Hadoop Distributed File System (HDFS).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_hdfs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#create_location_hdfs)
         """
@@ -340,15 +340,15 @@
     async def create_location_nfs(
         self,
         *,
         Subdirectory: str,
         ServerHostname: str,
         OnPremConfig: OnPremConfigTypeDef,
         MountOptions: NfsMountOptionsTypeDef = ...,
-        Tags: Sequence[TagListEntryTypeDef] = ...
+        Tags: Sequence[TagListEntryTypeDef] = ...,
     ) -> CreateLocationNfsResponseTypeDef:
         """
         Creates an endpoint for a Network File System (NFS) file server that DataSync
         can use for a data
         transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_nfs)
@@ -363,15 +363,15 @@
         AgentArns: Sequence[str],
         ServerPort: int = ...,
         ServerProtocol: ObjectStorageServerProtocolType = ...,
         Subdirectory: str = ...,
         AccessKey: str = ...,
         SecretKey: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
-        ServerCertificate: BlobTypeDef = ...
+        ServerCertificate: BlobTypeDef = ...,
     ) -> CreateLocationObjectStorageResponseTypeDef:
         """
         Creates an endpoint for an object storage system that DataSync can access for a
         transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_object_storage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#create_location_object_storage)
@@ -381,15 +381,15 @@
         self,
         *,
         S3BucketArn: str,
         S3Config: S3ConfigTypeDef,
         Subdirectory: str = ...,
         S3StorageClass: S3StorageClassType = ...,
         AgentArns: Sequence[str] = ...,
-        Tags: Sequence[TagListEntryTypeDef] = ...
+        Tags: Sequence[TagListEntryTypeDef] = ...,
     ) -> CreateLocationS3ResponseTypeDef:
         """
         A *location* is an endpoint for an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_s3)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#create_location_s3)
         """
@@ -400,15 +400,15 @@
         Subdirectory: str,
         ServerHostname: str,
         User: str,
         Password: str,
         AgentArns: Sequence[str],
         Domain: str = ...,
         MountOptions: SmbMountOptionsTypeDef = ...,
-        Tags: Sequence[TagListEntryTypeDef] = ...
+        Tags: Sequence[TagListEntryTypeDef] = ...,
     ) -> CreateLocationSmbResponseTypeDef:
         """
         Creates an endpoint for a Server Message Block (SMB) file server that DataSync
         can use for a data
         transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_smb)
@@ -423,15 +423,15 @@
         CloudWatchLogGroupArn: str = ...,
         Name: str = ...,
         Options: OptionsTypeDef = ...,
         Excludes: Sequence[FilterRuleTypeDef] = ...,
         Schedule: TaskScheduleTypeDef = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         Includes: Sequence[FilterRuleTypeDef] = ...,
-        TaskReportConfig: TaskReportConfigTypeDef = ...
+        TaskReportConfig: TaskReportConfigTypeDef = ...,
     ) -> CreateTaskResponseTypeDef:
         """
         Configures a transfer task, which defines where and how DataSync moves your
         data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#create_task)
@@ -620,15 +620,15 @@
         *,
         DiscoveryJobArn: str,
         ResourceType: DiscoveryResourceTypeType,
         ResourceId: str,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeStorageSystemResourceMetricsResponseTypeDef:
         """
         Returns information, including performance data and capacity usage, which
         DataSync Discovery collects about a specific resource in your-premises storage
         system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_storage_system_resource_metrics)
@@ -639,15 +639,15 @@
         self,
         *,
         DiscoveryJobArn: str,
         ResourceType: DiscoveryResourceTypeType,
         ResourceIds: Sequence[str] = ...,
         Filter: Mapping[Literal["SVM"], Sequence[str]] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeStorageSystemResourcesResponseTypeDef:
         """
         Returns information that DataSync Discovery collects about resources in your
         on-premises storage
         system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_storage_system_resources)
@@ -687,15 +687,15 @@
         """
 
     async def generate_recommendations(
         self,
         *,
         DiscoveryJobArn: str,
         ResourceIds: Sequence[str],
-        ResourceType: DiscoveryResourceTypeType
+        ResourceType: DiscoveryResourceTypeType,
     ) -> Dict[str, Any]:
         """
         Creates recommendations about where to migrate your data to in Amazon Web
         Services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.generate_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#generate_recommendations)
@@ -726,15 +726,15 @@
         """
 
     async def list_locations(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Filters: Sequence[LocationFilterTypeDef] = ...
+        Filters: Sequence[LocationFilterTypeDef] = ...,
     ) -> ListLocationsResponseTypeDef:
         """
         Returns a list of source and destination locations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_locations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#list_locations)
         """
@@ -770,15 +770,15 @@
         """
 
     async def list_tasks(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Filters: Sequence[TaskFilterTypeDef] = ...
+        Filters: Sequence[TaskFilterTypeDef] = ...,
     ) -> ListTasksResponseTypeDef:
         """
         Returns a list of the DataSync tasks you created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#list_tasks)
         """
@@ -795,15 +795,15 @@
 
     async def start_discovery_job(
         self,
         *,
         StorageSystemArn: str,
         CollectionDurationMinutes: int,
         ClientToken: str,
-        Tags: Sequence[TagListEntryTypeDef] = ...
+        Tags: Sequence[TagListEntryTypeDef] = ...,
     ) -> StartDiscoveryJobResponseTypeDef:
         """
         Runs a DataSync discovery job on your on-premises storage system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.start_discovery_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#start_discovery_job)
         """
@@ -812,15 +812,15 @@
         self,
         *,
         TaskArn: str,
         OverrideOptions: OptionsTypeDef = ...,
         Includes: Sequence[FilterRuleTypeDef] = ...,
         Excludes: Sequence[FilterRuleTypeDef] = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
-        TaskReportConfig: TaskReportConfigTypeDef = ...
+        TaskReportConfig: TaskReportConfigTypeDef = ...,
     ) -> StartTaskExecutionResponseTypeDef:
         """
         Starts an DataSync transfer task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.start_task_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#start_task_execution)
         """
@@ -874,15 +874,15 @@
         *,
         LocationArn: str,
         Subdirectory: str = ...,
         AuthenticationType: Literal["SAS"] = ...,
         SasConfiguration: AzureBlobSasConfigurationTypeDef = ...,
         BlobType: Literal["BLOCK"] = ...,
         AccessTier: AzureAccessTierType = ...,
-        AgentArns: Sequence[str] = ...
+        AgentArns: Sequence[str] = ...,
     ) -> Dict[str, Any]:
         """
         Modifies some configurations of the Microsoft Azure Blob Storage transfer
         location that you're using with
         DataSync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_location_azure_blob)
@@ -900,15 +900,15 @@
         KmsKeyProviderUri: str = ...,
         QopConfiguration: QopConfigurationTypeDef = ...,
         AuthenticationType: HdfsAuthenticationTypeType = ...,
         SimpleUser: str = ...,
         KerberosPrincipal: str = ...,
         KerberosKeytab: BlobTypeDef = ...,
         KerberosKrb5Conf: BlobTypeDef = ...,
-        AgentArns: Sequence[str] = ...
+        AgentArns: Sequence[str] = ...,
     ) -> Dict[str, Any]:
         """
         Updates some parameters of a previously created location for a Hadoop
         Distributed File System
         cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_location_hdfs)
@@ -917,15 +917,15 @@
 
     async def update_location_nfs(
         self,
         *,
         LocationArn: str,
         Subdirectory: str = ...,
         OnPremConfig: OnPremConfigTypeDef = ...,
-        MountOptions: NfsMountOptionsTypeDef = ...
+        MountOptions: NfsMountOptionsTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Modifies some configurations of the Network File System (NFS) transfer location
         that you're using with
         DataSync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_location_nfs)
@@ -938,15 +938,15 @@
         LocationArn: str,
         ServerPort: int = ...,
         ServerProtocol: ObjectStorageServerProtocolType = ...,
         Subdirectory: str = ...,
         AccessKey: str = ...,
         SecretKey: str = ...,
         AgentArns: Sequence[str] = ...,
-        ServerCertificate: BlobTypeDef = ...
+        ServerCertificate: BlobTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates some parameters of an existing object storage location that DataSync
         accesses for a
         transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_location_object_storage)
@@ -958,15 +958,15 @@
         *,
         LocationArn: str,
         Subdirectory: str = ...,
         User: str = ...,
         Domain: str = ...,
         Password: str = ...,
         AgentArns: Sequence[str] = ...,
-        MountOptions: SmbMountOptionsTypeDef = ...
+        MountOptions: SmbMountOptionsTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates some of the parameters of a Server Message Block (SMB) file server
         location that you can use for DataSync
         transfers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_location_smb)
@@ -977,15 +977,15 @@
         self,
         *,
         StorageSystemArn: str,
         ServerConfiguration: DiscoveryServerConfigurationTypeDef = ...,
         AgentArns: Sequence[str] = ...,
         Name: str = ...,
         CloudWatchLogGroupArn: str = ...,
-        Credentials: CredentialsTypeDef = ...
+        Credentials: CredentialsTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Modifies some configurations of an on-premises storage system resource that
         you're using with DataSync
         Discovery.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_storage_system)
@@ -998,15 +998,15 @@
         TaskArn: str,
         Options: OptionsTypeDef = ...,
         Excludes: Sequence[FilterRuleTypeDef] = ...,
         Schedule: TaskScheduleTypeDef = ...,
         Name: str = ...,
         CloudWatchLogGroupArn: str = ...,
         Includes: Sequence[FilterRuleTypeDef] = ...,
-        TaskReportConfig: TaskReportConfigTypeDef = ...
+        TaskReportConfig: TaskReportConfigTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the configuration of a DataSync transfer task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#update_task)
         """
```

### Comparing `types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync/literals.py` & `types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync/literals.py`

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
     "AgentStatusType",
     "AtimeType",
     "AzureAccessTierType",
     "AzureBlobAuthenticationTypeType",
     "AzureBlobTypeType",
     "DescribeStorageSystemResourceMetricsPaginatorName",
@@ -75,15 +74,14 @@
     "DataSyncServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AgentStatusType = Literal["OFFLINE", "ONLINE"]
 AtimeType = Literal["BEST_EFFORT", "NONE"]
 AzureAccessTierType = Literal["ARCHIVE", "COOL", "HOT"]
 AzureBlobAuthenticationTypeType = Literal["SAS"]
 AzureBlobTypeType = Literal["BLOCK"]
 DescribeStorageSystemResourceMetricsPaginatorName = Literal[
     "describe_storage_system_resource_metrics"
```

### Comparing `types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync/literals.pyi` & `types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync/paginator.py` & `types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,14 @@
     "ListLocationsPaginator",
     "ListStorageSystemsPaginator",
     "ListTagsForResourcePaginator",
     "ListTaskExecutionsPaginator",
     "ListTasksPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -88,15 +87,15 @@
         self,
         *,
         DiscoveryJobArn: str,
         ResourceType: DiscoveryResourceTypeType,
         ResourceId: str,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeStorageSystemResourceMetricsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.DescribeStorageSystemResourceMetrics.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/paginators/#describestoragesystemresourcemetricspaginator)
         """
 
 
@@ -136,15 +135,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/paginators/#listlocationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[LocationFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListLocationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListLocations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/paginators/#listlocationspaginator)
         """
 
 
@@ -199,13 +198,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/paginators/#listtaskspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[TaskFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/paginators/#listtaskspaginator)
         """
```

### Comparing `types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync/paginator.pyi` & `types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         self,
         *,
         DiscoveryJobArn: str,
         ResourceType: DiscoveryResourceTypeType,
         ResourceId: str,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeStorageSystemResourceMetricsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.DescribeStorageSystemResourceMetrics.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/paginators/#describestoragesystemresourcemetricspaginator)
         """
 
 class ListAgentsPaginator(AioPaginator):
@@ -130,15 +130,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/paginators/#listlocationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[LocationFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListLocationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListLocations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/paginators/#listlocationspaginator)
         """
 
 class ListStorageSystemsPaginator(AioPaginator):
@@ -189,13 +189,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/paginators/#listtaskspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[TaskFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/paginators/#listtaskspaginator)
         """
```

### Comparing `types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync/type_defs.py` & `types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CredentialsTypeDef",
     "DiscoveryServerConfigurationTypeDef",
     "TagListEntryTypeDef",
     "ResponseMetadataTypeDef",
     "PlatformTypeDef",
     "AzureBlobSasConfigurationTypeDef",
```

### Comparing `types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync/type_defs.pyi` & `types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync.egg-info/PKG-INFO` & `types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-datasync
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.DataSync 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.DataSync 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/
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
 
 <a id="types-aiobotocore-datasync"></a>
 
 # types-aiobotocore-datasync
 
 [![PyPI - types-aiobotocore-datasync](https://img.shields.io/pypi/v/types-aiobotocore-datasync.svg?color=blue)](https://pypi.org/project/types-aiobotocore-datasync)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-datasync.svg?color=blue)](https://pypi.org/project/types-aiobotocore-datasync)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-datasync)](https://pepy.tech/project/types-aiobotocore-datasync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DataSync 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
+[aiobotocore.DataSync 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
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
 [types-aiobotocore-datasync docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-datasync-2.9.0/types_aiobotocore_datasync.egg-info/SOURCES.txt` & `types-aiobotocore-datasync-2.9.1/types_aiobotocore_datasync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

