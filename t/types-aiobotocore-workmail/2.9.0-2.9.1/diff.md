# Comparing `tmp/types-aiobotocore-workmail-2.9.0.tar.gz` & `tmp/types-aiobotocore-workmail-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-workmail-2.9.0.tar", last modified: Wed Dec 13 20:00:47 2023, max compression
+gzip compressed data, was "types-aiobotocore-workmail-2.9.1.tar", last modified: Thu Jan 18 01:22:03 2024, max compression
```

## Comparing `types-aiobotocore-workmail-2.9.0.tar` & `types-aiobotocore-workmail-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:47.120995 types-aiobotocore-workmail-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:58:00.000000 types-aiobotocore-workmail-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14212 2023-12-13 20:00:47.120995 types-aiobotocore-workmail-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12645 2023-12-13 19:58:00.000000 types-aiobotocore-workmail-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:47.120995 types-aiobotocore-workmail-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-12-13 19:58:00.000000 types-aiobotocore-workmail-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:47.120995 types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail/
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2023-12-13 19:58:00.000000 types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2023-12-13 19:58:00.000000 types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-12-13 19:58:00.000000 types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    64117 2023-12-13 19:58:01.000000 types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    64113 2023-12-13 19:58:01.000000 types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10743 2023-12-13 19:58:01.000000 types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10741 2023-12-13 19:58:01.000000 types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11382 2023-12-13 19:58:01.000000 types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11371 2023-12-13 19:58:01.000000 types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:00.000000 types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    52721 2023-12-13 19:58:02.000000 types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    52720 2023-12-13 19:58:02.000000 types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:58:00.000000 types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:47.120995 types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14212 2023-12-13 20:00:47.000000 types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-12-13 20:00:47.000000 types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:47.000000 types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:47.000000 types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:47.000000 types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-13 20:00:47.000000 types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:03.980965 types-aiobotocore-workmail-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:19:29.000000 types-aiobotocore-workmail-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14232 2024-01-18 01:22:03.980965 types-aiobotocore-workmail-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12645 2024-01-18 01:19:29.000000 types-aiobotocore-workmail-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:22:03.980965 types-aiobotocore-workmail-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-18 01:19:29.000000 types-aiobotocore-workmail-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:03.980965 types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail/
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-01-18 01:19:29.000000 types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-01-18 01:19:29.000000 types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-01-18 01:19:29.000000 types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64141 2024-01-18 01:19:29.000000 types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64138 2024-01-18 01:19:29.000000 types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-01-18 01:19:30.000000 types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-01-18 01:19:30.000000 types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11385 2024-01-18 01:19:29.000000 types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-01-18 01:19:29.000000 types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:29.000000 types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    52720 2024-01-18 01:19:31.000000 types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52720 2024-01-18 01:19:30.000000 types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:19:29.000000 types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:03.980965 types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14232 2024-01-18 01:22:03.000000 types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-01-18 01:22:03.000000 types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:22:03.000000 types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:22:03.000000 types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:22:03.000000 types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-18 01:22:03.000000 types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-workmail-2.9.0/LICENSE` & `types-aiobotocore-workmail-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-workmail-2.9.0/PKG-INFO` & `types-aiobotocore-workmail-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-workmail
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.WorkMail 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.WorkMail 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/
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
 
 <a id="types-aiobotocore-workmail"></a>
 
 # types-aiobotocore-workmail
 
 [![PyPI - types-aiobotocore-workmail](https://img.shields.io/pypi/v/types-aiobotocore-workmail.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workmail)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-workmail.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workmail)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-workmail)](https://pepy.tech/project/types-aiobotocore-workmail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WorkMail 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
+[aiobotocore.WorkMail 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
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
 [types-aiobotocore-workmail docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-workmail-2.9.0/README.md` & `types-aiobotocore-workmail-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-workmail.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workmail)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-workmail)](https://pepy.tech/project/types-aiobotocore-workmail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WorkMail 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
+[aiobotocore.WorkMail 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
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
 [types-aiobotocore-workmail docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-workmail-2.9.0/setup.py` & `types-aiobotocore-workmail-2.9.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-workmail",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_workmail"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.WorkMail 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.WorkMail 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore workmail type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_workmail": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail/__init__.py` & `types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
     ListResourceDelegatesPaginator,
     ListResourcesPaginator,
     ListUsersPaginator,
 )
 
 Client = WorkMailClient
 
-
 __all__ = (
     "Client",
     "ListAliasesPaginator",
     "ListAvailabilityConfigurationsPaginator",
     "ListGroupMembersPaginator",
     "ListGroupsPaginator",
     "ListMailboxPermissionsPaginator",
```

### Comparing `types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail/__init__.pyi` & `types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail/__main__.py` & `types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.WorkMail 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.WorkMail 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail\nOther"
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

### Comparing `types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail/client.py` & `types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("WorkMailClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -226,15 +225,15 @@
     async def create_availability_configuration(
         self,
         *,
         OrganizationId: str,
         DomainName: str,
         ClientToken: str = ...,
         EwsProvider: EwsAvailabilityProviderTypeDef = ...,
-        LambdaProvider: LambdaAvailabilityProviderTypeDef = ...
+        LambdaProvider: LambdaAvailabilityProviderTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Creates an `AvailabilityConfiguration` for the given WorkMail organization and
         domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.create_availability_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#create_availability_configuration)
@@ -255,15 +254,15 @@
         self,
         *,
         OrganizationId: str,
         Name: str,
         Type: ImpersonationRoleTypeType,
         Rules: Sequence[ImpersonationRuleTypeDef],
         ClientToken: str = ...,
-        Description: str = ...
+        Description: str = ...,
     ) -> CreateImpersonationRoleResponseTypeDef:
         """
         Creates an impersonation role for the given WorkMail organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.create_impersonation_role)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#create_impersonation_role)
         """
@@ -279,15 +278,15 @@
         DeviceTypes: Sequence[str] = ...,
         NotDeviceTypes: Sequence[str] = ...,
         DeviceModels: Sequence[str] = ...,
         NotDeviceModels: Sequence[str] = ...,
         DeviceOperatingSystems: Sequence[str] = ...,
         NotDeviceOperatingSystems: Sequence[str] = ...,
         DeviceUserAgents: Sequence[str] = ...,
-        NotDeviceUserAgents: Sequence[str] = ...
+        NotDeviceUserAgents: Sequence[str] = ...,
     ) -> CreateMobileDeviceAccessRuleResponseTypeDef:
         """
         Creates a new mobile device access rule for the specified WorkMail organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.create_mobile_device_access_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#create_mobile_device_access_rule)
         """
@@ -296,15 +295,15 @@
         self,
         *,
         Alias: str,
         DirectoryId: str = ...,
         ClientToken: str = ...,
         Domains: Sequence[DomainTypeDef] = ...,
         KmsKeyArn: str = ...,
-        EnableInteroperability: bool = ...
+        EnableInteroperability: bool = ...,
     ) -> CreateOrganizationResponseTypeDef:
         """
         Creates a new WorkMail organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.create_organization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#create_organization)
         """
@@ -312,15 +311,15 @@
     async def create_resource(
         self,
         *,
         OrganizationId: str,
         Name: str,
         Type: ResourceTypeType,
         Description: str = ...,
-        HiddenFromGlobalAddressList: bool = ...
+        HiddenFromGlobalAddressList: bool = ...,
     ) -> CreateResourceResponseTypeDef:
         """
         Creates a new WorkMail resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.create_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#create_resource)
         """
@@ -331,15 +330,15 @@
         OrganizationId: str,
         Name: str,
         DisplayName: str,
         Password: str = ...,
         Role: UserRoleType = ...,
         FirstName: str = ...,
         LastName: str = ...,
-        HiddenFromGlobalAddressList: bool = ...
+        HiddenFromGlobalAddressList: bool = ...,
     ) -> CreateUserResponseTypeDef:
         """
         Creates a user who can be used in WorkMail by calling the  RegisterToWorkMail
         operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.create_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#create_user)
@@ -434,15 +433,15 @@
 
     async def delete_organization(
         self,
         *,
         OrganizationId: str,
         DeleteDirectory: bool,
         ClientToken: str = ...,
-        ForceDelete: bool = ...
+        ForceDelete: bool = ...,
     ) -> DeleteOrganizationResponseTypeDef:
         """
         Deletes an WorkMail organization and all underlying AWS resources managed by
         WorkMail as part of the
         organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.delete_organization)
@@ -614,15 +613,15 @@
     async def get_access_control_effect(
         self,
         *,
         OrganizationId: str,
         IpAddress: str,
         Action: str,
         UserId: str = ...,
-        ImpersonationRoleId: str = ...
+        ImpersonationRoleId: str = ...,
     ) -> GetAccessControlEffectResponseTypeDef:
         """
         Gets the effects of an organization's access control rules as they apply to a
         specified IPv4 address, access protocol action, and user ID or impersonation
         role
         ID.
 
@@ -685,15 +684,15 @@
     async def get_mobile_device_access_effect(
         self,
         *,
         OrganizationId: str,
         DeviceType: str = ...,
         DeviceModel: str = ...,
         DeviceOperatingSystem: str = ...,
-        DeviceUserAgent: str = ...
+        DeviceUserAgent: str = ...,
     ) -> GetMobileDeviceAccessEffectResponseTypeDef:
         """
         Simulates the effect of the mobile device access rules for the given attributes
         of a sample access
         event.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.get_mobile_device_access_effect)
@@ -754,15 +753,15 @@
 
     async def list_groups(
         self,
         *,
         OrganizationId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Filters: ListGroupsFiltersTypeDef = ...
+        Filters: ListGroupsFiltersTypeDef = ...,
     ) -> ListGroupsResponseTypeDef:
         """
         Returns summaries of the organization's groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.list_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#list_groups)
         """
@@ -770,15 +769,15 @@
     async def list_groups_for_entity(
         self,
         *,
         OrganizationId: str,
         EntityId: str,
         Filters: ListGroupsForEntityFiltersTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListGroupsForEntityResponseTypeDef:
         """
         Returns all the groups to which an entity belongs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.list_groups_for_entity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#list_groups_for_entity)
         """
@@ -829,15 +828,15 @@
     async def list_mobile_device_access_overrides(
         self,
         *,
         OrganizationId: str,
         UserId: str = ...,
         DeviceId: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListMobileDeviceAccessOverridesResponseTypeDef:
         """
         Lists all the mobile device access overrides for any given combination of
         WorkMail organization, user, or
         device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.list_mobile_device_access_overrides)
@@ -876,15 +875,15 @@
 
     async def list_resources(
         self,
         *,
         OrganizationId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Filters: ListResourcesFiltersTypeDef = ...
+        Filters: ListResourcesFiltersTypeDef = ...,
     ) -> ListResourcesResponseTypeDef:
         """
         Returns summaries of the organization's resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.list_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#list_resources)
         """
@@ -901,15 +900,15 @@
 
     async def list_users(
         self,
         *,
         OrganizationId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Filters: ListUsersFiltersTypeDef = ...
+        Filters: ListUsersFiltersTypeDef = ...,
     ) -> ListUsersResponseTypeDef:
         """
         Returns summaries of the organization's users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.list_users)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#list_users)
         """
@@ -924,15 +923,15 @@
         IpRanges: Sequence[str] = ...,
         NotIpRanges: Sequence[str] = ...,
         Actions: Sequence[str] = ...,
         NotActions: Sequence[str] = ...,
         UserIds: Sequence[str] = ...,
         NotUserIds: Sequence[str] = ...,
         ImpersonationRoleIds: Sequence[str] = ...,
-        NotImpersonationRoleIds: Sequence[str] = ...
+        NotImpersonationRoleIds: Sequence[str] = ...,
     ) -> Dict[str, Any]:
         """
         Adds a new access control rule for the specified organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.put_access_control_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#put_access_control_rule)
         """
@@ -960,15 +959,15 @@
 
     async def put_mailbox_permissions(
         self,
         *,
         OrganizationId: str,
         EntityId: str,
         GranteeId: str,
-        PermissionValues: Sequence[PermissionTypeType]
+        PermissionValues: Sequence[PermissionTypeType],
     ) -> Dict[str, Any]:
         """
         Sets permissions for a user, group, or resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.put_mailbox_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#put_mailbox_permissions)
         """
@@ -976,15 +975,15 @@
     async def put_mobile_device_access_override(
         self,
         *,
         OrganizationId: str,
         UserId: str,
         DeviceId: str,
         Effect: MobileDeviceAccessRuleEffectType,
-        Description: str = ...
+        Description: str = ...,
     ) -> Dict[str, Any]:
         """
         Creates or updates a mobile device access override for the given WorkMail
         organization, user, and
         device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.put_mobile_device_access_override)
@@ -994,15 +993,15 @@
     async def put_retention_policy(
         self,
         *,
         OrganizationId: str,
         Name: str,
         FolderConfigurations: Sequence[FolderConfigurationTypeDef],
         Id: str = ...,
-        Description: str = ...
+        Description: str = ...,
     ) -> Dict[str, Any]:
         """
         Puts a retention policy to the specified organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.put_retention_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#put_retention_policy)
         """
@@ -1046,15 +1045,15 @@
         ClientToken: str,
         OrganizationId: str,
         EntityId: str,
         RoleArn: str,
         KmsKeyArn: str,
         S3BucketName: str,
         S3Prefix: str,
-        Description: str = ...
+        Description: str = ...,
     ) -> StartMailboxExportJobResponseTypeDef:
         """
         Starts a mailbox export job to export MIME-format email messages and calendar
         items from the specified mailbox to the specified Amazon Simple Storage Service
         (Amazon S3)
         bucket.
 
@@ -1072,15 +1071,15 @@
 
     async def test_availability_configuration(
         self,
         *,
         OrganizationId: str,
         DomainName: str = ...,
         EwsProvider: EwsAvailabilityProviderTypeDef = ...,
-        LambdaProvider: LambdaAvailabilityProviderTypeDef = ...
+        LambdaProvider: LambdaAvailabilityProviderTypeDef = ...,
     ) -> TestAvailabilityConfigurationResponseTypeDef:
         """
         Performs a test on an availability provider to ensure that access is allowed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.test_availability_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#test_availability_configuration)
         """
@@ -1095,15 +1094,15 @@
 
     async def update_availability_configuration(
         self,
         *,
         OrganizationId: str,
         DomainName: str,
         EwsProvider: EwsAvailabilityProviderTypeDef = ...,
-        LambdaProvider: LambdaAvailabilityProviderTypeDef = ...
+        LambdaProvider: LambdaAvailabilityProviderTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates an existing `AvailabilityConfiguration` for the given WorkMail
         organization and
         domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.update_availability_configuration)
@@ -1134,15 +1133,15 @@
         self,
         *,
         OrganizationId: str,
         ImpersonationRoleId: str,
         Name: str,
         Type: ImpersonationRoleTypeType,
         Rules: Sequence[ImpersonationRuleTypeDef],
-        Description: str = ...
+        Description: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates an impersonation role for the given WorkMail organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.update_impersonation_role)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#update_impersonation_role)
         """
@@ -1168,15 +1167,15 @@
         DeviceTypes: Sequence[str] = ...,
         NotDeviceTypes: Sequence[str] = ...,
         DeviceModels: Sequence[str] = ...,
         NotDeviceModels: Sequence[str] = ...,
         DeviceOperatingSystems: Sequence[str] = ...,
         NotDeviceOperatingSystems: Sequence[str] = ...,
         DeviceUserAgents: Sequence[str] = ...,
-        NotDeviceUserAgents: Sequence[str] = ...
+        NotDeviceUserAgents: Sequence[str] = ...,
     ) -> Dict[str, Any]:
         """
         Updates a mobile device access rule for the specified WorkMail organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.update_mobile_device_access_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#update_mobile_device_access_rule)
         """
@@ -1196,15 +1195,15 @@
         *,
         OrganizationId: str,
         ResourceId: str,
         Name: str = ...,
         BookingOptions: BookingOptionsTypeDef = ...,
         Description: str = ...,
         Type: ResourceTypeType = ...,
-        HiddenFromGlobalAddressList: bool = ...
+        HiddenFromGlobalAddressList: bool = ...,
     ) -> Dict[str, Any]:
         """
         Updates data for the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.update_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#update_resource)
         """
@@ -1224,15 +1223,15 @@
         Street: str = ...,
         JobTitle: str = ...,
         City: str = ...,
         Company: str = ...,
         ZipCode: str = ...,
         Department: str = ...,
         Country: str = ...,
-        Office: str = ...
+        Office: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates data for the user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.update_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#update_user)
         """
```

### Comparing `types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail/client.pyi` & `types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,15 @@
     async def create_availability_configuration(
         self,
         *,
         OrganizationId: str,
         DomainName: str,
         ClientToken: str = ...,
         EwsProvider: EwsAvailabilityProviderTypeDef = ...,
-        LambdaProvider: LambdaAvailabilityProviderTypeDef = ...
+        LambdaProvider: LambdaAvailabilityProviderTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Creates an `AvailabilityConfiguration` for the given WorkMail organization and
         domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.create_availability_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#create_availability_configuration)
@@ -251,15 +251,15 @@
         self,
         *,
         OrganizationId: str,
         Name: str,
         Type: ImpersonationRoleTypeType,
         Rules: Sequence[ImpersonationRuleTypeDef],
         ClientToken: str = ...,
-        Description: str = ...
+        Description: str = ...,
     ) -> CreateImpersonationRoleResponseTypeDef:
         """
         Creates an impersonation role for the given WorkMail organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.create_impersonation_role)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#create_impersonation_role)
         """
@@ -275,15 +275,15 @@
         DeviceTypes: Sequence[str] = ...,
         NotDeviceTypes: Sequence[str] = ...,
         DeviceModels: Sequence[str] = ...,
         NotDeviceModels: Sequence[str] = ...,
         DeviceOperatingSystems: Sequence[str] = ...,
         NotDeviceOperatingSystems: Sequence[str] = ...,
         DeviceUserAgents: Sequence[str] = ...,
-        NotDeviceUserAgents: Sequence[str] = ...
+        NotDeviceUserAgents: Sequence[str] = ...,
     ) -> CreateMobileDeviceAccessRuleResponseTypeDef:
         """
         Creates a new mobile device access rule for the specified WorkMail organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.create_mobile_device_access_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#create_mobile_device_access_rule)
         """
@@ -292,15 +292,15 @@
         self,
         *,
         Alias: str,
         DirectoryId: str = ...,
         ClientToken: str = ...,
         Domains: Sequence[DomainTypeDef] = ...,
         KmsKeyArn: str = ...,
-        EnableInteroperability: bool = ...
+        EnableInteroperability: bool = ...,
     ) -> CreateOrganizationResponseTypeDef:
         """
         Creates a new WorkMail organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.create_organization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#create_organization)
         """
@@ -308,15 +308,15 @@
     async def create_resource(
         self,
         *,
         OrganizationId: str,
         Name: str,
         Type: ResourceTypeType,
         Description: str = ...,
-        HiddenFromGlobalAddressList: bool = ...
+        HiddenFromGlobalAddressList: bool = ...,
     ) -> CreateResourceResponseTypeDef:
         """
         Creates a new WorkMail resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.create_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#create_resource)
         """
@@ -327,15 +327,15 @@
         OrganizationId: str,
         Name: str,
         DisplayName: str,
         Password: str = ...,
         Role: UserRoleType = ...,
         FirstName: str = ...,
         LastName: str = ...,
-        HiddenFromGlobalAddressList: bool = ...
+        HiddenFromGlobalAddressList: bool = ...,
     ) -> CreateUserResponseTypeDef:
         """
         Creates a user who can be used in WorkMail by calling the  RegisterToWorkMail
         operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.create_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#create_user)
@@ -430,15 +430,15 @@
 
     async def delete_organization(
         self,
         *,
         OrganizationId: str,
         DeleteDirectory: bool,
         ClientToken: str = ...,
-        ForceDelete: bool = ...
+        ForceDelete: bool = ...,
     ) -> DeleteOrganizationResponseTypeDef:
         """
         Deletes an WorkMail organization and all underlying AWS resources managed by
         WorkMail as part of the
         organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.delete_organization)
@@ -610,15 +610,15 @@
     async def get_access_control_effect(
         self,
         *,
         OrganizationId: str,
         IpAddress: str,
         Action: str,
         UserId: str = ...,
-        ImpersonationRoleId: str = ...
+        ImpersonationRoleId: str = ...,
     ) -> GetAccessControlEffectResponseTypeDef:
         """
         Gets the effects of an organization's access control rules as they apply to a
         specified IPv4 address, access protocol action, and user ID or impersonation
         role
         ID.
 
@@ -681,15 +681,15 @@
     async def get_mobile_device_access_effect(
         self,
         *,
         OrganizationId: str,
         DeviceType: str = ...,
         DeviceModel: str = ...,
         DeviceOperatingSystem: str = ...,
-        DeviceUserAgent: str = ...
+        DeviceUserAgent: str = ...,
     ) -> GetMobileDeviceAccessEffectResponseTypeDef:
         """
         Simulates the effect of the mobile device access rules for the given attributes
         of a sample access
         event.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.get_mobile_device_access_effect)
@@ -750,15 +750,15 @@
 
     async def list_groups(
         self,
         *,
         OrganizationId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Filters: ListGroupsFiltersTypeDef = ...
+        Filters: ListGroupsFiltersTypeDef = ...,
     ) -> ListGroupsResponseTypeDef:
         """
         Returns summaries of the organization's groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.list_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#list_groups)
         """
@@ -766,15 +766,15 @@
     async def list_groups_for_entity(
         self,
         *,
         OrganizationId: str,
         EntityId: str,
         Filters: ListGroupsForEntityFiltersTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListGroupsForEntityResponseTypeDef:
         """
         Returns all the groups to which an entity belongs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.list_groups_for_entity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#list_groups_for_entity)
         """
@@ -825,15 +825,15 @@
     async def list_mobile_device_access_overrides(
         self,
         *,
         OrganizationId: str,
         UserId: str = ...,
         DeviceId: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListMobileDeviceAccessOverridesResponseTypeDef:
         """
         Lists all the mobile device access overrides for any given combination of
         WorkMail organization, user, or
         device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.list_mobile_device_access_overrides)
@@ -872,15 +872,15 @@
 
     async def list_resources(
         self,
         *,
         OrganizationId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Filters: ListResourcesFiltersTypeDef = ...
+        Filters: ListResourcesFiltersTypeDef = ...,
     ) -> ListResourcesResponseTypeDef:
         """
         Returns summaries of the organization's resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.list_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#list_resources)
         """
@@ -897,15 +897,15 @@
 
     async def list_users(
         self,
         *,
         OrganizationId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Filters: ListUsersFiltersTypeDef = ...
+        Filters: ListUsersFiltersTypeDef = ...,
     ) -> ListUsersResponseTypeDef:
         """
         Returns summaries of the organization's users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.list_users)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#list_users)
         """
@@ -920,15 +920,15 @@
         IpRanges: Sequence[str] = ...,
         NotIpRanges: Sequence[str] = ...,
         Actions: Sequence[str] = ...,
         NotActions: Sequence[str] = ...,
         UserIds: Sequence[str] = ...,
         NotUserIds: Sequence[str] = ...,
         ImpersonationRoleIds: Sequence[str] = ...,
-        NotImpersonationRoleIds: Sequence[str] = ...
+        NotImpersonationRoleIds: Sequence[str] = ...,
     ) -> Dict[str, Any]:
         """
         Adds a new access control rule for the specified organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.put_access_control_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#put_access_control_rule)
         """
@@ -956,15 +956,15 @@
 
     async def put_mailbox_permissions(
         self,
         *,
         OrganizationId: str,
         EntityId: str,
         GranteeId: str,
-        PermissionValues: Sequence[PermissionTypeType]
+        PermissionValues: Sequence[PermissionTypeType],
     ) -> Dict[str, Any]:
         """
         Sets permissions for a user, group, or resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.put_mailbox_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#put_mailbox_permissions)
         """
@@ -972,15 +972,15 @@
     async def put_mobile_device_access_override(
         self,
         *,
         OrganizationId: str,
         UserId: str,
         DeviceId: str,
         Effect: MobileDeviceAccessRuleEffectType,
-        Description: str = ...
+        Description: str = ...,
     ) -> Dict[str, Any]:
         """
         Creates or updates a mobile device access override for the given WorkMail
         organization, user, and
         device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.put_mobile_device_access_override)
@@ -990,15 +990,15 @@
     async def put_retention_policy(
         self,
         *,
         OrganizationId: str,
         Name: str,
         FolderConfigurations: Sequence[FolderConfigurationTypeDef],
         Id: str = ...,
-        Description: str = ...
+        Description: str = ...,
     ) -> Dict[str, Any]:
         """
         Puts a retention policy to the specified organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.put_retention_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#put_retention_policy)
         """
@@ -1042,15 +1042,15 @@
         ClientToken: str,
         OrganizationId: str,
         EntityId: str,
         RoleArn: str,
         KmsKeyArn: str,
         S3BucketName: str,
         S3Prefix: str,
-        Description: str = ...
+        Description: str = ...,
     ) -> StartMailboxExportJobResponseTypeDef:
         """
         Starts a mailbox export job to export MIME-format email messages and calendar
         items from the specified mailbox to the specified Amazon Simple Storage Service
         (Amazon S3)
         bucket.
 
@@ -1068,15 +1068,15 @@
 
     async def test_availability_configuration(
         self,
         *,
         OrganizationId: str,
         DomainName: str = ...,
         EwsProvider: EwsAvailabilityProviderTypeDef = ...,
-        LambdaProvider: LambdaAvailabilityProviderTypeDef = ...
+        LambdaProvider: LambdaAvailabilityProviderTypeDef = ...,
     ) -> TestAvailabilityConfigurationResponseTypeDef:
         """
         Performs a test on an availability provider to ensure that access is allowed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.test_availability_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#test_availability_configuration)
         """
@@ -1091,15 +1091,15 @@
 
     async def update_availability_configuration(
         self,
         *,
         OrganizationId: str,
         DomainName: str,
         EwsProvider: EwsAvailabilityProviderTypeDef = ...,
-        LambdaProvider: LambdaAvailabilityProviderTypeDef = ...
+        LambdaProvider: LambdaAvailabilityProviderTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates an existing `AvailabilityConfiguration` for the given WorkMail
         organization and
         domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.update_availability_configuration)
@@ -1130,15 +1130,15 @@
         self,
         *,
         OrganizationId: str,
         ImpersonationRoleId: str,
         Name: str,
         Type: ImpersonationRoleTypeType,
         Rules: Sequence[ImpersonationRuleTypeDef],
-        Description: str = ...
+        Description: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates an impersonation role for the given WorkMail organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.update_impersonation_role)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#update_impersonation_role)
         """
@@ -1164,15 +1164,15 @@
         DeviceTypes: Sequence[str] = ...,
         NotDeviceTypes: Sequence[str] = ...,
         DeviceModels: Sequence[str] = ...,
         NotDeviceModels: Sequence[str] = ...,
         DeviceOperatingSystems: Sequence[str] = ...,
         NotDeviceOperatingSystems: Sequence[str] = ...,
         DeviceUserAgents: Sequence[str] = ...,
-        NotDeviceUserAgents: Sequence[str] = ...
+        NotDeviceUserAgents: Sequence[str] = ...,
     ) -> Dict[str, Any]:
         """
         Updates a mobile device access rule for the specified WorkMail organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.update_mobile_device_access_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#update_mobile_device_access_rule)
         """
@@ -1192,15 +1192,15 @@
         *,
         OrganizationId: str,
         ResourceId: str,
         Name: str = ...,
         BookingOptions: BookingOptionsTypeDef = ...,
         Description: str = ...,
         Type: ResourceTypeType = ...,
-        HiddenFromGlobalAddressList: bool = ...
+        HiddenFromGlobalAddressList: bool = ...,
     ) -> Dict[str, Any]:
         """
         Updates data for the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.update_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#update_resource)
         """
@@ -1220,15 +1220,15 @@
         Street: str = ...,
         JobTitle: str = ...,
         City: str = ...,
         Company: str = ...,
         ZipCode: str = ...,
         Department: str = ...,
         Country: str = ...,
-        Office: str = ...
+        Office: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates data for the user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.update_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#update_user)
         """
```

### Comparing `types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail/literals.py` & `types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail/literals.py`

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
     "AccessControlRuleEffectType",
     "AccessEffectType",
     "AvailabilityProviderTypeType",
     "DnsRecordVerificationStatusType",
     "EntityStateType",
     "EntityTypeType",
@@ -48,15 +47,14 @@
     "WorkMailServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AccessControlRuleEffectType = Literal["ALLOW", "DENY"]
 AccessEffectType = Literal["ALLOW", "DENY"]
 AvailabilityProviderTypeType = Literal["EWS", "LAMBDA"]
 DnsRecordVerificationStatusType = Literal["FAILED", "PENDING", "VERIFIED"]
 EntityStateType = Literal["DELETED", "DISABLED", "ENABLED"]
 EntityTypeType = Literal["GROUP", "RESOURCE", "USER"]
 FolderNameType = Literal["DELETED_ITEMS", "DRAFTS", "INBOX", "JUNK_EMAIL", "SENT_ITEMS"]
```

### Comparing `types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail/literals.pyi` & `types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail/paginator.py` & `types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,14 @@
     "ListMailboxPermissionsPaginator",
     "ListOrganizationsPaginator",
     "ListResourceDelegatesPaginator",
     "ListResourcesPaginator",
     "ListUsersPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -133,15 +132,15 @@
     """
 
     def paginate(
         self,
         *,
         OrganizationId: str,
         Filters: ListGroupsFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/paginators/#listgroupspaginator)
         """
 
 
@@ -182,15 +181,15 @@
     """
 
     def paginate(
         self,
         *,
         OrganizationId: str,
         ResourceId: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResourceDelegatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListResourceDelegates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/paginators/#listresourcedelegatespaginator)
         """
 
 
@@ -201,15 +200,15 @@
     """
 
     def paginate(
         self,
         *,
         OrganizationId: str,
         Filters: ListResourcesFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/paginators/#listresourcespaginator)
         """
 
 
@@ -220,13 +219,13 @@
     """
 
     def paginate(
         self,
         *,
         OrganizationId: str,
         Filters: ListUsersFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/paginators/#listuserspaginator)
         """
```

### Comparing `types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail/paginator.pyi` & `types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     """
 
     def paginate(
         self,
         *,
         OrganizationId: str,
         Filters: ListGroupsFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/paginators/#listgroupspaginator)
         """
 
 class ListMailboxPermissionsPaginator(AioPaginator):
@@ -173,15 +173,15 @@
     """
 
     def paginate(
         self,
         *,
         OrganizationId: str,
         ResourceId: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResourceDelegatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListResourceDelegates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/paginators/#listresourcedelegatespaginator)
         """
 
 class ListResourcesPaginator(AioPaginator):
@@ -191,15 +191,15 @@
     """
 
     def paginate(
         self,
         *,
         OrganizationId: str,
         Filters: ListResourcesFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/paginators/#listresourcespaginator)
         """
 
 class ListUsersPaginator(AioPaginator):
@@ -209,13 +209,13 @@
     """
 
     def paginate(
         self,
         *,
         OrganizationId: str,
         Filters: ListUsersFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/paginators/#listuserspaginator)
         """
```

### Comparing `types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail/type_defs.py` & `types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccessControlRuleTypeDef",
     "AssociateDelegateToResourceRequestRequestTypeDef",
     "AssociateMemberToGroupRequestRequestTypeDef",
     "AssumeImpersonationRoleRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "LambdaAvailabilityProviderTypeDef",
```

### Comparing `types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail/type_defs.pyi` & `types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail.egg-info/PKG-INFO` & `types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-workmail
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.WorkMail 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.WorkMail 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/
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
 
 <a id="types-aiobotocore-workmail"></a>
 
 # types-aiobotocore-workmail
 
 [![PyPI - types-aiobotocore-workmail](https://img.shields.io/pypi/v/types-aiobotocore-workmail.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workmail)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-workmail.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workmail)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-workmail)](https://pepy.tech/project/types-aiobotocore-workmail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WorkMail 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
+[aiobotocore.WorkMail 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
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
 [types-aiobotocore-workmail docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-workmail-2.9.0/types_aiobotocore_workmail.egg-info/SOURCES.txt` & `types-aiobotocore-workmail-2.9.1/types_aiobotocore_workmail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

