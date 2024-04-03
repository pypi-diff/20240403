# Comparing `tmp/types-aiobotocore-organizations-2.9.0.tar.gz` & `tmp/types-aiobotocore-organizations-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-organizations-2.9.0.tar", last modified: Wed Dec 13 20:00:04 2023, max compression
+gzip compressed data, was "types-aiobotocore-organizations-2.9.1.tar", last modified: Thu Jan 18 01:21:25 2024, max compression
```

## Comparing `types-aiobotocore-organizations-2.9.0.tar` & `types-aiobotocore-organizations-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:04.797360 types-aiobotocore-organizations-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:51:19.000000 types-aiobotocore-organizations-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15903 2023-12-13 20:00:04.797360 types-aiobotocore-organizations-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14316 2023-12-13 19:51:19.000000 types-aiobotocore-organizations-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:04.797360 types-aiobotocore-organizations-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2023-12-13 19:51:17.000000 types-aiobotocore-organizations-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:04.797360 types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations/
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2023-12-13 19:51:19.000000 types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2023-12-13 19:51:19.000000 types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      956 2023-12-13 19:51:19.000000 types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49837 2023-12-13 19:51:19.000000 types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    49833 2023-12-13 19:51:19.000000 types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12829 2023-12-13 19:51:19.000000 types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    12827 2023-12-13 19:51:19.000000 types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    20504 2023-12-13 19:51:19.000000 types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    20486 2023-12-13 19:51:19.000000 types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:51:19.000000 types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    35440 2023-12-13 19:51:20.000000 types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    35439 2023-12-13 19:51:20.000000 types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:51:19.000000 types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:04.797360 types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15903 2023-12-13 20:00:04.000000 types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      927 2023-12-13 20:00:04.000000 types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:04.000000 types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:04.000000 types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:04.000000 types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-13 20:00:04.000000 types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:25.661138 types-aiobotocore-organizations-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:12:59.000000 types-aiobotocore-organizations-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15923 2024-01-18 01:21:25.661138 types-aiobotocore-organizations-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14316 2024-01-18 01:12:59.000000 types-aiobotocore-organizations-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:25.661138 types-aiobotocore-organizations-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-01-18 01:12:57.000000 types-aiobotocore-organizations-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:25.657138 types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-01-18 01:12:59.000000 types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-01-18 01:12:59.000000 types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-01-18 01:12:59.000000 types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49841 2024-01-18 01:12:59.000000 types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49838 2024-01-18 01:12:59.000000 types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12827 2024-01-18 01:13:00.000000 types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12827 2024-01-18 01:13:00.000000 types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    20508 2024-01-18 01:13:00.000000 types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20491 2024-01-18 01:12:59.000000 types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:12:59.000000 types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    35439 2024-01-18 01:13:00.000000 types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35439 2024-01-18 01:13:00.000000 types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:12:59.000000 types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:25.657138 types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15923 2024-01-18 01:21:25.000000 types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-01-18 01:21:25.000000 types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:25.000000 types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:25.000000 types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:25.000000 types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-18 01:21:25.000000 types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-organizations-2.9.0/LICENSE` & `types-aiobotocore-organizations-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-organizations-2.9.0/PKG-INFO` & `types-aiobotocore-organizations-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-organizations
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Organizations 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Organizations 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/
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
 
 <a id="types-aiobotocore-organizations"></a>
 
 # types-aiobotocore-organizations
 
 [![PyPI - types-aiobotocore-organizations](https://img.shields.io/pypi/v/types-aiobotocore-organizations.svg?color=blue)](https://pypi.org/project/types-aiobotocore-organizations)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-organizations.svg?color=blue)](https://pypi.org/project/types-aiobotocore-organizations)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-organizations)](https://pepy.tech/project/types-aiobotocore-organizations)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Organizations 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations)
+[aiobotocore.Organizations 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations)
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
 [types-aiobotocore-organizations docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-organizations-2.9.0/README.md` & `types-aiobotocore-organizations-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-organizations.svg?color=blue)](https://pypi.org/project/types-aiobotocore-organizations)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-organizations)](https://pepy.tech/project/types-aiobotocore-organizations)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Organizations 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations)
+[aiobotocore.Organizations 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations)
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
 [types-aiobotocore-organizations docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-organizations-2.9.0/setup.py` & `types-aiobotocore-organizations-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-organizations",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_organizations"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Organizations 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.Organizations 2.9.1 service generated with"
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
     keywords="aiobotocore organizations type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_organizations": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations/__init__.py` & `types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,14 @@
     ListRootsPaginator,
     ListTagsForResourcePaginator,
     ListTargetsForPolicyPaginator,
 )
 
 Client = OrganizationsClient
 
-
 __all__ = (
     "Client",
     "ListAWSServiceAccessForOrganizationPaginator",
     "ListAccountsForParentPaginator",
     "ListAccountsPaginator",
     "ListChildrenPaginator",
     "ListCreateAccountStatusPaginator",
```

### Comparing `types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations/__init__.pyi` & `types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations/__main__.py` & `types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Organizations 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Organizations 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations\nOther"
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

### Comparing `types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations/client.py` & `types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("OrganizationsClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -232,15 +231,15 @@
     async def create_account(
         self,
         *,
         Email: str,
         AccountName: str,
         RoleName: str = ...,
         IamUserAccessToBilling: IAMUserAccessToBillingType = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAccountResponseTypeDef:
         """
         Creates an Amazon Web Services account that is automatically a member of the
         organization whose credentials made the
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Client.create_account)
@@ -250,15 +249,15 @@
     async def create_gov_cloud_account(
         self,
         *,
         Email: str,
         AccountName: str,
         RoleName: str = ...,
         IamUserAccessToBilling: IAMUserAccessToBillingType = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateGovCloudAccountResponseTypeDef:
         """
         This action is available if all of the following are true: * You're authorized
         to create accounts in the Amazon Web Services GovCloud (US)
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Client.create_gov_cloud_account)
@@ -288,15 +287,15 @@
     async def create_policy(
         self,
         *,
         Content: str,
         Description: str,
         Name: str,
         Type: PolicyTypeType,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreatePolicyResponseTypeDef:
         """
         Creates a policy of a specified type that you can attach to a root, an
         organizational unit (OU), or an individual Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Client.create_policy)
@@ -557,15 +556,15 @@
 
     async def list_children(
         self,
         *,
         ParentId: str,
         ChildType: ChildTypeType,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListChildrenResponseTypeDef:
         """
         Lists all of the organizational units (OUs) or accounts that are contained in
         the specified parent OU or
         root.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Client.list_children)
@@ -573,15 +572,15 @@
         """
 
     async def list_create_account_status(
         self,
         *,
         States: Sequence[CreateAccountStateType] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListCreateAccountStatusResponseTypeDef:
         """
         Lists the account creation requests that match the specified status that is
         currently being tracked for the
         organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Client.list_create_account_status)
```

### Comparing `types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations/client.pyi` & `types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -228,15 +228,15 @@
     async def create_account(
         self,
         *,
         Email: str,
         AccountName: str,
         RoleName: str = ...,
         IamUserAccessToBilling: IAMUserAccessToBillingType = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAccountResponseTypeDef:
         """
         Creates an Amazon Web Services account that is automatically a member of the
         organization whose credentials made the
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Client.create_account)
@@ -246,15 +246,15 @@
     async def create_gov_cloud_account(
         self,
         *,
         Email: str,
         AccountName: str,
         RoleName: str = ...,
         IamUserAccessToBilling: IAMUserAccessToBillingType = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateGovCloudAccountResponseTypeDef:
         """
         This action is available if all of the following are true: * You're authorized
         to create accounts in the Amazon Web Services GovCloud (US)
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Client.create_gov_cloud_account)
@@ -284,15 +284,15 @@
     async def create_policy(
         self,
         *,
         Content: str,
         Description: str,
         Name: str,
         Type: PolicyTypeType,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreatePolicyResponseTypeDef:
         """
         Creates a policy of a specified type that you can attach to a root, an
         organizational unit (OU), or an individual Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Client.create_policy)
@@ -553,15 +553,15 @@
 
     async def list_children(
         self,
         *,
         ParentId: str,
         ChildType: ChildTypeType,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListChildrenResponseTypeDef:
         """
         Lists all of the organizational units (OUs) or accounts that are contained in
         the specified parent OU or
         root.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Client.list_children)
@@ -569,15 +569,15 @@
         """
 
     async def list_create_account_status(
         self,
         *,
         States: Sequence[CreateAccountStateType] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListCreateAccountStatusResponseTypeDef:
         """
         Lists the account creation requests that match the specified status that is
         currently being tracked for the
         organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Client.list_create_account_status)
```

### Comparing `types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations/literals.py` & `types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations/literals.py`

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
     "AccountJoinedMethodType",
     "AccountStatusType",
     "ActionTypeType",
     "ChildTypeType",
     "CreateAccountFailureReasonType",
     "CreateAccountStateType",
@@ -55,15 +54,14 @@
     "TargetTypeType",
     "OrganizationsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 AccountJoinedMethodType = Literal["CREATED", "INVITED"]
 AccountStatusType = Literal["ACTIVE", "PENDING_CLOSURE", "SUSPENDED"]
 ActionTypeType = Literal[
     "ADD_ORGANIZATIONS_SERVICE_LINKED_ROLE", "APPROVE_ALL_FEATURES", "ENABLE_ALL_FEATURES", "INVITE"
 ]
 ChildTypeType = Literal["ACCOUNT", "ORGANIZATIONAL_UNIT"]
 CreateAccountFailureReasonType = Literal[
```

### Comparing `types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations/literals.pyi` & `types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations/paginator.py` & `types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,14 @@
     "ListPoliciesPaginator",
     "ListPoliciesForTargetPaginator",
     "ListRootsPaginator",
     "ListTagsForResourcePaginator",
     "ListTargetsForPolicyPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -160,15 +159,15 @@
     """
 
     def paginate(
         self,
         *,
         ParentId: str,
         ChildType: ChildTypeType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListChildrenResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListChildren.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/paginators/#listchildrenpaginator)
         """
 
 
@@ -178,15 +177,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/paginators/#listcreateaccountstatuspaginator)
     """
 
     def paginate(
         self,
         *,
         States: Sequence[CreateAccountStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCreateAccountStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListCreateAccountStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/paginators/#listcreateaccountstatuspaginator)
         """
 
 
@@ -226,15 +225,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/paginators/#listhandshakesforaccountpaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: HandshakeFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListHandshakesForAccountResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListHandshakesForAccount.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/paginators/#listhandshakesforaccountpaginator)
         """
 
 
@@ -244,15 +243,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/paginators/#listhandshakesfororganizationpaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: HandshakeFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListHandshakesForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListHandshakesForOrganization.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/paginators/#listhandshakesfororganizationpaginator)
         """
 
 
@@ -308,15 +307,15 @@
     """
 
     def paginate(
         self,
         *,
         TargetId: str,
         Filter: PolicyTypeType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPoliciesForTargetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListPoliciesForTarget.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/paginators/#listpoliciesfortargetpaginator)
         """
```

### Comparing `types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations/paginator.pyi` & `types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
     """
 
     def paginate(
         self,
         *,
         ParentId: str,
         ChildType: ChildTypeType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListChildrenResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListChildren.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/paginators/#listchildrenpaginator)
         """
 
 class ListCreateAccountStatusPaginator(AioPaginator):
@@ -171,15 +171,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/paginators/#listcreateaccountstatuspaginator)
     """
 
     def paginate(
         self,
         *,
         States: Sequence[CreateAccountStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCreateAccountStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListCreateAccountStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/paginators/#listcreateaccountstatuspaginator)
         """
 
 class ListDelegatedAdministratorsPaginator(AioPaginator):
@@ -216,15 +216,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/paginators/#listhandshakesforaccountpaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: HandshakeFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListHandshakesForAccountResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListHandshakesForAccount.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/paginators/#listhandshakesforaccountpaginator)
         """
 
 class ListHandshakesForOrganizationPaginator(AioPaginator):
@@ -233,15 +233,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/paginators/#listhandshakesfororganizationpaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: HandshakeFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListHandshakesForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListHandshakesForOrganization.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/paginators/#listhandshakesfororganizationpaginator)
         """
 
 class ListOrganizationalUnitsForParentPaginator(AioPaginator):
@@ -293,15 +293,15 @@
     """
 
     def paginate(
         self,
         *,
         TargetId: str,
         Filter: PolicyTypeType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPoliciesForTargetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListPoliciesForTarget.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/paginators/#listpoliciesfortargetpaginator)
         """
 
 class ListRootsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations/type_defs.py` & `types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations/type_defs.py`

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
     "AcceptHandshakeRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AccountTypeDef",
     "AttachPolicyRequestRequestTypeDef",
     "CancelHandshakeRequestRequestTypeDef",
     "ChildTypeDef",
```

### Comparing `types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations/type_defs.pyi` & `types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations.egg-info/PKG-INFO` & `types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-organizations
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Organizations 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Organizations 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/
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
 
 <a id="types-aiobotocore-organizations"></a>
 
 # types-aiobotocore-organizations
 
 [![PyPI - types-aiobotocore-organizations](https://img.shields.io/pypi/v/types-aiobotocore-organizations.svg?color=blue)](https://pypi.org/project/types-aiobotocore-organizations)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-organizations.svg?color=blue)](https://pypi.org/project/types-aiobotocore-organizations)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-organizations)](https://pepy.tech/project/types-aiobotocore-organizations)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Organizations 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations)
+[aiobotocore.Organizations 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations)
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
 [types-aiobotocore-organizations docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-organizations-2.9.0/types_aiobotocore_organizations.egg-info/SOURCES.txt` & `types-aiobotocore-organizations-2.9.1/types_aiobotocore_organizations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

