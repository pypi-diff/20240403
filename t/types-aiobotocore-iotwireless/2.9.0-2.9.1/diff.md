# Comparing `tmp/types-aiobotocore-iotwireless-2.9.0.tar.gz` & `tmp/types-aiobotocore-iotwireless-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotwireless-2.9.0.tar", last modified: Wed Dec 13 19:59:35 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotwireless-2.9.1.tar", last modified: Thu Jan 18 01:20:59 2024, max compression
```

## Comparing `types-aiobotocore-iotwireless-2.9.0.tar` & `types-aiobotocore-iotwireless-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:35.881606 types-aiobotocore-iotwireless-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:48:12.000000 types-aiobotocore-iotwireless-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12463 2023-12-13 19:59:35.881606 types-aiobotocore-iotwireless-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10884 2023-12-13 19:48:12.000000 types-aiobotocore-iotwireless-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:35.881606 types-aiobotocore-iotwireless-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2023-12-13 19:48:12.000000 types-aiobotocore-iotwireless-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:35.881606 types-aiobotocore-iotwireless-2.9.0/types_aiobotocore_iotwireless/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2023-12-13 19:48:12.000000 types-aiobotocore-iotwireless-2.9.0/types_aiobotocore_iotwireless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2023-12-13 19:48:12.000000 types-aiobotocore-iotwireless-2.9.0/types_aiobotocore_iotwireless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      948 2023-12-13 19:48:12.000000 types-aiobotocore-iotwireless-2.9.0/types_aiobotocore_iotwireless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    75854 2023-12-13 19:48:13.000000 types-aiobotocore-iotwireless-2.9.0/types_aiobotocore_iotwireless/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    75850 2023-12-13 19:48:12.000000 types-aiobotocore-iotwireless-2.9.0/types_aiobotocore_iotwireless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12807 2023-12-13 19:48:13.000000 types-aiobotocore-iotwireless-2.9.0/types_aiobotocore_iotwireless/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    12805 2023-12-13 19:48:13.000000 types-aiobotocore-iotwireless-2.9.0/types_aiobotocore_iotwireless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:48:12.000000 types-aiobotocore-iotwireless-2.9.0/types_aiobotocore_iotwireless/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    87218 2023-12-13 19:48:14.000000 types-aiobotocore-iotwireless-2.9.0/types_aiobotocore_iotwireless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    87217 2023-12-13 19:48:14.000000 types-aiobotocore-iotwireless-2.9.0/types_aiobotocore_iotwireless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:48:12.000000 types-aiobotocore-iotwireless-2.9.0/types_aiobotocore_iotwireless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:35.881606 types-aiobotocore-iotwireless-2.9.0/types_aiobotocore_iotwireless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12463 2023-12-13 19:59:35.000000 types-aiobotocore-iotwireless-2.9.0/types_aiobotocore_iotwireless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      802 2023-12-13 19:59:35.000000 types-aiobotocore-iotwireless-2.9.0/types_aiobotocore_iotwireless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:35.000000 types-aiobotocore-iotwireless-2.9.0/types_aiobotocore_iotwireless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:35.000000 types-aiobotocore-iotwireless-2.9.0/types_aiobotocore_iotwireless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:35.000000 types-aiobotocore-iotwireless-2.9.0/types_aiobotocore_iotwireless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 19:59:35.000000 types-aiobotocore-iotwireless-2.9.0/types_aiobotocore_iotwireless.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:59.125258 types-aiobotocore-iotwireless-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:10:02.000000 types-aiobotocore-iotwireless-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12483 2024-01-18 01:20:59.125258 types-aiobotocore-iotwireless-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10884 2024-01-18 01:10:02.000000 types-aiobotocore-iotwireless-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:59.125258 types-aiobotocore-iotwireless-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-01-18 01:10:02.000000 types-aiobotocore-iotwireless-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:59.125258 types-aiobotocore-iotwireless-2.9.1/types_aiobotocore_iotwireless/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-01-18 01:10:02.000000 types-aiobotocore-iotwireless-2.9.1/types_aiobotocore_iotwireless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-01-18 01:10:02.000000 types-aiobotocore-iotwireless-2.9.1/types_aiobotocore_iotwireless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-01-18 01:10:02.000000 types-aiobotocore-iotwireless-2.9.1/types_aiobotocore_iotwireless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75888 2024-01-18 01:10:02.000000 types-aiobotocore-iotwireless-2.9.1/types_aiobotocore_iotwireless/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75885 2024-01-18 01:10:02.000000 types-aiobotocore-iotwireless-2.9.1/types_aiobotocore_iotwireless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12805 2024-01-18 01:10:03.000000 types-aiobotocore-iotwireless-2.9.1/types_aiobotocore_iotwireless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12805 2024-01-18 01:10:03.000000 types-aiobotocore-iotwireless-2.9.1/types_aiobotocore_iotwireless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:10:02.000000 types-aiobotocore-iotwireless-2.9.1/types_aiobotocore_iotwireless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    87217 2024-01-18 01:10:04.000000 types-aiobotocore-iotwireless-2.9.1/types_aiobotocore_iotwireless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87217 2024-01-18 01:10:04.000000 types-aiobotocore-iotwireless-2.9.1/types_aiobotocore_iotwireless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:10:02.000000 types-aiobotocore-iotwireless-2.9.1/types_aiobotocore_iotwireless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:59.125258 types-aiobotocore-iotwireless-2.9.1/types_aiobotocore_iotwireless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12483 2024-01-18 01:20:59.000000 types-aiobotocore-iotwireless-2.9.1/types_aiobotocore_iotwireless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-01-18 01:20:59.000000 types-aiobotocore-iotwireless-2.9.1/types_aiobotocore_iotwireless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:59.000000 types-aiobotocore-iotwireless-2.9.1/types_aiobotocore_iotwireless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:59.000000 types-aiobotocore-iotwireless-2.9.1/types_aiobotocore_iotwireless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:59.000000 types-aiobotocore-iotwireless-2.9.1/types_aiobotocore_iotwireless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-18 01:20:59.000000 types-aiobotocore-iotwireless-2.9.1/types_aiobotocore_iotwireless.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotwireless-2.9.0/LICENSE` & `types-aiobotocore-iotwireless-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-iotwireless-2.9.0/PKG-INFO` & `types-aiobotocore-iotwireless-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotwireless
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IoTWireless 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IoTWireless 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/
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
 
 <a id="types-aiobotocore-iotwireless"></a>
 
 # types-aiobotocore-iotwireless
 
 [![PyPI - types-aiobotocore-iotwireless](https://img.shields.io/pypi/v/types-aiobotocore-iotwireless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotwireless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotwireless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotwireless)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotwireless)](https://pepy.tech/project/types-aiobotocore-iotwireless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTWireless 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
+[aiobotocore.IoTWireless 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
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
 [types-aiobotocore-iotwireless docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iotwireless-2.9.0/README.md` & `types-aiobotocore-iotwireless-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotwireless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotwireless)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotwireless)](https://pepy.tech/project/types-aiobotocore-iotwireless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTWireless 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
+[aiobotocore.IoTWireless 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
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
 [types-aiobotocore-iotwireless docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iotwireless-2.9.0/setup.py` & `types-aiobotocore-iotwireless-2.9.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotwireless",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_iotwireless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.IoTWireless 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.IoTWireless 2.9.1 service generated with"
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
     keywords="aiobotocore iotwireless type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_iotwireless": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-iotwireless-2.9.0/types_aiobotocore_iotwireless/__main__.py` & `types-aiobotocore-iotwireless-2.9.1/types_aiobotocore_iotwireless/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTWireless 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.IoTWireless 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless\nOther"
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

### Comparing `types-aiobotocore-iotwireless-2.9.0/types_aiobotocore_iotwireless/client.py` & `types-aiobotocore-iotwireless-2.9.1/types_aiobotocore_iotwireless/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("IoTWirelessClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -183,15 +182,15 @@
         """
 
     async def associate_aws_account_with_partner_account(
         self,
         *,
         Sidewalk: SidewalkAccountInfoTypeDef,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> AssociateAwsAccountWithPartnerAccountResponseTypeDef:
         """
         Associates a partner account with your AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.associate_aws_account_with_partner_account)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#associate_aws_account_with_partner_account)
         """
@@ -285,15 +284,15 @@
         *,
         Name: str,
         ExpressionType: ExpressionTypeType,
         Expression: str,
         RoleArn: str,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> CreateDestinationResponseTypeDef:
         """
         Creates a new destination that maps a device message to an AWS IoT rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#create_destination)
         """
@@ -301,15 +300,15 @@
     async def create_device_profile(
         self,
         *,
         Name: str = ...,
         LoRaWAN: LoRaWANDeviceProfileTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...,
-        Sidewalk: Mapping[str, Any] = ...
+        Sidewalk: Mapping[str, Any] = ...,
     ) -> CreateDeviceProfileResponseTypeDef:
         """
         Creates a new device profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_device_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#create_device_profile)
         """
@@ -322,15 +321,15 @@
         Name: str = ...,
         Description: str = ...,
         ClientRequestToken: str = ...,
         LoRaWAN: LoRaWANFuotaTaskTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         RedundancyPercent: int = ...,
         FragmentSizeBytes: int = ...,
-        FragmentIntervalMS: int = ...
+        FragmentIntervalMS: int = ...,
     ) -> CreateFuotaTaskResponseTypeDef:
         """
         Creates a FUOTA task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_fuota_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#create_fuota_task)
         """
@@ -338,15 +337,15 @@
     async def create_multicast_group(
         self,
         *,
         LoRaWAN: LoRaWANMulticastTypeDef,
         Name: str = ...,
         Description: str = ...,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMulticastGroupResponseTypeDef:
         """
         Creates a multicast group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_multicast_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#create_multicast_group)
         """
@@ -357,30 +356,30 @@
         Name: str,
         TraceContent: TraceContentTypeDef = ...,
         WirelessDevices: Sequence[str] = ...,
         WirelessGateways: Sequence[str] = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...,
-        MulticastGroups: Sequence[str] = ...
+        MulticastGroups: Sequence[str] = ...,
     ) -> CreateNetworkAnalyzerConfigurationResponseTypeDef:
         """
         Creates a new network analyzer configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_network_analyzer_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#create_network_analyzer_configuration)
         """
 
     async def create_service_profile(
         self,
         *,
         Name: str = ...,
         LoRaWAN: LoRaWANServiceProfileTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> CreateServiceProfileResponseTypeDef:
         """
         Creates a new service profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_service_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#create_service_profile)
         """
@@ -392,15 +391,15 @@
         DestinationName: str,
         Name: str = ...,
         Description: str = ...,
         ClientRequestToken: str = ...,
         LoRaWAN: LoRaWANDeviceTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Positioning: PositioningConfigStatusType = ...,
-        Sidewalk: SidewalkCreateWirelessDeviceTypeDef = ...
+        Sidewalk: SidewalkCreateWirelessDeviceTypeDef = ...,
     ) -> CreateWirelessDeviceResponseTypeDef:
         """
         Provisions a wireless device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_wireless_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#create_wireless_device)
         """
@@ -408,15 +407,15 @@
     async def create_wireless_gateway(
         self,
         *,
         LoRaWAN: LoRaWANGatewayTypeDef,
         Name: str = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> CreateWirelessGatewayResponseTypeDef:
         """
         Provisions a wireless gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_wireless_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#create_wireless_gateway)
         """
@@ -434,15 +433,15 @@
     async def create_wireless_gateway_task_definition(
         self,
         *,
         AutoCreateTasks: bool,
         Name: str = ...,
         Update: UpdateWirelessGatewayTaskCreateTypeDef = ...,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateWirelessGatewayTaskDefinitionResponseTypeDef:
         """
         Creates a gateway task definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_wireless_gateway_task_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#create_wireless_gateway_task_definition)
         """
@@ -738,29 +737,29 @@
     async def get_position_estimate(
         self,
         *,
         WiFiAccessPoints: Sequence[WiFiAccessPointTypeDef] = ...,
         CellTowers: CellTowersTypeDef = ...,
         Ip: IpTypeDef = ...,
         Gnss: GnssTypeDef = ...,
-        Timestamp: TimestampTypeDef = ...
+        Timestamp: TimestampTypeDef = ...,
     ) -> GetPositionEstimateResponseTypeDef:
         """
         Get estimated position information as a payload in GeoJSON format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_position_estimate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#get_position_estimate)
         """
 
     async def get_resource_event_configuration(
         self,
         *,
         Identifier: str,
         IdentifierType: IdentifierTypeType,
-        PartnerType: Literal["Sidewalk"] = ...
+        PartnerType: Literal["Sidewalk"] = ...,
     ) -> GetResourceEventConfigurationResponseTypeDef:
         """
         Get the event configuration for a particular resource identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_resource_event_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#get_resource_event_configuration)
         """
@@ -909,44 +908,44 @@
         """
 
     async def list_device_profiles(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
-        DeviceProfileType: DeviceProfileTypeType = ...
+        DeviceProfileType: DeviceProfileTypeType = ...,
     ) -> ListDeviceProfilesResponseTypeDef:
         """
         Lists the device profiles registered to your AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.list_device_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#list_device_profiles)
         """
 
     async def list_devices_for_wireless_device_import_task(
         self,
         *,
         Id: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Status: OnboardStatusType = ...
+        Status: OnboardStatusType = ...,
     ) -> ListDevicesForWirelessDeviceImportTaskResponseTypeDef:
         """
         List the Sidewalk devices in an import task and their onboarding status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.list_devices_for_wireless_device_import_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#list_devices_for_wireless_device_import_task)
         """
 
     async def list_event_configurations(
         self,
         *,
         ResourceType: EventNotificationResourceTypeType,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListEventConfigurationsResponseTypeDef:
         """
         List event configurations where at least one event topic has been enabled.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.list_event_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#list_event_configurations)
         """
@@ -1002,30 +1001,30 @@
         """
 
     async def list_position_configurations(
         self,
         *,
         ResourceType: PositionResourceTypeType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListPositionConfigurationsResponseTypeDef:
         """
         List position configurations for a given resource, such as positioning solvers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.list_position_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#list_position_configurations)
         """
 
     async def list_queued_messages(
         self,
         *,
         Id: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        WirelessDeviceType: WirelessDeviceTypeType = ...
+        WirelessDeviceType: WirelessDeviceTypeType = ...,
     ) -> ListQueuedMessagesResponseTypeDef:
         """
         List queued messages in the downlink queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.list_queued_messages)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#list_queued_messages)
         """
@@ -1066,29 +1065,29 @@
         MaxResults: int = ...,
         NextToken: str = ...,
         DestinationName: str = ...,
         DeviceProfileId: str = ...,
         ServiceProfileId: str = ...,
         WirelessDeviceType: WirelessDeviceTypeType = ...,
         FuotaTaskId: str = ...,
-        MulticastGroupId: str = ...
+        MulticastGroupId: str = ...,
     ) -> ListWirelessDevicesResponseTypeDef:
         """
         Lists the wireless devices registered to your AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.list_wireless_devices)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#list_wireless_devices)
         """
 
     async def list_wireless_gateway_task_definitions(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
-        TaskDefinitionType: Literal["UPDATE"] = ...
+        TaskDefinitionType: Literal["UPDATE"] = ...,
     ) -> ListWirelessGatewayTaskDefinitionsResponseTypeDef:
         """
         List the wireless gateway tasks definitions registered to your AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.list_wireless_gateway_task_definitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#list_wireless_gateway_task_definitions)
         """
@@ -1105,15 +1104,15 @@
 
     async def put_position_configuration(
         self,
         *,
         ResourceIdentifier: str,
         ResourceType: PositionResourceTypeType,
         Solvers: PositionSolverConfigurationsTypeDef = ...,
-        Destination: str = ...
+        Destination: str = ...,
     ) -> Dict[str, Any]:
         """
         Put position configuration for a given resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.put_position_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#put_position_configuration)
         """
@@ -1161,15 +1160,15 @@
 
     async def send_data_to_wireless_device(
         self,
         *,
         Id: str,
         TransmitMode: int,
         PayloadData: str,
-        WirelessMetadata: WirelessMetadataTypeDef = ...
+        WirelessMetadata: WirelessMetadataTypeDef = ...,
     ) -> SendDataToWirelessDeviceResponseTypeDef:
         """
         Sends a decrypted application data frame to a device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.send_data_to_wireless_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#send_data_to_wireless_device)
         """
@@ -1219,30 +1218,30 @@
     async def start_single_wireless_device_import_task(
         self,
         *,
         DestinationName: str,
         Sidewalk: SidewalkSingleStartImportInfoTypeDef,
         ClientRequestToken: str = ...,
         DeviceName: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> StartSingleWirelessDeviceImportTaskResponseTypeDef:
         """
         Start import task for a single wireless device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.start_single_wireless_device_import_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#start_single_wireless_device_import_task)
         """
 
     async def start_wireless_device_import_task(
         self,
         *,
         DestinationName: str,
         Sidewalk: SidewalkStartImportInfoTypeDef,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> StartWirelessDeviceImportTaskResponseTypeDef:
         """
         Start import task for provisioning Sidewalk devices in bulk using an S3 CSV
         file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.start_wireless_device_import_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#start_wireless_device_import_task)
@@ -1275,15 +1274,15 @@
     async def update_destination(
         self,
         *,
         Name: str,
         ExpressionType: ExpressionTypeType = ...,
         Expression: str = ...,
         Description: str = ...,
-        RoleArn: str = ...
+        RoleArn: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates properties of a destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#update_destination)
         """
@@ -1291,15 +1290,15 @@
     async def update_event_configuration_by_resource_types(
         self,
         *,
         DeviceRegistrationState: DeviceRegistrationStateResourceTypeEventConfigurationTypeDef = ...,
         Proximity: ProximityResourceTypeEventConfigurationTypeDef = ...,
         Join: JoinResourceTypeEventConfigurationTypeDef = ...,
         ConnectionStatus: ConnectionStatusResourceTypeEventConfigurationTypeDef = ...,
-        MessageDeliveryStatus: MessageDeliveryStatusResourceTypeEventConfigurationTypeDef = ...
+        MessageDeliveryStatus: MessageDeliveryStatusResourceTypeEventConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Update the event configuration based on resource types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_event_configuration_by_resource_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#update_event_configuration_by_resource_types)
         """
@@ -1311,44 +1310,44 @@
         Name: str = ...,
         Description: str = ...,
         LoRaWAN: LoRaWANFuotaTaskTypeDef = ...,
         FirmwareUpdateImage: str = ...,
         FirmwareUpdateRole: str = ...,
         RedundancyPercent: int = ...,
         FragmentSizeBytes: int = ...,
-        FragmentIntervalMS: int = ...
+        FragmentIntervalMS: int = ...,
     ) -> Dict[str, Any]:
         """
         Updates properties of a FUOTA task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_fuota_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#update_fuota_task)
         """
 
     async def update_log_levels_by_resource_types(
         self,
         *,
         DefaultLogLevel: LogLevelType = ...,
         WirelessDeviceLogOptions: Sequence[WirelessDeviceLogOptionTypeDef] = ...,
-        WirelessGatewayLogOptions: Sequence[WirelessGatewayLogOptionTypeDef] = ...
+        WirelessGatewayLogOptions: Sequence[WirelessGatewayLogOptionTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Set default log level, or log levels by resource types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_log_levels_by_resource_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#update_log_levels_by_resource_types)
         """
 
     async def update_multicast_group(
         self,
         *,
         Id: str,
         Name: str = ...,
         Description: str = ...,
-        LoRaWAN: LoRaWANMulticastTypeDef = ...
+        LoRaWAN: LoRaWANMulticastTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates properties of a multicast group session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_multicast_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#update_multicast_group)
         """
@@ -1360,43 +1359,43 @@
         TraceContent: TraceContentTypeDef = ...,
         WirelessDevicesToAdd: Sequence[str] = ...,
         WirelessDevicesToRemove: Sequence[str] = ...,
         WirelessGatewaysToAdd: Sequence[str] = ...,
         WirelessGatewaysToRemove: Sequence[str] = ...,
         Description: str = ...,
         MulticastGroupsToAdd: Sequence[str] = ...,
-        MulticastGroupsToRemove: Sequence[str] = ...
+        MulticastGroupsToRemove: Sequence[str] = ...,
     ) -> Dict[str, Any]:
         """
         Update network analyzer configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_network_analyzer_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#update_network_analyzer_configuration)
         """
 
     async def update_partner_account(
         self,
         *,
         Sidewalk: SidewalkUpdateAccountTypeDef,
         PartnerAccountId: str,
-        PartnerType: Literal["Sidewalk"]
+        PartnerType: Literal["Sidewalk"],
     ) -> Dict[str, Any]:
         """
         Updates properties of a partner account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_partner_account)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#update_partner_account)
         """
 
     async def update_position(
         self,
         *,
         ResourceIdentifier: str,
         ResourceType: PositionResourceTypeType,
-        Position: Sequence[float]
+        Position: Sequence[float],
     ) -> Dict[str, Any]:
         """
         Update the position information of a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_position)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#update_position)
         """
@@ -1407,29 +1406,29 @@
         Identifier: str,
         IdentifierType: IdentifierTypeType,
         PartnerType: Literal["Sidewalk"] = ...,
         DeviceRegistrationState: DeviceRegistrationStateEventConfigurationTypeDef = ...,
         Proximity: ProximityEventConfigurationTypeDef = ...,
         Join: JoinEventConfigurationTypeDef = ...,
         ConnectionStatus: ConnectionStatusEventConfigurationTypeDef = ...,
-        MessageDeliveryStatus: MessageDeliveryStatusEventConfigurationTypeDef = ...
+        MessageDeliveryStatus: MessageDeliveryStatusEventConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Update the event configuration for a particular resource identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_resource_event_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#update_resource_event_configuration)
         """
 
     async def update_resource_position(
         self,
         *,
         ResourceIdentifier: str,
         ResourceType: PositionResourceTypeType,
-        GeoJsonPayload: BlobTypeDef = ...
+        GeoJsonPayload: BlobTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Update the position information of a given wireless device or a wireless
         gateway
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_resource_position)
@@ -1440,15 +1439,15 @@
         self,
         *,
         Id: str,
         DestinationName: str = ...,
         Name: str = ...,
         Description: str = ...,
         LoRaWAN: LoRaWANUpdateDeviceTypeDef = ...,
-        Positioning: PositioningConfigStatusType = ...
+        Positioning: PositioningConfigStatusType = ...,
     ) -> Dict[str, Any]:
         """
         Updates properties of a wireless device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_wireless_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#update_wireless_device)
         """
@@ -1467,15 +1466,15 @@
         self,
         *,
         Id: str,
         Name: str = ...,
         Description: str = ...,
         JoinEuiFilters: Sequence[Sequence[str]] = ...,
         NetIdFilters: Sequence[str] = ...,
-        MaxEirp: float = ...
+        MaxEirp: float = ...,
     ) -> Dict[str, Any]:
         """
         Updates properties of a wireless gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_wireless_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#update_wireless_gateway)
         """
```

### Comparing `types-aiobotocore-iotwireless-2.9.0/types_aiobotocore_iotwireless/client.pyi` & `types-aiobotocore-iotwireless-2.9.1/types_aiobotocore_iotwireless/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,15 @@
         """
 
     async def associate_aws_account_with_partner_account(
         self,
         *,
         Sidewalk: SidewalkAccountInfoTypeDef,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> AssociateAwsAccountWithPartnerAccountResponseTypeDef:
         """
         Associates a partner account with your AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.associate_aws_account_with_partner_account)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#associate_aws_account_with_partner_account)
         """
@@ -281,15 +281,15 @@
         *,
         Name: str,
         ExpressionType: ExpressionTypeType,
         Expression: str,
         RoleArn: str,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> CreateDestinationResponseTypeDef:
         """
         Creates a new destination that maps a device message to an AWS IoT rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#create_destination)
         """
@@ -297,15 +297,15 @@
     async def create_device_profile(
         self,
         *,
         Name: str = ...,
         LoRaWAN: LoRaWANDeviceProfileTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...,
-        Sidewalk: Mapping[str, Any] = ...
+        Sidewalk: Mapping[str, Any] = ...,
     ) -> CreateDeviceProfileResponseTypeDef:
         """
         Creates a new device profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_device_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#create_device_profile)
         """
@@ -318,15 +318,15 @@
         Name: str = ...,
         Description: str = ...,
         ClientRequestToken: str = ...,
         LoRaWAN: LoRaWANFuotaTaskTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         RedundancyPercent: int = ...,
         FragmentSizeBytes: int = ...,
-        FragmentIntervalMS: int = ...
+        FragmentIntervalMS: int = ...,
     ) -> CreateFuotaTaskResponseTypeDef:
         """
         Creates a FUOTA task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_fuota_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#create_fuota_task)
         """
@@ -334,15 +334,15 @@
     async def create_multicast_group(
         self,
         *,
         LoRaWAN: LoRaWANMulticastTypeDef,
         Name: str = ...,
         Description: str = ...,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMulticastGroupResponseTypeDef:
         """
         Creates a multicast group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_multicast_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#create_multicast_group)
         """
@@ -353,30 +353,30 @@
         Name: str,
         TraceContent: TraceContentTypeDef = ...,
         WirelessDevices: Sequence[str] = ...,
         WirelessGateways: Sequence[str] = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...,
-        MulticastGroups: Sequence[str] = ...
+        MulticastGroups: Sequence[str] = ...,
     ) -> CreateNetworkAnalyzerConfigurationResponseTypeDef:
         """
         Creates a new network analyzer configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_network_analyzer_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#create_network_analyzer_configuration)
         """
 
     async def create_service_profile(
         self,
         *,
         Name: str = ...,
         LoRaWAN: LoRaWANServiceProfileTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> CreateServiceProfileResponseTypeDef:
         """
         Creates a new service profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_service_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#create_service_profile)
         """
@@ -388,15 +388,15 @@
         DestinationName: str,
         Name: str = ...,
         Description: str = ...,
         ClientRequestToken: str = ...,
         LoRaWAN: LoRaWANDeviceTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Positioning: PositioningConfigStatusType = ...,
-        Sidewalk: SidewalkCreateWirelessDeviceTypeDef = ...
+        Sidewalk: SidewalkCreateWirelessDeviceTypeDef = ...,
     ) -> CreateWirelessDeviceResponseTypeDef:
         """
         Provisions a wireless device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_wireless_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#create_wireless_device)
         """
@@ -404,15 +404,15 @@
     async def create_wireless_gateway(
         self,
         *,
         LoRaWAN: LoRaWANGatewayTypeDef,
         Name: str = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> CreateWirelessGatewayResponseTypeDef:
         """
         Provisions a wireless gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_wireless_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#create_wireless_gateway)
         """
@@ -430,15 +430,15 @@
     async def create_wireless_gateway_task_definition(
         self,
         *,
         AutoCreateTasks: bool,
         Name: str = ...,
         Update: UpdateWirelessGatewayTaskCreateTypeDef = ...,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateWirelessGatewayTaskDefinitionResponseTypeDef:
         """
         Creates a gateway task definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_wireless_gateway_task_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#create_wireless_gateway_task_definition)
         """
@@ -734,29 +734,29 @@
     async def get_position_estimate(
         self,
         *,
         WiFiAccessPoints: Sequence[WiFiAccessPointTypeDef] = ...,
         CellTowers: CellTowersTypeDef = ...,
         Ip: IpTypeDef = ...,
         Gnss: GnssTypeDef = ...,
-        Timestamp: TimestampTypeDef = ...
+        Timestamp: TimestampTypeDef = ...,
     ) -> GetPositionEstimateResponseTypeDef:
         """
         Get estimated position information as a payload in GeoJSON format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_position_estimate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#get_position_estimate)
         """
 
     async def get_resource_event_configuration(
         self,
         *,
         Identifier: str,
         IdentifierType: IdentifierTypeType,
-        PartnerType: Literal["Sidewalk"] = ...
+        PartnerType: Literal["Sidewalk"] = ...,
     ) -> GetResourceEventConfigurationResponseTypeDef:
         """
         Get the event configuration for a particular resource identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_resource_event_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#get_resource_event_configuration)
         """
@@ -905,44 +905,44 @@
         """
 
     async def list_device_profiles(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
-        DeviceProfileType: DeviceProfileTypeType = ...
+        DeviceProfileType: DeviceProfileTypeType = ...,
     ) -> ListDeviceProfilesResponseTypeDef:
         """
         Lists the device profiles registered to your AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.list_device_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#list_device_profiles)
         """
 
     async def list_devices_for_wireless_device_import_task(
         self,
         *,
         Id: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Status: OnboardStatusType = ...
+        Status: OnboardStatusType = ...,
     ) -> ListDevicesForWirelessDeviceImportTaskResponseTypeDef:
         """
         List the Sidewalk devices in an import task and their onboarding status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.list_devices_for_wireless_device_import_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#list_devices_for_wireless_device_import_task)
         """
 
     async def list_event_configurations(
         self,
         *,
         ResourceType: EventNotificationResourceTypeType,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListEventConfigurationsResponseTypeDef:
         """
         List event configurations where at least one event topic has been enabled.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.list_event_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#list_event_configurations)
         """
@@ -998,30 +998,30 @@
         """
 
     async def list_position_configurations(
         self,
         *,
         ResourceType: PositionResourceTypeType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListPositionConfigurationsResponseTypeDef:
         """
         List position configurations for a given resource, such as positioning solvers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.list_position_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#list_position_configurations)
         """
 
     async def list_queued_messages(
         self,
         *,
         Id: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        WirelessDeviceType: WirelessDeviceTypeType = ...
+        WirelessDeviceType: WirelessDeviceTypeType = ...,
     ) -> ListQueuedMessagesResponseTypeDef:
         """
         List queued messages in the downlink queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.list_queued_messages)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#list_queued_messages)
         """
@@ -1062,29 +1062,29 @@
         MaxResults: int = ...,
         NextToken: str = ...,
         DestinationName: str = ...,
         DeviceProfileId: str = ...,
         ServiceProfileId: str = ...,
         WirelessDeviceType: WirelessDeviceTypeType = ...,
         FuotaTaskId: str = ...,
-        MulticastGroupId: str = ...
+        MulticastGroupId: str = ...,
     ) -> ListWirelessDevicesResponseTypeDef:
         """
         Lists the wireless devices registered to your AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.list_wireless_devices)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#list_wireless_devices)
         """
 
     async def list_wireless_gateway_task_definitions(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
-        TaskDefinitionType: Literal["UPDATE"] = ...
+        TaskDefinitionType: Literal["UPDATE"] = ...,
     ) -> ListWirelessGatewayTaskDefinitionsResponseTypeDef:
         """
         List the wireless gateway tasks definitions registered to your AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.list_wireless_gateway_task_definitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#list_wireless_gateway_task_definitions)
         """
@@ -1101,15 +1101,15 @@
 
     async def put_position_configuration(
         self,
         *,
         ResourceIdentifier: str,
         ResourceType: PositionResourceTypeType,
         Solvers: PositionSolverConfigurationsTypeDef = ...,
-        Destination: str = ...
+        Destination: str = ...,
     ) -> Dict[str, Any]:
         """
         Put position configuration for a given resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.put_position_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#put_position_configuration)
         """
@@ -1157,15 +1157,15 @@
 
     async def send_data_to_wireless_device(
         self,
         *,
         Id: str,
         TransmitMode: int,
         PayloadData: str,
-        WirelessMetadata: WirelessMetadataTypeDef = ...
+        WirelessMetadata: WirelessMetadataTypeDef = ...,
     ) -> SendDataToWirelessDeviceResponseTypeDef:
         """
         Sends a decrypted application data frame to a device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.send_data_to_wireless_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#send_data_to_wireless_device)
         """
@@ -1215,30 +1215,30 @@
     async def start_single_wireless_device_import_task(
         self,
         *,
         DestinationName: str,
         Sidewalk: SidewalkSingleStartImportInfoTypeDef,
         ClientRequestToken: str = ...,
         DeviceName: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> StartSingleWirelessDeviceImportTaskResponseTypeDef:
         """
         Start import task for a single wireless device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.start_single_wireless_device_import_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#start_single_wireless_device_import_task)
         """
 
     async def start_wireless_device_import_task(
         self,
         *,
         DestinationName: str,
         Sidewalk: SidewalkStartImportInfoTypeDef,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> StartWirelessDeviceImportTaskResponseTypeDef:
         """
         Start import task for provisioning Sidewalk devices in bulk using an S3 CSV
         file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.start_wireless_device_import_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#start_wireless_device_import_task)
@@ -1271,15 +1271,15 @@
     async def update_destination(
         self,
         *,
         Name: str,
         ExpressionType: ExpressionTypeType = ...,
         Expression: str = ...,
         Description: str = ...,
-        RoleArn: str = ...
+        RoleArn: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates properties of a destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#update_destination)
         """
@@ -1287,15 +1287,15 @@
     async def update_event_configuration_by_resource_types(
         self,
         *,
         DeviceRegistrationState: DeviceRegistrationStateResourceTypeEventConfigurationTypeDef = ...,
         Proximity: ProximityResourceTypeEventConfigurationTypeDef = ...,
         Join: JoinResourceTypeEventConfigurationTypeDef = ...,
         ConnectionStatus: ConnectionStatusResourceTypeEventConfigurationTypeDef = ...,
-        MessageDeliveryStatus: MessageDeliveryStatusResourceTypeEventConfigurationTypeDef = ...
+        MessageDeliveryStatus: MessageDeliveryStatusResourceTypeEventConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Update the event configuration based on resource types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_event_configuration_by_resource_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#update_event_configuration_by_resource_types)
         """
@@ -1307,44 +1307,44 @@
         Name: str = ...,
         Description: str = ...,
         LoRaWAN: LoRaWANFuotaTaskTypeDef = ...,
         FirmwareUpdateImage: str = ...,
         FirmwareUpdateRole: str = ...,
         RedundancyPercent: int = ...,
         FragmentSizeBytes: int = ...,
-        FragmentIntervalMS: int = ...
+        FragmentIntervalMS: int = ...,
     ) -> Dict[str, Any]:
         """
         Updates properties of a FUOTA task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_fuota_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#update_fuota_task)
         """
 
     async def update_log_levels_by_resource_types(
         self,
         *,
         DefaultLogLevel: LogLevelType = ...,
         WirelessDeviceLogOptions: Sequence[WirelessDeviceLogOptionTypeDef] = ...,
-        WirelessGatewayLogOptions: Sequence[WirelessGatewayLogOptionTypeDef] = ...
+        WirelessGatewayLogOptions: Sequence[WirelessGatewayLogOptionTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Set default log level, or log levels by resource types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_log_levels_by_resource_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#update_log_levels_by_resource_types)
         """
 
     async def update_multicast_group(
         self,
         *,
         Id: str,
         Name: str = ...,
         Description: str = ...,
-        LoRaWAN: LoRaWANMulticastTypeDef = ...
+        LoRaWAN: LoRaWANMulticastTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates properties of a multicast group session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_multicast_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#update_multicast_group)
         """
@@ -1356,43 +1356,43 @@
         TraceContent: TraceContentTypeDef = ...,
         WirelessDevicesToAdd: Sequence[str] = ...,
         WirelessDevicesToRemove: Sequence[str] = ...,
         WirelessGatewaysToAdd: Sequence[str] = ...,
         WirelessGatewaysToRemove: Sequence[str] = ...,
         Description: str = ...,
         MulticastGroupsToAdd: Sequence[str] = ...,
-        MulticastGroupsToRemove: Sequence[str] = ...
+        MulticastGroupsToRemove: Sequence[str] = ...,
     ) -> Dict[str, Any]:
         """
         Update network analyzer configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_network_analyzer_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#update_network_analyzer_configuration)
         """
 
     async def update_partner_account(
         self,
         *,
         Sidewalk: SidewalkUpdateAccountTypeDef,
         PartnerAccountId: str,
-        PartnerType: Literal["Sidewalk"]
+        PartnerType: Literal["Sidewalk"],
     ) -> Dict[str, Any]:
         """
         Updates properties of a partner account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_partner_account)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#update_partner_account)
         """
 
     async def update_position(
         self,
         *,
         ResourceIdentifier: str,
         ResourceType: PositionResourceTypeType,
-        Position: Sequence[float]
+        Position: Sequence[float],
     ) -> Dict[str, Any]:
         """
         Update the position information of a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_position)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#update_position)
         """
@@ -1403,29 +1403,29 @@
         Identifier: str,
         IdentifierType: IdentifierTypeType,
         PartnerType: Literal["Sidewalk"] = ...,
         DeviceRegistrationState: DeviceRegistrationStateEventConfigurationTypeDef = ...,
         Proximity: ProximityEventConfigurationTypeDef = ...,
         Join: JoinEventConfigurationTypeDef = ...,
         ConnectionStatus: ConnectionStatusEventConfigurationTypeDef = ...,
-        MessageDeliveryStatus: MessageDeliveryStatusEventConfigurationTypeDef = ...
+        MessageDeliveryStatus: MessageDeliveryStatusEventConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Update the event configuration for a particular resource identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_resource_event_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#update_resource_event_configuration)
         """
 
     async def update_resource_position(
         self,
         *,
         ResourceIdentifier: str,
         ResourceType: PositionResourceTypeType,
-        GeoJsonPayload: BlobTypeDef = ...
+        GeoJsonPayload: BlobTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Update the position information of a given wireless device or a wireless
         gateway
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_resource_position)
@@ -1436,15 +1436,15 @@
         self,
         *,
         Id: str,
         DestinationName: str = ...,
         Name: str = ...,
         Description: str = ...,
         LoRaWAN: LoRaWANUpdateDeviceTypeDef = ...,
-        Positioning: PositioningConfigStatusType = ...
+        Positioning: PositioningConfigStatusType = ...,
     ) -> Dict[str, Any]:
         """
         Updates properties of a wireless device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_wireless_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#update_wireless_device)
         """
@@ -1463,15 +1463,15 @@
         self,
         *,
         Id: str,
         Name: str = ...,
         Description: str = ...,
         JoinEuiFilters: Sequence[Sequence[str]] = ...,
         NetIdFilters: Sequence[str] = ...,
-        MaxEirp: float = ...
+        MaxEirp: float = ...,
     ) -> Dict[str, Any]:
         """
         Updates properties of a wireless gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_wireless_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#update_wireless_gateway)
         """
```

### Comparing `types-aiobotocore-iotwireless-2.9.0/types_aiobotocore_iotwireless/literals.py` & `types-aiobotocore-iotwireless-2.9.1/types_aiobotocore_iotwireless/literals.py`

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
     "ApplicationConfigTypeType",
     "BatteryLevelType",
     "ConnectionStatusType",
     "DeviceProfileTypeType",
     "DeviceStateType",
     "DlClassType",
@@ -63,15 +62,14 @@
     "WirelessGatewayTypeType",
     "IoTWirelessServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 ApplicationConfigTypeType = Literal["SemtechGeolocation"]
 BatteryLevelType = Literal["critical", "low", "normal"]
 ConnectionStatusType = Literal["Connected", "Disconnected"]
 DeviceProfileTypeType = Literal["LoRaWAN", "Sidewalk"]
 DeviceStateType = Literal[
     "Provisioned", "RegisteredNotSeen", "RegisteredReachable", "RegisteredUnreachable"
 ]
```

### Comparing `types-aiobotocore-iotwireless-2.9.0/types_aiobotocore_iotwireless/literals.pyi` & `types-aiobotocore-iotwireless-2.9.1/types_aiobotocore_iotwireless/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotwireless-2.9.0/types_aiobotocore_iotwireless/type_defs.py` & `types-aiobotocore-iotwireless-2.9.1/types_aiobotocore_iotwireless/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "SessionKeysAbpV10XTypeDef",
     "SessionKeysAbpV11TypeDef",
     "AccuracyTypeDef",
     "ApplicationConfigTypeDef",
     "SidewalkAccountInfoTypeDef",
     "TagTypeDef",
```

### Comparing `types-aiobotocore-iotwireless-2.9.0/types_aiobotocore_iotwireless/type_defs.pyi` & `types-aiobotocore-iotwireless-2.9.1/types_aiobotocore_iotwireless/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotwireless-2.9.0/types_aiobotocore_iotwireless.egg-info/PKG-INFO` & `types-aiobotocore-iotwireless-2.9.1/types_aiobotocore_iotwireless.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotwireless
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IoTWireless 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IoTWireless 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/
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
 
 <a id="types-aiobotocore-iotwireless"></a>
 
 # types-aiobotocore-iotwireless
 
 [![PyPI - types-aiobotocore-iotwireless](https://img.shields.io/pypi/v/types-aiobotocore-iotwireless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotwireless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotwireless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotwireless)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotwireless)](https://pepy.tech/project/types-aiobotocore-iotwireless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTWireless 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
+[aiobotocore.IoTWireless 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
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
 [types-aiobotocore-iotwireless docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iotwireless-2.9.0/types_aiobotocore_iotwireless.egg-info/SOURCES.txt` & `types-aiobotocore-iotwireless-2.9.1/types_aiobotocore_iotwireless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

