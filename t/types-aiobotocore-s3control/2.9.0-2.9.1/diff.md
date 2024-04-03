# Comparing `tmp/types-aiobotocore-s3control-2.9.0.tar.gz` & `tmp/types-aiobotocore-s3control-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-s3control-2.9.0.tar", last modified: Wed Dec 13 20:00:23 2023, max compression
+gzip compressed data, was "types-aiobotocore-s3control-2.9.1.tar", last modified: Thu Jan 18 01:21:42 2024, max compression
```

## Comparing `types-aiobotocore-s3control-2.9.0.tar` & `types-aiobotocore-s3control-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:23.037201 types-aiobotocore-s3control-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:55:13.000000 types-aiobotocore-s3control-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13190 2023-12-13 20:00:23.037201 types-aiobotocore-s3control-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11619 2023-12-13 19:55:13.000000 types-aiobotocore-s3control-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:23.037201 types-aiobotocore-s3control-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2023-12-13 19:55:13.000000 types-aiobotocore-s3control-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:23.037201 types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control/
--rw-r--r--   0 runner    (1001) docker     (127)      774 2023-12-13 19:55:13.000000 types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2023-12-13 19:55:13.000000 types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-12-13 19:55:13.000000 types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    60804 2023-12-13 19:55:14.000000 types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    60800 2023-12-13 19:55:13.000000 types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14485 2023-12-13 19:55:14.000000 types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14483 2023-12-13 19:55:14.000000 types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2023-12-13 19:55:14.000000 types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2023-12-13 19:55:14.000000 types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:55:13.000000 types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    80742 2023-12-13 19:55:15.000000 types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    80741 2023-12-13 19:55:14.000000 types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:55:13.000000 types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:23.037201 types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13190 2023-12-13 20:00:23.000000 types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-12-13 20:00:23.000000 types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:23.000000 types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:23.000000 types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:23.000000 types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-13 20:00:23.000000 types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:42.109065 types-aiobotocore-s3control-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:16:45.000000 types-aiobotocore-s3control-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13210 2024-01-18 01:21:42.109065 types-aiobotocore-s3control-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11619 2024-01-18 01:16:45.000000 types-aiobotocore-s3control-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:42.109065 types-aiobotocore-s3control-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-01-18 01:16:45.000000 types-aiobotocore-s3control-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:42.105065 types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-01-18 01:16:45.000000 types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-01-18 01:16:45.000000 types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-01-18 01:16:45.000000 types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60821 2024-01-18 01:16:46.000000 types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60818 2024-01-18 01:16:45.000000 types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14483 2024-01-18 01:16:46.000000 types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14483 2024-01-18 01:16:46.000000 types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-01-18 01:16:46.000000 types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-01-18 01:16:46.000000 types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:16:45.000000 types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    80741 2024-01-18 01:16:47.000000 types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80741 2024-01-18 01:16:47.000000 types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:16:45.000000 types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:42.109065 types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13210 2024-01-18 01:21:42.000000 types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-01-18 01:21:42.000000 types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:42.000000 types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:42.000000 types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:42.000000 types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-18 01:21:42.000000 types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-s3control-2.9.0/LICENSE` & `types-aiobotocore-s3control-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-s3control-2.9.0/PKG-INFO` & `types-aiobotocore-s3control-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-s3control
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.S3Control 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.S3Control 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/
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
 
 <a id="types-aiobotocore-s3control"></a>
 
 # types-aiobotocore-s3control
 
 [![PyPI - types-aiobotocore-s3control](https://img.shields.io/pypi/v/types-aiobotocore-s3control.svg?color=blue)](https://pypi.org/project/types-aiobotocore-s3control)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-s3control.svg?color=blue)](https://pypi.org/project/types-aiobotocore-s3control)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-s3control)](https://pepy.tech/project/types-aiobotocore-s3control)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.S3Control 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
+[aiobotocore.S3Control 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
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
 [types-aiobotocore-s3control docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-s3control-2.9.0/README.md` & `types-aiobotocore-s3control-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-s3control.svg?color=blue)](https://pypi.org/project/types-aiobotocore-s3control)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-s3control)](https://pepy.tech/project/types-aiobotocore-s3control)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.S3Control 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
+[aiobotocore.S3Control 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
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
 [types-aiobotocore-s3control docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-s3control-2.9.0/setup.py` & `types-aiobotocore-s3control-2.9.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-s3control",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_s3control"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.S3Control 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.S3Control 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore s3control type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_s3control": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control/__init__.py` & `types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,9 +22,8 @@
 """
 
 from .client import S3ControlClient
 from .paginator import ListAccessPointsForObjectLambdaPaginator
 
 Client = S3ControlClient
 
-
 __all__ = ("Client", "ListAccessPointsForObjectLambdaPaginator", "S3ControlClient")
```

### Comparing `types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control/__init__.pyi` & `types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control/__main__.py` & `types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.S3Control 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.S3Control 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control\nOther"
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

### Comparing `types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control/client.py` & `types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("S3ControlClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -196,15 +195,15 @@
         AccountId: str,
         AccessGrantsLocationId: str,
         Grantee: GranteeTypeDef,
         Permission: PermissionType,
         AccessGrantsLocationConfiguration: AccessGrantsLocationConfigurationTypeDef = ...,
         ApplicationArn: str = ...,
         S3PrefixType: Literal["Object"] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAccessGrantResultTypeDef:
         """
         Creates an access grant that gives a grantee access to your S3 data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_access_grant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#create_access_grant)
         """
@@ -223,15 +222,15 @@
 
     async def create_access_grants_location(
         self,
         *,
         AccountId: str,
         LocationScope: str,
         IAMRoleArn: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAccessGrantsLocationResultTypeDef:
         """
         The S3 data location that you would like to register in your S3 Access Grants
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_access_grants_location)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#create_access_grants_location)
@@ -241,15 +240,15 @@
         self,
         *,
         AccountId: str,
         Name: str,
         Bucket: str,
         VpcConfiguration: VpcConfigurationTypeDef = ...,
         PublicAccessBlockConfiguration: PublicAccessBlockConfigurationTypeDef = ...,
-        BucketAccountId: str = ...
+        BucketAccountId: str = ...,
     ) -> CreateAccessPointResultTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_access_point)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#create_access_point)
         """
@@ -272,15 +271,15 @@
         CreateBucketConfiguration: CreateBucketConfigurationTypeDef = ...,
         GrantFullControl: str = ...,
         GrantRead: str = ...,
         GrantReadACP: str = ...,
         GrantWrite: str = ...,
         GrantWriteACP: str = ...,
         ObjectLockEnabledForBucket: bool = ...,
-        OutpostId: str = ...
+        OutpostId: str = ...,
     ) -> CreateBucketResultTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#create_bucket)
         """
@@ -294,15 +293,15 @@
         ClientRequestToken: str,
         Priority: int,
         RoleArn: str,
         ConfirmationRequired: bool = ...,
         Manifest: JobManifestTypeDef = ...,
         Description: str = ...,
         Tags: Sequence[S3TagTypeDef] = ...,
-        ManifestGenerator: JobManifestGeneratorTypeDef = ...
+        ManifestGenerator: JobManifestGeneratorTypeDef = ...,
     ) -> CreateJobResultTypeDef:
         """
         This operation creates an S3 Batch Operations job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#create_job)
         """
@@ -318,15 +317,15 @@
         """
 
     async def create_storage_lens_group(
         self,
         *,
         AccountId: str,
         StorageLensGroup: StorageLensGroupTypeDef,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates a new S3 Storage Lens group and associates it with the specified Amazon
         Web Services account
         ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_storage_lens_group)
@@ -743,15 +742,15 @@
         self,
         *,
         AccountId: str,
         Target: str,
         Permission: PermissionType,
         DurationSeconds: int = ...,
         Privilege: PrivilegeType = ...,
-        TargetType: Literal["Object"] = ...
+        TargetType: Literal["Object"] = ...,
     ) -> GetDataAccessResultTypeDef:
         """
         Returns a temporary access credential from S3 Access Grants to the grantee or
         client
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_data_access)
@@ -850,15 +849,15 @@
         AccountId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         GranteeType: GranteeTypeType = ...,
         GranteeIdentifier: str = ...,
         Permission: PermissionType = ...,
         GrantScope: str = ...,
-        ApplicationArn: str = ...
+        ApplicationArn: str = ...,
     ) -> ListAccessGrantsResultTypeDef:
         """
         Returns the list of access grants in your S3 Access Grants instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_access_grants)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#list_access_grants)
         """
@@ -875,15 +874,15 @@
 
     async def list_access_grants_locations(
         self,
         *,
         AccountId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        LocationScope: str = ...
+        LocationScope: str = ...,
     ) -> ListAccessGrantsLocationsResultTypeDef:
         """
         Returns a list of the locations registered in your S3 Access Grants instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_access_grants_locations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#list_access_grants_locations)
         """
@@ -910,15 +909,15 @@
 
     async def list_jobs(
         self,
         *,
         AccountId: str,
         JobStatuses: Sequence[JobStatusType] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListJobsResultTypeDef:
         """
         Lists current S3 Batch Operations jobs as well as the jobs that have ended
         within the last 30 days for the Amazon Web Services account making the
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_jobs)
@@ -1018,15 +1017,15 @@
         """
 
     async def put_bucket_lifecycle_configuration(
         self,
         *,
         AccountId: str,
         Bucket: str,
-        LifecycleConfiguration: LifecycleConfigurationTypeDef = ...
+        LifecycleConfiguration: LifecycleConfigurationTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_bucket_lifecycle_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_bucket_lifecycle_configuration)
         """
@@ -1042,15 +1041,15 @@
         """
 
     async def put_bucket_replication(
         self,
         *,
         AccountId: str,
         Bucket: str,
-        ReplicationConfiguration: ReplicationConfigurationTypeDef
+        ReplicationConfiguration: ReplicationConfigurationTypeDef,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_bucket_replication)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_bucket_replication)
         """
@@ -1067,15 +1066,15 @@
 
     async def put_bucket_versioning(
         self,
         *,
         AccountId: str,
         Bucket: str,
         VersioningConfiguration: VersioningConfigurationTypeDef,
-        MFA: str = ...
+        MFA: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_bucket_versioning)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_bucket_versioning)
         """
@@ -1091,43 +1090,43 @@
         """
 
     async def put_multi_region_access_point_policy(
         self,
         *,
         AccountId: str,
         ClientToken: str,
-        Details: PutMultiRegionAccessPointPolicyInputTypeDef
+        Details: PutMultiRegionAccessPointPolicyInputTypeDef,
     ) -> PutMultiRegionAccessPointPolicyResultTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_multi_region_access_point_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_multi_region_access_point_policy)
         """
 
     async def put_public_access_block(
         self,
         *,
         PublicAccessBlockConfiguration: PublicAccessBlockConfigurationTypeDef,
-        AccountId: str
+        AccountId: str,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_public_access_block)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_public_access_block)
         """
 
     async def put_storage_lens_configuration(
         self,
         *,
         ConfigId: str,
         AccountId: str,
         StorageLensConfiguration: StorageLensConfigurationTypeDef,
-        Tags: Sequence[StorageLensTagTypeDef] = ...
+        Tags: Sequence[StorageLensTagTypeDef] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_storage_lens_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_storage_lens_configuration)
         """
@@ -1143,15 +1142,15 @@
         """
 
     async def submit_multi_region_access_point_routes(
         self,
         *,
         AccountId: str,
         Mrap: str,
-        RouteUpdates: Sequence[MultiRegionAccessPointRouteTypeDef]
+        RouteUpdates: Sequence[MultiRegionAccessPointRouteTypeDef],
     ) -> Dict[str, Any]:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.submit_multi_region_access_point_routes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#submit_multi_region_access_point_routes)
         """
@@ -1201,15 +1200,15 @@
 
     async def update_job_status(
         self,
         *,
         AccountId: str,
         JobId: str,
         RequestedJobStatus: RequestedJobStatusType,
-        StatusUpdateReason: str = ...
+        StatusUpdateReason: str = ...,
     ) -> UpdateJobStatusResultTypeDef:
         """
         Updates the status for the specified job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.update_job_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#update_job_status)
         """
```

### Comparing `types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control/client.pyi` & `types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
         AccountId: str,
         AccessGrantsLocationId: str,
         Grantee: GranteeTypeDef,
         Permission: PermissionType,
         AccessGrantsLocationConfiguration: AccessGrantsLocationConfigurationTypeDef = ...,
         ApplicationArn: str = ...,
         S3PrefixType: Literal["Object"] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAccessGrantResultTypeDef:
         """
         Creates an access grant that gives a grantee access to your S3 data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_access_grant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#create_access_grant)
         """
@@ -219,15 +219,15 @@
 
     async def create_access_grants_location(
         self,
         *,
         AccountId: str,
         LocationScope: str,
         IAMRoleArn: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAccessGrantsLocationResultTypeDef:
         """
         The S3 data location that you would like to register in your S3 Access Grants
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_access_grants_location)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#create_access_grants_location)
@@ -237,15 +237,15 @@
         self,
         *,
         AccountId: str,
         Name: str,
         Bucket: str,
         VpcConfiguration: VpcConfigurationTypeDef = ...,
         PublicAccessBlockConfiguration: PublicAccessBlockConfigurationTypeDef = ...,
-        BucketAccountId: str = ...
+        BucketAccountId: str = ...,
     ) -> CreateAccessPointResultTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_access_point)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#create_access_point)
         """
@@ -268,15 +268,15 @@
         CreateBucketConfiguration: CreateBucketConfigurationTypeDef = ...,
         GrantFullControl: str = ...,
         GrantRead: str = ...,
         GrantReadACP: str = ...,
         GrantWrite: str = ...,
         GrantWriteACP: str = ...,
         ObjectLockEnabledForBucket: bool = ...,
-        OutpostId: str = ...
+        OutpostId: str = ...,
     ) -> CreateBucketResultTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#create_bucket)
         """
@@ -290,15 +290,15 @@
         ClientRequestToken: str,
         Priority: int,
         RoleArn: str,
         ConfirmationRequired: bool = ...,
         Manifest: JobManifestTypeDef = ...,
         Description: str = ...,
         Tags: Sequence[S3TagTypeDef] = ...,
-        ManifestGenerator: JobManifestGeneratorTypeDef = ...
+        ManifestGenerator: JobManifestGeneratorTypeDef = ...,
     ) -> CreateJobResultTypeDef:
         """
         This operation creates an S3 Batch Operations job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#create_job)
         """
@@ -314,15 +314,15 @@
         """
 
     async def create_storage_lens_group(
         self,
         *,
         AccountId: str,
         StorageLensGroup: StorageLensGroupTypeDef,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates a new S3 Storage Lens group and associates it with the specified Amazon
         Web Services account
         ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_storage_lens_group)
@@ -739,15 +739,15 @@
         self,
         *,
         AccountId: str,
         Target: str,
         Permission: PermissionType,
         DurationSeconds: int = ...,
         Privilege: PrivilegeType = ...,
-        TargetType: Literal["Object"] = ...
+        TargetType: Literal["Object"] = ...,
     ) -> GetDataAccessResultTypeDef:
         """
         Returns a temporary access credential from S3 Access Grants to the grantee or
         client
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_data_access)
@@ -846,15 +846,15 @@
         AccountId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         GranteeType: GranteeTypeType = ...,
         GranteeIdentifier: str = ...,
         Permission: PermissionType = ...,
         GrantScope: str = ...,
-        ApplicationArn: str = ...
+        ApplicationArn: str = ...,
     ) -> ListAccessGrantsResultTypeDef:
         """
         Returns the list of access grants in your S3 Access Grants instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_access_grants)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#list_access_grants)
         """
@@ -871,15 +871,15 @@
 
     async def list_access_grants_locations(
         self,
         *,
         AccountId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        LocationScope: str = ...
+        LocationScope: str = ...,
     ) -> ListAccessGrantsLocationsResultTypeDef:
         """
         Returns a list of the locations registered in your S3 Access Grants instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_access_grants_locations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#list_access_grants_locations)
         """
@@ -906,15 +906,15 @@
 
     async def list_jobs(
         self,
         *,
         AccountId: str,
         JobStatuses: Sequence[JobStatusType] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListJobsResultTypeDef:
         """
         Lists current S3 Batch Operations jobs as well as the jobs that have ended
         within the last 30 days for the Amazon Web Services account making the
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_jobs)
@@ -1014,15 +1014,15 @@
         """
 
     async def put_bucket_lifecycle_configuration(
         self,
         *,
         AccountId: str,
         Bucket: str,
-        LifecycleConfiguration: LifecycleConfigurationTypeDef = ...
+        LifecycleConfiguration: LifecycleConfigurationTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_bucket_lifecycle_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_bucket_lifecycle_configuration)
         """
@@ -1038,15 +1038,15 @@
         """
 
     async def put_bucket_replication(
         self,
         *,
         AccountId: str,
         Bucket: str,
-        ReplicationConfiguration: ReplicationConfigurationTypeDef
+        ReplicationConfiguration: ReplicationConfigurationTypeDef,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_bucket_replication)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_bucket_replication)
         """
@@ -1063,15 +1063,15 @@
 
     async def put_bucket_versioning(
         self,
         *,
         AccountId: str,
         Bucket: str,
         VersioningConfiguration: VersioningConfigurationTypeDef,
-        MFA: str = ...
+        MFA: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_bucket_versioning)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_bucket_versioning)
         """
@@ -1087,43 +1087,43 @@
         """
 
     async def put_multi_region_access_point_policy(
         self,
         *,
         AccountId: str,
         ClientToken: str,
-        Details: PutMultiRegionAccessPointPolicyInputTypeDef
+        Details: PutMultiRegionAccessPointPolicyInputTypeDef,
     ) -> PutMultiRegionAccessPointPolicyResultTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_multi_region_access_point_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_multi_region_access_point_policy)
         """
 
     async def put_public_access_block(
         self,
         *,
         PublicAccessBlockConfiguration: PublicAccessBlockConfigurationTypeDef,
-        AccountId: str
+        AccountId: str,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_public_access_block)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_public_access_block)
         """
 
     async def put_storage_lens_configuration(
         self,
         *,
         ConfigId: str,
         AccountId: str,
         StorageLensConfiguration: StorageLensConfigurationTypeDef,
-        Tags: Sequence[StorageLensTagTypeDef] = ...
+        Tags: Sequence[StorageLensTagTypeDef] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_storage_lens_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_storage_lens_configuration)
         """
@@ -1139,15 +1139,15 @@
         """
 
     async def submit_multi_region_access_point_routes(
         self,
         *,
         AccountId: str,
         Mrap: str,
-        RouteUpdates: Sequence[MultiRegionAccessPointRouteTypeDef]
+        RouteUpdates: Sequence[MultiRegionAccessPointRouteTypeDef],
     ) -> Dict[str, Any]:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.submit_multi_region_access_point_routes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#submit_multi_region_access_point_routes)
         """
@@ -1197,15 +1197,15 @@
 
     async def update_job_status(
         self,
         *,
         AccountId: str,
         JobId: str,
         RequestedJobStatus: RequestedJobStatusType,
-        StatusUpdateReason: str = ...
+        StatusUpdateReason: str = ...,
     ) -> UpdateJobStatusResultTypeDef:
         """
         Updates the status for the specified job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.update_job_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#update_job_status)
         """
```

### Comparing `types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control/literals.py` & `types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control/literals.py`

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
     "AsyncOperationNameType",
     "BucketCannedACLType",
     "BucketLocationConstraintType",
     "BucketVersioningStatusType",
     "DeleteMarkerReplicationStatusType",
     "ExistingObjectReplicationStatusType",
@@ -73,15 +72,14 @@
     "S3ControlServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AsyncOperationNameType = Literal[
     "CreateMultiRegionAccessPoint",
     "DeleteMultiRegionAccessPoint",
     "PutMultiRegionAccessPointPolicy",
 ]
 BucketCannedACLType = Literal["authenticated-read", "private", "public-read", "public-read-write"]
 BucketLocationConstraintType = Literal[
```

### Comparing `types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control/literals.pyi` & `types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control/paginator.py` & `types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import ListAccessPointsForObjectLambdaResultTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListAccessPointsForObjectLambdaPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control/paginator.pyi` & `types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control/type_defs.py` & `types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AbortIncompleteMultipartUploadTypeDef",
     "AccessControlTranslationTypeDef",
     "AccessGrantsLocationConfigurationTypeDef",
     "VpcConfigurationTypeDef",
     "ActivityMetricsTypeDef",
     "AdvancedCostOptimizationMetricsTypeDef",
```

### Comparing `types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control/type_defs.pyi` & `types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control.egg-info/PKG-INFO` & `types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-s3control
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.S3Control 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.S3Control 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/
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
 
 <a id="types-aiobotocore-s3control"></a>
 
 # types-aiobotocore-s3control
 
 [![PyPI - types-aiobotocore-s3control](https://img.shields.io/pypi/v/types-aiobotocore-s3control.svg?color=blue)](https://pypi.org/project/types-aiobotocore-s3control)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-s3control.svg?color=blue)](https://pypi.org/project/types-aiobotocore-s3control)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-s3control)](https://pepy.tech/project/types-aiobotocore-s3control)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.S3Control 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
+[aiobotocore.S3Control 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
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
 [types-aiobotocore-s3control docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-s3control-2.9.0/types_aiobotocore_s3control.egg-info/SOURCES.txt` & `types-aiobotocore-s3control-2.9.1/types_aiobotocore_s3control.egg-info/SOURCES.txt`

 * *Files identical despite different names*

