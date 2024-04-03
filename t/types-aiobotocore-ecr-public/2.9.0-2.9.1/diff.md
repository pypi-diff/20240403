# Comparing `tmp/types-aiobotocore-ecr-public-2.9.0.tar.gz` & `tmp/types-aiobotocore-ecr-public-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ecr-public-2.9.0.tar", last modified: Wed Dec 13 19:59:11 2023, max compression
+gzip compressed data, was "types-aiobotocore-ecr-public-2.9.1.tar", last modified: Thu Jan 18 01:20:36 2024, max compression
```

## Comparing `types-aiobotocore-ecr-public-2.9.0.tar` & `types-aiobotocore-ecr-public-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:11.937790 types-aiobotocore-ecr-public-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:45:24.000000 types-aiobotocore-ecr-public-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13619 2023-12-13 19:59:11.937790 types-aiobotocore-ecr-public-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12045 2023-12-13 19:45:24.000000 types-aiobotocore-ecr-public-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:11.937790 types-aiobotocore-ecr-public-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2023-12-13 19:45:24.000000 types-aiobotocore-ecr-public-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:11.937790 types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public/
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2023-12-13 19:45:24.000000 types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2023-12-13 19:45:24.000000 types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      942 2023-12-13 19:45:24.000000 types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22148 2023-12-13 19:45:24.000000 types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    22144 2023-12-13 19:45:24.000000 types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9290 2023-12-13 19:45:26.000000 types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9288 2023-12-13 19:45:24.000000 types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2023-12-13 19:45:24.000000 types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2023-12-13 19:45:24.000000 types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:45:24.000000 types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    18899 2023-12-13 19:45:26.000000 types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18898 2023-12-13 19:45:26.000000 types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:45:24.000000 types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:11.937790 types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13619 2023-12-13 19:59:11.000000 types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      870 2023-12-13 19:59:11.000000 types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:11.000000 types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:11.000000 types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:11.000000 types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-13 19:59:11.000000 types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:36.973360 types-aiobotocore-ecr-public-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:07:20.000000 types-aiobotocore-ecr-public-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13639 2024-01-18 01:20:36.973360 types-aiobotocore-ecr-public-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-01-18 01:07:20.000000 types-aiobotocore-ecr-public-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:36.973360 types-aiobotocore-ecr-public-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-01-18 01:07:20.000000 types-aiobotocore-ecr-public-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:36.969360 types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public/
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-01-18 01:07:20.000000 types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-01-18 01:07:20.000000 types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-01-18 01:07:20.000000 types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22156 2024-01-18 01:07:20.000000 types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22153 2024-01-18 01:07:20.000000 types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9288 2024-01-18 01:07:20.000000 types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9288 2024-01-18 01:07:20.000000 types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-01-18 01:07:20.000000 types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-01-18 01:07:20.000000 types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:07:20.000000 types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    18898 2024-01-18 01:07:21.000000 types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18898 2024-01-18 01:07:20.000000 types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:07:20.000000 types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:36.973360 types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13639 2024-01-18 01:20:36.000000 types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-01-18 01:20:36.000000 types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:36.000000 types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:36.000000 types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:36.000000 types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-18 01:20:36.000000 types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ecr-public-2.9.0/LICENSE` & `types-aiobotocore-ecr-public-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-ecr-public-2.9.0/PKG-INFO` & `types-aiobotocore-ecr-public-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ecr-public
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ECRPublic 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ECRPublic 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/
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
 
 <a id="types-aiobotocore-ecr-public"></a>
 
 # types-aiobotocore-ecr-public
 
 [![PyPI - types-aiobotocore-ecr-public](https://img.shields.io/pypi/v/types-aiobotocore-ecr-public.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecr-public)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ecr-public.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecr-public)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ecr-public)](https://pepy.tech/project/types-aiobotocore-ecr-public)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ECRPublic 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
+[aiobotocore.ECRPublic 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
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
 [types-aiobotocore-ecr-public docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ecr-public-2.9.0/README.md` & `types-aiobotocore-ecr-public-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ecr-public.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecr-public)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ecr-public)](https://pepy.tech/project/types-aiobotocore-ecr-public)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ECRPublic 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
+[aiobotocore.ECRPublic 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
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
 [types-aiobotocore-ecr-public docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ecr-public-2.9.0/setup.py` & `types-aiobotocore-ecr-public-2.9.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ecr-public",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_ecr_public"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ECRPublic 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.ECRPublic 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore ecr-public type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_ecr_public": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public/__init__.py` & `types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     DescribeImageTagsPaginator,
     DescribeRegistriesPaginator,
     DescribeRepositoriesPaginator,
 )
 
 Client = ECRPublicClient
 
-
 __all__ = (
     "Client",
     "DescribeImageTagsPaginator",
     "DescribeImagesPaginator",
     "DescribeRegistriesPaginator",
     "DescribeRepositoriesPaginator",
     "ECRPublicClient",
```

### Comparing `types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public/__init__.pyi` & `types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public/__main__.py` & `types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ECRPublic 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ECRPublic 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic\nOther"
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

### Comparing `types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public/client.py` & `types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ECRPublicClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -130,15 +129,15 @@
         """
 
     async def batch_delete_image(
         self,
         *,
         repositoryName: str,
         imageIds: Sequence[ImageIdentifierTypeDef],
-        registryId: str = ...
+        registryId: str = ...,
     ) -> BatchDeleteImageResponseTypeDef:
         """
         Deletes a list of specified images that are within a repository in a public
         registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.batch_delete_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/client/#batch_delete_image)
@@ -162,15 +161,15 @@
 
     async def complete_layer_upload(
         self,
         *,
         repositoryName: str,
         uploadId: str,
         layerDigests: Sequence[str],
-        registryId: str = ...
+        registryId: str = ...,
     ) -> CompleteLayerUploadResponseTypeDef:
         """
         Informs Amazon ECR that the image layer upload is complete for a specified
         public registry, repository name, and upload
         ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.complete_layer_upload)
@@ -178,15 +177,15 @@
         """
 
     async def create_repository(
         self,
         *,
         repositoryName: str,
         catalogData: RepositoryCatalogDataInputTypeDef = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRepositoryResponseTypeDef:
         """
         Creates a repository in a public registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.create_repository)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/client/#create_repository)
         """
@@ -213,15 +212,15 @@
 
     async def describe_image_tags(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribeImageTagsResponseTypeDef:
         """
         Returns the image tag details for a repository in a public registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.describe_image_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/client/#describe_image_tags)
         """
@@ -229,15 +228,15 @@
     async def describe_images(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         imageIds: Sequence[ImageIdentifierTypeDef] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribeImagesResponseTypeDef:
         """
         Returns metadata that's related to the images in a repository in a public
         registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.describe_images)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/client/#describe_images)
@@ -255,15 +254,15 @@
 
     async def describe_repositories(
         self,
         *,
         registryId: str = ...,
         repositoryNames: Sequence[str] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribeRepositoriesResponseTypeDef:
         """
         Describes repositories that are in a public registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.describe_repositories)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/client/#describe_repositories)
         """
@@ -342,15 +341,15 @@
         self,
         *,
         repositoryName: str,
         imageManifest: str,
         registryId: str = ...,
         imageManifestMediaType: str = ...,
         imageTag: str = ...,
-        imageDigest: str = ...
+        imageDigest: str = ...,
     ) -> PutImageResponseTypeDef:
         """
         Creates or updates the image manifest and tags that are associated with an
         image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.put_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/client/#put_image)
@@ -367,15 +366,15 @@
         """
 
     async def put_repository_catalog_data(
         self,
         *,
         repositoryName: str,
         catalogData: RepositoryCatalogDataInputTypeDef,
-        registryId: str = ...
+        registryId: str = ...,
     ) -> PutRepositoryCatalogDataResponseTypeDef:
         """
         Creates or updates the catalog data for a repository in a public registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.put_repository_catalog_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/client/#put_repository_catalog_data)
         """
@@ -412,15 +411,15 @@
         self,
         *,
         repositoryName: str,
         uploadId: str,
         partFirstByte: int,
         partLastByte: int,
         layerPartBlob: BlobTypeDef,
-        registryId: str = ...
+        registryId: str = ...,
     ) -> UploadLayerPartResponseTypeDef:
         """
         Uploads an image layer part to Amazon ECR.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.upload_layer_part)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/client/#upload_layer_part)
         """
```

### Comparing `types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public/client.pyi` & `types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         """
 
     async def batch_delete_image(
         self,
         *,
         repositoryName: str,
         imageIds: Sequence[ImageIdentifierTypeDef],
-        registryId: str = ...
+        registryId: str = ...,
     ) -> BatchDeleteImageResponseTypeDef:
         """
         Deletes a list of specified images that are within a repository in a public
         registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.batch_delete_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/client/#batch_delete_image)
@@ -158,15 +158,15 @@
 
     async def complete_layer_upload(
         self,
         *,
         repositoryName: str,
         uploadId: str,
         layerDigests: Sequence[str],
-        registryId: str = ...
+        registryId: str = ...,
     ) -> CompleteLayerUploadResponseTypeDef:
         """
         Informs Amazon ECR that the image layer upload is complete for a specified
         public registry, repository name, and upload
         ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.complete_layer_upload)
@@ -174,15 +174,15 @@
         """
 
     async def create_repository(
         self,
         *,
         repositoryName: str,
         catalogData: RepositoryCatalogDataInputTypeDef = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRepositoryResponseTypeDef:
         """
         Creates a repository in a public registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.create_repository)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/client/#create_repository)
         """
@@ -209,15 +209,15 @@
 
     async def describe_image_tags(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribeImageTagsResponseTypeDef:
         """
         Returns the image tag details for a repository in a public registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.describe_image_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/client/#describe_image_tags)
         """
@@ -225,15 +225,15 @@
     async def describe_images(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         imageIds: Sequence[ImageIdentifierTypeDef] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribeImagesResponseTypeDef:
         """
         Returns metadata that's related to the images in a repository in a public
         registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.describe_images)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/client/#describe_images)
@@ -251,15 +251,15 @@
 
     async def describe_repositories(
         self,
         *,
         registryId: str = ...,
         repositoryNames: Sequence[str] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribeRepositoriesResponseTypeDef:
         """
         Describes repositories that are in a public registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.describe_repositories)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/client/#describe_repositories)
         """
@@ -338,15 +338,15 @@
         self,
         *,
         repositoryName: str,
         imageManifest: str,
         registryId: str = ...,
         imageManifestMediaType: str = ...,
         imageTag: str = ...,
-        imageDigest: str = ...
+        imageDigest: str = ...,
     ) -> PutImageResponseTypeDef:
         """
         Creates or updates the image manifest and tags that are associated with an
         image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.put_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/client/#put_image)
@@ -363,15 +363,15 @@
         """
 
     async def put_repository_catalog_data(
         self,
         *,
         repositoryName: str,
         catalogData: RepositoryCatalogDataInputTypeDef,
-        registryId: str = ...
+        registryId: str = ...,
     ) -> PutRepositoryCatalogDataResponseTypeDef:
         """
         Creates or updates the catalog data for a repository in a public registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.put_repository_catalog_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/client/#put_repository_catalog_data)
         """
@@ -408,15 +408,15 @@
         self,
         *,
         repositoryName: str,
         uploadId: str,
         partFirstByte: int,
         partLastByte: int,
         layerPartBlob: BlobTypeDef,
-        registryId: str = ...
+        registryId: str = ...,
     ) -> UploadLayerPartResponseTypeDef:
         """
         Uploads an image layer part to Amazon ECR.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Client.upload_layer_part)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/client/#upload_layer_part)
         """
```

### Comparing `types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public/literals.py` & `types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public/literals.py`

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
     "DescribeImageTagsPaginatorName",
     "DescribeImagesPaginatorName",
     "DescribeRegistriesPaginatorName",
     "DescribeRepositoriesPaginatorName",
     "ImageFailureCodeType",
     "LayerAvailabilityType",
@@ -32,15 +31,14 @@
     "ECRPublicServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DescribeImageTagsPaginatorName = Literal["describe_image_tags"]
 DescribeImagesPaginatorName = Literal["describe_images"]
 DescribeRegistriesPaginatorName = Literal["describe_registries"]
 DescribeRepositoriesPaginatorName = Literal["describe_repositories"]
 ImageFailureCodeType = Literal[
     "ImageNotFound",
     "ImageReferencedByManifestList",
```

### Comparing `types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public/literals.pyi` & `types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public/paginator.py` & `types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 __all__ = (
     "DescribeImageTagsPaginator",
     "DescribeImagesPaginator",
     "DescribeRegistriesPaginator",
     "DescribeRepositoriesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -66,15 +65,15 @@
     """
 
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeImageTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeImageTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/paginators/#describeimagetagspaginator)
         """
 
 
@@ -86,15 +85,15 @@
 
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         imageIds: Sequence[ImageIdentifierTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeImagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeImages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/paginators/#describeimagespaginator)
         """
 
 
@@ -120,13 +119,13 @@
     """
 
     def paginate(
         self,
         *,
         registryId: str = ...,
         repositoryNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRepositoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeRepositories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/paginators/#describerepositoriespaginator)
         """
```

### Comparing `types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public/paginator.pyi` & `types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     """
 
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeImageTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeImageTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/paginators/#describeimagetagspaginator)
         """
 
 class DescribeImagesPaginator(AioPaginator):
@@ -82,15 +82,15 @@
 
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         imageIds: Sequence[ImageIdentifierTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeImagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeImages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/paginators/#describeimagespaginator)
         """
 
 class DescribeRegistriesPaginator(AioPaginator):
@@ -114,13 +114,13 @@
     """
 
     def paginate(
         self,
         *,
         registryId: str = ...,
         repositoryNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRepositoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeRepositories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/paginators/#describerepositoriespaginator)
         """
```

### Comparing `types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public/type_defs.py` & `types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AuthorizationDataTypeDef",
     "BatchCheckLayerAvailabilityRequestRequestTypeDef",
     "LayerFailureTypeDef",
     "LayerTypeDef",
     "ResponseMetadataTypeDef",
     "ImageIdentifierTypeDef",
```

### Comparing `types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public/type_defs.pyi` & `types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public.egg-info/PKG-INFO` & `types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ecr-public
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ECRPublic 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ECRPublic 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/
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
 
 <a id="types-aiobotocore-ecr-public"></a>
 
 # types-aiobotocore-ecr-public
 
 [![PyPI - types-aiobotocore-ecr-public](https://img.shields.io/pypi/v/types-aiobotocore-ecr-public.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecr-public)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ecr-public.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecr-public)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ecr-public)](https://pepy.tech/project/types-aiobotocore-ecr-public)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ECRPublic 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
+[aiobotocore.ECRPublic 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
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
 [types-aiobotocore-ecr-public docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ecr-public-2.9.0/types_aiobotocore_ecr_public.egg-info/SOURCES.txt` & `types-aiobotocore-ecr-public-2.9.1/types_aiobotocore_ecr_public.egg-info/SOURCES.txt`

 * *Files identical despite different names*

