# Comparing `tmp/types-aiobotocore-cognito-identity-2.9.0.tar.gz` & `tmp/types-aiobotocore-cognito-identity-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cognito-identity-2.9.0.tar", last modified: Wed Dec 13 19:58:57 2023, max compression
+gzip compressed data, was "types-aiobotocore-cognito-identity-2.9.1.tar", last modified: Thu Jan 18 01:20:23 2024, max compression
```

## Comparing `types-aiobotocore-cognito-identity-2.9.0.tar` & `types-aiobotocore-cognito-identity-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:57.065912 types-aiobotocore-cognito-identity-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:43:02.000000 types-aiobotocore-cognito-identity-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13532 2023-12-13 19:58:57.065912 types-aiobotocore-cognito-identity-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11934 2023-12-13 19:43:02.000000 types-aiobotocore-cognito-identity-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:57.065912 types-aiobotocore-cognito-identity-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2023-12-13 19:43:02.000000 types-aiobotocore-cognito-identity-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:57.065912 types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2023-12-13 19:43:02.000000 types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2023-12-13 19:43:02.000000 types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      966 2023-12-13 19:43:02.000000 types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21160 2023-12-13 19:43:02.000000 types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    21156 2023-12-13 19:43:02.000000 types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9150 2023-12-13 19:43:02.000000 types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9148 2023-12-13 19:43:02.000000 types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2023-12-13 19:43:02.000000 types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2023-12-13 19:43:02.000000 types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:43:02.000000 types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    15072 2023-12-13 19:43:03.000000 types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15071 2023-12-13 19:43:03.000000 types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:43:02.000000 types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:57.065912 types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13532 2023-12-13 19:58:57.000000 types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      984 2023-12-13 19:58:57.000000 types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:57.000000 types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:57.000000 types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:57.000000 types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-13 19:58:57.000000 types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:23.193430 types-aiobotocore-cognito-identity-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:04:59.000000 types-aiobotocore-cognito-identity-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13552 2024-01-18 01:20:23.193430 types-aiobotocore-cognito-identity-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11934 2024-01-18 01:04:59.000000 types-aiobotocore-cognito-identity-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:23.193430 types-aiobotocore-cognito-identity-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-01-18 01:04:59.000000 types-aiobotocore-cognito-identity-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:23.193430 types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity/
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-01-18 01:04:59.000000 types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-01-18 01:04:59.000000 types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-01-18 01:04:59.000000 types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21168 2024-01-18 01:04:59.000000 types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21165 2024-01-18 01:04:59.000000 types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9148 2024-01-18 01:04:59.000000 types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9148 2024-01-18 01:04:59.000000 types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-01-18 01:04:59.000000 types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-01-18 01:04:59.000000 types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:04:59.000000 types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    15071 2024-01-18 01:04:59.000000 types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15071 2024-01-18 01:04:59.000000 types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:04:59.000000 types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:23.193430 types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13552 2024-01-18 01:20:23.000000 types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-18 01:20:23.000000 types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:23.000000 types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:23.000000 types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:23.000000 types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-18 01:20:23.000000 types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cognito-identity-2.9.0/LICENSE` & `types-aiobotocore-cognito-identity-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-cognito-identity-2.9.0/PKG-INFO` & `types-aiobotocore-cognito-identity-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cognito-identity
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CognitoIdentity 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CognitoIdentity 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/
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
 
 <a id="types-aiobotocore-cognito-identity"></a>
 
 # types-aiobotocore-cognito-identity
 
 [![PyPI - types-aiobotocore-cognito-identity](https://img.shields.io/pypi/v/types-aiobotocore-cognito-identity.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-identity)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cognito-identity.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-identity)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cognito-identity)](https://pepy.tech/project/types-aiobotocore-cognito-identity)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CognitoIdentity 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
+[aiobotocore.CognitoIdentity 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
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
 [types-aiobotocore-cognito-identity docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cognito-identity-2.9.0/README.md` & `types-aiobotocore-cognito-identity-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cognito-identity.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-identity)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cognito-identity)](https://pepy.tech/project/types-aiobotocore-cognito-identity)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CognitoIdentity 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
+[aiobotocore.CognitoIdentity 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
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
 [types-aiobotocore-cognito-identity docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cognito-identity-2.9.0/setup.py` & `types-aiobotocore-cognito-identity-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cognito-identity",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_cognito_identity"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CognitoIdentity 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.CognitoIdentity 2.9.1 service generated with"
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
     keywords="aiobotocore cognito-identity type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_cognito_identity": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity/__init__.py` & `types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,9 +22,8 @@
 """
 
 from .client import CognitoIdentityClient
 from .paginator import ListIdentityPoolsPaginator
 
 Client = CognitoIdentityClient
 
-
 __all__ = ("Client", "CognitoIdentityClient", "ListIdentityPoolsPaginator")
```

### Comparing `types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity/__init__.pyi` & `types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity/__main__.py` & `types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CognitoIdentity 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CognitoIdentity 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity\nOther"
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

### Comparing `types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity/client.py` & `types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CognitoIdentityClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -115,15 +114,15 @@
         AllowUnauthenticatedIdentities: bool,
         AllowClassicFlow: bool = ...,
         SupportedLoginProviders: Mapping[str, str] = ...,
         DeveloperProviderName: str = ...,
         OpenIdConnectProviderARNs: Sequence[str] = ...,
         CognitoIdentityProviders: Sequence[CognitoIdentityProviderTypeDef] = ...,
         SamlProviderARNs: Sequence[str] = ...,
-        IdentityPoolTags: Mapping[str, str] = ...
+        IdentityPoolTags: Mapping[str, str] = ...,
     ) -> IdentityPoolTypeDef:
         """
         Creates a new identity pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.create_identity_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/client/#create_identity_pool)
         """
@@ -223,15 +222,15 @@
     async def get_open_id_token_for_developer_identity(
         self,
         *,
         IdentityPoolId: str,
         Logins: Mapping[str, str],
         IdentityId: str = ...,
         PrincipalTags: Mapping[str, str] = ...,
-        TokenDuration: int = ...
+        TokenDuration: int = ...,
     ) -> GetOpenIdTokenForDeveloperIdentityResponseTypeDef:
         """
         Registers (or retrieves) a Cognito `IdentityId` and an OpenID Connect token for
         a user authenticated by your backend authentication
         process.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.get_open_id_token_for_developer_identity)
@@ -252,15 +251,15 @@
 
     async def list_identities(
         self,
         *,
         IdentityPoolId: str,
         MaxResults: int,
         NextToken: str = ...,
-        HideDisabled: bool = ...
+        HideDisabled: bool = ...,
     ) -> ListIdentitiesResponseTypeDef:
         """
         Lists the identities in an identity pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.list_identities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/client/#list_identities)
         """
@@ -288,15 +287,15 @@
     async def lookup_developer_identity(
         self,
         *,
         IdentityPoolId: str,
         IdentityId: str = ...,
         DeveloperUserIdentifier: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> LookupDeveloperIdentityResponseTypeDef:
         """
         Retrieves the `IdentityID` associated with a `DeveloperUserIdentifier` or the
         list of `DeveloperUserIdentifier` values associated with an `IdentityId` for an
         existing
         identity.
 
@@ -306,15 +305,15 @@
 
     async def merge_developer_identities(
         self,
         *,
         SourceUserIdentifier: str,
         DestinationUserIdentifier: str,
         DeveloperProviderName: str,
-        IdentityPoolId: str
+        IdentityPoolId: str,
     ) -> MergeDeveloperIdentitiesResponseTypeDef:
         """
         Merges two users having different `IdentityId`s, existing in the same identity
         pool, and identified by the same developer
         provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.merge_developer_identities)
@@ -322,30 +321,30 @@
         """
 
     async def set_identity_pool_roles(
         self,
         *,
         IdentityPoolId: str,
         Roles: Mapping[str, str],
-        RoleMappings: Mapping[str, RoleMappingTypeDef] = ...
+        RoleMappings: Mapping[str, RoleMappingTypeDef] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets the roles for an identity pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.set_identity_pool_roles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/client/#set_identity_pool_roles)
         """
 
     async def set_principal_tag_attribute_map(
         self,
         *,
         IdentityPoolId: str,
         IdentityProviderName: str,
         UseDefaults: bool = ...,
-        PrincipalTags: Mapping[str, str] = ...
+        PrincipalTags: Mapping[str, str] = ...,
     ) -> SetPrincipalTagAttributeMapResponseTypeDef:
         """
         You can use this operation to use default (username and clientID) attribute or
         custom attribute
         mappings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.set_principal_tag_attribute_map)
@@ -362,15 +361,15 @@
 
     async def unlink_developer_identity(
         self,
         *,
         IdentityId: str,
         IdentityPoolId: str,
         DeveloperProviderName: str,
-        DeveloperUserIdentifier: str
+        DeveloperUserIdentifier: str,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Unlinks a `DeveloperUserIdentifier` from an existing identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.unlink_developer_identity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/client/#unlink_developer_identity)
         """
@@ -401,15 +400,15 @@
         AllowUnauthenticatedIdentities: bool,
         AllowClassicFlow: bool = ...,
         SupportedLoginProviders: Mapping[str, str] = ...,
         DeveloperProviderName: str = ...,
         OpenIdConnectProviderARNs: Sequence[str] = ...,
         CognitoIdentityProviders: Sequence[CognitoIdentityProviderTypeDef] = ...,
         SamlProviderARNs: Sequence[str] = ...,
-        IdentityPoolTags: Mapping[str, str] = ...
+        IdentityPoolTags: Mapping[str, str] = ...,
     ) -> IdentityPoolTypeDef:
         """
         Updates an identity pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.update_identity_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/client/#update_identity_pool)
         """
```

### Comparing `types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity/client.pyi` & `types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         AllowUnauthenticatedIdentities: bool,
         AllowClassicFlow: bool = ...,
         SupportedLoginProviders: Mapping[str, str] = ...,
         DeveloperProviderName: str = ...,
         OpenIdConnectProviderARNs: Sequence[str] = ...,
         CognitoIdentityProviders: Sequence[CognitoIdentityProviderTypeDef] = ...,
         SamlProviderARNs: Sequence[str] = ...,
-        IdentityPoolTags: Mapping[str, str] = ...
+        IdentityPoolTags: Mapping[str, str] = ...,
     ) -> IdentityPoolTypeDef:
         """
         Creates a new identity pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.create_identity_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/client/#create_identity_pool)
         """
@@ -219,15 +219,15 @@
     async def get_open_id_token_for_developer_identity(
         self,
         *,
         IdentityPoolId: str,
         Logins: Mapping[str, str],
         IdentityId: str = ...,
         PrincipalTags: Mapping[str, str] = ...,
-        TokenDuration: int = ...
+        TokenDuration: int = ...,
     ) -> GetOpenIdTokenForDeveloperIdentityResponseTypeDef:
         """
         Registers (or retrieves) a Cognito `IdentityId` and an OpenID Connect token for
         a user authenticated by your backend authentication
         process.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.get_open_id_token_for_developer_identity)
@@ -248,15 +248,15 @@
 
     async def list_identities(
         self,
         *,
         IdentityPoolId: str,
         MaxResults: int,
         NextToken: str = ...,
-        HideDisabled: bool = ...
+        HideDisabled: bool = ...,
     ) -> ListIdentitiesResponseTypeDef:
         """
         Lists the identities in an identity pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.list_identities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/client/#list_identities)
         """
@@ -284,15 +284,15 @@
     async def lookup_developer_identity(
         self,
         *,
         IdentityPoolId: str,
         IdentityId: str = ...,
         DeveloperUserIdentifier: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> LookupDeveloperIdentityResponseTypeDef:
         """
         Retrieves the `IdentityID` associated with a `DeveloperUserIdentifier` or the
         list of `DeveloperUserIdentifier` values associated with an `IdentityId` for an
         existing
         identity.
 
@@ -302,15 +302,15 @@
 
     async def merge_developer_identities(
         self,
         *,
         SourceUserIdentifier: str,
         DestinationUserIdentifier: str,
         DeveloperProviderName: str,
-        IdentityPoolId: str
+        IdentityPoolId: str,
     ) -> MergeDeveloperIdentitiesResponseTypeDef:
         """
         Merges two users having different `IdentityId`s, existing in the same identity
         pool, and identified by the same developer
         provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.merge_developer_identities)
@@ -318,30 +318,30 @@
         """
 
     async def set_identity_pool_roles(
         self,
         *,
         IdentityPoolId: str,
         Roles: Mapping[str, str],
-        RoleMappings: Mapping[str, RoleMappingTypeDef] = ...
+        RoleMappings: Mapping[str, RoleMappingTypeDef] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets the roles for an identity pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.set_identity_pool_roles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/client/#set_identity_pool_roles)
         """
 
     async def set_principal_tag_attribute_map(
         self,
         *,
         IdentityPoolId: str,
         IdentityProviderName: str,
         UseDefaults: bool = ...,
-        PrincipalTags: Mapping[str, str] = ...
+        PrincipalTags: Mapping[str, str] = ...,
     ) -> SetPrincipalTagAttributeMapResponseTypeDef:
         """
         You can use this operation to use default (username and clientID) attribute or
         custom attribute
         mappings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.set_principal_tag_attribute_map)
@@ -358,15 +358,15 @@
 
     async def unlink_developer_identity(
         self,
         *,
         IdentityId: str,
         IdentityPoolId: str,
         DeveloperProviderName: str,
-        DeveloperUserIdentifier: str
+        DeveloperUserIdentifier: str,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Unlinks a `DeveloperUserIdentifier` from an existing identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.unlink_developer_identity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/client/#unlink_developer_identity)
         """
@@ -397,15 +397,15 @@
         AllowUnauthenticatedIdentities: bool,
         AllowClassicFlow: bool = ...,
         SupportedLoginProviders: Mapping[str, str] = ...,
         DeveloperProviderName: str = ...,
         OpenIdConnectProviderARNs: Sequence[str] = ...,
         CognitoIdentityProviders: Sequence[CognitoIdentityProviderTypeDef] = ...,
         SamlProviderARNs: Sequence[str] = ...,
-        IdentityPoolTags: Mapping[str, str] = ...
+        IdentityPoolTags: Mapping[str, str] = ...,
     ) -> IdentityPoolTypeDef:
         """
         Updates an identity pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.update_identity_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/client/#update_identity_pool)
         """
```

### Comparing `types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity/literals.py` & `types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,29 +15,27 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AmbiguousRoleResolutionTypeType",
     "ErrorCodeType",
     "ListIdentityPoolsPaginatorName",
     "MappingRuleMatchTypeType",
     "RoleMappingTypeType",
     "CognitoIdentityServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AmbiguousRoleResolutionTypeType = Literal["AuthenticatedRole", "Deny"]
 ErrorCodeType = Literal["AccessDenied", "InternalServerError"]
 ListIdentityPoolsPaginatorName = Literal["list_identity_pools"]
 MappingRuleMatchTypeType = Literal["Contains", "Equals", "NotEqual", "StartsWith"]
 RoleMappingTypeType = Literal["Rules", "Token"]
 CognitoIdentityServiceName = Literal["cognito-identity"]
 ServiceName = Literal[
```

### Comparing `types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity/literals.pyi` & `types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity/paginator.py` & `types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import ListIdentityPoolsResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListIdentityPoolsPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity/paginator.pyi` & `types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity/type_defs.py` & `types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CognitoIdentityProviderTypeDef",
     "CredentialsTypeDef",
     "DeleteIdentitiesInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "UnprocessedIdentityIdTypeDef",
     "DeleteIdentityPoolInputRequestTypeDef",
```

### Comparing `types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity/type_defs.pyi` & `types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity.egg-info/PKG-INFO` & `types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cognito-identity
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CognitoIdentity 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CognitoIdentity 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/
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
 
 <a id="types-aiobotocore-cognito-identity"></a>
 
 # types-aiobotocore-cognito-identity
 
 [![PyPI - types-aiobotocore-cognito-identity](https://img.shields.io/pypi/v/types-aiobotocore-cognito-identity.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-identity)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cognito-identity.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-identity)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cognito-identity)](https://pepy.tech/project/types-aiobotocore-cognito-identity)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CognitoIdentity 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
+[aiobotocore.CognitoIdentity 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
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
 [types-aiobotocore-cognito-identity docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cognito-identity-2.9.0/types_aiobotocore_cognito_identity.egg-info/SOURCES.txt` & `types-aiobotocore-cognito-identity-2.9.1/types_aiobotocore_cognito_identity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

