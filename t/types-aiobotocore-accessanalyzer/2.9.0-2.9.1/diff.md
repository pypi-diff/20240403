# Comparing `tmp/types-aiobotocore-accessanalyzer-2.9.0.tar.gz` & `tmp/types-aiobotocore-accessanalyzer-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-accessanalyzer-2.9.0.tar", last modified: Wed Dec 13 19:58:28 2023, max compression
+gzip compressed data, was "types-aiobotocore-accessanalyzer-2.9.1.tar", last modified: Thu Jan 18 01:19:57 2024, max compression
```

## Comparing `types-aiobotocore-accessanalyzer-2.9.0.tar` & `types-aiobotocore-accessanalyzer-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:28.642145 types-aiobotocore-accessanalyzer-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:40:33.000000 types-aiobotocore-accessanalyzer-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14724 2023-12-13 19:58:28.642145 types-aiobotocore-accessanalyzer-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13133 2023-12-13 19:40:33.000000 types-aiobotocore-accessanalyzer-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:28.642145 types-aiobotocore-accessanalyzer-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2023-12-13 19:40:33.000000 types-aiobotocore-accessanalyzer-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:28.642145 types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer/
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2023-12-13 19:40:33.000000 types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2023-12-13 19:40:33.000000 types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      960 2023-12-13 19:40:33.000000 types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30621 2023-12-13 19:40:33.000000 types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    30617 2023-12-13 19:40:33.000000 types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13413 2023-12-13 19:40:33.000000 types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13411 2023-12-13 19:40:33.000000 types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13296 2023-12-13 19:40:33.000000 types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13284 2023-12-13 19:40:33.000000 types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:40:33.000000 types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    39300 2023-12-13 19:40:34.000000 types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    39299 2023-12-13 19:40:34.000000 types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:40:33.000000 types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:28.642145 types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14724 2023-12-13 19:58:28.000000 types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-12-13 19:58:28.000000 types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:28.000000 types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:28.000000 types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:28.000000 types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-13 19:58:28.000000 types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:57.265542 types-aiobotocore-accessanalyzer-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:02:32.000000 types-aiobotocore-accessanalyzer-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14744 2024-01-18 01:19:57.265542 types-aiobotocore-accessanalyzer-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13133 2024-01-18 01:02:32.000000 types-aiobotocore-accessanalyzer-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:19:57.265542 types-aiobotocore-accessanalyzer-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-01-18 01:02:32.000000 types-aiobotocore-accessanalyzer-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:57.261541 types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-01-18 01:02:32.000000 types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-01-18 01:02:32.000000 types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-01-18 01:02:32.000000 types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30634 2024-01-18 01:02:32.000000 types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30631 2024-01-18 01:02:32.000000 types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13411 2024-01-18 01:02:33.000000 types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13411 2024-01-18 01:02:33.000000 types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13300 2024-01-18 01:02:33.000000 types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13289 2024-01-18 01:02:32.000000 types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:02:32.000000 types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    39299 2024-01-18 01:02:34.000000 types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39299 2024-01-18 01:02:34.000000 types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:02:32.000000 types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:57.265542 types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14744 2024-01-18 01:19:57.000000 types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-01-18 01:19:57.000000 types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:19:57.000000 types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:19:57.000000 types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:19:57.000000 types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-18 01:19:57.000000 types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-accessanalyzer-2.9.0/LICENSE` & `types-aiobotocore-accessanalyzer-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-accessanalyzer-2.9.0/PKG-INFO` & `types-aiobotocore-accessanalyzer-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-accessanalyzer
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AccessAnalyzer 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AccessAnalyzer 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/
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
 
 <a id="types-aiobotocore-accessanalyzer"></a>
 
 # types-aiobotocore-accessanalyzer
 
 [![PyPI - types-aiobotocore-accessanalyzer](https://img.shields.io/pypi/v/types-aiobotocore-accessanalyzer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-accessanalyzer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-accessanalyzer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-accessanalyzer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-accessanalyzer)](https://pepy.tech/project/types-aiobotocore-accessanalyzer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AccessAnalyzer 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
+[aiobotocore.AccessAnalyzer 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
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
 [types-aiobotocore-accessanalyzer docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-accessanalyzer-2.9.0/README.md` & `types-aiobotocore-accessanalyzer-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-accessanalyzer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-accessanalyzer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-accessanalyzer)](https://pepy.tech/project/types-aiobotocore-accessanalyzer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AccessAnalyzer 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
+[aiobotocore.AccessAnalyzer 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
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
 [types-aiobotocore-accessanalyzer docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-accessanalyzer-2.9.0/setup.py` & `types-aiobotocore-accessanalyzer-2.9.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-accessanalyzer",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_accessanalyzer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.AccessAnalyzer 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.AccessAnalyzer 2.9.1 service generated with"
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
     keywords="aiobotocore accessanalyzer type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_accessanalyzer": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer/__init__.py` & `types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     ListFindingsV2Paginator,
     ListPolicyGenerationsPaginator,
     ValidatePolicyPaginator,
 )
 
 Client = AccessAnalyzerClient
 
-
 __all__ = (
     "AccessAnalyzerClient",
     "Client",
     "GetFindingV2Paginator",
     "ListAccessPreviewFindingsPaginator",
     "ListAccessPreviewsPaginator",
     "ListAnalyzedResourcesPaginator",
```

### Comparing `types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer/__init__.pyi` & `types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer/__main__.py` & `types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AccessAnalyzer 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.AccessAnalyzer 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer\nOther"
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

### Comparing `types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer/client.py` & `types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,15 +77,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("AccessAnalyzerClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -152,29 +151,29 @@
         """
 
     async def check_access_not_granted(
         self,
         *,
         policyDocument: str,
         access: Sequence[AccessTypeDef],
-        policyType: AccessCheckPolicyTypeType
+        policyType: AccessCheckPolicyTypeType,
     ) -> CheckAccessNotGrantedResponseTypeDef:
         """
         Checks whether the specified access isn't allowed by a policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.check_access_not_granted)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/client/#check_access_not_granted)
         """
 
     async def check_no_new_access(
         self,
         *,
         newPolicyDocument: str,
         existingPolicyDocument: str,
-        policyType: AccessCheckPolicyTypeType
+        policyType: AccessCheckPolicyTypeType,
     ) -> CheckNoNewAccessResponseTypeDef:
         """
         Checks whether new access is allowed for an updated policy when compared to the
         existing
         policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.check_no_new_access)
@@ -190,15 +189,15 @@
         """
 
     async def create_access_preview(
         self,
         *,
         analyzerArn: str,
         configurations: Mapping[str, ConfigurationTypeDef],
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateAccessPreviewResponseTypeDef:
         """
         Creates an access preview that allows you to preview IAM Access Analyzer
         findings for your resource before deploying resource
         permissions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.create_access_preview)
@@ -209,30 +208,30 @@
         self,
         *,
         analyzerName: str,
         type: TypeType,
         archiveRules: Sequence[InlineArchiveRuleTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         clientToken: str = ...,
-        configuration: AnalyzerConfigurationTypeDef = ...
+        configuration: AnalyzerConfigurationTypeDef = ...,
     ) -> CreateAnalyzerResponseTypeDef:
         """
         Creates an analyzer for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.create_analyzer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/client/#create_analyzer)
         """
 
     async def create_archive_rule(
         self,
         *,
         analyzerName: str,
         ruleName: str,
         filter: Mapping[str, CriterionTypeDef],
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates an archive rule for the specified analyzer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.create_archive_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/client/#create_archive_rule)
         """
@@ -328,15 +327,15 @@
         """
 
     async def get_generated_policy(
         self,
         *,
         jobId: str,
         includeResourcePlaceholders: bool = ...,
-        includeServiceLevelTemplate: bool = ...
+        includeServiceLevelTemplate: bool = ...,
     ) -> GetGeneratedPolicyResponseTypeDef:
         """
         Retrieves the policy that was generated using `StartPolicyGeneration`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.get_generated_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/client/#get_generated_policy)
         """
@@ -344,15 +343,15 @@
     async def list_access_preview_findings(
         self,
         *,
         accessPreviewId: str,
         analyzerArn: str,
         filter: Mapping[str, CriterionTypeDef] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListAccessPreviewFindingsResponseTypeDef:
         """
         Retrieves a list of access preview findings generated by the specified access
         preview.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.list_access_preview_findings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/client/#list_access_preview_findings)
@@ -370,15 +369,15 @@
 
     async def list_analyzed_resources(
         self,
         *,
         analyzerArn: str,
         resourceType: ResourceTypeType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListAnalyzedResourcesResponseTypeDef:
         """
         Retrieves a list of resources of the specified type that have been analyzed by
         the specified
         analyzer..
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.list_analyzed_resources)
@@ -408,15 +407,15 @@
     async def list_findings(
         self,
         *,
         analyzerArn: str,
         filter: Mapping[str, CriterionTypeDef] = ...,
         sort: SortCriteriaTypeDef = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListFindingsResponseTypeDef:
         """
         Retrieves a list of findings generated by the specified analyzer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.list_findings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/client/#list_findings)
         """
@@ -424,15 +423,15 @@
     async def list_findings_v2(
         self,
         *,
         analyzerArn: str,
         filter: Mapping[str, CriterionTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        sort: SortCriteriaTypeDef = ...
+        sort: SortCriteriaTypeDef = ...,
     ) -> ListFindingsV2ResponseTypeDef:
         """
         Retrieves a list of findings generated by the specified analyzer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.list_findings_v2)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/client/#list_findings_v2)
         """
@@ -458,15 +457,15 @@
         """
 
     async def start_policy_generation(
         self,
         *,
         policyGenerationDetails: PolicyGenerationDetailsTypeDef,
         cloudTrailDetails: CloudTrailDetailsTypeDef = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> StartPolicyGenerationResponseTypeDef:
         """
         Starts the policy generation request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.start_policy_generation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/client/#start_policy_generation)
         """
@@ -499,15 +498,15 @@
 
     async def update_archive_rule(
         self,
         *,
         analyzerName: str,
         ruleName: str,
         filter: Mapping[str, CriterionTypeDef],
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the criteria and values for the specified archive rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.update_archive_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/client/#update_archive_rule)
         """
@@ -515,15 +514,15 @@
     async def update_findings(
         self,
         *,
         analyzerArn: str,
         status: FindingStatusUpdateType,
         ids: Sequence[str] = ...,
         resourceArn: str = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the status for the specified findings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.update_findings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/client/#update_findings)
         """
@@ -532,15 +531,15 @@
         self,
         *,
         policyDocument: str,
         policyType: PolicyTypeType,
         locale: LocaleType = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        validatePolicyResourceType: ValidatePolicyResourceTypeType = ...
+        validatePolicyResourceType: ValidatePolicyResourceTypeType = ...,
     ) -> ValidatePolicyResponseTypeDef:
         """
         Requests the validation of a policy and returns a list of findings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.validate_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/client/#validate_policy)
         """
```

### Comparing `types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer/client.pyi` & `types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -148,29 +148,29 @@
         """
 
     async def check_access_not_granted(
         self,
         *,
         policyDocument: str,
         access: Sequence[AccessTypeDef],
-        policyType: AccessCheckPolicyTypeType
+        policyType: AccessCheckPolicyTypeType,
     ) -> CheckAccessNotGrantedResponseTypeDef:
         """
         Checks whether the specified access isn't allowed by a policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.check_access_not_granted)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/client/#check_access_not_granted)
         """
 
     async def check_no_new_access(
         self,
         *,
         newPolicyDocument: str,
         existingPolicyDocument: str,
-        policyType: AccessCheckPolicyTypeType
+        policyType: AccessCheckPolicyTypeType,
     ) -> CheckNoNewAccessResponseTypeDef:
         """
         Checks whether new access is allowed for an updated policy when compared to the
         existing
         policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.check_no_new_access)
@@ -186,15 +186,15 @@
         """
 
     async def create_access_preview(
         self,
         *,
         analyzerArn: str,
         configurations: Mapping[str, ConfigurationTypeDef],
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateAccessPreviewResponseTypeDef:
         """
         Creates an access preview that allows you to preview IAM Access Analyzer
         findings for your resource before deploying resource
         permissions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.create_access_preview)
@@ -205,30 +205,30 @@
         self,
         *,
         analyzerName: str,
         type: TypeType,
         archiveRules: Sequence[InlineArchiveRuleTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         clientToken: str = ...,
-        configuration: AnalyzerConfigurationTypeDef = ...
+        configuration: AnalyzerConfigurationTypeDef = ...,
     ) -> CreateAnalyzerResponseTypeDef:
         """
         Creates an analyzer for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.create_analyzer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/client/#create_analyzer)
         """
 
     async def create_archive_rule(
         self,
         *,
         analyzerName: str,
         ruleName: str,
         filter: Mapping[str, CriterionTypeDef],
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates an archive rule for the specified analyzer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.create_archive_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/client/#create_archive_rule)
         """
@@ -324,15 +324,15 @@
         """
 
     async def get_generated_policy(
         self,
         *,
         jobId: str,
         includeResourcePlaceholders: bool = ...,
-        includeServiceLevelTemplate: bool = ...
+        includeServiceLevelTemplate: bool = ...,
     ) -> GetGeneratedPolicyResponseTypeDef:
         """
         Retrieves the policy that was generated using `StartPolicyGeneration`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.get_generated_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/client/#get_generated_policy)
         """
@@ -340,15 +340,15 @@
     async def list_access_preview_findings(
         self,
         *,
         accessPreviewId: str,
         analyzerArn: str,
         filter: Mapping[str, CriterionTypeDef] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListAccessPreviewFindingsResponseTypeDef:
         """
         Retrieves a list of access preview findings generated by the specified access
         preview.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.list_access_preview_findings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/client/#list_access_preview_findings)
@@ -366,15 +366,15 @@
 
     async def list_analyzed_resources(
         self,
         *,
         analyzerArn: str,
         resourceType: ResourceTypeType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListAnalyzedResourcesResponseTypeDef:
         """
         Retrieves a list of resources of the specified type that have been analyzed by
         the specified
         analyzer..
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.list_analyzed_resources)
@@ -404,15 +404,15 @@
     async def list_findings(
         self,
         *,
         analyzerArn: str,
         filter: Mapping[str, CriterionTypeDef] = ...,
         sort: SortCriteriaTypeDef = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListFindingsResponseTypeDef:
         """
         Retrieves a list of findings generated by the specified analyzer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.list_findings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/client/#list_findings)
         """
@@ -420,15 +420,15 @@
     async def list_findings_v2(
         self,
         *,
         analyzerArn: str,
         filter: Mapping[str, CriterionTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        sort: SortCriteriaTypeDef = ...
+        sort: SortCriteriaTypeDef = ...,
     ) -> ListFindingsV2ResponseTypeDef:
         """
         Retrieves a list of findings generated by the specified analyzer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.list_findings_v2)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/client/#list_findings_v2)
         """
@@ -454,15 +454,15 @@
         """
 
     async def start_policy_generation(
         self,
         *,
         policyGenerationDetails: PolicyGenerationDetailsTypeDef,
         cloudTrailDetails: CloudTrailDetailsTypeDef = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> StartPolicyGenerationResponseTypeDef:
         """
         Starts the policy generation request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.start_policy_generation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/client/#start_policy_generation)
         """
@@ -495,15 +495,15 @@
 
     async def update_archive_rule(
         self,
         *,
         analyzerName: str,
         ruleName: str,
         filter: Mapping[str, CriterionTypeDef],
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the criteria and values for the specified archive rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.update_archive_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/client/#update_archive_rule)
         """
@@ -511,15 +511,15 @@
     async def update_findings(
         self,
         *,
         analyzerArn: str,
         status: FindingStatusUpdateType,
         ids: Sequence[str] = ...,
         resourceArn: str = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the status for the specified findings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.update_findings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/client/#update_findings)
         """
@@ -528,15 +528,15 @@
         self,
         *,
         policyDocument: str,
         policyType: PolicyTypeType,
         locale: LocaleType = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        validatePolicyResourceType: ValidatePolicyResourceTypeType = ...
+        validatePolicyResourceType: ValidatePolicyResourceTypeType = ...,
     ) -> ValidatePolicyResponseTypeDef:
         """
         Requests the validation of a policy and returns a list of findings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.validate_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/client/#validate_policy)
         """
```

### Comparing `types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer/literals.py` & `types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AccessCheckPolicyTypeType",
     "AccessPreviewStatusReasonCodeType",
     "AccessPreviewStatusType",
     "AclPermissionType",
     "AnalyzerStatusType",
     "CheckAccessNotGrantedResultType",
@@ -57,15 +56,14 @@
     "AccessAnalyzerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AccessCheckPolicyTypeType = Literal["IDENTITY_POLICY", "RESOURCE_POLICY"]
 AccessPreviewStatusReasonCodeType = Literal["INTERNAL_ERROR", "INVALID_CONFIGURATION"]
 AccessPreviewStatusType = Literal["COMPLETED", "CREATING", "FAILED"]
 AclPermissionType = Literal["FULL_CONTROL", "READ", "READ_ACP", "WRITE", "WRITE_ACP"]
 AnalyzerStatusType = Literal["ACTIVE", "CREATING", "DISABLED", "FAILED"]
 CheckAccessNotGrantedResultType = Literal["FAIL", "PASS"]
 CheckNoNewAccessResultType = Literal["FAIL", "PASS"]
```

### Comparing `types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer/literals.pyi` & `types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer/paginator.py` & `types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,14 @@
     "ListArchiveRulesPaginator",
     "ListFindingsPaginator",
     "ListFindingsV2Paginator",
     "ListPolicyGenerationsPaginator",
     "ValidatePolicyPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -114,15 +113,15 @@
 
     def paginate(
         self,
         *,
         accessPreviewId: str,
         analyzerArn: str,
         filter: Mapping[str, CriterionTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAccessPreviewFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListAccessPreviewFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/paginators/#listaccesspreviewfindingspaginator)
         """
 
 
@@ -148,15 +147,15 @@
     """
 
     def paginate(
         self,
         *,
         analyzerArn: str,
         resourceType: ResourceTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAnalyzedResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListAnalyzedResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/paginators/#listanalyzedresourcespaginator)
         """
 
 
@@ -198,15 +197,15 @@
 
     def paginate(
         self,
         *,
         analyzerArn: str,
         filter: Mapping[str, CriterionTypeDef] = ...,
         sort: SortCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/paginators/#listfindingspaginator)
         """
 
 
@@ -218,15 +217,15 @@
 
     def paginate(
         self,
         *,
         analyzerArn: str,
         filter: Mapping[str, CriterionTypeDef] = ...,
         sort: SortCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFindingsV2ResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListFindingsV2.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/paginators/#listfindingsv2paginator)
         """
 
 
@@ -254,13 +253,13 @@
     def paginate(
         self,
         *,
         policyDocument: str,
         policyType: PolicyTypeType,
         locale: LocaleType = ...,
         validatePolicyResourceType: ValidatePolicyResourceTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ValidatePolicyResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ValidatePolicy.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/paginators/#validatepolicypaginator)
         """
```

### Comparing `types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer/paginator.pyi` & `types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
     def paginate(
         self,
         *,
         accessPreviewId: str,
         analyzerArn: str,
         filter: Mapping[str, CriterionTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAccessPreviewFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListAccessPreviewFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/paginators/#listaccesspreviewfindingspaginator)
         """
 
 class ListAccessPreviewsPaginator(AioPaginator):
@@ -142,15 +142,15 @@
     """
 
     def paginate(
         self,
         *,
         analyzerArn: str,
         resourceType: ResourceTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAnalyzedResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListAnalyzedResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/paginators/#listanalyzedresourcespaginator)
         """
 
 class ListAnalyzersPaginator(AioPaginator):
@@ -189,15 +189,15 @@
 
     def paginate(
         self,
         *,
         analyzerArn: str,
         filter: Mapping[str, CriterionTypeDef] = ...,
         sort: SortCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/paginators/#listfindingspaginator)
         """
 
 class ListFindingsV2Paginator(AioPaginator):
@@ -208,15 +208,15 @@
 
     def paginate(
         self,
         *,
         analyzerArn: str,
         filter: Mapping[str, CriterionTypeDef] = ...,
         sort: SortCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFindingsV2ResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListFindingsV2.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/paginators/#listfindingsv2paginator)
         """
 
 class ListPolicyGenerationsPaginator(AioPaginator):
@@ -242,13 +242,13 @@
     def paginate(
         self,
         *,
         policyDocument: str,
         policyType: PolicyTypeType,
         locale: LocaleType = ...,
         validatePolicyResourceType: ValidatePolicyResourceTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ValidatePolicyResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ValidatePolicy.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/paginators/#validatepolicypaginator)
         """
```

### Comparing `types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer/type_defs.py` & `types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccessPreviewStatusReasonTypeDef",
     "AccessTypeDef",
     "AclGranteeTypeDef",
     "AnalyzedResourceSummaryTypeDef",
     "AnalyzedResourceTypeDef",
     "UnusedAccessConfigurationTypeDef",
```

### Comparing `types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer/type_defs.pyi` & `types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer.egg-info/PKG-INFO` & `types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-accessanalyzer
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AccessAnalyzer 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AccessAnalyzer 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/
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
 
 <a id="types-aiobotocore-accessanalyzer"></a>
 
 # types-aiobotocore-accessanalyzer
 
 [![PyPI - types-aiobotocore-accessanalyzer](https://img.shields.io/pypi/v/types-aiobotocore-accessanalyzer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-accessanalyzer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-accessanalyzer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-accessanalyzer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-accessanalyzer)](https://pepy.tech/project/types-aiobotocore-accessanalyzer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AccessAnalyzer 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
+[aiobotocore.AccessAnalyzer 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
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
 [types-aiobotocore-accessanalyzer docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-accessanalyzer-2.9.0/types_aiobotocore_accessanalyzer.egg-info/SOURCES.txt` & `types-aiobotocore-accessanalyzer-2.9.1/types_aiobotocore_accessanalyzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

