# Comparing `tmp/types-aiobotocore-fms-2.9.0.tar.gz` & `tmp/types-aiobotocore-fms-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-fms-2.9.0.tar", last modified: Wed Dec 13 19:59:20 2023, max compression
+gzip compressed data, was "types-aiobotocore-fms-2.9.1.tar", last modified: Thu Jan 18 01:20:44 2024, max compression
```

## Comparing `types-aiobotocore-fms-2.9.0.tar` & `types-aiobotocore-fms-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:20.145746 types-aiobotocore-fms-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:46:17.000000 types-aiobotocore-fms-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13967 2023-12-13 19:59:20.145746 types-aiobotocore-fms-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12420 2023-12-13 19:46:17.000000 types-aiobotocore-fms-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:20.145746 types-aiobotocore-fms-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-12-13 19:46:17.000000 types-aiobotocore-fms-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:20.145746 types-aiobotocore-fms-2.9.0/types_aiobotocore_fms/
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2023-12-13 19:46:17.000000 types-aiobotocore-fms-2.9.0/types_aiobotocore_fms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2023-12-13 19:46:17.000000 types-aiobotocore-fms-2.9.0/types_aiobotocore_fms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-13 19:46:17.000000 types-aiobotocore-fms-2.9.0/types_aiobotocore_fms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33032 2023-12-13 19:46:17.000000 types-aiobotocore-fms-2.9.0/types_aiobotocore_fms/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    33028 2023-12-13 19:46:17.000000 types-aiobotocore-fms-2.9.0/types_aiobotocore_fms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13587 2023-12-13 19:46:18.000000 types-aiobotocore-fms-2.9.0/types_aiobotocore_fms/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13585 2023-12-13 19:46:18.000000 types-aiobotocore-fms-2.9.0/types_aiobotocore_fms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10159 2023-12-13 19:46:17.000000 types-aiobotocore-fms-2.9.0/types_aiobotocore_fms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10149 2023-12-13 19:46:17.000000 types-aiobotocore-fms-2.9.0/types_aiobotocore_fms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:46:17.000000 types-aiobotocore-fms-2.9.0/types_aiobotocore_fms/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    52856 2023-12-13 19:46:20.000000 types-aiobotocore-fms-2.9.0/types_aiobotocore_fms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    52855 2023-12-13 19:46:19.000000 types-aiobotocore-fms-2.9.0/types_aiobotocore_fms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:46:17.000000 types-aiobotocore-fms-2.9.0/types_aiobotocore_fms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:20.145746 types-aiobotocore-fms-2.9.0/types_aiobotocore_fms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13967 2023-12-13 19:59:20.000000 types-aiobotocore-fms-2.9.0/types_aiobotocore_fms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      737 2023-12-13 19:59:20.000000 types-aiobotocore-fms-2.9.0/types_aiobotocore_fms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:20.000000 types-aiobotocore-fms-2.9.0/types_aiobotocore_fms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:20.000000 types-aiobotocore-fms-2.9.0/types_aiobotocore_fms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:20.000000 types-aiobotocore-fms-2.9.0/types_aiobotocore_fms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 19:59:20.000000 types-aiobotocore-fms-2.9.0/types_aiobotocore_fms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:44.537325 types-aiobotocore-fms-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:08:11.000000 types-aiobotocore-fms-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13987 2024-01-18 01:20:44.537325 types-aiobotocore-fms-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12420 2024-01-18 01:08:11.000000 types-aiobotocore-fms-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:44.537325 types-aiobotocore-fms-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-01-18 01:08:11.000000 types-aiobotocore-fms-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:44.537325 types-aiobotocore-fms-2.9.1/types_aiobotocore_fms/
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-01-18 01:08:11.000000 types-aiobotocore-fms-2.9.1/types_aiobotocore_fms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-01-18 01:08:11.000000 types-aiobotocore-fms-2.9.1/types_aiobotocore_fms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-18 01:08:11.000000 types-aiobotocore-fms-2.9.1/types_aiobotocore_fms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33033 2024-01-18 01:08:11.000000 types-aiobotocore-fms-2.9.1/types_aiobotocore_fms/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33030 2024-01-18 01:08:11.000000 types-aiobotocore-fms-2.9.1/types_aiobotocore_fms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13585 2024-01-18 01:08:13.000000 types-aiobotocore-fms-2.9.1/types_aiobotocore_fms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13585 2024-01-18 01:08:12.000000 types-aiobotocore-fms-2.9.1/types_aiobotocore_fms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10159 2024-01-18 01:08:11.000000 types-aiobotocore-fms-2.9.1/types_aiobotocore_fms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10150 2024-01-18 01:08:11.000000 types-aiobotocore-fms-2.9.1/types_aiobotocore_fms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:08:11.000000 types-aiobotocore-fms-2.9.1/types_aiobotocore_fms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    52855 2024-01-18 01:08:14.000000 types-aiobotocore-fms-2.9.1/types_aiobotocore_fms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52855 2024-01-18 01:08:14.000000 types-aiobotocore-fms-2.9.1/types_aiobotocore_fms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:08:11.000000 types-aiobotocore-fms-2.9.1/types_aiobotocore_fms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:44.537325 types-aiobotocore-fms-2.9.1/types_aiobotocore_fms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13987 2024-01-18 01:20:44.000000 types-aiobotocore-fms-2.9.1/types_aiobotocore_fms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-01-18 01:20:44.000000 types-aiobotocore-fms-2.9.1/types_aiobotocore_fms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:44.000000 types-aiobotocore-fms-2.9.1/types_aiobotocore_fms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:44.000000 types-aiobotocore-fms-2.9.1/types_aiobotocore_fms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:44.000000 types-aiobotocore-fms-2.9.1/types_aiobotocore_fms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:20:44.000000 types-aiobotocore-fms-2.9.1/types_aiobotocore_fms.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-fms-2.9.0/LICENSE` & `types-aiobotocore-fms-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-fms-2.9.0/PKG-INFO` & `types-aiobotocore-fms-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-fms
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.FMS 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.FMS 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/
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
 
 <a id="types-aiobotocore-fms"></a>
 
 # types-aiobotocore-fms
 
 [![PyPI - types-aiobotocore-fms](https://img.shields.io/pypi/v/types-aiobotocore-fms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-fms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-fms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-fms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-fms)](https://pepy.tech/project/types-aiobotocore-fms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.FMS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
+[aiobotocore.FMS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
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
 [types-aiobotocore-fms docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-fms-2.9.0/README.md` & `types-aiobotocore-fms-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-fms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-fms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-fms)](https://pepy.tech/project/types-aiobotocore-fms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.FMS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
+[aiobotocore.FMS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
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
 [types-aiobotocore-fms docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-fms-2.9.0/setup.py` & `types-aiobotocore-fms-2.9.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-fms",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_fms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.FMS 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.FMS 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore fms type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_fms": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-fms-2.9.0/types_aiobotocore_fms/__init__.py` & `types-aiobotocore-fms-2.9.1/types_aiobotocore_fms/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     ListPoliciesPaginator,
     ListProtocolsListsPaginator,
     ListThirdPartyFirewallFirewallPoliciesPaginator,
 )
 
 Client = FMSClient
 
-
 __all__ = (
     "Client",
     "FMSClient",
     "ListAdminAccountsForOrganizationPaginator",
     "ListAdminsManagingAccountPaginator",
     "ListAppsListsPaginator",
     "ListComplianceStatusPaginator",
```

### Comparing `types-aiobotocore-fms-2.9.0/types_aiobotocore_fms/__init__.pyi` & `types-aiobotocore-fms-2.9.1/types_aiobotocore_fms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fms-2.9.0/types_aiobotocore_fms/__main__.py` & `types-aiobotocore-fms-2.9.1/types_aiobotocore_fms/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.FMS 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.FMS 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS\nOther"
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

### Comparing `types-aiobotocore-fms-2.9.0/types_aiobotocore_fms/client.py` & `types-aiobotocore-fms-2.9.1/types_aiobotocore_fms/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("FMSClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -312,15 +311,15 @@
         self,
         *,
         PolicyId: str,
         MemberAccountId: str = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetProtectionStatusResponseTypeDef:
         """
         If you created a Shield Advanced policy, returns policy-level attack summary
         information in the event of a potential DDoS
         attack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_protection_status)
@@ -413,15 +412,15 @@
 
     async def list_discovered_resources(
         self,
         *,
         MemberAccountIds: Sequence[str],
         ResourceType: str,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListDiscoveredResourcesResponseTypeDef:
         """
         Returns an array of resources in the organization's accounts that are available
         to be associated with a resource
         set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_discovered_resources)
```

### Comparing `types-aiobotocore-fms-2.9.0/types_aiobotocore_fms/client.pyi` & `types-aiobotocore-fms-2.9.1/types_aiobotocore_fms/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -308,15 +308,15 @@
         self,
         *,
         PolicyId: str,
         MemberAccountId: str = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetProtectionStatusResponseTypeDef:
         """
         If you created a Shield Advanced policy, returns policy-level attack summary
         information in the event of a potential DDoS
         attack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_protection_status)
@@ -409,15 +409,15 @@
 
     async def list_discovered_resources(
         self,
         *,
         MemberAccountIds: Sequence[str],
         ResourceType: str,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListDiscoveredResourcesResponseTypeDef:
         """
         Returns an array of resources in the organization's accounts that are available
         to be associated with a resource
         set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_discovered_resources)
```

### Comparing `types-aiobotocore-fms-2.9.0/types_aiobotocore_fms/literals.py` & `types-aiobotocore-fms-2.9.1/types_aiobotocore_fms/literals.py`

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
     "AccountRoleStatusType",
     "CustomerPolicyScopeIdTypeType",
     "CustomerPolicyStatusType",
     "DependentServiceNameType",
     "DestinationTypeType",
     "FailedItemReasonType",
@@ -51,15 +50,14 @@
     "FMSServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AccountRoleStatusType = Literal["CREATING", "DELETED", "DELETING", "PENDING_DELETION", "READY"]
 CustomerPolicyScopeIdTypeType = Literal["ACCOUNT", "ORG_UNIT"]
 CustomerPolicyStatusType = Literal["ACTIVE", "OUT_OF_ADMIN_SCOPE"]
 DependentServiceNameType = Literal["AWSCONFIG", "AWSSHIELD_ADVANCED", "AWSVPC", "AWSWAF"]
 DestinationTypeType = Literal["IPV4", "IPV6", "PREFIX_LIST"]
 FailedItemReasonType = Literal[
     "NOT_VALID_ACCOUNT_ID",
```

### Comparing `types-aiobotocore-fms-2.9.0/types_aiobotocore_fms/literals.pyi` & `types-aiobotocore-fms-2.9.1/types_aiobotocore_fms/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fms-2.9.0/types_aiobotocore_fms/paginator.py` & `types-aiobotocore-fms-2.9.1/types_aiobotocore_fms/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,14 @@
     "ListComplianceStatusPaginator",
     "ListMemberAccountsPaginator",
     "ListPoliciesPaginator",
     "ListProtocolsListsPaginator",
     "ListThirdPartyFirewallFirewallPoliciesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -186,13 +185,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listthirdpartyfirewallfirewallpoliciespaginator)
     """
 
     def paginate(
         self,
         *,
         ThirdPartyFirewall: ThirdPartyFirewallType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListThirdPartyFirewallFirewallPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListThirdPartyFirewallFirewallPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listthirdpartyfirewallfirewallpoliciespaginator)
         """
```

### Comparing `types-aiobotocore-fms-2.9.0/types_aiobotocore_fms/paginator.pyi` & `types-aiobotocore-fms-2.9.1/types_aiobotocore_fms/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -176,13 +176,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listthirdpartyfirewallfirewallpoliciespaginator)
     """
 
     def paginate(
         self,
         *,
         ThirdPartyFirewall: ThirdPartyFirewallType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListThirdPartyFirewallFirewallPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListThirdPartyFirewallFirewallPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listthirdpartyfirewallfirewallpoliciespaginator)
         """
```

### Comparing `types-aiobotocore-fms-2.9.0/types_aiobotocore_fms/type_defs.py` & `types-aiobotocore-fms-2.9.1/types_aiobotocore_fms/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountScopeTypeDef",
     "ActionTargetTypeDef",
     "AdminAccountSummaryTypeDef",
     "OrganizationalUnitScopeTypeDef",
     "PolicyTypeScopeTypeDef",
     "RegionScopeTypeDef",
```

### Comparing `types-aiobotocore-fms-2.9.0/types_aiobotocore_fms/type_defs.pyi` & `types-aiobotocore-fms-2.9.1/types_aiobotocore_fms/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fms-2.9.0/types_aiobotocore_fms.egg-info/PKG-INFO` & `types-aiobotocore-fms-2.9.1/types_aiobotocore_fms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-fms
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.FMS 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.FMS 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/
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
 
 <a id="types-aiobotocore-fms"></a>
 
 # types-aiobotocore-fms
 
 [![PyPI - types-aiobotocore-fms](https://img.shields.io/pypi/v/types-aiobotocore-fms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-fms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-fms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-fms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-fms)](https://pepy.tech/project/types-aiobotocore-fms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.FMS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
+[aiobotocore.FMS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
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
 [types-aiobotocore-fms docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-fms-2.9.0/types_aiobotocore_fms.egg-info/SOURCES.txt` & `types-aiobotocore-fms-2.9.1/types_aiobotocore_fms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

