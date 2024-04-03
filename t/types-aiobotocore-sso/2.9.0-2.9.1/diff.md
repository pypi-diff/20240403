# Comparing `tmp/types-aiobotocore-sso-2.9.0.tar.gz` & `tmp/types-aiobotocore-sso-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sso-2.9.0.tar", last modified: Wed Dec 13 20:00:37 2023, max compression
+gzip compressed data, was "types-aiobotocore-sso-2.9.1.tar", last modified: Thu Jan 18 01:21:55 2024, max compression
```

## Comparing `types-aiobotocore-sso-2.9.0.tar` & `types-aiobotocore-sso-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:37.421078 types-aiobotocore-sso-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:57:00.000000 types-aiobotocore-sso-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12856 2023-12-13 20:00:37.421078 types-aiobotocore-sso-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11309 2023-12-13 19:57:00.000000 types-aiobotocore-sso-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:37.421078 types-aiobotocore-sso-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-12-13 19:57:00.000000 types-aiobotocore-sso-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:37.421078 types-aiobotocore-sso-2.9.0/types_aiobotocore_sso/
--rw-r--r--   0 runner    (1001) docker     (127)      800 2023-12-13 19:57:00.000000 types-aiobotocore-sso-2.9.0/types_aiobotocore_sso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2023-12-13 19:57:00.000000 types-aiobotocore-sso-2.9.0/types_aiobotocore_sso/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-13 19:57:00.000000 types-aiobotocore-sso-2.9.0/types_aiobotocore_sso/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7384 2023-12-13 19:57:00.000000 types-aiobotocore-sso-2.9.0/types_aiobotocore_sso/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7380 2023-12-13 19:57:00.000000 types-aiobotocore-sso-2.9.0/types_aiobotocore_sso/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8863 2023-12-13 19:57:00.000000 types-aiobotocore-sso-2.9.0/types_aiobotocore_sso/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8861 2023-12-13 19:57:00.000000 types-aiobotocore-sso-2.9.0/types_aiobotocore_sso/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2023-12-13 19:57:00.000000 types-aiobotocore-sso-2.9.0/types_aiobotocore_sso/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2023-12-13 19:57:00.000000 types-aiobotocore-sso-2.9.0/types_aiobotocore_sso/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:57:00.000000 types-aiobotocore-sso-2.9.0/types_aiobotocore_sso/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4234 2023-12-13 19:57:00.000000 types-aiobotocore-sso-2.9.0/types_aiobotocore_sso/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4233 2023-12-13 19:57:00.000000 types-aiobotocore-sso-2.9.0/types_aiobotocore_sso/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:57:00.000000 types-aiobotocore-sso-2.9.0/types_aiobotocore_sso/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:37.421078 types-aiobotocore-sso-2.9.0/types_aiobotocore_sso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12856 2023-12-13 20:00:37.000000 types-aiobotocore-sso-2.9.0/types_aiobotocore_sso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      737 2023-12-13 20:00:37.000000 types-aiobotocore-sso-2.9.0/types_aiobotocore_sso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:37.000000 types-aiobotocore-sso-2.9.0/types_aiobotocore_sso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:37.000000 types-aiobotocore-sso-2.9.0/types_aiobotocore_sso.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:37.000000 types-aiobotocore-sso-2.9.0/types_aiobotocore_sso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 20:00:37.000000 types-aiobotocore-sso-2.9.0/types_aiobotocore_sso.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:55.133006 types-aiobotocore-sso-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:18:27.000000 types-aiobotocore-sso-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12876 2024-01-18 01:21:55.133006 types-aiobotocore-sso-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11309 2024-01-18 01:18:27.000000 types-aiobotocore-sso-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:55.133006 types-aiobotocore-sso-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-01-18 01:18:27.000000 types-aiobotocore-sso-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:55.133006 types-aiobotocore-sso-2.9.1/types_aiobotocore_sso/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-01-18 01:18:27.000000 types-aiobotocore-sso-2.9.1/types_aiobotocore_sso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-01-18 01:18:27.000000 types-aiobotocore-sso-2.9.1/types_aiobotocore_sso/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-18 01:18:27.000000 types-aiobotocore-sso-2.9.1/types_aiobotocore_sso/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7383 2024-01-18 01:18:27.000000 types-aiobotocore-sso-2.9.1/types_aiobotocore_sso/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-01-18 01:18:27.000000 types-aiobotocore-sso-2.9.1/types_aiobotocore_sso/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8861 2024-01-18 01:18:27.000000 types-aiobotocore-sso-2.9.1/types_aiobotocore_sso/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8861 2024-01-18 01:18:27.000000 types-aiobotocore-sso-2.9.1/types_aiobotocore_sso/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-01-18 01:18:27.000000 types-aiobotocore-sso-2.9.1/types_aiobotocore_sso/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-01-18 01:18:27.000000 types-aiobotocore-sso-2.9.1/types_aiobotocore_sso/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:18:27.000000 types-aiobotocore-sso-2.9.1/types_aiobotocore_sso/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-01-18 01:18:27.000000 types-aiobotocore-sso-2.9.1/types_aiobotocore_sso/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-01-18 01:18:27.000000 types-aiobotocore-sso-2.9.1/types_aiobotocore_sso/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:18:27.000000 types-aiobotocore-sso-2.9.1/types_aiobotocore_sso/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:55.133006 types-aiobotocore-sso-2.9.1/types_aiobotocore_sso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12876 2024-01-18 01:21:55.000000 types-aiobotocore-sso-2.9.1/types_aiobotocore_sso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-01-18 01:21:55.000000 types-aiobotocore-sso-2.9.1/types_aiobotocore_sso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:55.000000 types-aiobotocore-sso-2.9.1/types_aiobotocore_sso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:55.000000 types-aiobotocore-sso-2.9.1/types_aiobotocore_sso.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:55.000000 types-aiobotocore-sso-2.9.1/types_aiobotocore_sso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:21:55.000000 types-aiobotocore-sso-2.9.1/types_aiobotocore_sso.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sso-2.9.0/LICENSE` & `types-aiobotocore-sso-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-sso-2.9.0/PKG-INFO` & `types-aiobotocore-sso-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sso
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SSO 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SSO 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/
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
 
 <a id="types-aiobotocore-sso"></a>
 
 # types-aiobotocore-sso
 
 [![PyPI - types-aiobotocore-sso](https://img.shields.io/pypi/v/types-aiobotocore-sso.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sso)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sso.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sso)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sso)](https://pepy.tech/project/types-aiobotocore-sso)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SSO 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
+[aiobotocore.SSO 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
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
 [types-aiobotocore-sso docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-sso-2.9.0/README.md` & `types-aiobotocore-sso-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sso.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sso)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sso)](https://pepy.tech/project/types-aiobotocore-sso)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SSO 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
+[aiobotocore.SSO 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
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
 [types-aiobotocore-sso docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-sso-2.9.0/setup.py` & `types-aiobotocore-sso-2.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sso",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_sso"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SSO 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.SSO 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore sso type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_sso": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-sso-2.9.0/types_aiobotocore_sso/__init__.py` & `types-aiobotocore-sso-2.9.1/types_aiobotocore_sso/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,9 +24,8 @@
 """
 
 from .client import SSOClient
 from .paginator import ListAccountRolesPaginator, ListAccountsPaginator
 
 Client = SSOClient
 
-
 __all__ = ("Client", "ListAccountRolesPaginator", "ListAccountsPaginator", "SSOClient")
```

### Comparing `types-aiobotocore-sso-2.9.0/types_aiobotocore_sso/__init__.pyi` & `types-aiobotocore-sso-2.9.1/types_aiobotocore_sso/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-2.9.0/types_aiobotocore_sso/__main__.py` & `types-aiobotocore-sso-2.9.1/types_aiobotocore_sso/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SSO 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.SSO 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO\nOther"
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

### Comparing `types-aiobotocore-sso-2.9.0/types_aiobotocore_sso/client.py` & `types-aiobotocore-sso-2.9.1/types_aiobotocore_sso/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SSOClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
```

### Comparing `types-aiobotocore-sso-2.9.0/types_aiobotocore_sso/client.pyi` & `types-aiobotocore-sso-2.9.1/types_aiobotocore_sso/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-2.9.0/types_aiobotocore_sso/literals.py` & `types-aiobotocore-sso-2.9.1/types_aiobotocore_sso/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,26 +15,24 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListAccountRolesPaginatorName",
     "ListAccountsPaginatorName",
     "SSOServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ListAccountRolesPaginatorName = Literal["list_account_roles"]
 ListAccountsPaginatorName = Literal["list_accounts"]
 SSOServiceName = Literal["sso"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
```

### Comparing `types-aiobotocore-sso-2.9.0/types_aiobotocore_sso/literals.pyi` & `types-aiobotocore-sso-2.9.1/types_aiobotocore_sso/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-2.9.0/types_aiobotocore_sso/paginator.py` & `types-aiobotocore-sso-2.9.1/types_aiobotocore_sso/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     ListAccountRolesResponseTypeDef,
     ListAccountsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListAccountRolesPaginator", "ListAccountsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-sso-2.9.0/types_aiobotocore_sso/paginator.pyi` & `types-aiobotocore-sso-2.9.1/types_aiobotocore_sso/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-2.9.0/types_aiobotocore_sso/type_defs.py` & `types-aiobotocore-sso-2.9.1/types_aiobotocore_sso/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountInfoTypeDef",
     "ResponseMetadataTypeDef",
     "GetRoleCredentialsRequestRequestTypeDef",
     "RoleCredentialsTypeDef",
     "PaginatorConfigTypeDef",
     "ListAccountRolesRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-sso-2.9.0/types_aiobotocore_sso/type_defs.pyi` & `types-aiobotocore-sso-2.9.1/types_aiobotocore_sso/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-2.9.0/types_aiobotocore_sso.egg-info/PKG-INFO` & `types-aiobotocore-sso-2.9.1/types_aiobotocore_sso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sso
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SSO 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SSO 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/
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
 
 <a id="types-aiobotocore-sso"></a>
 
 # types-aiobotocore-sso
 
 [![PyPI - types-aiobotocore-sso](https://img.shields.io/pypi/v/types-aiobotocore-sso.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sso)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sso.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sso)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sso)](https://pepy.tech/project/types-aiobotocore-sso)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SSO 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
+[aiobotocore.SSO 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
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
 [types-aiobotocore-sso docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-sso-2.9.0/types_aiobotocore_sso.egg-info/SOURCES.txt` & `types-aiobotocore-sso-2.9.1/types_aiobotocore_sso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

