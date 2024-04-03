# Comparing `tmp/types-aiobotocore-chime-sdk-identity-2.9.0.tar.gz` & `tmp/types-aiobotocore-chime-sdk-identity-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-chime-sdk-identity-2.9.0.tar", last modified: Wed Dec 13 19:58:45 2023, max compression
+gzip compressed data, was "types-aiobotocore-chime-sdk-identity-2.9.1.tar", last modified: Thu Jan 18 01:20:12 2024, max compression
```

## Comparing `types-aiobotocore-chime-sdk-identity-2.9.0.tar` & `types-aiobotocore-chime-sdk-identity-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:45.098007 types-aiobotocore-chime-sdk-identity-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:41:59.000000 types-aiobotocore-chime-sdk-identity-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12780 2023-12-13 19:58:45.094007 types-aiobotocore-chime-sdk-identity-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11175 2023-12-13 19:41:59.000000 types-aiobotocore-chime-sdk-identity-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:45.098007 types-aiobotocore-chime-sdk-identity-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2023-12-13 19:41:59.000000 types-aiobotocore-chime-sdk-identity-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:45.094007 types-aiobotocore-chime-sdk-identity-2.9.0/types_aiobotocore_chime_sdk_identity/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2023-12-13 19:41:59.000000 types-aiobotocore-chime-sdk-identity-2.9.0/types_aiobotocore_chime_sdk_identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2023-12-13 19:41:59.000000 types-aiobotocore-chime-sdk-identity-2.9.0/types_aiobotocore_chime_sdk_identity/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      972 2023-12-13 19:41:59.000000 types-aiobotocore-chime-sdk-identity-2.9.0/types_aiobotocore_chime_sdk_identity/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24648 2023-12-13 19:41:59.000000 types-aiobotocore-chime-sdk-identity-2.9.0/types_aiobotocore_chime_sdk_identity/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    24645 2023-12-13 19:41:59.000000 types-aiobotocore-chime-sdk-identity-2.9.0/types_aiobotocore_chime_sdk_identity/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8906 2023-12-13 19:41:59.000000 types-aiobotocore-chime-sdk-identity-2.9.0/types_aiobotocore_chime_sdk_identity/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8904 2023-12-13 19:41:59.000000 types-aiobotocore-chime-sdk-identity-2.9.0/types_aiobotocore_chime_sdk_identity/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:41:59.000000 types-aiobotocore-chime-sdk-identity-2.9.0/types_aiobotocore_chime_sdk_identity/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    21408 2023-12-13 19:41:59.000000 types-aiobotocore-chime-sdk-identity-2.9.0/types_aiobotocore_chime_sdk_identity/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21407 2023-12-13 19:41:59.000000 types-aiobotocore-chime-sdk-identity-2.9.0/types_aiobotocore_chime_sdk_identity/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:41:59.000000 types-aiobotocore-chime-sdk-identity-2.9.0/types_aiobotocore_chime_sdk_identity/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:45.094007 types-aiobotocore-chime-sdk-identity-2.9.0/types_aiobotocore_chime_sdk_identity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12780 2023-12-13 19:58:45.000000 types-aiobotocore-chime-sdk-identity-2.9.0/types_aiobotocore_chime_sdk_identity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      921 2023-12-13 19:58:45.000000 types-aiobotocore-chime-sdk-identity-2.9.0/types_aiobotocore_chime_sdk_identity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:45.000000 types-aiobotocore-chime-sdk-identity-2.9.0/types_aiobotocore_chime_sdk_identity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:45.000000 types-aiobotocore-chime-sdk-identity-2.9.0/types_aiobotocore_chime_sdk_identity.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:45.000000 types-aiobotocore-chime-sdk-identity-2.9.0/types_aiobotocore_chime_sdk_identity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-13 19:58:45.000000 types-aiobotocore-chime-sdk-identity-2.9.0/types_aiobotocore_chime_sdk_identity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:12.245480 types-aiobotocore-chime-sdk-identity-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:03:56.000000 types-aiobotocore-chime-sdk-identity-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12800 2024-01-18 01:20:12.245480 types-aiobotocore-chime-sdk-identity-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11175 2024-01-18 01:03:56.000000 types-aiobotocore-chime-sdk-identity-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:12.245480 types-aiobotocore-chime-sdk-identity-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-01-18 01:03:56.000000 types-aiobotocore-chime-sdk-identity-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:12.241480 types-aiobotocore-chime-sdk-identity-2.9.1/types_aiobotocore_chime_sdk_identity/
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-01-18 01:03:56.000000 types-aiobotocore-chime-sdk-identity-2.9.1/types_aiobotocore_chime_sdk_identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-01-18 01:03:56.000000 types-aiobotocore-chime-sdk-identity-2.9.1/types_aiobotocore_chime_sdk_identity/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-01-18 01:03:56.000000 types-aiobotocore-chime-sdk-identity-2.9.1/types_aiobotocore_chime_sdk_identity/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24655 2024-01-18 01:03:56.000000 types-aiobotocore-chime-sdk-identity-2.9.1/types_aiobotocore_chime_sdk_identity/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24652 2024-01-18 01:03:56.000000 types-aiobotocore-chime-sdk-identity-2.9.1/types_aiobotocore_chime_sdk_identity/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-01-18 01:03:56.000000 types-aiobotocore-chime-sdk-identity-2.9.1/types_aiobotocore_chime_sdk_identity/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-01-18 01:03:56.000000 types-aiobotocore-chime-sdk-identity-2.9.1/types_aiobotocore_chime_sdk_identity/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:03:56.000000 types-aiobotocore-chime-sdk-identity-2.9.1/types_aiobotocore_chime_sdk_identity/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    21407 2024-01-18 01:03:57.000000 types-aiobotocore-chime-sdk-identity-2.9.1/types_aiobotocore_chime_sdk_identity/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21407 2024-01-18 01:03:57.000000 types-aiobotocore-chime-sdk-identity-2.9.1/types_aiobotocore_chime_sdk_identity/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:03:56.000000 types-aiobotocore-chime-sdk-identity-2.9.1/types_aiobotocore_chime_sdk_identity/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:12.245480 types-aiobotocore-chime-sdk-identity-2.9.1/types_aiobotocore_chime_sdk_identity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12800 2024-01-18 01:20:12.000000 types-aiobotocore-chime-sdk-identity-2.9.1/types_aiobotocore_chime_sdk_identity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-01-18 01:20:12.000000 types-aiobotocore-chime-sdk-identity-2.9.1/types_aiobotocore_chime_sdk_identity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:12.000000 types-aiobotocore-chime-sdk-identity-2.9.1/types_aiobotocore_chime_sdk_identity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:12.000000 types-aiobotocore-chime-sdk-identity-2.9.1/types_aiobotocore_chime_sdk_identity.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:12.000000 types-aiobotocore-chime-sdk-identity-2.9.1/types_aiobotocore_chime_sdk_identity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-01-18 01:20:12.000000 types-aiobotocore-chime-sdk-identity-2.9.1/types_aiobotocore_chime_sdk_identity.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-chime-sdk-identity-2.9.0/LICENSE` & `types-aiobotocore-chime-sdk-identity-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-chime-sdk-identity-2.9.0/PKG-INFO` & `types-aiobotocore-chime-sdk-identity-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-chime-sdk-identity
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ChimeSDKIdentity 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ChimeSDKIdentity 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/
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
 
 <a id="types-aiobotocore-chime-sdk-identity"></a>
 
 # types-aiobotocore-chime-sdk-identity
 
 [![PyPI - types-aiobotocore-chime-sdk-identity](https://img.shields.io/pypi/v/types-aiobotocore-chime-sdk-identity.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-identity)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime-sdk-identity.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-identity)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime-sdk-identity)](https://pepy.tech/project/types-aiobotocore-chime-sdk-identity)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ChimeSDKIdentity 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity)
+[aiobotocore.ChimeSDKIdentity 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity)
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
 [types-aiobotocore-chime-sdk-identity docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-chime-sdk-identity-2.9.0/README.md` & `types-aiobotocore-chime-sdk-identity-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime-sdk-identity.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-identity)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime-sdk-identity)](https://pepy.tech/project/types-aiobotocore-chime-sdk-identity)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ChimeSDKIdentity 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity)
+[aiobotocore.ChimeSDKIdentity 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity)
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
 [types-aiobotocore-chime-sdk-identity docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-chime-sdk-identity-2.9.0/setup.py` & `types-aiobotocore-chime-sdk-identity-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-chime-sdk-identity",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_chime_sdk_identity"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ChimeSDKIdentity 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ChimeSDKIdentity 2.9.1 service generated with"
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
     keywords="aiobotocore chime-sdk-identity type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_chime_sdk_identity": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-chime-sdk-identity-2.9.0/types_aiobotocore_chime_sdk_identity/__init__.py` & `types-aiobotocore-chime-sdk-identity-2.9.1/types_aiobotocore_chime_sdk_identity/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,9 +18,8 @@
     ```
 """
 
 from .client import ChimeSDKIdentityClient
 
 Client = ChimeSDKIdentityClient
 
-
 __all__ = ("ChimeSDKIdentityClient", "Client")
```

### Comparing `types-aiobotocore-chime-sdk-identity-2.9.0/types_aiobotocore_chime_sdk_identity/__init__.pyi` & `types-aiobotocore-chime-sdk-identity-2.9.1/types_aiobotocore_chime_sdk_identity/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-identity-2.9.0/types_aiobotocore_chime_sdk_identity/__main__.py` & `types-aiobotocore-chime-sdk-identity-2.9.1/types_aiobotocore_chime_sdk_identity/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ChimeSDKIdentity 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ChimeSDKIdentity 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity\nOther"
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

### Comparing `types-aiobotocore-chime-sdk-identity-2.9.0/types_aiobotocore_chime_sdk_identity/client.py` & `types-aiobotocore-chime-sdk-identity-2.9.1/types_aiobotocore_chime_sdk_identity/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
     async def create_app_instance(
         self,
         *,
         Name: str,
         ClientRequestToken: str,
         Metadata: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAppInstanceResponseTypeDef:
         """
         Creates an Amazon Chime SDK messaging `AppInstance` under an AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity.Client.create_app_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/client/#create_app_instance)
         """
@@ -139,15 +139,15 @@
         self,
         *,
         AppInstanceArn: str,
         ClientRequestToken: str,
         Configuration: ConfigurationTypeDef,
         Name: str = ...,
         Metadata: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAppInstanceBotResponseTypeDef:
         """
         Creates a bot under an Amazon Chime `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity.Client.create_app_instance_bot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/client/#create_app_instance_bot)
         """
@@ -157,15 +157,15 @@
         *,
         AppInstanceArn: str,
         AppInstanceUserId: str,
         Name: str,
         ClientRequestToken: str,
         Metadata: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ExpirationSettings: ExpirationSettingsTypeDef = ...
+        ExpirationSettings: ExpirationSettingsTypeDef = ...,
     ) -> CreateAppInstanceUserResponseTypeDef:
         """
         Creates a user under an Amazon Chime `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity.Client.create_app_instance_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/client/#create_app_instance_user)
         """
@@ -353,15 +353,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/client/#list_tags_for_resource)
         """
 
     async def put_app_instance_retention_settings(
         self,
         *,
         AppInstanceArn: str,
-        AppInstanceRetentionSettings: AppInstanceRetentionSettingsTypeDef
+        AppInstanceRetentionSettings: AppInstanceRetentionSettingsTypeDef,
     ) -> PutAppInstanceRetentionSettingsResponseTypeDef:
         """
         Sets the amount of time in days that a given `AppInstance` retains data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity.Client.put_app_instance_retention_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/client/#put_app_instance_retention_settings)
         """
@@ -381,15 +381,15 @@
         *,
         AppInstanceUserArn: str,
         Type: AppInstanceUserEndpointTypeType,
         ResourceArn: str,
         EndpointAttributes: EndpointAttributesTypeDef,
         ClientRequestToken: str,
         Name: str = ...,
-        AllowMessages: AllowMessagesType = ...
+        AllowMessages: AllowMessagesType = ...,
     ) -> RegisterAppInstanceUserEndpointResponseTypeDef:
         """
         Registers an endpoint under an Amazon Chime `AppInstanceUser`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity.Client.register_app_instance_user_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/client/#register_app_instance_user_endpoint)
         """
@@ -427,15 +427,15 @@
 
     async def update_app_instance_bot(
         self,
         *,
         AppInstanceBotArn: str,
         Name: str,
         Metadata: str,
-        Configuration: ConfigurationTypeDef = ...
+        Configuration: ConfigurationTypeDef = ...,
     ) -> UpdateAppInstanceBotResponseTypeDef:
         """
         Updates the name and metadata of an `AppInstanceBot`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity.Client.update_app_instance_bot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/client/#update_app_instance_bot)
         """
@@ -452,15 +452,15 @@
 
     async def update_app_instance_user_endpoint(
         self,
         *,
         AppInstanceUserArn: str,
         EndpointId: str,
         Name: str = ...,
-        AllowMessages: AllowMessagesType = ...
+        AllowMessages: AllowMessagesType = ...,
     ) -> UpdateAppInstanceUserEndpointResponseTypeDef:
         """
         Updates the details of an `AppInstanceUserEndpoint`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity.Client.update_app_instance_user_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/client/#update_app_instance_user_endpoint)
         """
```

### Comparing `types-aiobotocore-chime-sdk-identity-2.9.0/types_aiobotocore_chime_sdk_identity/client.pyi` & `types-aiobotocore-chime-sdk-identity-2.9.1/types_aiobotocore_chime_sdk_identity/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
     async def create_app_instance(
         self,
         *,
         Name: str,
         ClientRequestToken: str,
         Metadata: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAppInstanceResponseTypeDef:
         """
         Creates an Amazon Chime SDK messaging `AppInstance` under an AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity.Client.create_app_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/client/#create_app_instance)
         """
@@ -136,15 +136,15 @@
         self,
         *,
         AppInstanceArn: str,
         ClientRequestToken: str,
         Configuration: ConfigurationTypeDef,
         Name: str = ...,
         Metadata: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAppInstanceBotResponseTypeDef:
         """
         Creates a bot under an Amazon Chime `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity.Client.create_app_instance_bot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/client/#create_app_instance_bot)
         """
@@ -154,15 +154,15 @@
         *,
         AppInstanceArn: str,
         AppInstanceUserId: str,
         Name: str,
         ClientRequestToken: str,
         Metadata: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ExpirationSettings: ExpirationSettingsTypeDef = ...
+        ExpirationSettings: ExpirationSettingsTypeDef = ...,
     ) -> CreateAppInstanceUserResponseTypeDef:
         """
         Creates a user under an Amazon Chime `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity.Client.create_app_instance_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/client/#create_app_instance_user)
         """
@@ -350,15 +350,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/client/#list_tags_for_resource)
         """
 
     async def put_app_instance_retention_settings(
         self,
         *,
         AppInstanceArn: str,
-        AppInstanceRetentionSettings: AppInstanceRetentionSettingsTypeDef
+        AppInstanceRetentionSettings: AppInstanceRetentionSettingsTypeDef,
     ) -> PutAppInstanceRetentionSettingsResponseTypeDef:
         """
         Sets the amount of time in days that a given `AppInstance` retains data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity.Client.put_app_instance_retention_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/client/#put_app_instance_retention_settings)
         """
@@ -378,15 +378,15 @@
         *,
         AppInstanceUserArn: str,
         Type: AppInstanceUserEndpointTypeType,
         ResourceArn: str,
         EndpointAttributes: EndpointAttributesTypeDef,
         ClientRequestToken: str,
         Name: str = ...,
-        AllowMessages: AllowMessagesType = ...
+        AllowMessages: AllowMessagesType = ...,
     ) -> RegisterAppInstanceUserEndpointResponseTypeDef:
         """
         Registers an endpoint under an Amazon Chime `AppInstanceUser`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity.Client.register_app_instance_user_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/client/#register_app_instance_user_endpoint)
         """
@@ -424,15 +424,15 @@
 
     async def update_app_instance_bot(
         self,
         *,
         AppInstanceBotArn: str,
         Name: str,
         Metadata: str,
-        Configuration: ConfigurationTypeDef = ...
+        Configuration: ConfigurationTypeDef = ...,
     ) -> UpdateAppInstanceBotResponseTypeDef:
         """
         Updates the name and metadata of an `AppInstanceBot`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity.Client.update_app_instance_bot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/client/#update_app_instance_bot)
         """
@@ -449,15 +449,15 @@
 
     async def update_app_instance_user_endpoint(
         self,
         *,
         AppInstanceUserArn: str,
         EndpointId: str,
         Name: str = ...,
-        AllowMessages: AllowMessagesType = ...
+        AllowMessages: AllowMessagesType = ...,
     ) -> UpdateAppInstanceUserEndpointResponseTypeDef:
         """
         Updates the details of an `AppInstanceUserEndpoint`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity.Client.update_app_instance_user_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/client/#update_app_instance_user_endpoint)
         """
```

### Comparing `types-aiobotocore-chime-sdk-identity-2.9.0/types_aiobotocore_chime_sdk_identity/literals.py` & `types-aiobotocore-chime-sdk-identity-2.9.1/types_aiobotocore_chime_sdk_identity/literals.py`

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
     "AllowMessagesType",
     "AppInstanceUserEndpointTypeType",
     "EndpointStatusReasonType",
     "EndpointStatusType",
     "ExpirationCriterionType",
     "RespondsToType",
@@ -31,15 +30,14 @@
     "TargetedMessagesType",
     "ChimeSDKIdentityServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AllowMessagesType = Literal["ALL", "NONE"]
 AppInstanceUserEndpointTypeType = Literal["APNS", "APNS_SANDBOX", "GCM"]
 EndpointStatusReasonType = Literal["INVALID_DEVICE_TOKEN", "INVALID_PINPOINT_ARN"]
 EndpointStatusType = Literal["ACTIVE", "INACTIVE"]
 ExpirationCriterionType = Literal["CREATED_TIMESTAMP"]
 RespondsToType = Literal["STANDARD_MESSAGES"]
 StandardMessagesType = Literal["ALL", "AUTO", "MENTIONS", "NONE"]
```

### Comparing `types-aiobotocore-chime-sdk-identity-2.9.0/types_aiobotocore_chime_sdk_identity/literals.pyi` & `types-aiobotocore-chime-sdk-identity-2.9.1/types_aiobotocore_chime_sdk_identity/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-identity-2.9.0/types_aiobotocore_chime_sdk_identity/type_defs.py` & `types-aiobotocore-chime-sdk-identity-2.9.1/types_aiobotocore_chime_sdk_identity/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "IdentityTypeDef",
     "AppInstanceBotSummaryTypeDef",
     "ChannelRetentionSettingsTypeDef",
     "AppInstanceSummaryTypeDef",
     "AppInstanceTypeDef",
     "EndpointStateTypeDef",
```

### Comparing `types-aiobotocore-chime-sdk-identity-2.9.0/types_aiobotocore_chime_sdk_identity/type_defs.pyi` & `types-aiobotocore-chime-sdk-identity-2.9.1/types_aiobotocore_chime_sdk_identity/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-identity-2.9.0/types_aiobotocore_chime_sdk_identity.egg-info/PKG-INFO` & `types-aiobotocore-chime-sdk-identity-2.9.1/types_aiobotocore_chime_sdk_identity.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-chime-sdk-identity
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ChimeSDKIdentity 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ChimeSDKIdentity 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/
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
 
 <a id="types-aiobotocore-chime-sdk-identity"></a>
 
 # types-aiobotocore-chime-sdk-identity
 
 [![PyPI - types-aiobotocore-chime-sdk-identity](https://img.shields.io/pypi/v/types-aiobotocore-chime-sdk-identity.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-identity)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime-sdk-identity.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-identity)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime-sdk-identity)](https://pepy.tech/project/types-aiobotocore-chime-sdk-identity)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ChimeSDKIdentity 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity)
+[aiobotocore.ChimeSDKIdentity 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity)
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
 [types-aiobotocore-chime-sdk-identity docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-chime-sdk-identity-2.9.0/types_aiobotocore_chime_sdk_identity.egg-info/SOURCES.txt` & `types-aiobotocore-chime-sdk-identity-2.9.1/types_aiobotocore_chime_sdk_identity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

