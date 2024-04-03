# Comparing `tmp/types-aiobotocore-cognito-idp-2.9.0.tar.gz` & `tmp/types-aiobotocore-cognito-idp-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cognito-idp-2.9.0.tar", last modified: Wed Dec 13 19:58:57 2023, max compression
+gzip compressed data, was "types-aiobotocore-cognito-idp-2.9.1.tar", last modified: Thu Jan 18 01:20:23 2024, max compression
```

## Comparing `types-aiobotocore-cognito-idp-2.9.0.tar` & `types-aiobotocore-cognito-idp-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:57.437909 types-aiobotocore-cognito-idp-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:43:04.000000 types-aiobotocore-cognito-idp-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14579 2023-12-13 19:58:57.437909 types-aiobotocore-cognito-idp-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12988 2023-12-13 19:43:04.000000 types-aiobotocore-cognito-idp-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:57.437909 types-aiobotocore-cognito-idp-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2023-12-13 19:43:04.000000 types-aiobotocore-cognito-idp-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:57.433909 types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp/
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2023-12-13 19:43:04.000000 types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2023-12-13 19:43:04.000000 types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      972 2023-12-13 19:43:04.000000 types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    83745 2023-12-13 19:43:05.000000 types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    83741 2023-12-13 19:43:04.000000 types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14365 2023-12-13 19:43:05.000000 types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14363 2023-12-13 19:43:05.000000 types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11574 2023-12-13 19:43:05.000000 types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11563 2023-12-13 19:43:05.000000 types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:43:04.000000 types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    81010 2023-12-13 19:43:07.000000 types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    81009 2023-12-13 19:43:06.000000 types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:43:04.000000 types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:57.437909 types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14579 2023-12-13 19:58:57.000000 types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      889 2023-12-13 19:58:57.000000 types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:57.000000 types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:57.000000 types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:57.000000 types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 19:58:57.000000 types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:23.533428 types-aiobotocore-cognito-idp-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:05:00.000000 types-aiobotocore-cognito-idp-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14599 2024-01-18 01:20:23.529428 types-aiobotocore-cognito-idp-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12988 2024-01-18 01:05:00.000000 types-aiobotocore-cognito-idp-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:23.533428 types-aiobotocore-cognito-idp-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-01-18 01:05:00.000000 types-aiobotocore-cognito-idp-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:23.529428 types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp/
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-01-18 01:05:00.000000 types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-01-18 01:05:00.000000 types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-01-18 01:05:00.000000 types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83778 2024-01-18 01:05:02.000000 types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83775 2024-01-18 01:05:00.000000 types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14363 2024-01-18 01:05:02.000000 types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14363 2024-01-18 01:05:02.000000 types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11574 2024-01-18 01:05:02.000000 types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11564 2024-01-18 01:05:02.000000 types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:05:00.000000 types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    81009 2024-01-18 01:05:03.000000 types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81009 2024-01-18 01:05:03.000000 types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:05:00.000000 types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:23.529428 types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14599 2024-01-18 01:20:23.000000 types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-01-18 01:20:23.000000 types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:23.000000 types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:23.000000 types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:23.000000 types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-18 01:20:23.000000 types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cognito-idp-2.9.0/LICENSE` & `types-aiobotocore-cognito-idp-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-cognito-idp-2.9.0/PKG-INFO` & `types-aiobotocore-cognito-idp-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cognito-idp
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CognitoIdentityProvider 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CognitoIdentityProvider 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/
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
 
 <a id="types-aiobotocore-cognito-idp"></a>
 
 # types-aiobotocore-cognito-idp
 
 [![PyPI - types-aiobotocore-cognito-idp](https://img.shields.io/pypi/v/types-aiobotocore-cognito-idp.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-idp)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cognito-idp.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-idp)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cognito-idp)](https://pepy.tech/project/types-aiobotocore-cognito-idp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CognitoIdentityProvider 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
+[aiobotocore.CognitoIdentityProvider 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
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
 [types-aiobotocore-cognito-idp docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cognito-idp-2.9.0/README.md` & `types-aiobotocore-cognito-idp-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cognito-idp.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-idp)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cognito-idp)](https://pepy.tech/project/types-aiobotocore-cognito-idp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CognitoIdentityProvider 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
+[aiobotocore.CognitoIdentityProvider 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
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
 [types-aiobotocore-cognito-idp docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cognito-idp-2.9.0/setup.py` & `types-aiobotocore-cognito-idp-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cognito-idp",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_cognito_idp"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CognitoIdentityProvider 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.CognitoIdentityProvider 2.9.1 service generated with"
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
     keywords="aiobotocore cognito-idp type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_cognito_idp": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp/__init__.py` & `types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
     ListUserPoolsPaginator,
     ListUsersInGroupPaginator,
     ListUsersPaginator,
 )
 
 Client = CognitoIdentityProviderClient
 
-
 __all__ = (
     "AdminListGroupsForUserPaginator",
     "AdminListUserAuthEventsPaginator",
     "Client",
     "CognitoIdentityProviderClient",
     "ListGroupsPaginator",
     "ListIdentityProvidersPaginator",
```

### Comparing `types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp/__init__.pyi` & `types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp/__main__.py` & `types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CognitoIdentityProvider 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CognitoIdentityProvider 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider\nOther"
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

### Comparing `types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp/client.py` & `types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CognitoIdentityProviderClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -263,15 +262,15 @@
         Username: str,
         UserAttributes: Sequence[AttributeTypeTypeDef] = ...,
         ValidationData: Sequence[AttributeTypeTypeDef] = ...,
         TemporaryPassword: str = ...,
         ForceAliasCreation: bool = ...,
         MessageAction: MessageActionTypeType = ...,
         DesiredDeliveryMediums: Sequence[DeliveryMediumTypeType] = ...,
-        ClientMetadata: Mapping[str, str] = ...
+        ClientMetadata: Mapping[str, str] = ...,
     ) -> AdminCreateUserResponseTypeDef:
         """
         Creates a new user in the specified user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_create_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#admin_create_user)
         """
@@ -359,29 +358,29 @@
         *,
         UserPoolId: str,
         ClientId: str,
         AuthFlow: AuthFlowTypeType,
         AuthParameters: Mapping[str, str] = ...,
         ClientMetadata: Mapping[str, str] = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
-        ContextData: ContextDataTypeTypeDef = ...
+        ContextData: ContextDataTypeTypeDef = ...,
     ) -> AdminInitiateAuthResponseTypeDef:
         """
         Initiates the authentication flow, as an administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_initiate_auth)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#admin_initiate_auth)
         """
 
     async def admin_link_provider_for_user(
         self,
         *,
         UserPoolId: str,
         DestinationUser: ProviderUserIdentifierTypeTypeDef,
-        SourceUser: ProviderUserIdentifierTypeTypeDef
+        SourceUser: ProviderUserIdentifierTypeTypeDef,
     ) -> Dict[str, Any]:
         """
         Links an existing user account in a user pool ( `DestinationUser`) to an
         identity from an external IdP ( `SourceUser`) based on a specified attribute
         name and value from the external
         IdP.
 
@@ -447,30 +446,30 @@
         UserPoolId: str,
         ClientId: str,
         ChallengeName: ChallengeNameTypeType,
         ChallengeResponses: Mapping[str, str] = ...,
         Session: str = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         ContextData: ContextDataTypeTypeDef = ...,
-        ClientMetadata: Mapping[str, str] = ...
+        ClientMetadata: Mapping[str, str] = ...,
     ) -> AdminRespondToAuthChallengeResponseTypeDef:
         """
         Responds to an authentication challenge, as an administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_respond_to_auth_challenge)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#admin_respond_to_auth_challenge)
         """
 
     async def admin_set_user_mfa_preference(
         self,
         *,
         Username: str,
         UserPoolId: str,
         SMSMfaSettings: SMSMfaSettingsTypeTypeDef = ...,
-        SoftwareTokenMfaSettings: SoftwareTokenMfaSettingsTypeTypeDef = ...
+        SoftwareTokenMfaSettings: SoftwareTokenMfaSettingsTypeTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         The user's multi-factor authentication (MFA) preference, including which MFA
         options are activated, and if any are
         preferred.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_set_user_mfa_preference)
@@ -510,30 +509,30 @@
 
     async def admin_update_device_status(
         self,
         *,
         UserPoolId: str,
         Username: str,
         DeviceKey: str,
-        DeviceRememberedStatus: DeviceRememberedStatusTypeType = ...
+        DeviceRememberedStatus: DeviceRememberedStatusTypeType = ...,
     ) -> Dict[str, Any]:
         """
         Updates the device status as an administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_update_device_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#admin_update_device_status)
         """
 
     async def admin_update_user_attributes(
         self,
         *,
         UserPoolId: str,
         Username: str,
         UserAttributes: Sequence[AttributeTypeTypeDef],
-        ClientMetadata: Mapping[str, str] = ...
+        ClientMetadata: Mapping[str, str] = ...,
     ) -> Dict[str, Any]:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_update_user_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#admin_update_user_attributes)
         """
@@ -587,15 +586,15 @@
 
     async def confirm_device(
         self,
         *,
         AccessToken: str,
         DeviceKey: str,
         DeviceSecretVerifierConfig: DeviceSecretVerifierConfigTypeTypeDef = ...,
-        DeviceName: str = ...
+        DeviceName: str = ...,
     ) -> ConfirmDeviceResponseTypeDef:
         """
         Confirms tracking of the device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.confirm_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#confirm_device)
         """
@@ -606,15 +605,15 @@
         ClientId: str,
         Username: str,
         ConfirmationCode: str,
         Password: str,
         SecretHash: str = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         UserContextData: UserContextDataTypeTypeDef = ...,
-        ClientMetadata: Mapping[str, str] = ...
+        ClientMetadata: Mapping[str, str] = ...,
     ) -> Dict[str, Any]:
         """
         Allows a user to enter a confirmation code to reset a forgotten password.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.confirm_forgot_password)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#confirm_forgot_password)
         """
@@ -625,15 +624,15 @@
         ClientId: str,
         Username: str,
         ConfirmationCode: str,
         SecretHash: str = ...,
         ForceAliasCreation: bool = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         UserContextData: UserContextDataTypeTypeDef = ...,
-        ClientMetadata: Mapping[str, str] = ...
+        ClientMetadata: Mapping[str, str] = ...,
     ) -> Dict[str, Any]:
         """
         Confirms registration of a new user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.confirm_sign_up)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#confirm_sign_up)
         """
@@ -641,15 +640,15 @@
     async def create_group(
         self,
         *,
         GroupName: str,
         UserPoolId: str,
         Description: str = ...,
         RoleArn: str = ...,
-        Precedence: int = ...
+        Precedence: int = ...,
     ) -> CreateGroupResponseTypeDef:
         """
         Creates a new group in the specified user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#create_group)
         """
@@ -658,30 +657,30 @@
         self,
         *,
         UserPoolId: str,
         ProviderName: str,
         ProviderType: IdentityProviderTypeTypeType,
         ProviderDetails: Mapping[str, str],
         AttributeMapping: Mapping[str, str] = ...,
-        IdpIdentifiers: Sequence[str] = ...
+        IdpIdentifiers: Sequence[str] = ...,
     ) -> CreateIdentityProviderResponseTypeDef:
         """
         Creates an IdP for a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_identity_provider)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#create_identity_provider)
         """
 
     async def create_resource_server(
         self,
         *,
         UserPoolId: str,
         Identifier: str,
         Name: str,
-        Scopes: Sequence[ResourceServerScopeTypeTypeDef] = ...
+        Scopes: Sequence[ResourceServerScopeTypeTypeDef] = ...,
     ) -> CreateResourceServerResponseTypeDef:
         """
         Creates a new OAuth2.0 resource server and defines custom scopes within it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_resource_server)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#create_resource_server)
         """
@@ -717,15 +716,15 @@
         EmailConfiguration: EmailConfigurationTypeTypeDef = ...,
         SmsConfiguration: SmsConfigurationTypeTypeDef = ...,
         UserPoolTags: Mapping[str, str] = ...,
         AdminCreateUserConfig: AdminCreateUserConfigTypeTypeDef = ...,
         Schema: Sequence[SchemaAttributeTypeTypeDef] = ...,
         UserPoolAddOns: UserPoolAddOnsTypeTypeDef = ...,
         UsernameConfiguration: UsernameConfigurationTypeTypeDef = ...,
-        AccountRecoverySetting: AccountRecoverySettingTypeTypeDef = ...
+        AccountRecoverySetting: AccountRecoverySettingTypeTypeDef = ...,
     ) -> CreateUserPoolResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_user_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#create_user_pool)
         """
@@ -750,29 +749,29 @@
         AllowedOAuthFlows: Sequence[OAuthFlowTypeType] = ...,
         AllowedOAuthScopes: Sequence[str] = ...,
         AllowedOAuthFlowsUserPoolClient: bool = ...,
         AnalyticsConfiguration: AnalyticsConfigurationTypeTypeDef = ...,
         PreventUserExistenceErrors: PreventUserExistenceErrorTypesType = ...,
         EnableTokenRevocation: bool = ...,
         EnablePropagateAdditionalUserContextData: bool = ...,
-        AuthSessionValidity: int = ...
+        AuthSessionValidity: int = ...,
     ) -> CreateUserPoolClientResponseTypeDef:
         """
         Creates the user pool client.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_user_pool_client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#create_user_pool_client)
         """
 
     async def create_user_pool_domain(
         self,
         *,
         Domain: str,
         UserPoolId: str,
-        CustomDomainConfig: CustomDomainConfigTypeTypeDef = ...
+        CustomDomainConfig: CustomDomainConfigTypeTypeDef = ...,
     ) -> CreateUserPoolDomainResponseTypeDef:
         """
         Creates a new domain for a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_user_pool_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#create_user_pool_domain)
         """
@@ -935,15 +934,15 @@
         self,
         *,
         ClientId: str,
         Username: str,
         SecretHash: str = ...,
         UserContextData: UserContextDataTypeTypeDef = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
-        ClientMetadata: Mapping[str, str] = ...
+        ClientMetadata: Mapping[str, str] = ...,
     ) -> ForgotPasswordResponseTypeDef:
         """
         Calling this API causes a message to be sent to the end user with a
         confirmation code that is required to change the user's
         password.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.forgot_password)
@@ -1074,15 +1073,15 @@
         self,
         *,
         AuthFlow: AuthFlowTypeType,
         ClientId: str,
         AuthParameters: Mapping[str, str] = ...,
         ClientMetadata: Mapping[str, str] = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
-        UserContextData: UserContextDataTypeTypeDef = ...
+        UserContextData: UserContextDataTypeTypeDef = ...,
     ) -> InitiateAuthResponseTypeDef:
         """
         Initiates sign-in for a user in the Amazon Cognito user directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.initiate_auth)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#initiate_auth)
         """
@@ -1171,15 +1170,15 @@
     async def list_users(
         self,
         *,
         UserPoolId: str,
         AttributesToGet: Sequence[str] = ...,
         Limit: int = ...,
         PaginationToken: str = ...,
-        Filter: str = ...
+        Filter: str = ...,
     ) -> ListUsersResponseTypeDef:
         """
         Lists users and their basic details in a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_users)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#list_users)
         """
@@ -1198,15 +1197,15 @@
         self,
         *,
         ClientId: str,
         Username: str,
         SecretHash: str = ...,
         UserContextData: UserContextDataTypeTypeDef = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
-        ClientMetadata: Mapping[str, str] = ...
+        ClientMetadata: Mapping[str, str] = ...,
     ) -> ResendConfirmationCodeResponseTypeDef:
         """
         Resends the confirmation (for confirmation of registration) to a specific user
         in the user
         pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.resend_confirmation_code)
@@ -1218,15 +1217,15 @@
         *,
         ClientId: str,
         ChallengeName: ChallengeNameTypeType,
         Session: str = ...,
         ChallengeResponses: Mapping[str, str] = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         UserContextData: UserContextDataTypeTypeDef = ...,
-        ClientMetadata: Mapping[str, str] = ...
+        ClientMetadata: Mapping[str, str] = ...,
     ) -> RespondToAuthChallengeResponseTypeDef:
         """
         Responds to the authentication challenge.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.respond_to_auth_challenge)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#respond_to_auth_challenge)
         """
@@ -1256,15 +1255,15 @@
     async def set_risk_configuration(
         self,
         *,
         UserPoolId: str,
         ClientId: str = ...,
         CompromisedCredentialsRiskConfiguration: CompromisedCredentialsRiskConfigurationTypeTypeDef = ...,
         AccountTakeoverRiskConfiguration: AccountTakeoverRiskConfigurationTypeTypeDef = ...,
-        RiskExceptionConfiguration: RiskExceptionConfigurationTypeTypeDef = ...
+        RiskExceptionConfiguration: RiskExceptionConfigurationTypeTypeDef = ...,
     ) -> SetRiskConfigurationResponseTypeDef:
         """
         Configures actions on detected risks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.set_risk_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#set_risk_configuration)
         """
@@ -1282,15 +1281,15 @@
         """
 
     async def set_user_mfa_preference(
         self,
         *,
         AccessToken: str,
         SMSMfaSettings: SMSMfaSettingsTypeTypeDef = ...,
-        SoftwareTokenMfaSettings: SoftwareTokenMfaSettingsTypeTypeDef = ...
+        SoftwareTokenMfaSettings: SoftwareTokenMfaSettingsTypeTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Set the user's multi-factor authentication (MFA) method preference, including
         which MFA factors are activated and if any are
         preferred.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.set_user_mfa_preference)
@@ -1299,15 +1298,15 @@
 
     async def set_user_pool_mfa_config(
         self,
         *,
         UserPoolId: str,
         SmsMfaConfiguration: SmsMfaConfigTypeTypeDef = ...,
         SoftwareTokenMfaConfiguration: SoftwareTokenMfaConfigTypeTypeDef = ...,
-        MfaConfiguration: UserPoolMfaTypeType = ...
+        MfaConfiguration: UserPoolMfaTypeType = ...,
     ) -> SetUserPoolMfaConfigResponseTypeDef:
         """
         Sets the user pool multi-factor authentication (MFA) configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.set_user_pool_mfa_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#set_user_pool_mfa_config)
         """
@@ -1329,15 +1328,15 @@
         Username: str,
         Password: str,
         SecretHash: str = ...,
         UserAttributes: Sequence[AttributeTypeTypeDef] = ...,
         ValidationData: Sequence[AttributeTypeTypeDef] = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         UserContextData: UserContextDataTypeTypeDef = ...,
-        ClientMetadata: Mapping[str, str] = ...
+        ClientMetadata: Mapping[str, str] = ...,
     ) -> SignUpResponseTypeDef:
         """
         Registers the user in the specified user pool and creates a user name,
         password, and user
         attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.sign_up)
@@ -1383,15 +1382,15 @@
     async def update_auth_event_feedback(
         self,
         *,
         UserPoolId: str,
         Username: str,
         EventId: str,
         FeedbackToken: str,
-        FeedbackValue: FeedbackValueTypeType
+        FeedbackValue: FeedbackValueTypeType,
     ) -> Dict[str, Any]:
         """
         Provides the feedback for an authentication event, whether it was from a valid
         user or
         not.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_auth_event_feedback)
@@ -1399,15 +1398,15 @@
         """
 
     async def update_device_status(
         self,
         *,
         AccessToken: str,
         DeviceKey: str,
-        DeviceRememberedStatus: DeviceRememberedStatusTypeType = ...
+        DeviceRememberedStatus: DeviceRememberedStatusTypeType = ...,
     ) -> Dict[str, Any]:
         """
         Updates the device status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_device_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#update_device_status)
         """
@@ -1415,15 +1414,15 @@
     async def update_group(
         self,
         *,
         GroupName: str,
         UserPoolId: str,
         Description: str = ...,
         RoleArn: str = ...,
-        Precedence: int = ...
+        Precedence: int = ...,
     ) -> UpdateGroupResponseTypeDef:
         """
         Updates the specified group with the specified attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#update_group)
         """
@@ -1431,44 +1430,44 @@
     async def update_identity_provider(
         self,
         *,
         UserPoolId: str,
         ProviderName: str,
         ProviderDetails: Mapping[str, str] = ...,
         AttributeMapping: Mapping[str, str] = ...,
-        IdpIdentifiers: Sequence[str] = ...
+        IdpIdentifiers: Sequence[str] = ...,
     ) -> UpdateIdentityProviderResponseTypeDef:
         """
         Updates IdP information for a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_identity_provider)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#update_identity_provider)
         """
 
     async def update_resource_server(
         self,
         *,
         UserPoolId: str,
         Identifier: str,
         Name: str,
-        Scopes: Sequence[ResourceServerScopeTypeTypeDef] = ...
+        Scopes: Sequence[ResourceServerScopeTypeTypeDef] = ...,
     ) -> UpdateResourceServerResponseTypeDef:
         """
         Updates the name and scopes of resource server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_resource_server)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#update_resource_server)
         """
 
     async def update_user_attributes(
         self,
         *,
         UserAttributes: Sequence[AttributeTypeTypeDef],
         AccessToken: str,
-        ClientMetadata: Mapping[str, str] = ...
+        ClientMetadata: Mapping[str, str] = ...,
     ) -> UpdateUserAttributesResponseTypeDef:
         """
         Allows a user to update a specific attribute (one at a time).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_user_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#update_user_attributes)
         """
@@ -1490,15 +1489,15 @@
         MfaConfiguration: UserPoolMfaTypeType = ...,
         DeviceConfiguration: DeviceConfigurationTypeTypeDef = ...,
         EmailConfiguration: EmailConfigurationTypeTypeDef = ...,
         SmsConfiguration: SmsConfigurationTypeTypeDef = ...,
         UserPoolTags: Mapping[str, str] = ...,
         AdminCreateUserConfig: AdminCreateUserConfigTypeTypeDef = ...,
         UserPoolAddOns: UserPoolAddOnsTypeTypeDef = ...,
-        AccountRecoverySetting: AccountRecoverySettingTypeTypeDef = ...
+        AccountRecoverySetting: AccountRecoverySettingTypeTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_user_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#update_user_pool)
         """
@@ -1523,15 +1522,15 @@
         AllowedOAuthFlows: Sequence[OAuthFlowTypeType] = ...,
         AllowedOAuthScopes: Sequence[str] = ...,
         AllowedOAuthFlowsUserPoolClient: bool = ...,
         AnalyticsConfiguration: AnalyticsConfigurationTypeTypeDef = ...,
         PreventUserExistenceErrors: PreventUserExistenceErrorTypesType = ...,
         EnableTokenRevocation: bool = ...,
         EnablePropagateAdditionalUserContextData: bool = ...,
-        AuthSessionValidity: int = ...
+        AuthSessionValidity: int = ...,
     ) -> UpdateUserPoolClientResponseTypeDef:
         """
         Updates the specified user pool app client with the specified attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_user_pool_client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#update_user_pool_client)
         """
@@ -1550,15 +1549,15 @@
 
     async def verify_software_token(
         self,
         *,
         UserCode: str,
         AccessToken: str = ...,
         Session: str = ...,
-        FriendlyDeviceName: str = ...
+        FriendlyDeviceName: str = ...,
     ) -> VerifySoftwareTokenResponseTypeDef:
         """
         Use this API to register a user's entered time-based one-time password (TOTP)
         code and mark the user's software token MFA status as "verified" if
         successful.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.verify_software_token)
```

### Comparing `types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp/client.pyi` & `types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -259,15 +259,15 @@
         Username: str,
         UserAttributes: Sequence[AttributeTypeTypeDef] = ...,
         ValidationData: Sequence[AttributeTypeTypeDef] = ...,
         TemporaryPassword: str = ...,
         ForceAliasCreation: bool = ...,
         MessageAction: MessageActionTypeType = ...,
         DesiredDeliveryMediums: Sequence[DeliveryMediumTypeType] = ...,
-        ClientMetadata: Mapping[str, str] = ...
+        ClientMetadata: Mapping[str, str] = ...,
     ) -> AdminCreateUserResponseTypeDef:
         """
         Creates a new user in the specified user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_create_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#admin_create_user)
         """
@@ -355,29 +355,29 @@
         *,
         UserPoolId: str,
         ClientId: str,
         AuthFlow: AuthFlowTypeType,
         AuthParameters: Mapping[str, str] = ...,
         ClientMetadata: Mapping[str, str] = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
-        ContextData: ContextDataTypeTypeDef = ...
+        ContextData: ContextDataTypeTypeDef = ...,
     ) -> AdminInitiateAuthResponseTypeDef:
         """
         Initiates the authentication flow, as an administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_initiate_auth)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#admin_initiate_auth)
         """
 
     async def admin_link_provider_for_user(
         self,
         *,
         UserPoolId: str,
         DestinationUser: ProviderUserIdentifierTypeTypeDef,
-        SourceUser: ProviderUserIdentifierTypeTypeDef
+        SourceUser: ProviderUserIdentifierTypeTypeDef,
     ) -> Dict[str, Any]:
         """
         Links an existing user account in a user pool ( `DestinationUser`) to an
         identity from an external IdP ( `SourceUser`) based on a specified attribute
         name and value from the external
         IdP.
 
@@ -443,30 +443,30 @@
         UserPoolId: str,
         ClientId: str,
         ChallengeName: ChallengeNameTypeType,
         ChallengeResponses: Mapping[str, str] = ...,
         Session: str = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         ContextData: ContextDataTypeTypeDef = ...,
-        ClientMetadata: Mapping[str, str] = ...
+        ClientMetadata: Mapping[str, str] = ...,
     ) -> AdminRespondToAuthChallengeResponseTypeDef:
         """
         Responds to an authentication challenge, as an administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_respond_to_auth_challenge)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#admin_respond_to_auth_challenge)
         """
 
     async def admin_set_user_mfa_preference(
         self,
         *,
         Username: str,
         UserPoolId: str,
         SMSMfaSettings: SMSMfaSettingsTypeTypeDef = ...,
-        SoftwareTokenMfaSettings: SoftwareTokenMfaSettingsTypeTypeDef = ...
+        SoftwareTokenMfaSettings: SoftwareTokenMfaSettingsTypeTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         The user's multi-factor authentication (MFA) preference, including which MFA
         options are activated, and if any are
         preferred.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_set_user_mfa_preference)
@@ -506,30 +506,30 @@
 
     async def admin_update_device_status(
         self,
         *,
         UserPoolId: str,
         Username: str,
         DeviceKey: str,
-        DeviceRememberedStatus: DeviceRememberedStatusTypeType = ...
+        DeviceRememberedStatus: DeviceRememberedStatusTypeType = ...,
     ) -> Dict[str, Any]:
         """
         Updates the device status as an administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_update_device_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#admin_update_device_status)
         """
 
     async def admin_update_user_attributes(
         self,
         *,
         UserPoolId: str,
         Username: str,
         UserAttributes: Sequence[AttributeTypeTypeDef],
-        ClientMetadata: Mapping[str, str] = ...
+        ClientMetadata: Mapping[str, str] = ...,
     ) -> Dict[str, Any]:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_update_user_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#admin_update_user_attributes)
         """
@@ -583,15 +583,15 @@
 
     async def confirm_device(
         self,
         *,
         AccessToken: str,
         DeviceKey: str,
         DeviceSecretVerifierConfig: DeviceSecretVerifierConfigTypeTypeDef = ...,
-        DeviceName: str = ...
+        DeviceName: str = ...,
     ) -> ConfirmDeviceResponseTypeDef:
         """
         Confirms tracking of the device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.confirm_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#confirm_device)
         """
@@ -602,15 +602,15 @@
         ClientId: str,
         Username: str,
         ConfirmationCode: str,
         Password: str,
         SecretHash: str = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         UserContextData: UserContextDataTypeTypeDef = ...,
-        ClientMetadata: Mapping[str, str] = ...
+        ClientMetadata: Mapping[str, str] = ...,
     ) -> Dict[str, Any]:
         """
         Allows a user to enter a confirmation code to reset a forgotten password.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.confirm_forgot_password)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#confirm_forgot_password)
         """
@@ -621,15 +621,15 @@
         ClientId: str,
         Username: str,
         ConfirmationCode: str,
         SecretHash: str = ...,
         ForceAliasCreation: bool = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         UserContextData: UserContextDataTypeTypeDef = ...,
-        ClientMetadata: Mapping[str, str] = ...
+        ClientMetadata: Mapping[str, str] = ...,
     ) -> Dict[str, Any]:
         """
         Confirms registration of a new user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.confirm_sign_up)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#confirm_sign_up)
         """
@@ -637,15 +637,15 @@
     async def create_group(
         self,
         *,
         GroupName: str,
         UserPoolId: str,
         Description: str = ...,
         RoleArn: str = ...,
-        Precedence: int = ...
+        Precedence: int = ...,
     ) -> CreateGroupResponseTypeDef:
         """
         Creates a new group in the specified user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#create_group)
         """
@@ -654,30 +654,30 @@
         self,
         *,
         UserPoolId: str,
         ProviderName: str,
         ProviderType: IdentityProviderTypeTypeType,
         ProviderDetails: Mapping[str, str],
         AttributeMapping: Mapping[str, str] = ...,
-        IdpIdentifiers: Sequence[str] = ...
+        IdpIdentifiers: Sequence[str] = ...,
     ) -> CreateIdentityProviderResponseTypeDef:
         """
         Creates an IdP for a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_identity_provider)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#create_identity_provider)
         """
 
     async def create_resource_server(
         self,
         *,
         UserPoolId: str,
         Identifier: str,
         Name: str,
-        Scopes: Sequence[ResourceServerScopeTypeTypeDef] = ...
+        Scopes: Sequence[ResourceServerScopeTypeTypeDef] = ...,
     ) -> CreateResourceServerResponseTypeDef:
         """
         Creates a new OAuth2.0 resource server and defines custom scopes within it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_resource_server)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#create_resource_server)
         """
@@ -713,15 +713,15 @@
         EmailConfiguration: EmailConfigurationTypeTypeDef = ...,
         SmsConfiguration: SmsConfigurationTypeTypeDef = ...,
         UserPoolTags: Mapping[str, str] = ...,
         AdminCreateUserConfig: AdminCreateUserConfigTypeTypeDef = ...,
         Schema: Sequence[SchemaAttributeTypeTypeDef] = ...,
         UserPoolAddOns: UserPoolAddOnsTypeTypeDef = ...,
         UsernameConfiguration: UsernameConfigurationTypeTypeDef = ...,
-        AccountRecoverySetting: AccountRecoverySettingTypeTypeDef = ...
+        AccountRecoverySetting: AccountRecoverySettingTypeTypeDef = ...,
     ) -> CreateUserPoolResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_user_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#create_user_pool)
         """
@@ -746,29 +746,29 @@
         AllowedOAuthFlows: Sequence[OAuthFlowTypeType] = ...,
         AllowedOAuthScopes: Sequence[str] = ...,
         AllowedOAuthFlowsUserPoolClient: bool = ...,
         AnalyticsConfiguration: AnalyticsConfigurationTypeTypeDef = ...,
         PreventUserExistenceErrors: PreventUserExistenceErrorTypesType = ...,
         EnableTokenRevocation: bool = ...,
         EnablePropagateAdditionalUserContextData: bool = ...,
-        AuthSessionValidity: int = ...
+        AuthSessionValidity: int = ...,
     ) -> CreateUserPoolClientResponseTypeDef:
         """
         Creates the user pool client.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_user_pool_client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#create_user_pool_client)
         """
 
     async def create_user_pool_domain(
         self,
         *,
         Domain: str,
         UserPoolId: str,
-        CustomDomainConfig: CustomDomainConfigTypeTypeDef = ...
+        CustomDomainConfig: CustomDomainConfigTypeTypeDef = ...,
     ) -> CreateUserPoolDomainResponseTypeDef:
         """
         Creates a new domain for a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_user_pool_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#create_user_pool_domain)
         """
@@ -931,15 +931,15 @@
         self,
         *,
         ClientId: str,
         Username: str,
         SecretHash: str = ...,
         UserContextData: UserContextDataTypeTypeDef = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
-        ClientMetadata: Mapping[str, str] = ...
+        ClientMetadata: Mapping[str, str] = ...,
     ) -> ForgotPasswordResponseTypeDef:
         """
         Calling this API causes a message to be sent to the end user with a
         confirmation code that is required to change the user's
         password.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.forgot_password)
@@ -1070,15 +1070,15 @@
         self,
         *,
         AuthFlow: AuthFlowTypeType,
         ClientId: str,
         AuthParameters: Mapping[str, str] = ...,
         ClientMetadata: Mapping[str, str] = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
-        UserContextData: UserContextDataTypeTypeDef = ...
+        UserContextData: UserContextDataTypeTypeDef = ...,
     ) -> InitiateAuthResponseTypeDef:
         """
         Initiates sign-in for a user in the Amazon Cognito user directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.initiate_auth)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#initiate_auth)
         """
@@ -1167,15 +1167,15 @@
     async def list_users(
         self,
         *,
         UserPoolId: str,
         AttributesToGet: Sequence[str] = ...,
         Limit: int = ...,
         PaginationToken: str = ...,
-        Filter: str = ...
+        Filter: str = ...,
     ) -> ListUsersResponseTypeDef:
         """
         Lists users and their basic details in a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_users)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#list_users)
         """
@@ -1194,15 +1194,15 @@
         self,
         *,
         ClientId: str,
         Username: str,
         SecretHash: str = ...,
         UserContextData: UserContextDataTypeTypeDef = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
-        ClientMetadata: Mapping[str, str] = ...
+        ClientMetadata: Mapping[str, str] = ...,
     ) -> ResendConfirmationCodeResponseTypeDef:
         """
         Resends the confirmation (for confirmation of registration) to a specific user
         in the user
         pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.resend_confirmation_code)
@@ -1214,15 +1214,15 @@
         *,
         ClientId: str,
         ChallengeName: ChallengeNameTypeType,
         Session: str = ...,
         ChallengeResponses: Mapping[str, str] = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         UserContextData: UserContextDataTypeTypeDef = ...,
-        ClientMetadata: Mapping[str, str] = ...
+        ClientMetadata: Mapping[str, str] = ...,
     ) -> RespondToAuthChallengeResponseTypeDef:
         """
         Responds to the authentication challenge.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.respond_to_auth_challenge)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#respond_to_auth_challenge)
         """
@@ -1252,15 +1252,15 @@
     async def set_risk_configuration(
         self,
         *,
         UserPoolId: str,
         ClientId: str = ...,
         CompromisedCredentialsRiskConfiguration: CompromisedCredentialsRiskConfigurationTypeTypeDef = ...,
         AccountTakeoverRiskConfiguration: AccountTakeoverRiskConfigurationTypeTypeDef = ...,
-        RiskExceptionConfiguration: RiskExceptionConfigurationTypeTypeDef = ...
+        RiskExceptionConfiguration: RiskExceptionConfigurationTypeTypeDef = ...,
     ) -> SetRiskConfigurationResponseTypeDef:
         """
         Configures actions on detected risks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.set_risk_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#set_risk_configuration)
         """
@@ -1278,15 +1278,15 @@
         """
 
     async def set_user_mfa_preference(
         self,
         *,
         AccessToken: str,
         SMSMfaSettings: SMSMfaSettingsTypeTypeDef = ...,
-        SoftwareTokenMfaSettings: SoftwareTokenMfaSettingsTypeTypeDef = ...
+        SoftwareTokenMfaSettings: SoftwareTokenMfaSettingsTypeTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Set the user's multi-factor authentication (MFA) method preference, including
         which MFA factors are activated and if any are
         preferred.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.set_user_mfa_preference)
@@ -1295,15 +1295,15 @@
 
     async def set_user_pool_mfa_config(
         self,
         *,
         UserPoolId: str,
         SmsMfaConfiguration: SmsMfaConfigTypeTypeDef = ...,
         SoftwareTokenMfaConfiguration: SoftwareTokenMfaConfigTypeTypeDef = ...,
-        MfaConfiguration: UserPoolMfaTypeType = ...
+        MfaConfiguration: UserPoolMfaTypeType = ...,
     ) -> SetUserPoolMfaConfigResponseTypeDef:
         """
         Sets the user pool multi-factor authentication (MFA) configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.set_user_pool_mfa_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#set_user_pool_mfa_config)
         """
@@ -1325,15 +1325,15 @@
         Username: str,
         Password: str,
         SecretHash: str = ...,
         UserAttributes: Sequence[AttributeTypeTypeDef] = ...,
         ValidationData: Sequence[AttributeTypeTypeDef] = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         UserContextData: UserContextDataTypeTypeDef = ...,
-        ClientMetadata: Mapping[str, str] = ...
+        ClientMetadata: Mapping[str, str] = ...,
     ) -> SignUpResponseTypeDef:
         """
         Registers the user in the specified user pool and creates a user name,
         password, and user
         attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.sign_up)
@@ -1379,15 +1379,15 @@
     async def update_auth_event_feedback(
         self,
         *,
         UserPoolId: str,
         Username: str,
         EventId: str,
         FeedbackToken: str,
-        FeedbackValue: FeedbackValueTypeType
+        FeedbackValue: FeedbackValueTypeType,
     ) -> Dict[str, Any]:
         """
         Provides the feedback for an authentication event, whether it was from a valid
         user or
         not.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_auth_event_feedback)
@@ -1395,15 +1395,15 @@
         """
 
     async def update_device_status(
         self,
         *,
         AccessToken: str,
         DeviceKey: str,
-        DeviceRememberedStatus: DeviceRememberedStatusTypeType = ...
+        DeviceRememberedStatus: DeviceRememberedStatusTypeType = ...,
     ) -> Dict[str, Any]:
         """
         Updates the device status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_device_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#update_device_status)
         """
@@ -1411,15 +1411,15 @@
     async def update_group(
         self,
         *,
         GroupName: str,
         UserPoolId: str,
         Description: str = ...,
         RoleArn: str = ...,
-        Precedence: int = ...
+        Precedence: int = ...,
     ) -> UpdateGroupResponseTypeDef:
         """
         Updates the specified group with the specified attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#update_group)
         """
@@ -1427,44 +1427,44 @@
     async def update_identity_provider(
         self,
         *,
         UserPoolId: str,
         ProviderName: str,
         ProviderDetails: Mapping[str, str] = ...,
         AttributeMapping: Mapping[str, str] = ...,
-        IdpIdentifiers: Sequence[str] = ...
+        IdpIdentifiers: Sequence[str] = ...,
     ) -> UpdateIdentityProviderResponseTypeDef:
         """
         Updates IdP information for a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_identity_provider)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#update_identity_provider)
         """
 
     async def update_resource_server(
         self,
         *,
         UserPoolId: str,
         Identifier: str,
         Name: str,
-        Scopes: Sequence[ResourceServerScopeTypeTypeDef] = ...
+        Scopes: Sequence[ResourceServerScopeTypeTypeDef] = ...,
     ) -> UpdateResourceServerResponseTypeDef:
         """
         Updates the name and scopes of resource server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_resource_server)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#update_resource_server)
         """
 
     async def update_user_attributes(
         self,
         *,
         UserAttributes: Sequence[AttributeTypeTypeDef],
         AccessToken: str,
-        ClientMetadata: Mapping[str, str] = ...
+        ClientMetadata: Mapping[str, str] = ...,
     ) -> UpdateUserAttributesResponseTypeDef:
         """
         Allows a user to update a specific attribute (one at a time).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_user_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#update_user_attributes)
         """
@@ -1486,15 +1486,15 @@
         MfaConfiguration: UserPoolMfaTypeType = ...,
         DeviceConfiguration: DeviceConfigurationTypeTypeDef = ...,
         EmailConfiguration: EmailConfigurationTypeTypeDef = ...,
         SmsConfiguration: SmsConfigurationTypeTypeDef = ...,
         UserPoolTags: Mapping[str, str] = ...,
         AdminCreateUserConfig: AdminCreateUserConfigTypeTypeDef = ...,
         UserPoolAddOns: UserPoolAddOnsTypeTypeDef = ...,
-        AccountRecoverySetting: AccountRecoverySettingTypeTypeDef = ...
+        AccountRecoverySetting: AccountRecoverySettingTypeTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_user_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#update_user_pool)
         """
@@ -1519,15 +1519,15 @@
         AllowedOAuthFlows: Sequence[OAuthFlowTypeType] = ...,
         AllowedOAuthScopes: Sequence[str] = ...,
         AllowedOAuthFlowsUserPoolClient: bool = ...,
         AnalyticsConfiguration: AnalyticsConfigurationTypeTypeDef = ...,
         PreventUserExistenceErrors: PreventUserExistenceErrorTypesType = ...,
         EnableTokenRevocation: bool = ...,
         EnablePropagateAdditionalUserContextData: bool = ...,
-        AuthSessionValidity: int = ...
+        AuthSessionValidity: int = ...,
     ) -> UpdateUserPoolClientResponseTypeDef:
         """
         Updates the specified user pool app client with the specified attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_user_pool_client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#update_user_pool_client)
         """
@@ -1546,15 +1546,15 @@
 
     async def verify_software_token(
         self,
         *,
         UserCode: str,
         AccessToken: str = ...,
         Session: str = ...,
-        FriendlyDeviceName: str = ...
+        FriendlyDeviceName: str = ...,
     ) -> VerifySoftwareTokenResponseTypeDef:
         """
         Use this API to register a user's entered time-based one-time password (TOTP)
         code and mark the user's software token MFA status as "verified" if
         successful.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.verify_software_token)
```

### Comparing `types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp/literals.py` & `types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp/literals.py`

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
     "AccountTakeoverEventActionTypeType",
     "AdminListGroupsForUserPaginatorName",
     "AdminListUserAuthEventsPaginatorName",
     "AdvancedSecurityModeTypeType",
     "AliasAttributeTypeType",
     "AttributeDataTypeType",
@@ -72,15 +71,14 @@
     "CognitoIdentityProviderServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AccountTakeoverEventActionTypeType = Literal[
     "BLOCK", "MFA_IF_CONFIGURED", "MFA_REQUIRED", "NO_ACTION"
 ]
 AdminListGroupsForUserPaginatorName = Literal["admin_list_groups_for_user"]
 AdminListUserAuthEventsPaginatorName = Literal["admin_list_user_auth_events"]
 AdvancedSecurityModeTypeType = Literal["AUDIT", "ENFORCED", "OFF"]
 AliasAttributeTypeType = Literal["email", "phone_number", "preferred_username"]
```

### Comparing `types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp/literals.pyi` & `types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp/paginator.py` & `types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,14 @@
     "ListResourceServersPaginator",
     "ListUserPoolClientsPaginator",
     "ListUserPoolsPaginator",
     "ListUsersPaginator",
     "ListUsersInGroupPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -191,15 +190,15 @@
 
     def paginate(
         self,
         *,
         UserPoolId: str,
         AttributesToGet: Sequence[str] = ...,
         Filter: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#listuserspaginator)
         """
```

### Comparing `types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp/paginator.pyi` & `types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,15 @@
 
     def paginate(
         self,
         *,
         UserPoolId: str,
         AttributesToGet: Sequence[str] = ...,
         Filter: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#listuserspaginator)
         """
 
 class ListUsersInGroupPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp/type_defs.py` & `types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "RecoveryOptionTypeTypeDef",
     "AccountTakeoverActionTypeTypeDef",
     "AdminAddUserToGroupRequestRequestTypeDef",
     "AdminConfirmSignUpRequestRequestTypeDef",
     "MessageTemplateTypeTypeDef",
     "AttributeTypeTypeDef",
```

### Comparing `types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp/type_defs.pyi` & `types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp.egg-info/PKG-INFO` & `types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cognito-idp
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CognitoIdentityProvider 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CognitoIdentityProvider 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/
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
 
 <a id="types-aiobotocore-cognito-idp"></a>
 
 # types-aiobotocore-cognito-idp
 
 [![PyPI - types-aiobotocore-cognito-idp](https://img.shields.io/pypi/v/types-aiobotocore-cognito-idp.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-idp)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cognito-idp.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-idp)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cognito-idp)](https://pepy.tech/project/types-aiobotocore-cognito-idp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CognitoIdentityProvider 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
+[aiobotocore.CognitoIdentityProvider 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
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
 [types-aiobotocore-cognito-idp docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cognito-idp-2.9.0/types_aiobotocore_cognito_idp.egg-info/SOURCES.txt` & `types-aiobotocore-cognito-idp-2.9.1/types_aiobotocore_cognito_idp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

