# Comparing `tmp/types-aiobotocore-worklink-2.9.0.tar.gz` & `tmp/types-aiobotocore-worklink-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-worklink-2.9.0.tar", last modified: Wed Dec 13 20:00:46 2023, max compression
+gzip compressed data, was "types-aiobotocore-worklink-2.9.1.tar", last modified: Thu Jan 18 01:22:03 2024, max compression
```

## Comparing `types-aiobotocore-worklink-2.9.0.tar` & `types-aiobotocore-worklink-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:46.756998 types-aiobotocore-worklink-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:57:59.000000 types-aiobotocore-worklink-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12334 2023-12-13 20:00:46.756998 types-aiobotocore-worklink-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10767 2023-12-13 19:57:59.000000 types-aiobotocore-worklink-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:46.756998 types-aiobotocore-worklink-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-12-13 19:57:59.000000 types-aiobotocore-worklink-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:46.756998 types-aiobotocore-worklink-2.9.0/types_aiobotocore_worklink/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2023-12-13 19:57:59.000000 types-aiobotocore-worklink-2.9.0/types_aiobotocore_worklink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2023-12-13 19:57:59.000000 types-aiobotocore-worklink-2.9.0/types_aiobotocore_worklink/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-12-13 19:57:59.000000 types-aiobotocore-worklink-2.9.0/types_aiobotocore_worklink/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23856 2023-12-13 19:58:00.000000 types-aiobotocore-worklink-2.9.0/types_aiobotocore_worklink/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    23852 2023-12-13 19:57:59.000000 types-aiobotocore-worklink-2.9.0/types_aiobotocore_worklink/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2023-12-13 19:58:00.000000 types-aiobotocore-worklink-2.9.0/types_aiobotocore_worklink/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8715 2023-12-13 19:58:00.000000 types-aiobotocore-worklink-2.9.0/types_aiobotocore_worklink/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:57:59.000000 types-aiobotocore-worklink-2.9.0/types_aiobotocore_worklink/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    16344 2023-12-13 19:58:00.000000 types-aiobotocore-worklink-2.9.0/types_aiobotocore_worklink/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16343 2023-12-13 19:58:00.000000 types-aiobotocore-worklink-2.9.0/types_aiobotocore_worklink/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:57:59.000000 types-aiobotocore-worklink-2.9.0/types_aiobotocore_worklink/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:46.756998 types-aiobotocore-worklink-2.9.0/types_aiobotocore_worklink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12334 2023-12-13 20:00:46.000000 types-aiobotocore-worklink-2.9.0/types_aiobotocore_worklink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      751 2023-12-13 20:00:46.000000 types-aiobotocore-worklink-2.9.0/types_aiobotocore_worklink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:46.000000 types-aiobotocore-worklink-2.9.0/types_aiobotocore_worklink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:46.000000 types-aiobotocore-worklink-2.9.0/types_aiobotocore_worklink.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:46.000000 types-aiobotocore-worklink-2.9.0/types_aiobotocore_worklink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-13 20:00:46.000000 types-aiobotocore-worklink-2.9.0/types_aiobotocore_worklink.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:03.644967 types-aiobotocore-worklink-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:19:28.000000 types-aiobotocore-worklink-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-01-18 01:22:03.644967 types-aiobotocore-worklink-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10767 2024-01-18 01:19:28.000000 types-aiobotocore-worklink-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:22:03.644967 types-aiobotocore-worklink-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-18 01:19:28.000000 types-aiobotocore-worklink-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:03.644967 types-aiobotocore-worklink-2.9.1/types_aiobotocore_worklink/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-01-18 01:19:28.000000 types-aiobotocore-worklink-2.9.1/types_aiobotocore_worklink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-01-18 01:19:28.000000 types-aiobotocore-worklink-2.9.1/types_aiobotocore_worklink/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-01-18 01:19:28.000000 types-aiobotocore-worklink-2.9.1/types_aiobotocore_worklink/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23858 2024-01-18 01:19:28.000000 types-aiobotocore-worklink-2.9.1/types_aiobotocore_worklink/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23855 2024-01-18 01:19:28.000000 types-aiobotocore-worklink-2.9.1/types_aiobotocore_worklink/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-01-18 01:19:28.000000 types-aiobotocore-worklink-2.9.1/types_aiobotocore_worklink/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-01-18 01:19:28.000000 types-aiobotocore-worklink-2.9.1/types_aiobotocore_worklink/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:28.000000 types-aiobotocore-worklink-2.9.1/types_aiobotocore_worklink/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16343 2024-01-18 01:19:28.000000 types-aiobotocore-worklink-2.9.1/types_aiobotocore_worklink/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16343 2024-01-18 01:19:28.000000 types-aiobotocore-worklink-2.9.1/types_aiobotocore_worklink/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:19:28.000000 types-aiobotocore-worklink-2.9.1/types_aiobotocore_worklink/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:03.644967 types-aiobotocore-worklink-2.9.1/types_aiobotocore_worklink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-01-18 01:22:03.000000 types-aiobotocore-worklink-2.9.1/types_aiobotocore_worklink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-01-18 01:22:03.000000 types-aiobotocore-worklink-2.9.1/types_aiobotocore_worklink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:22:03.000000 types-aiobotocore-worklink-2.9.1/types_aiobotocore_worklink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:22:03.000000 types-aiobotocore-worklink-2.9.1/types_aiobotocore_worklink.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:22:03.000000 types-aiobotocore-worklink-2.9.1/types_aiobotocore_worklink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-18 01:22:03.000000 types-aiobotocore-worklink-2.9.1/types_aiobotocore_worklink.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-worklink-2.9.0/LICENSE` & `types-aiobotocore-worklink-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-worklink-2.9.0/PKG-INFO` & `types-aiobotocore-worklink-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-worklink
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.WorkLink 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.WorkLink 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink/
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
 
 <a id="types-aiobotocore-worklink"></a>
 
 # types-aiobotocore-worklink
 
 [![PyPI - types-aiobotocore-worklink](https://img.shields.io/pypi/v/types-aiobotocore-worklink.svg?color=blue)](https://pypi.org/project/types-aiobotocore-worklink)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-worklink.svg?color=blue)](https://pypi.org/project/types-aiobotocore-worklink)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-worklink)](https://pepy.tech/project/types-aiobotocore-worklink)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WorkLink 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink)
+[aiobotocore.WorkLink 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink)
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
 [types-aiobotocore-worklink docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-worklink-2.9.0/README.md` & `types-aiobotocore-worklink-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-worklink.svg?color=blue)](https://pypi.org/project/types-aiobotocore-worklink)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-worklink)](https://pepy.tech/project/types-aiobotocore-worklink)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WorkLink 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink)
+[aiobotocore.WorkLink 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink)
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
 [types-aiobotocore-worklink docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-worklink-2.9.0/setup.py` & `types-aiobotocore-worklink-2.9.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-worklink",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_worklink"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.WorkLink 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.WorkLink 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore worklink type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_worklink": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-worklink-2.9.0/types_aiobotocore_worklink/__main__.py` & `types-aiobotocore-worklink-2.9.1/types_aiobotocore_worklink/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.WorkLink 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.WorkLink 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink\nOther"
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

### Comparing `types-aiobotocore-worklink-2.9.0/types_aiobotocore_worklink/client.py` & `types-aiobotocore-worklink-2.9.1/types_aiobotocore_worklink/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("WorkLinkClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -135,15 +134,15 @@
 
     async def create_fleet(
         self,
         *,
         FleetName: str,
         DisplayName: str = ...,
         OptimizeForEndUserLocation: bool = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateFleetResponseTypeDef:
         """
         Creates a fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.create_fleet)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink/client/#create_fleet)
         """
@@ -397,15 +396,15 @@
 
     async def update_company_network_configuration(
         self,
         *,
         FleetArn: str,
         VpcId: str,
         SubnetIds: Sequence[str],
-        SecurityGroupIds: Sequence[str]
+        SecurityGroupIds: Sequence[str],
     ) -> Dict[str, Any]:
         """
         Updates the company network configuration for the fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.update_company_network_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink/client/#update_company_network_configuration)
         """
@@ -441,15 +440,15 @@
         """
 
     async def update_identity_provider_configuration(
         self,
         *,
         FleetArn: str,
         IdentityProviderType: Literal["SAML"],
-        IdentityProviderSamlMetadata: str = ...
+        IdentityProviderSamlMetadata: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the identity provider configuration for the fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.update_identity_provider_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink/client/#update_identity_provider_configuration)
         """
```

### Comparing `types-aiobotocore-worklink-2.9.0/types_aiobotocore_worklink/client.pyi` & `types-aiobotocore-worklink-2.9.1/types_aiobotocore_worklink/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 
     async def create_fleet(
         self,
         *,
         FleetName: str,
         DisplayName: str = ...,
         OptimizeForEndUserLocation: bool = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateFleetResponseTypeDef:
         """
         Creates a fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.create_fleet)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink/client/#create_fleet)
         """
@@ -393,15 +393,15 @@
 
     async def update_company_network_configuration(
         self,
         *,
         FleetArn: str,
         VpcId: str,
         SubnetIds: Sequence[str],
-        SecurityGroupIds: Sequence[str]
+        SecurityGroupIds: Sequence[str],
     ) -> Dict[str, Any]:
         """
         Updates the company network configuration for the fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.update_company_network_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink/client/#update_company_network_configuration)
         """
@@ -437,15 +437,15 @@
         """
 
     async def update_identity_provider_configuration(
         self,
         *,
         FleetArn: str,
         IdentityProviderType: Literal["SAML"],
-        IdentityProviderSamlMetadata: str = ...
+        IdentityProviderSamlMetadata: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the identity provider configuration for the fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink.Client.update_identity_provider_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink/client/#update_identity_provider_configuration)
         """
```

### Comparing `types-aiobotocore-worklink-2.9.0/types_aiobotocore_worklink/literals.py` & `types-aiobotocore-worklink-2.9.1/types_aiobotocore_worklink/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,27 +15,25 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AuthorizationProviderTypeType",
     "DeviceStatusType",
     "DomainStatusType",
     "FleetStatusType",
     "IdentityProviderTypeType",
     "WorkLinkServiceName",
     "ServiceName",
     "ResourceServiceName",
 )
 
-
 AuthorizationProviderTypeType = Literal["SAML"]
 DeviceStatusType = Literal["ACTIVE", "SIGNED_OUT"]
 DomainStatusType = Literal[
     "ACTIVE",
     "ASSOCIATING",
     "DISASSOCIATED",
     "DISASSOCIATING",
```

### Comparing `types-aiobotocore-worklink-2.9.0/types_aiobotocore_worklink/literals.pyi` & `types-aiobotocore-worklink-2.9.1/types_aiobotocore_worklink/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-worklink-2.9.0/types_aiobotocore_worklink/type_defs.py` & `types-aiobotocore-worklink-2.9.1/types_aiobotocore_worklink/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssociateDomainRequestRequestTypeDef",
     "AssociateWebsiteAuthorizationProviderRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociateWebsiteCertificateAuthorityRequestRequestTypeDef",
     "CreateFleetRequestRequestTypeDef",
     "DeleteFleetRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-worklink-2.9.0/types_aiobotocore_worklink/type_defs.pyi` & `types-aiobotocore-worklink-2.9.1/types_aiobotocore_worklink/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-worklink-2.9.0/types_aiobotocore_worklink.egg-info/PKG-INFO` & `types-aiobotocore-worklink-2.9.1/types_aiobotocore_worklink.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-worklink
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.WorkLink 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.WorkLink 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink/
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
 
 <a id="types-aiobotocore-worklink"></a>
 
 # types-aiobotocore-worklink
 
 [![PyPI - types-aiobotocore-worklink](https://img.shields.io/pypi/v/types-aiobotocore-worklink.svg?color=blue)](https://pypi.org/project/types-aiobotocore-worklink)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-worklink.svg?color=blue)](https://pypi.org/project/types-aiobotocore-worklink)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-worklink)](https://pepy.tech/project/types-aiobotocore-worklink)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WorkLink 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink)
+[aiobotocore.WorkLink 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink)
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
 [types-aiobotocore-worklink docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-worklink-2.9.0/types_aiobotocore_worklink.egg-info/SOURCES.txt` & `types-aiobotocore-worklink-2.9.1/types_aiobotocore_worklink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

