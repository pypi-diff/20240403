# Comparing `tmp/types-aiobotocore-drs-2.9.0.tar.gz` & `tmp/types-aiobotocore-drs-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-drs-2.9.0.tar", last modified: Wed Dec 13 19:59:08 2023, max compression
+gzip compressed data, was "types-aiobotocore-drs-2.9.1.tar", last modified: Thu Jan 18 01:20:33 2024, max compression
```

## Comparing `types-aiobotocore-drs-2.9.0.tar` & `types-aiobotocore-drs-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:08.697816 types-aiobotocore-drs-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:44:23.000000 types-aiobotocore-drs-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14599 2023-12-13 19:59:08.697816 types-aiobotocore-drs-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13052 2023-12-13 19:44:23.000000 types-aiobotocore-drs-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:08.697816 types-aiobotocore-drs-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-12-13 19:44:23.000000 types-aiobotocore-drs-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:08.693816 types-aiobotocore-drs-2.9.0/types_aiobotocore_drs/
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2023-12-13 19:44:23.000000 types-aiobotocore-drs-2.9.0/types_aiobotocore_drs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2023-12-13 19:44:23.000000 types-aiobotocore-drs-2.9.0/types_aiobotocore_drs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-13 19:44:23.000000 types-aiobotocore-drs-2.9.0/types_aiobotocore_drs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44865 2023-12-13 19:44:23.000000 types-aiobotocore-drs-2.9.0/types_aiobotocore_drs/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    44861 2023-12-13 19:44:23.000000 types-aiobotocore-drs-2.9.0/types_aiobotocore_drs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18301 2023-12-13 19:44:25.000000 types-aiobotocore-drs-2.9.0/types_aiobotocore_drs/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    18299 2023-12-13 19:44:25.000000 types-aiobotocore-drs-2.9.0/types_aiobotocore_drs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14761 2023-12-13 19:44:23.000000 types-aiobotocore-drs-2.9.0/types_aiobotocore_drs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    14748 2023-12-13 19:44:23.000000 types-aiobotocore-drs-2.9.0/types_aiobotocore_drs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:44:23.000000 types-aiobotocore-drs-2.9.0/types_aiobotocore_drs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    56469 2023-12-13 19:44:26.000000 types-aiobotocore-drs-2.9.0/types_aiobotocore_drs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    56468 2023-12-13 19:44:25.000000 types-aiobotocore-drs-2.9.0/types_aiobotocore_drs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:44:23.000000 types-aiobotocore-drs-2.9.0/types_aiobotocore_drs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:08.697816 types-aiobotocore-drs-2.9.0/types_aiobotocore_drs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14599 2023-12-13 19:59:08.000000 types-aiobotocore-drs-2.9.0/types_aiobotocore_drs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      737 2023-12-13 19:59:08.000000 types-aiobotocore-drs-2.9.0/types_aiobotocore_drs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:08.000000 types-aiobotocore-drs-2.9.0/types_aiobotocore_drs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:08.000000 types-aiobotocore-drs-2.9.0/types_aiobotocore_drs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:08.000000 types-aiobotocore-drs-2.9.0/types_aiobotocore_drs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 19:59:08.000000 types-aiobotocore-drs-2.9.0/types_aiobotocore_drs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:33.949375 types-aiobotocore-drs-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:06:18.000000 types-aiobotocore-drs-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14619 2024-01-18 01:20:33.949375 types-aiobotocore-drs-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13052 2024-01-18 01:06:18.000000 types-aiobotocore-drs-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:33.949375 types-aiobotocore-drs-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-01-18 01:06:18.000000 types-aiobotocore-drs-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:33.945375 types-aiobotocore-drs-2.9.1/types_aiobotocore_drs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-01-18 01:06:18.000000 types-aiobotocore-drs-2.9.1/types_aiobotocore_drs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-01-18 01:06:18.000000 types-aiobotocore-drs-2.9.1/types_aiobotocore_drs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-18 01:06:18.000000 types-aiobotocore-drs-2.9.1/types_aiobotocore_drs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44882 2024-01-18 01:06:18.000000 types-aiobotocore-drs-2.9.1/types_aiobotocore_drs/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44879 2024-01-18 01:06:18.000000 types-aiobotocore-drs-2.9.1/types_aiobotocore_drs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18299 2024-01-18 01:06:19.000000 types-aiobotocore-drs-2.9.1/types_aiobotocore_drs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18299 2024-01-18 01:06:19.000000 types-aiobotocore-drs-2.9.1/types_aiobotocore_drs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14768 2024-01-18 01:06:18.000000 types-aiobotocore-drs-2.9.1/types_aiobotocore_drs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14756 2024-01-18 01:06:18.000000 types-aiobotocore-drs-2.9.1/types_aiobotocore_drs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:06:18.000000 types-aiobotocore-drs-2.9.1/types_aiobotocore_drs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    56468 2024-01-18 01:06:21.000000 types-aiobotocore-drs-2.9.1/types_aiobotocore_drs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56468 2024-01-18 01:06:20.000000 types-aiobotocore-drs-2.9.1/types_aiobotocore_drs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:06:18.000000 types-aiobotocore-drs-2.9.1/types_aiobotocore_drs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:33.949375 types-aiobotocore-drs-2.9.1/types_aiobotocore_drs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14619 2024-01-18 01:20:33.000000 types-aiobotocore-drs-2.9.1/types_aiobotocore_drs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-01-18 01:20:33.000000 types-aiobotocore-drs-2.9.1/types_aiobotocore_drs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:33.000000 types-aiobotocore-drs-2.9.1/types_aiobotocore_drs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:33.000000 types-aiobotocore-drs-2.9.1/types_aiobotocore_drs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:33.000000 types-aiobotocore-drs-2.9.1/types_aiobotocore_drs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:20:33.000000 types-aiobotocore-drs-2.9.1/types_aiobotocore_drs.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-drs-2.9.0/LICENSE` & `types-aiobotocore-drs-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-drs-2.9.0/PKG-INFO` & `types-aiobotocore-drs-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-drs
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.drs 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.drs 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/
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
 
 <a id="types-aiobotocore-drs"></a>
 
 # types-aiobotocore-drs
 
 [![PyPI - types-aiobotocore-drs](https://img.shields.io/pypi/v/types-aiobotocore-drs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-drs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-drs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-drs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-drs)](https://pepy.tech/project/types-aiobotocore-drs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.drs 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
+[aiobotocore.drs 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
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
 [types-aiobotocore-drs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-drs-2.9.0/README.md` & `types-aiobotocore-drs-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-drs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-drs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-drs)](https://pepy.tech/project/types-aiobotocore-drs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.drs 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
+[aiobotocore.drs 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
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
 [types-aiobotocore-drs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-drs-2.9.0/setup.py` & `types-aiobotocore-drs-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-drs",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_drs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.drs 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.drs 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore drs type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_drs": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-drs-2.9.0/types_aiobotocore_drs/__init__.py` & `types-aiobotocore-drs-2.9.1/types_aiobotocore_drs/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,14 @@
     ListExtensibleSourceServersPaginator,
     ListLaunchActionsPaginator,
     ListStagingAccountsPaginator,
 )
 
 Client = drsClient
 
-
 __all__ = (
     "Client",
     "DescribeJobLogItemsPaginator",
     "DescribeJobsPaginator",
     "DescribeLaunchConfigurationTemplatesPaginator",
     "DescribeRecoveryInstancesPaginator",
     "DescribeRecoverySnapshotsPaginator",
```

### Comparing `types-aiobotocore-drs-2.9.0/types_aiobotocore_drs/__init__.pyi` & `types-aiobotocore-drs-2.9.1/types_aiobotocore_drs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.9.0/types_aiobotocore_drs/__main__.py` & `types-aiobotocore-drs-2.9.1/types_aiobotocore_drs/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.drs 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.drs 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs\nOther"
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

### Comparing `types-aiobotocore-drs-2.9.0/types_aiobotocore_drs/client.py` & `types-aiobotocore-drs-2.9.1/types_aiobotocore_drs/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("drsClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -186,15 +185,15 @@
         copyTags: bool = ...,
         exportBucketArn: str = ...,
         launchDisposition: LaunchDispositionType = ...,
         launchIntoSourceInstance: bool = ...,
         licensing: LicensingTypeDef = ...,
         postLaunchEnabled: bool = ...,
         tags: Mapping[str, str] = ...,
-        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
+        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...,
     ) -> CreateLaunchConfigurationTemplateResponseTypeDef:
         """
         Creates a new Launch Configuration Template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.create_launch_configuration_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#create_launch_configuration_template)
         """
@@ -212,15 +211,15 @@
         replicationServerInstanceType: str,
         replicationServersSecurityGroupsIDs: Sequence[str],
         stagingAreaSubnetId: str,
         stagingAreaTags: Mapping[str, str],
         useDedicatedReplicationServer: bool,
         autoReplicateNewDisks: bool = ...,
         ebsEncryptionKeyArn: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> ReplicationConfigurationTemplateResponseTypeDef:
         """
         Creates a new ReplicationConfigurationTemplate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.create_replication_configuration_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#create_replication_configuration_template)
         """
@@ -309,29 +308,29 @@
         """
 
     async def describe_jobs(
         self,
         *,
         filters: DescribeJobsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeJobsResponseTypeDef:
         """
         Returns a list of Jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.describe_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#describe_jobs)
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
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/drs-2020-02-26/DescribeLaunchConfigurationTemplates).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.describe_launch_configuration_templates)
@@ -339,15 +338,15 @@
         """
 
     async def describe_recovery_instances(
         self,
         *,
         filters: DescribeRecoveryInstancesRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeRecoveryInstancesResponseTypeDef:
         """
         Lists all Recovery Instances or multiple Recovery Instances by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.describe_recovery_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#describe_recovery_instances)
         """
@@ -355,57 +354,57 @@
     async def describe_recovery_snapshots(
         self,
         *,
         sourceServerID: str,
         filters: DescribeRecoverySnapshotsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        order: RecoverySnapshotsOrderType = ...
+        order: RecoverySnapshotsOrderType = ...,
     ) -> DescribeRecoverySnapshotsResponseTypeDef:
         """
         Lists all Recovery Snapshots for a single Source Server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.describe_recovery_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#describe_recovery_snapshots)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.describe_replication_configuration_templates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#describe_replication_configuration_templates)
         """
 
     async def describe_source_networks(
         self,
         *,
         filters: DescribeSourceNetworksRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeSourceNetworksResponseTypeDef:
         """
         Lists all Source Networks or multiple Source Networks filtered by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.describe_source_networks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#describe_source_networks)
         """
 
     async def describe_source_servers(
         self,
         *,
         filters: DescribeSourceServersRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeSourceServersResponseTypeDef:
         """
         Lists all Source Servers or multiple Source Servers filtered by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.describe_source_servers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#describe_source_servers)
         """
@@ -502,15 +501,15 @@
 
     async def list_launch_actions(
         self,
         *,
         resourceId: str,
         filters: LaunchActionsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListLaunchActionsResponseTypeDef:
         """
         Lists resource launch actions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.list_launch_actions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#list_launch_actions)
         """
@@ -544,15 +543,15 @@
         active: bool,
         category: LaunchActionCategoryType,
         description: str,
         name: str,
         optional: bool,
         order: int,
         resourceId: str,
-        parameters: Mapping[str, LaunchActionParameterTypeDef] = ...
+        parameters: Mapping[str, LaunchActionParameterTypeDef] = ...,
     ) -> PutLaunchActionResponseTypeDef:
         """
         Puts a resource launch action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.put_launch_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#put_launch_action)
         """
@@ -590,15 +589,15 @@
         """
 
     async def start_recovery(
         self,
         *,
         sourceServers: Sequence[StartRecoveryRequestSourceServerTypeDef],
         isDrill: bool = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> StartRecoveryResponseTypeDef:
         """
         Launches Recovery Instances for the specified Source Servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.start_recovery)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#start_recovery)
         """
@@ -612,15 +611,15 @@
         """
 
     async def start_source_network_recovery(
         self,
         *,
         sourceNetworks: Sequence[StartSourceNetworkRecoveryRequestNetworkEntryTypeDef],
         deployAsNew: bool = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> StartSourceNetworkRecoveryResponseTypeDef:
         """
         Deploy VPC for the specified Source Network and modify launch templates to use
         this
         network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.start_source_network_recovery)
@@ -702,15 +701,15 @@
 
     async def update_failback_replication_configuration(
         self,
         *,
         recoveryInstanceID: str,
         bandwidthThrottling: int = ...,
         name: str = ...,
-        usePrivateIP: bool = ...
+        usePrivateIP: bool = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Allows you to update the failback replication configuration of a Recovery
         Instance by
         ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.update_failback_replication_configuration)
@@ -724,15 +723,15 @@
         copyPrivateIp: bool = ...,
         copyTags: bool = ...,
         launchDisposition: LaunchDispositionType = ...,
         launchIntoInstanceProperties: LaunchIntoInstancePropertiesTypeDef = ...,
         licensing: LicensingTypeDef = ...,
         name: str = ...,
         postLaunchEnabled: bool = ...,
-        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
+        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...,
     ) -> LaunchConfigurationTypeDef:
         """
         Updates a LaunchConfiguration by Source Server ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.update_launch_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#update_launch_configuration)
         """
@@ -744,15 +743,15 @@
         copyPrivateIp: bool = ...,
         copyTags: bool = ...,
         exportBucketArn: str = ...,
         launchDisposition: LaunchDispositionType = ...,
         launchIntoSourceInstance: bool = ...,
         licensing: LicensingTypeDef = ...,
         postLaunchEnabled: bool = ...,
-        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
+        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...,
     ) -> UpdateLaunchConfigurationTemplateResponseTypeDef:
         """
         Updates an existing Launch Configuration Template by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.update_launch_configuration_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#update_launch_configuration_template)
         """
@@ -772,15 +771,15 @@
         name: str = ...,
         pitPolicy: Sequence[PITPolicyRuleTypeDef] = ...,
         replicatedDisks: Sequence[ReplicationConfigurationReplicatedDiskTypeDef] = ...,
         replicationServerInstanceType: str = ...,
         replicationServersSecurityGroupsIDs: Sequence[str] = ...,
         stagingAreaSubnetId: str = ...,
         stagingAreaTags: Mapping[str, str] = ...,
-        useDedicatedReplicationServer: bool = ...
+        useDedicatedReplicationServer: bool = ...,
     ) -> ReplicationConfigurationTypeDef:
         """
         Allows you to update a ReplicationConfiguration by Source Server ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.update_replication_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#update_replication_configuration)
         """
@@ -799,15 +798,15 @@
         ebsEncryption: ReplicationConfigurationEbsEncryptionType = ...,
         ebsEncryptionKeyArn: str = ...,
         pitPolicy: Sequence[PITPolicyRuleTypeDef] = ...,
         replicationServerInstanceType: str = ...,
         replicationServersSecurityGroupsIDs: Sequence[str] = ...,
         stagingAreaSubnetId: str = ...,
         stagingAreaTags: Mapping[str, str] = ...,
-        useDedicatedReplicationServer: bool = ...
+        useDedicatedReplicationServer: bool = ...,
     ) -> ReplicationConfigurationTemplateResponseTypeDef:
         """
         Updates a ReplicationConfigurationTemplate by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.update_replication_configuration_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#update_replication_configuration_template)
         """
```

### Comparing `types-aiobotocore-drs-2.9.0/types_aiobotocore_drs/client.pyi` & `types-aiobotocore-drs-2.9.1/types_aiobotocore_drs/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
         copyTags: bool = ...,
         exportBucketArn: str = ...,
         launchDisposition: LaunchDispositionType = ...,
         launchIntoSourceInstance: bool = ...,
         licensing: LicensingTypeDef = ...,
         postLaunchEnabled: bool = ...,
         tags: Mapping[str, str] = ...,
-        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
+        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...,
     ) -> CreateLaunchConfigurationTemplateResponseTypeDef:
         """
         Creates a new Launch Configuration Template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.create_launch_configuration_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#create_launch_configuration_template)
         """
@@ -208,15 +208,15 @@
         replicationServerInstanceType: str,
         replicationServersSecurityGroupsIDs: Sequence[str],
         stagingAreaSubnetId: str,
         stagingAreaTags: Mapping[str, str],
         useDedicatedReplicationServer: bool,
         autoReplicateNewDisks: bool = ...,
         ebsEncryptionKeyArn: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> ReplicationConfigurationTemplateResponseTypeDef:
         """
         Creates a new ReplicationConfigurationTemplate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.create_replication_configuration_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#create_replication_configuration_template)
         """
@@ -305,29 +305,29 @@
         """
 
     async def describe_jobs(
         self,
         *,
         filters: DescribeJobsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeJobsResponseTypeDef:
         """
         Returns a list of Jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.describe_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#describe_jobs)
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
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/drs-2020-02-26/DescribeLaunchConfigurationTemplates).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.describe_launch_configuration_templates)
@@ -335,15 +335,15 @@
         """
 
     async def describe_recovery_instances(
         self,
         *,
         filters: DescribeRecoveryInstancesRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeRecoveryInstancesResponseTypeDef:
         """
         Lists all Recovery Instances or multiple Recovery Instances by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.describe_recovery_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#describe_recovery_instances)
         """
@@ -351,57 +351,57 @@
     async def describe_recovery_snapshots(
         self,
         *,
         sourceServerID: str,
         filters: DescribeRecoverySnapshotsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        order: RecoverySnapshotsOrderType = ...
+        order: RecoverySnapshotsOrderType = ...,
     ) -> DescribeRecoverySnapshotsResponseTypeDef:
         """
         Lists all Recovery Snapshots for a single Source Server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.describe_recovery_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#describe_recovery_snapshots)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.describe_replication_configuration_templates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#describe_replication_configuration_templates)
         """
 
     async def describe_source_networks(
         self,
         *,
         filters: DescribeSourceNetworksRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeSourceNetworksResponseTypeDef:
         """
         Lists all Source Networks or multiple Source Networks filtered by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.describe_source_networks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#describe_source_networks)
         """
 
     async def describe_source_servers(
         self,
         *,
         filters: DescribeSourceServersRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeSourceServersResponseTypeDef:
         """
         Lists all Source Servers or multiple Source Servers filtered by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.describe_source_servers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#describe_source_servers)
         """
@@ -498,15 +498,15 @@
 
     async def list_launch_actions(
         self,
         *,
         resourceId: str,
         filters: LaunchActionsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListLaunchActionsResponseTypeDef:
         """
         Lists resource launch actions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.list_launch_actions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#list_launch_actions)
         """
@@ -540,15 +540,15 @@
         active: bool,
         category: LaunchActionCategoryType,
         description: str,
         name: str,
         optional: bool,
         order: int,
         resourceId: str,
-        parameters: Mapping[str, LaunchActionParameterTypeDef] = ...
+        parameters: Mapping[str, LaunchActionParameterTypeDef] = ...,
     ) -> PutLaunchActionResponseTypeDef:
         """
         Puts a resource launch action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.put_launch_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#put_launch_action)
         """
@@ -586,15 +586,15 @@
         """
 
     async def start_recovery(
         self,
         *,
         sourceServers: Sequence[StartRecoveryRequestSourceServerTypeDef],
         isDrill: bool = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> StartRecoveryResponseTypeDef:
         """
         Launches Recovery Instances for the specified Source Servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.start_recovery)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#start_recovery)
         """
@@ -608,15 +608,15 @@
         """
 
     async def start_source_network_recovery(
         self,
         *,
         sourceNetworks: Sequence[StartSourceNetworkRecoveryRequestNetworkEntryTypeDef],
         deployAsNew: bool = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> StartSourceNetworkRecoveryResponseTypeDef:
         """
         Deploy VPC for the specified Source Network and modify launch templates to use
         this
         network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.start_source_network_recovery)
@@ -698,15 +698,15 @@
 
     async def update_failback_replication_configuration(
         self,
         *,
         recoveryInstanceID: str,
         bandwidthThrottling: int = ...,
         name: str = ...,
-        usePrivateIP: bool = ...
+        usePrivateIP: bool = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Allows you to update the failback replication configuration of a Recovery
         Instance by
         ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.update_failback_replication_configuration)
@@ -720,15 +720,15 @@
         copyPrivateIp: bool = ...,
         copyTags: bool = ...,
         launchDisposition: LaunchDispositionType = ...,
         launchIntoInstanceProperties: LaunchIntoInstancePropertiesTypeDef = ...,
         licensing: LicensingTypeDef = ...,
         name: str = ...,
         postLaunchEnabled: bool = ...,
-        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
+        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...,
     ) -> LaunchConfigurationTypeDef:
         """
         Updates a LaunchConfiguration by Source Server ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.update_launch_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#update_launch_configuration)
         """
@@ -740,15 +740,15 @@
         copyPrivateIp: bool = ...,
         copyTags: bool = ...,
         exportBucketArn: str = ...,
         launchDisposition: LaunchDispositionType = ...,
         launchIntoSourceInstance: bool = ...,
         licensing: LicensingTypeDef = ...,
         postLaunchEnabled: bool = ...,
-        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
+        targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...,
     ) -> UpdateLaunchConfigurationTemplateResponseTypeDef:
         """
         Updates an existing Launch Configuration Template by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.update_launch_configuration_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#update_launch_configuration_template)
         """
@@ -768,15 +768,15 @@
         name: str = ...,
         pitPolicy: Sequence[PITPolicyRuleTypeDef] = ...,
         replicatedDisks: Sequence[ReplicationConfigurationReplicatedDiskTypeDef] = ...,
         replicationServerInstanceType: str = ...,
         replicationServersSecurityGroupsIDs: Sequence[str] = ...,
         stagingAreaSubnetId: str = ...,
         stagingAreaTags: Mapping[str, str] = ...,
-        useDedicatedReplicationServer: bool = ...
+        useDedicatedReplicationServer: bool = ...,
     ) -> ReplicationConfigurationTypeDef:
         """
         Allows you to update a ReplicationConfiguration by Source Server ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.update_replication_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#update_replication_configuration)
         """
@@ -795,15 +795,15 @@
         ebsEncryption: ReplicationConfigurationEbsEncryptionType = ...,
         ebsEncryptionKeyArn: str = ...,
         pitPolicy: Sequence[PITPolicyRuleTypeDef] = ...,
         replicationServerInstanceType: str = ...,
         replicationServersSecurityGroupsIDs: Sequence[str] = ...,
         stagingAreaSubnetId: str = ...,
         stagingAreaTags: Mapping[str, str] = ...,
-        useDedicatedReplicationServer: bool = ...
+        useDedicatedReplicationServer: bool = ...,
     ) -> ReplicationConfigurationTemplateResponseTypeDef:
         """
         Updates a ReplicationConfigurationTemplate by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.update_replication_configuration_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#update_replication_configuration_template)
         """
```

### Comparing `types-aiobotocore-drs-2.9.0/types_aiobotocore_drs/literals.py` & `types-aiobotocore-drs-2.9.1/types_aiobotocore_drs/literals.py`

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
     "DataReplicationErrorStringType",
     "DataReplicationInitiationStepNameType",
     "DataReplicationInitiationStepStatusType",
     "DataReplicationStateType",
     "DescribeJobLogItemsPaginatorName",
     "DescribeJobsPaginatorName",
@@ -70,15 +69,14 @@
     "drsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DataReplicationErrorStringType = Literal[
     "AGENT_NOT_SEEN",
     "FAILED_TO_ATTACH_STAGING_DISKS",
     "FAILED_TO_AUTHENTICATE_WITH_SERVICE",
     "FAILED_TO_BOOT_REPLICATION_SERVER",
     "FAILED_TO_CONNECT_AGENT_TO_REPLICATION_SERVER",
     "FAILED_TO_CREATE_SECURITY_GROUP",
```

### Comparing `types-aiobotocore-drs-2.9.0/types_aiobotocore_drs/literals.pyi` & `types-aiobotocore-drs-2.9.1/types_aiobotocore_drs/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.9.0/types_aiobotocore_drs/paginator.py` & `types-aiobotocore-drs-2.9.1/types_aiobotocore_drs/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,14 @@
     "DescribeSourceNetworksPaginator",
     "DescribeSourceServersPaginator",
     "ListExtensibleSourceServersPaginator",
     "ListLaunchActionsPaginator",
     "ListStagingAccountsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -114,15 +113,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describejobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeJobsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describejobspaginator)
         """
 
 
@@ -132,15 +131,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describelaunchconfigurationtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         launchConfigurationTemplateIDs: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeLaunchConfigurationTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeLaunchConfigurationTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describelaunchconfigurationtemplatespaginator)
         """
 
 
@@ -150,15 +149,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describerecoveryinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeRecoveryInstancesRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRecoveryInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeRecoveryInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describerecoveryinstancespaginator)
         """
 
 
@@ -170,15 +169,15 @@
 
     def paginate(
         self,
         *,
         sourceServerID: str,
         filters: DescribeRecoverySnapshotsRequestFiltersTypeDef = ...,
         order: RecoverySnapshotsOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRecoverySnapshotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeRecoverySnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describerecoverysnapshotspaginator)
         """
 
 
@@ -188,15 +187,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describereplicationconfigurationtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         replicationConfigurationTemplateIDs: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeReplicationConfigurationTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeReplicationConfigurationTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describereplicationconfigurationtemplatespaginator)
         """
 
 
@@ -206,15 +205,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describesourcenetworkspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeSourceNetworksRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeSourceNetworksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeSourceNetworks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describesourcenetworkspaginator)
         """
 
 
@@ -224,15 +223,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describesourceserverspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeSourceServersRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeSourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeSourceServers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describesourceserverspaginator)
         """
 
 
@@ -258,15 +257,15 @@
     """
 
     def paginate(
         self,
         *,
         resourceId: str,
         filters: LaunchActionsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListLaunchActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.ListLaunchActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#listlaunchactionspaginator)
         """
```

### Comparing `types-aiobotocore-drs-2.9.0/types_aiobotocore_drs/paginator.pyi` & `types-aiobotocore-drs-2.9.1/types_aiobotocore_drs/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describejobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeJobsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describejobspaginator)
         """
 
 class DescribeLaunchConfigurationTemplatesPaginator(AioPaginator):
@@ -127,15 +127,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describelaunchconfigurationtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         launchConfigurationTemplateIDs: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeLaunchConfigurationTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeLaunchConfigurationTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describelaunchconfigurationtemplatespaginator)
         """
 
 class DescribeRecoveryInstancesPaginator(AioPaginator):
@@ -144,15 +144,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describerecoveryinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeRecoveryInstancesRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRecoveryInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeRecoveryInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describerecoveryinstancespaginator)
         """
 
 class DescribeRecoverySnapshotsPaginator(AioPaginator):
@@ -163,15 +163,15 @@
 
     def paginate(
         self,
         *,
         sourceServerID: str,
         filters: DescribeRecoverySnapshotsRequestFiltersTypeDef = ...,
         order: RecoverySnapshotsOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRecoverySnapshotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeRecoverySnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describerecoverysnapshotspaginator)
         """
 
 class DescribeReplicationConfigurationTemplatesPaginator(AioPaginator):
@@ -180,15 +180,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describereplicationconfigurationtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         replicationConfigurationTemplateIDs: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeReplicationConfigurationTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeReplicationConfigurationTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describereplicationconfigurationtemplatespaginator)
         """
 
 class DescribeSourceNetworksPaginator(AioPaginator):
@@ -197,15 +197,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describesourcenetworkspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeSourceNetworksRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeSourceNetworksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeSourceNetworks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describesourcenetworkspaginator)
         """
 
 class DescribeSourceServersPaginator(AioPaginator):
@@ -214,15 +214,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describesourceserverspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeSourceServersRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeSourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeSourceServers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describesourceserverspaginator)
         """
 
 class ListExtensibleSourceServersPaginator(AioPaginator):
@@ -246,15 +246,15 @@
     """
 
     def paginate(
         self,
         *,
         resourceId: str,
         filters: LaunchActionsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListLaunchActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.ListLaunchActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#listlaunchactionspaginator)
         """
 
 class ListStagingAccountsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-drs-2.9.0/types_aiobotocore_drs/type_defs.py` & `types-aiobotocore-drs-2.9.1/types_aiobotocore_drs/type_defs.py`

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
     "AccountTypeDef",
     "AssociateSourceNetworkStackRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CPUTypeDef",
     "ConversionPropertiesTypeDef",
     "CreateExtendedSourceServerRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-drs-2.9.0/types_aiobotocore_drs/type_defs.pyi` & `types-aiobotocore-drs-2.9.1/types_aiobotocore_drs/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.9.0/types_aiobotocore_drs.egg-info/PKG-INFO` & `types-aiobotocore-drs-2.9.1/types_aiobotocore_drs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-drs
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.drs 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.drs 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/
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
 
 <a id="types-aiobotocore-drs"></a>
 
 # types-aiobotocore-drs
 
 [![PyPI - types-aiobotocore-drs](https://img.shields.io/pypi/v/types-aiobotocore-drs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-drs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-drs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-drs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-drs)](https://pepy.tech/project/types-aiobotocore-drs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.drs 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
+[aiobotocore.drs 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
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
 [types-aiobotocore-drs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-drs-2.9.0/types_aiobotocore_drs.egg-info/SOURCES.txt` & `types-aiobotocore-drs-2.9.1/types_aiobotocore_drs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

