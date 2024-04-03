# Comparing `tmp/types-aiobotocore-signer-2.9.0.tar.gz` & `tmp/types-aiobotocore-signer-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-signer-2.9.0.tar", last modified: Wed Dec 13 20:00:32 2023, max compression
+gzip compressed data, was "types-aiobotocore-signer-2.9.1.tar", last modified: Thu Jan 18 01:21:50 2024, max compression
```

## Comparing `types-aiobotocore-signer-2.9.0.tar` & `types-aiobotocore-signer-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:32.125123 types-aiobotocore-signer-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:56:33.000000 types-aiobotocore-signer-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13985 2023-12-13 20:00:32.125123 types-aiobotocore-signer-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12426 2023-12-13 19:56:33.000000 types-aiobotocore-signer-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:32.125123 types-aiobotocore-signer-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-12-13 19:56:33.000000 types-aiobotocore-signer-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:32.125123 types-aiobotocore-signer-2.9.0/types_aiobotocore_signer/
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2023-12-13 19:56:33.000000 types-aiobotocore-signer-2.9.0/types_aiobotocore_signer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2023-12-13 19:56:33.000000 types-aiobotocore-signer-2.9.0/types_aiobotocore_signer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      917 2023-12-13 19:56:33.000000 types-aiobotocore-signer-2.9.0/types_aiobotocore_signer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18596 2023-12-13 19:56:33.000000 types-aiobotocore-signer-2.9.0/types_aiobotocore_signer/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    18592 2023-12-13 19:56:33.000000 types-aiobotocore-signer-2.9.0/types_aiobotocore_signer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9646 2023-12-13 19:56:33.000000 types-aiobotocore-signer-2.9.0/types_aiobotocore_signer/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9644 2023-12-13 19:56:33.000000 types-aiobotocore-signer-2.9.0/types_aiobotocore_signer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4875 2023-12-13 19:56:33.000000 types-aiobotocore-signer-2.9.0/types_aiobotocore_signer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4870 2023-12-13 19:56:33.000000 types-aiobotocore-signer-2.9.0/types_aiobotocore_signer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:56:33.000000 types-aiobotocore-signer-2.9.0/types_aiobotocore_signer/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    20029 2023-12-13 19:56:34.000000 types-aiobotocore-signer-2.9.0/types_aiobotocore_signer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    20028 2023-12-13 19:56:33.000000 types-aiobotocore-signer-2.9.0/types_aiobotocore_signer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:56:33.000000 types-aiobotocore-signer-2.9.0/types_aiobotocore_signer/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2023-12-13 19:56:33.000000 types-aiobotocore-signer-2.9.0/types_aiobotocore_signer/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2023-12-13 19:56:33.000000 types-aiobotocore-signer-2.9.0/types_aiobotocore_signer/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:32.125123 types-aiobotocore-signer-2.9.0/types_aiobotocore_signer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13985 2023-12-13 20:00:32.000000 types-aiobotocore-signer-2.9.0/types_aiobotocore_signer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      865 2023-12-13 20:00:32.000000 types-aiobotocore-signer-2.9.0/types_aiobotocore_signer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:32.000000 types-aiobotocore-signer-2.9.0/types_aiobotocore_signer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:32.000000 types-aiobotocore-signer-2.9.0/types_aiobotocore_signer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:32.000000 types-aiobotocore-signer-2.9.0/types_aiobotocore_signer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-13 20:00:32.000000 types-aiobotocore-signer-2.9.0/types_aiobotocore_signer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:50.385027 types-aiobotocore-signer-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:18:01.000000 types-aiobotocore-signer-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14005 2024-01-18 01:21:50.385027 types-aiobotocore-signer-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12426 2024-01-18 01:18:01.000000 types-aiobotocore-signer-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:50.385027 types-aiobotocore-signer-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-01-18 01:18:01.000000 types-aiobotocore-signer-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:50.381027 types-aiobotocore-signer-2.9.1/types_aiobotocore_signer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-01-18 01:18:01.000000 types-aiobotocore-signer-2.9.1/types_aiobotocore_signer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-01-18 01:18:01.000000 types-aiobotocore-signer-2.9.1/types_aiobotocore_signer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-01-18 01:18:01.000000 types-aiobotocore-signer-2.9.1/types_aiobotocore_signer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18602 2024-01-18 01:18:01.000000 types-aiobotocore-signer-2.9.1/types_aiobotocore_signer/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18599 2024-01-18 01:18:01.000000 types-aiobotocore-signer-2.9.1/types_aiobotocore_signer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-01-18 01:18:01.000000 types-aiobotocore-signer-2.9.1/types_aiobotocore_signer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-01-18 01:18:01.000000 types-aiobotocore-signer-2.9.1/types_aiobotocore_signer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-01-18 01:18:01.000000 types-aiobotocore-signer-2.9.1/types_aiobotocore_signer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-01-18 01:18:01.000000 types-aiobotocore-signer-2.9.1/types_aiobotocore_signer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:18:01.000000 types-aiobotocore-signer-2.9.1/types_aiobotocore_signer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    20028 2024-01-18 01:18:02.000000 types-aiobotocore-signer-2.9.1/types_aiobotocore_signer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20028 2024-01-18 01:18:02.000000 types-aiobotocore-signer-2.9.1/types_aiobotocore_signer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:18:01.000000 types-aiobotocore-signer-2.9.1/types_aiobotocore_signer/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-01-18 01:18:01.000000 types-aiobotocore-signer-2.9.1/types_aiobotocore_signer/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-01-18 01:18:01.000000 types-aiobotocore-signer-2.9.1/types_aiobotocore_signer/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:50.385027 types-aiobotocore-signer-2.9.1/types_aiobotocore_signer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14005 2024-01-18 01:21:50.000000 types-aiobotocore-signer-2.9.1/types_aiobotocore_signer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-01-18 01:21:50.000000 types-aiobotocore-signer-2.9.1/types_aiobotocore_signer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:50.000000 types-aiobotocore-signer-2.9.1/types_aiobotocore_signer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:50.000000 types-aiobotocore-signer-2.9.1/types_aiobotocore_signer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:50.000000 types-aiobotocore-signer-2.9.1/types_aiobotocore_signer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-18 01:21:50.000000 types-aiobotocore-signer-2.9.1/types_aiobotocore_signer.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-signer-2.9.0/LICENSE` & `types-aiobotocore-signer-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-signer-2.9.0/PKG-INFO` & `types-aiobotocore-signer-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-signer
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.signer 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.signer 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/
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
 
 <a id="types-aiobotocore-signer"></a>
 
 # types-aiobotocore-signer
 
 [![PyPI - types-aiobotocore-signer](https://img.shields.io/pypi/v/types-aiobotocore-signer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-signer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-signer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-signer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-signer)](https://pepy.tech/project/types-aiobotocore-signer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.signer 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
+[aiobotocore.signer 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
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
 [types-aiobotocore-signer docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-signer-2.9.0/README.md` & `types-aiobotocore-signer-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-signer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-signer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-signer)](https://pepy.tech/project/types-aiobotocore-signer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.signer 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
+[aiobotocore.signer 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
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
 [types-aiobotocore-signer docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-signer-2.9.0/setup.py` & `types-aiobotocore-signer-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-signer",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_signer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.signer 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.signer 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore signer type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_signer": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-signer-2.9.0/types_aiobotocore_signer/__init__.py` & `types-aiobotocore-signer-2.9.1/types_aiobotocore_signer/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     ListSigningPlatformsPaginator,
     ListSigningProfilesPaginator,
 )
 from .waiter import SuccessfulSigningJobWaiter
 
 Client = signerClient
 
-
 __all__ = (
     "Client",
     "ListSigningJobsPaginator",
     "ListSigningPlatformsPaginator",
     "ListSigningProfilesPaginator",
     "SuccessfulSigningJobWaiter",
     "signerClient",
```

### Comparing `types-aiobotocore-signer-2.9.0/types_aiobotocore_signer/__init__.pyi` & `types-aiobotocore-signer-2.9.1/types_aiobotocore_signer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.9.0/types_aiobotocore_signer/__main__.py` & `types-aiobotocore-signer-2.9.1/types_aiobotocore_signer/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.signer 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.signer 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer\nOther"
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

### Comparing `types-aiobotocore-signer-2.9.0/types_aiobotocore_signer/client.py` & `types-aiobotocore-signer-2.9.1/types_aiobotocore_signer/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 from .waiter import SuccessfulSigningJobWaiter
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("signerClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -105,15 +104,15 @@
         self,
         *,
         profileName: str,
         action: str,
         principal: str,
         statementId: str,
         profileVersion: str = ...,
-        revisionId: str = ...
+        revisionId: str = ...,
     ) -> AddProfilePermissionResponseTypeDef:
         """
         Adds cross-account permissions to a signing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.add_profile_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#add_profile_permission)
         """
@@ -167,15 +166,15 @@
     async def get_revocation_status(
         self,
         *,
         signatureTimestamp: TimestampTypeDef,
         platformId: str,
         profileVersionArn: str,
         jobArn: str,
-        certificateHashes: Sequence[str]
+        certificateHashes: Sequence[str],
     ) -> GetRevocationStatusResponseTypeDef:
         """
         Retrieves the revocation status of one or more of the signing profile, signing
         job, and signing
         certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_revocation_status)
@@ -217,15 +216,15 @@
         platformId: str = ...,
         requestedBy: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         isRevoked: bool = ...,
         signatureExpiresBefore: TimestampTypeDef = ...,
         signatureExpiresAfter: TimestampTypeDef = ...,
-        jobInvoker: str = ...
+        jobInvoker: str = ...,
     ) -> ListSigningJobsResponseTypeDef:
         """
         Lists all your signing jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_signing_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#list_signing_jobs)
         """
@@ -233,15 +232,15 @@
     async def list_signing_platforms(
         self,
         *,
         category: str = ...,
         partner: str = ...,
         target: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListSigningPlatformsResponseTypeDef:
         """
         Lists all signing platforms available in AWS Signer that match the request
         parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_signing_platforms)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#list_signing_platforms)
@@ -250,15 +249,15 @@
     async def list_signing_profiles(
         self,
         *,
         includeCanceled: bool = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         platformId: str = ...,
-        statuses: Sequence[SigningProfileStatusType] = ...
+        statuses: Sequence[SigningProfileStatusType] = ...,
     ) -> ListSigningProfilesResponseTypeDef:
         """
         Lists all available signing profiles in your AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_signing_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#list_signing_profiles)
         """
@@ -278,15 +277,15 @@
         *,
         profileName: str,
         platformId: str,
         signingMaterial: SigningMaterialTypeDef = ...,
         signatureValidityPeriod: SignatureValidityPeriodTypeDef = ...,
         overrides: SigningPlatformOverridesTypeDef = ...,
         signingParameters: Mapping[str, str] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> PutSigningProfileResponseTypeDef:
         """
         Creates a signing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.put_signing_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#put_signing_profile)
         """
@@ -334,15 +333,15 @@
     async def start_signing_job(
         self,
         *,
         source: SourceTypeDef,
         destination: DestinationTypeDef,
         profileName: str,
         clientRequestToken: str,
-        profileOwner: str = ...
+        profileOwner: str = ...,
     ) -> StartSigningJobResponseTypeDef:
         """
         Initiates a signing job to be performed on the code provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.start_signing_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#start_signing_job)
         """
```

### Comparing `types-aiobotocore-signer-2.9.0/types_aiobotocore_signer/client.pyi` & `types-aiobotocore-signer-2.9.1/types_aiobotocore_signer/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         self,
         *,
         profileName: str,
         action: str,
         principal: str,
         statementId: str,
         profileVersion: str = ...,
-        revisionId: str = ...
+        revisionId: str = ...,
     ) -> AddProfilePermissionResponseTypeDef:
         """
         Adds cross-account permissions to a signing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.add_profile_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#add_profile_permission)
         """
@@ -163,15 +163,15 @@
     async def get_revocation_status(
         self,
         *,
         signatureTimestamp: TimestampTypeDef,
         platformId: str,
         profileVersionArn: str,
         jobArn: str,
-        certificateHashes: Sequence[str]
+        certificateHashes: Sequence[str],
     ) -> GetRevocationStatusResponseTypeDef:
         """
         Retrieves the revocation status of one or more of the signing profile, signing
         job, and signing
         certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_revocation_status)
@@ -213,15 +213,15 @@
         platformId: str = ...,
         requestedBy: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         isRevoked: bool = ...,
         signatureExpiresBefore: TimestampTypeDef = ...,
         signatureExpiresAfter: TimestampTypeDef = ...,
-        jobInvoker: str = ...
+        jobInvoker: str = ...,
     ) -> ListSigningJobsResponseTypeDef:
         """
         Lists all your signing jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_signing_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#list_signing_jobs)
         """
@@ -229,15 +229,15 @@
     async def list_signing_platforms(
         self,
         *,
         category: str = ...,
         partner: str = ...,
         target: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListSigningPlatformsResponseTypeDef:
         """
         Lists all signing platforms available in AWS Signer that match the request
         parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_signing_platforms)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#list_signing_platforms)
@@ -246,15 +246,15 @@
     async def list_signing_profiles(
         self,
         *,
         includeCanceled: bool = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         platformId: str = ...,
-        statuses: Sequence[SigningProfileStatusType] = ...
+        statuses: Sequence[SigningProfileStatusType] = ...,
     ) -> ListSigningProfilesResponseTypeDef:
         """
         Lists all available signing profiles in your AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_signing_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#list_signing_profiles)
         """
@@ -274,15 +274,15 @@
         *,
         profileName: str,
         platformId: str,
         signingMaterial: SigningMaterialTypeDef = ...,
         signatureValidityPeriod: SignatureValidityPeriodTypeDef = ...,
         overrides: SigningPlatformOverridesTypeDef = ...,
         signingParameters: Mapping[str, str] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> PutSigningProfileResponseTypeDef:
         """
         Creates a signing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.put_signing_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#put_signing_profile)
         """
@@ -330,15 +330,15 @@
     async def start_signing_job(
         self,
         *,
         source: SourceTypeDef,
         destination: DestinationTypeDef,
         profileName: str,
         clientRequestToken: str,
-        profileOwner: str = ...
+        profileOwner: str = ...,
     ) -> StartSigningJobResponseTypeDef:
         """
         Initiates a signing job to be performed on the code provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.start_signing_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#start_signing_job)
         """
```

### Comparing `types-aiobotocore-signer-2.9.0/types_aiobotocore_signer/literals.py` & `types-aiobotocore-signer-2.9.1/types_aiobotocore_signer/literals.py`

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
     "CategoryType",
     "EncryptionAlgorithmType",
     "HashAlgorithmType",
     "ImageFormatType",
     "ListSigningJobsPaginatorName",
     "ListSigningPlatformsPaginatorName",
@@ -36,15 +35,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 CategoryType = Literal["AWSIoT"]
 EncryptionAlgorithmType = Literal["ECDSA", "RSA"]
 HashAlgorithmType = Literal["SHA1", "SHA256"]
 ImageFormatType = Literal["JSON", "JSONDetached", "JSONEmbedded"]
 ListSigningJobsPaginatorName = Literal["list_signing_jobs"]
 ListSigningPlatformsPaginatorName = Literal["list_signing_platforms"]
 ListSigningProfilesPaginatorName = Literal["list_signing_profiles"]
```

### Comparing `types-aiobotocore-signer-2.9.0/types_aiobotocore_signer/literals.pyi` & `types-aiobotocore-signer-2.9.1/types_aiobotocore_signer/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.9.0/types_aiobotocore_signer/paginator.py` & `types-aiobotocore-signer-2.9.1/types_aiobotocore_signer/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -41,25 +41,22 @@
 
 __all__ = (
     "ListSigningJobsPaginator",
     "ListSigningPlatformsPaginator",
     "ListSigningProfilesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListSigningJobsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/paginators/#listsigningjobspaginator)
     """
 
     def paginate(
@@ -68,53 +65,51 @@
         status: SigningStatusType = ...,
         platformId: str = ...,
         requestedBy: str = ...,
         isRevoked: bool = ...,
         signatureExpiresBefore: TimestampTypeDef = ...,
         signatureExpiresAfter: TimestampTypeDef = ...,
         jobInvoker: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSigningJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/paginators/#listsigningjobspaginator)
         """
 
-
 class ListSigningPlatformsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningPlatforms)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/paginators/#listsigningplatformspaginator)
     """
 
     def paginate(
         self,
         *,
         category: str = ...,
         partner: str = ...,
         target: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSigningPlatformsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningPlatforms.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/paginators/#listsigningplatformspaginator)
         """
 
-
 class ListSigningProfilesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningProfiles)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/paginators/#listsigningprofilespaginator)
     """
 
     def paginate(
         self,
         *,
         includeCanceled: bool = ...,
         platformId: str = ...,
         statuses: Sequence[SigningProfileStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSigningProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/paginators/#listsigningprofilespaginator)
         """
```

### Comparing `types-aiobotocore-signer-2.9.0/types_aiobotocore_signer/paginator.pyi` & `types-aiobotocore-signer-2.9.1/types_aiobotocore_signer/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,20 +43,22 @@
     "ListSigningJobsPaginator",
     "ListSigningPlatformsPaginator",
     "ListSigningProfilesPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListSigningJobsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/paginators/#listsigningjobspaginator)
     """
 
     def paginate(
@@ -65,51 +67,53 @@
         status: SigningStatusType = ...,
         platformId: str = ...,
         requestedBy: str = ...,
         isRevoked: bool = ...,
         signatureExpiresBefore: TimestampTypeDef = ...,
         signatureExpiresAfter: TimestampTypeDef = ...,
         jobInvoker: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSigningJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/paginators/#listsigningjobspaginator)
         """
 
+
 class ListSigningPlatformsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningPlatforms)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/paginators/#listsigningplatformspaginator)
     """
 
     def paginate(
         self,
         *,
         category: str = ...,
         partner: str = ...,
         target: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSigningPlatformsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningPlatforms.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/paginators/#listsigningplatformspaginator)
         """
 
+
 class ListSigningProfilesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningProfiles)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/paginators/#listsigningprofilespaginator)
     """
 
     def paginate(
         self,
         *,
         includeCanceled: bool = ...,
         platformId: str = ...,
         statuses: Sequence[SigningProfileStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSigningProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/paginators/#listsigningprofilespaginator)
         """
```

### Comparing `types-aiobotocore-signer-2.9.0/types_aiobotocore_signer/type_defs.py` & `types-aiobotocore-signer-2.9.1/types_aiobotocore_signer/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AddProfilePermissionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "BlobTypeDef",
     "CancelSigningProfileRequestRequestTypeDef",
     "DescribeSigningJobRequestRequestTypeDef",
     "WaiterConfigTypeDef",
```

### Comparing `types-aiobotocore-signer-2.9.0/types_aiobotocore_signer/type_defs.pyi` & `types-aiobotocore-signer-2.9.1/types_aiobotocore_signer/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.9.0/types_aiobotocore_signer/waiter.py` & `types-aiobotocore-signer-2.9.1/types_aiobotocore_signer/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.9.0/types_aiobotocore_signer/waiter.pyi` & `types-aiobotocore-signer-2.9.1/types_aiobotocore_signer/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.9.0/types_aiobotocore_signer.egg-info/PKG-INFO` & `types-aiobotocore-signer-2.9.1/types_aiobotocore_signer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-signer
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.signer 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.signer 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/
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
 
 <a id="types-aiobotocore-signer"></a>
 
 # types-aiobotocore-signer
 
 [![PyPI - types-aiobotocore-signer](https://img.shields.io/pypi/v/types-aiobotocore-signer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-signer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-signer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-signer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-signer)](https://pepy.tech/project/types-aiobotocore-signer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.signer 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
+[aiobotocore.signer 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
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
 [types-aiobotocore-signer docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-signer-2.9.0/types_aiobotocore_signer.egg-info/SOURCES.txt` & `types-aiobotocore-signer-2.9.1/types_aiobotocore_signer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

