# Comparing `tmp/types-aiobotocore-ivs-2.9.0.tar.gz` & `tmp/types-aiobotocore-ivs-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ivs-2.9.0.tar", last modified: Wed Dec 13 19:59:36 2023, max compression
+gzip compressed data, was "types-aiobotocore-ivs-2.9.1.tar", last modified: Thu Jan 18 01:20:59 2024, max compression
```

## Comparing `types-aiobotocore-ivs-2.9.0.tar` & `types-aiobotocore-ivs-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:36.265603 types-aiobotocore-ivs-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:48:15.000000 types-aiobotocore-ivs-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13325 2023-12-13 19:59:36.265603 types-aiobotocore-ivs-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11778 2023-12-13 19:48:15.000000 types-aiobotocore-ivs-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:36.265603 types-aiobotocore-ivs-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-12-13 19:48:15.000000 types-aiobotocore-ivs-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:36.265603 types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs/
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2023-12-13 19:48:15.000000 types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2023-12-13 19:48:15.000000 types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-13 19:48:15.000000 types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24768 2023-12-13 19:48:16.000000 types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    24764 2023-12-13 19:48:15.000000 types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10089 2023-12-13 19:48:17.000000 types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10087 2023-12-13 19:48:16.000000 types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2023-12-13 19:48:16.000000 types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2023-12-13 19:48:16.000000 types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:48:15.000000 types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    23971 2023-12-13 19:48:17.000000 types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23970 2023-12-13 19:48:17.000000 types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:48:15.000000 types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:36.265603 types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13325 2023-12-13 19:59:36.000000 types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      737 2023-12-13 19:59:36.000000 types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:36.000000 types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:36.000000 types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:36.000000 types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 19:59:36.000000 types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:59.473256 types-aiobotocore-ivs-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:10:04.000000 types-aiobotocore-ivs-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13345 2024-01-18 01:20:59.473256 types-aiobotocore-ivs-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11778 2024-01-18 01:10:04.000000 types-aiobotocore-ivs-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:59.473256 types-aiobotocore-ivs-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-01-18 01:10:04.000000 types-aiobotocore-ivs-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:59.473256 types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-01-18 01:10:04.000000 types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-01-18 01:10:04.000000 types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-18 01:10:04.000000 types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24771 2024-01-18 01:10:05.000000 types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24768 2024-01-18 01:10:05.000000 types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-01-18 01:10:05.000000 types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-01-18 01:10:05.000000 types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-01-18 01:10:05.000000 types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-01-18 01:10:05.000000 types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:10:04.000000 types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    23970 2024-01-18 01:10:05.000000 types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23970 2024-01-18 01:10:05.000000 types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:10:04.000000 types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:59.473256 types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13345 2024-01-18 01:20:59.000000 types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-01-18 01:20:59.000000 types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:59.000000 types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:59.000000 types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:59.000000 types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:20:59.000000 types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ivs-2.9.0/LICENSE` & `types-aiobotocore-ivs-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-ivs-2.9.0/PKG-INFO` & `types-aiobotocore-ivs-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ivs
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IVS 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IVS 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/
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
 
 <a id="types-aiobotocore-ivs"></a>
 
 # types-aiobotocore-ivs
 
 [![PyPI - types-aiobotocore-ivs](https://img.shields.io/pypi/v/types-aiobotocore-ivs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ivs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ivs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ivs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ivs)](https://pepy.tech/project/types-aiobotocore-ivs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IVS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
+[aiobotocore.IVS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
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
 [types-aiobotocore-ivs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ivs-2.9.0/README.md` & `types-aiobotocore-ivs-2.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ivs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ivs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ivs)](https://pepy.tech/project/types-aiobotocore-ivs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IVS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
+[aiobotocore.IVS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
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
 [types-aiobotocore-ivs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ivs-2.9.0/setup.py` & `types-aiobotocore-ivs-2.9.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ivs",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_ivs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.IVS 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.IVS 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore ivs type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_ivs": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs/__init__.py` & `types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     ListRecordingConfigurationsPaginator,
     ListStreamKeysPaginator,
     ListStreamsPaginator,
 )
 
 Client = IVSClient
 
-
 __all__ = (
     "Client",
     "IVSClient",
     "ListChannelsPaginator",
     "ListPlaybackKeyPairsPaginator",
     "ListRecordingConfigurationsPaginator",
     "ListStreamKeysPaginator",
```

### Comparing `types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs/__init__.pyi` & `types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs/__main__.py` & `types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IVS 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.IVS 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS\nOther"
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

### Comparing `types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs/client.py` & `types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("IVSClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -159,15 +158,15 @@
         authorized: bool = ...,
         insecureIngest: bool = ...,
         latencyMode: ChannelLatencyModeType = ...,
         name: str = ...,
         preset: TranscodePresetType = ...,
         recordingConfigurationArn: str = ...,
         tags: Mapping[str, str] = ...,
-        type: ChannelTypeType = ...
+        type: ChannelTypeType = ...,
     ) -> CreateChannelResponseTypeDef:
         """
         Creates a new channel and an associated stream key to start streaming.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.create_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/client/#create_channel)
         """
@@ -176,15 +175,15 @@
         self,
         *,
         destinationConfiguration: DestinationConfigurationTypeDef,
         name: str = ...,
         recordingReconnectWindowSeconds: int = ...,
         renditionConfiguration: RenditionConfigurationTypeDef = ...,
         tags: Mapping[str, str] = ...,
-        thumbnailConfiguration: ThumbnailConfigurationTypeDef = ...
+        thumbnailConfiguration: ThumbnailConfigurationTypeDef = ...,
     ) -> CreateRecordingConfigurationResponseTypeDef:
         """
         Creates a new recording configuration, used to enable recording to Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.create_recording_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/client/#create_recording_configuration)
         """
@@ -312,15 +311,15 @@
 
     async def list_channels(
         self,
         *,
         filterByName: str = ...,
         filterByRecordingConfigurationArn: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListChannelsResponseTypeDef:
         """
         Gets summary information about all channels in your account, in the Amazon Web
         Services region where the API request is
         processed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.list_channels)
@@ -444,15 +443,15 @@
         arn: str,
         authorized: bool = ...,
         insecureIngest: bool = ...,
         latencyMode: ChannelLatencyModeType = ...,
         name: str = ...,
         preset: TranscodePresetType = ...,
         recordingConfigurationArn: str = ...,
-        type: ChannelTypeType = ...
+        type: ChannelTypeType = ...,
     ) -> UpdateChannelResponseTypeDef:
         """
         Updates a channel's configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.update_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/client/#update_channel)
         """
```

### Comparing `types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs/client.pyi` & `types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         authorized: bool = ...,
         insecureIngest: bool = ...,
         latencyMode: ChannelLatencyModeType = ...,
         name: str = ...,
         preset: TranscodePresetType = ...,
         recordingConfigurationArn: str = ...,
         tags: Mapping[str, str] = ...,
-        type: ChannelTypeType = ...
+        type: ChannelTypeType = ...,
     ) -> CreateChannelResponseTypeDef:
         """
         Creates a new channel and an associated stream key to start streaming.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.create_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/client/#create_channel)
         """
@@ -172,15 +172,15 @@
         self,
         *,
         destinationConfiguration: DestinationConfigurationTypeDef,
         name: str = ...,
         recordingReconnectWindowSeconds: int = ...,
         renditionConfiguration: RenditionConfigurationTypeDef = ...,
         tags: Mapping[str, str] = ...,
-        thumbnailConfiguration: ThumbnailConfigurationTypeDef = ...
+        thumbnailConfiguration: ThumbnailConfigurationTypeDef = ...,
     ) -> CreateRecordingConfigurationResponseTypeDef:
         """
         Creates a new recording configuration, used to enable recording to Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.create_recording_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/client/#create_recording_configuration)
         """
@@ -308,15 +308,15 @@
 
     async def list_channels(
         self,
         *,
         filterByName: str = ...,
         filterByRecordingConfigurationArn: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListChannelsResponseTypeDef:
         """
         Gets summary information about all channels in your account, in the Amazon Web
         Services region where the API request is
         processed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.list_channels)
@@ -440,15 +440,15 @@
         arn: str,
         authorized: bool = ...,
         insecureIngest: bool = ...,
         latencyMode: ChannelLatencyModeType = ...,
         name: str = ...,
         preset: TranscodePresetType = ...,
         recordingConfigurationArn: str = ...,
-        type: ChannelTypeType = ...
+        type: ChannelTypeType = ...,
     ) -> UpdateChannelResponseTypeDef:
         """
         Updates a channel's configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.update_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/client/#update_channel)
         """
```

### Comparing `types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs/literals.py` & `types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs/literals.py`

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
     "ChannelLatencyModeType",
     "ChannelTypeType",
     "ListChannelsPaginatorName",
     "ListPlaybackKeyPairsPaginatorName",
     "ListRecordingConfigurationsPaginatorName",
     "ListStreamKeysPaginatorName",
@@ -40,15 +39,14 @@
     "IVSServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ChannelLatencyModeType = Literal["LOW", "NORMAL"]
 ChannelTypeType = Literal["ADVANCED_HD", "ADVANCED_SD", "BASIC", "STANDARD"]
 ListChannelsPaginatorName = Literal["list_channels"]
 ListPlaybackKeyPairsPaginatorName = Literal["list_playback_key_pairs"]
 ListRecordingConfigurationsPaginatorName = Literal["list_recording_configurations"]
 ListStreamKeysPaginatorName = Literal["list_stream_keys"]
 ListStreamsPaginatorName = Literal["list_streams"]
```

### Comparing `types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs/literals.pyi` & `types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs/paginator.py` & `types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,14 @@
     "ListChannelsPaginator",
     "ListPlaybackKeyPairsPaginator",
     "ListRecordingConfigurationsPaginator",
     "ListStreamKeysPaginator",
     "ListStreamsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -70,15 +69,15 @@
     """
 
     def paginate(
         self,
         *,
         filterByName: str = ...,
         filterByRecordingConfigurationArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListChannels.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/paginators/#listchannelspaginator)
         """
 
 
@@ -133,13 +132,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/paginators/#liststreamspaginator)
     """
 
     def paginate(
         self,
         *,
         filterBy: StreamFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListStreamsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListStreams.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/paginators/#liststreamspaginator)
         """
```

### Comparing `types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs/paginator.pyi` & `types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     """
 
     def paginate(
         self,
         *,
         filterByName: str = ...,
         filterByRecordingConfigurationArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListChannels.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/paginators/#listchannelspaginator)
         """
 
 class ListPlaybackKeyPairsPaginator(AioPaginator):
@@ -126,13 +126,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/paginators/#liststreamspaginator)
     """
 
     def paginate(
         self,
         *,
         filterBy: StreamFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListStreamsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListStreams.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/paginators/#liststreamspaginator)
         """
```

### Comparing `types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs/type_defs.py` & `types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AudioConfigurationTypeDef",
     "BatchErrorTypeDef",
     "BatchGetChannelRequestRequestTypeDef",
     "ChannelTypeDef",
     "ResponseMetadataTypeDef",
     "BatchGetStreamKeyRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs/type_defs.pyi` & `types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs.egg-info/PKG-INFO` & `types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ivs
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IVS 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IVS 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/
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
 
 <a id="types-aiobotocore-ivs"></a>
 
 # types-aiobotocore-ivs
 
 [![PyPI - types-aiobotocore-ivs](https://img.shields.io/pypi/v/types-aiobotocore-ivs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ivs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ivs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ivs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ivs)](https://pepy.tech/project/types-aiobotocore-ivs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IVS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
+[aiobotocore.IVS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
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
 [types-aiobotocore-ivs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ivs-2.9.0/types_aiobotocore_ivs.egg-info/SOURCES.txt` & `types-aiobotocore-ivs-2.9.1/types_aiobotocore_ivs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

