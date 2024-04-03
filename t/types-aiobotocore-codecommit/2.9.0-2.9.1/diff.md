# Comparing `tmp/types-aiobotocore-codecommit-2.9.0.tar.gz` & `tmp/types-aiobotocore-codecommit-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codecommit-2.9.0.tar", last modified: Wed Dec 13 19:58:53 2023, max compression
+gzip compressed data, was "types-aiobotocore-codecommit-2.9.1.tar", last modified: Thu Jan 18 01:20:20 2024, max compression
```

## Comparing `types-aiobotocore-codecommit-2.9.0.tar` & `types-aiobotocore-codecommit-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:53.705940 types-aiobotocore-codecommit-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:42:47.000000 types-aiobotocore-codecommit-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14148 2023-12-13 19:58:53.705940 types-aiobotocore-codecommit-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12573 2023-12-13 19:42:47.000000 types-aiobotocore-codecommit-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:53.705940 types-aiobotocore-codecommit-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2023-12-13 19:42:47.000000 types-aiobotocore-codecommit-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:53.705940 types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit/
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2023-12-13 19:42:47.000000 types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2023-12-13 19:42:47.000000 types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      944 2023-12-13 19:42:47.000000 types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    75708 2023-12-13 19:42:48.000000 types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    75704 2023-12-13 19:42:48.000000 types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11503 2023-12-13 19:42:48.000000 types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11501 2023-12-13 19:42:48.000000 types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9886 2023-12-13 19:42:48.000000 types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9877 2023-12-13 19:42:48.000000 types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:42:47.000000 types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    67160 2023-12-13 19:42:50.000000 types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    67159 2023-12-13 19:42:50.000000 types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:42:47.000000 types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:53.705940 types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14148 2023-12-13 19:58:53.000000 types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      870 2023-12-13 19:58:53.000000 types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:53.000000 types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:53.000000 types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:53.000000 types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-13 19:58:53.000000 types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:20.129444 types-aiobotocore-codecommit-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:04:44.000000 types-aiobotocore-codecommit-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14168 2024-01-18 01:20:20.129444 types-aiobotocore-codecommit-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12573 2024-01-18 01:04:44.000000 types-aiobotocore-codecommit-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:20.129444 types-aiobotocore-codecommit-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-01-18 01:04:44.000000 types-aiobotocore-codecommit-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:20.129444 types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit/
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-18 01:04:44.000000 types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-18 01:04:44.000000 types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-01-18 01:04:44.000000 types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75735 2024-01-18 01:04:44.000000 types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75732 2024-01-18 01:04:44.000000 types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11501 2024-01-18 01:04:45.000000 types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11501 2024-01-18 01:04:45.000000 types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9891 2024-01-18 01:04:45.000000 types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9883 2024-01-18 01:04:44.000000 types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:04:44.000000 types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    67159 2024-01-18 01:04:47.000000 types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67159 2024-01-18 01:04:46.000000 types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:04:44.000000 types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:20.129444 types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14168 2024-01-18 01:20:20.000000 types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-01-18 01:20:20.000000 types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:20.000000 types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:20.000000 types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:20.000000 types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-18 01:20:20.000000 types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codecommit-2.9.0/LICENSE` & `types-aiobotocore-codecommit-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-codecommit-2.9.0/PKG-INFO` & `types-aiobotocore-codecommit-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codecommit
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CodeCommit 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CodeCommit 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/
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
 
 <a id="types-aiobotocore-codecommit"></a>
 
 # types-aiobotocore-codecommit
 
 [![PyPI - types-aiobotocore-codecommit](https://img.shields.io/pypi/v/types-aiobotocore-codecommit.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codecommit)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codecommit.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codecommit)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codecommit)](https://pepy.tech/project/types-aiobotocore-codecommit)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeCommit 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
+[aiobotocore.CodeCommit 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
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
 [types-aiobotocore-codecommit docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codecommit-2.9.0/README.md` & `types-aiobotocore-codecommit-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codecommit.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codecommit)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codecommit)](https://pepy.tech/project/types-aiobotocore-codecommit)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeCommit 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
+[aiobotocore.CodeCommit 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
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
 [types-aiobotocore-codecommit docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codecommit-2.9.0/setup.py` & `types-aiobotocore-codecommit-2.9.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codecommit",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_codecommit"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CodeCommit 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.CodeCommit 2.9.1 service generated with"
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
     keywords="aiobotocore codecommit type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_codecommit": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit/__init__.py` & `types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     ListBranchesPaginator,
     ListPullRequestsPaginator,
     ListRepositoriesPaginator,
 )
 
 Client = CodeCommitClient
 
-
 __all__ = (
     "Client",
     "CodeCommitClient",
     "DescribePullRequestEventsPaginator",
     "GetCommentsForComparedCommitPaginator",
     "GetCommentsForPullRequestPaginator",
     "GetDifferencesPaginator",
```

### Comparing `types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit/__init__.pyi` & `types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit/__main__.py` & `types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeCommit 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CodeCommit 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit\nOther"
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

### Comparing `types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit/client.py` & `types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CodeCommitClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -375,15 +374,15 @@
         sourceCommitSpecifier: str,
         mergeOption: MergeOptionTypeEnumType,
         maxMergeHunks: int = ...,
         maxConflictFiles: int = ...,
         filePaths: Sequence[str] = ...,
         conflictDetailLevel: ConflictDetailLevelTypeEnumType = ...,
         conflictResolutionStrategy: ConflictResolutionStrategyTypeEnumType = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> BatchDescribeMergeConflictsOutputTypeDef:
         """
         Returns information about one or more merge conflicts in the attempted merge of
         two commit specifiers using the squash or three-way merge
         strategy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.batch_describe_merge_conflicts)
@@ -439,15 +438,15 @@
         """
 
     async def create_approval_rule_template(
         self,
         *,
         approvalRuleTemplateName: str,
         approvalRuleTemplateContent: str,
-        approvalRuleTemplateDescription: str = ...
+        approvalRuleTemplateDescription: str = ...,
     ) -> CreateApprovalRuleTemplateOutputTypeDef:
         """
         Creates a template for approval rules that can then be associated with one or
         more repositories in your Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.create_approval_rule_template)
@@ -472,30 +471,30 @@
         parentCommitId: str = ...,
         authorName: str = ...,
         email: str = ...,
         commitMessage: str = ...,
         keepEmptyFolders: bool = ...,
         putFiles: Sequence[PutFileEntryTypeDef] = ...,
         deleteFiles: Sequence[DeleteFileEntryTypeDef] = ...,
-        setFileModes: Sequence[SetFileModeEntryTypeDef] = ...
+        setFileModes: Sequence[SetFileModeEntryTypeDef] = ...,
     ) -> CreateCommitOutputTypeDef:
         """
         Creates a commit for a repository on the tip of a specified branch.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.create_commit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#create_commit)
         """
 
     async def create_pull_request(
         self,
         *,
         title: str,
         targets: Sequence[TargetTypeDef],
         description: str = ...,
-        clientRequestToken: str = ...
+        clientRequestToken: str = ...,
     ) -> CreatePullRequestOutputTypeDef:
         """
         Creates a pull request in the specified repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.create_pull_request)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#create_pull_request)
         """
@@ -511,15 +510,15 @@
         """
 
     async def create_repository(
         self,
         *,
         repositoryName: str,
         repositoryDescription: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateRepositoryOutputTypeDef:
         """
         Creates a new, empty repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.create_repository)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#create_repository)
         """
@@ -533,15 +532,15 @@
         mergeOption: MergeOptionTypeEnumType,
         conflictDetailLevel: ConflictDetailLevelTypeEnumType = ...,
         conflictResolutionStrategy: ConflictResolutionStrategyTypeEnumType = ...,
         authorName: str = ...,
         email: str = ...,
         commitMessage: str = ...,
         keepEmptyFolders: bool = ...,
-        conflictResolution: ConflictResolutionTypeDef = ...
+        conflictResolution: ConflictResolutionTypeDef = ...,
     ) -> CreateUnreferencedMergeCommitOutputTypeDef:
         """
         Creates an unreferenced commit that represents the result of merging two
         branches using a specified merge
         strategy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.create_unreferenced_merge_commit)
@@ -585,15 +584,15 @@
         repositoryName: str,
         branchName: str,
         filePath: str,
         parentCommitId: str,
         keepEmptyFolders: bool = ...,
         commitMessage: str = ...,
         name: str = ...,
-        email: str = ...
+        email: str = ...,
     ) -> DeleteFileOutputTypeDef:
         """
         Deletes a specified file from a specified branch.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.delete_file)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#delete_file)
         """
@@ -623,15 +622,15 @@
         destinationCommitSpecifier: str,
         sourceCommitSpecifier: str,
         mergeOption: MergeOptionTypeEnumType,
         filePath: str,
         maxMergeHunks: int = ...,
         conflictDetailLevel: ConflictDetailLevelTypeEnumType = ...,
         conflictResolutionStrategy: ConflictResolutionStrategyTypeEnumType = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeMergeConflictsOutputTypeDef:
         """
         Returns information about one or more merge conflicts in the attempted merge of
         two commit specifiers using the squash or three-way merge
         strategy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.describe_merge_conflicts)
@@ -641,15 +640,15 @@
     async def describe_pull_request_events(
         self,
         *,
         pullRequestId: str,
         pullRequestEventType: PullRequestEventTypeType = ...,
         actorArn: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribePullRequestEventsOutputTypeDef:
         """
         Returns information about one or more pull request events.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.describe_pull_request_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#describe_pull_request_events)
         """
@@ -734,15 +733,15 @@
 
     async def get_comment_reactions(
         self,
         *,
         commentId: str,
         reactionUserArn: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetCommentReactionsOutputTypeDef:
         """
         Returns information about reactions to a specified comment ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.get_comment_reactions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#get_comment_reactions)
         """
@@ -750,15 +749,15 @@
     async def get_comments_for_compared_commit(
         self,
         *,
         repositoryName: str,
         afterCommitId: str,
         beforeCommitId: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetCommentsForComparedCommitOutputTypeDef:
         """
         Returns information about comments made on the comparison between two commits.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.get_comments_for_compared_commit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#get_comments_for_compared_commit)
         """
@@ -767,15 +766,15 @@
         self,
         *,
         pullRequestId: str,
         repositoryName: str = ...,
         beforeCommitId: str = ...,
         afterCommitId: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetCommentsForPullRequestOutputTypeDef:
         """
         Returns comments made on a pull request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.get_comments_for_pull_request)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#get_comments_for_pull_request)
         """
@@ -794,15 +793,15 @@
         *,
         repositoryName: str,
         afterCommitSpecifier: str,
         beforeCommitSpecifier: str = ...,
         beforePath: str = ...,
         afterPath: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetDifferencesOutputTypeDef:
         """
         Returns information about the differences in a valid commit specifier (such as
         a branch, tag, HEAD, commit ID, or other fully qualified
         reference).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.get_differences)
@@ -832,15 +831,15 @@
     async def get_merge_commit(
         self,
         *,
         repositoryName: str,
         sourceCommitSpecifier: str,
         destinationCommitSpecifier: str,
         conflictDetailLevel: ConflictDetailLevelTypeEnumType = ...,
-        conflictResolutionStrategy: ConflictResolutionStrategyTypeEnumType = ...
+        conflictResolutionStrategy: ConflictResolutionStrategyTypeEnumType = ...,
     ) -> GetMergeCommitOutputTypeDef:
         """
         Returns information about a specified merge commit.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.get_merge_commit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#get_merge_commit)
         """
@@ -851,15 +850,15 @@
         repositoryName: str,
         destinationCommitSpecifier: str,
         sourceCommitSpecifier: str,
         mergeOption: MergeOptionTypeEnumType,
         conflictDetailLevel: ConflictDetailLevelTypeEnumType = ...,
         maxConflictFiles: int = ...,
         conflictResolutionStrategy: ConflictResolutionStrategyTypeEnumType = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> GetMergeConflictsOutputTypeDef:
         """
         Returns information about merge conflicts between the before and after commit
         IDs for a pull request in a
         repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.get_merge_conflicts)
@@ -869,15 +868,15 @@
     async def get_merge_options(
         self,
         *,
         repositoryName: str,
         sourceCommitSpecifier: str,
         destinationCommitSpecifier: str,
         conflictDetailLevel: ConflictDetailLevelTypeEnumType = ...,
-        conflictResolutionStrategy: ConflictResolutionStrategyTypeEnumType = ...
+        conflictResolutionStrategy: ConflictResolutionStrategyTypeEnumType = ...,
     ) -> GetMergeOptionsOutputTypeDef:
         """
         Returns information about the merge options available for merging two specified
         branches.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.get_merge_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#get_merge_options)
@@ -969,15 +968,15 @@
     async def list_file_commit_history(
         self,
         *,
         repositoryName: str,
         filePath: str,
         commitSpecifier: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListFileCommitHistoryResponseTypeDef:
         """
         Retrieves a list of commits and changes to a specified file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.list_file_commit_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#list_file_commit_history)
         """
@@ -985,15 +984,15 @@
     async def list_pull_requests(
         self,
         *,
         repositoryName: str,
         authorArn: str = ...,
         pullRequestStatus: PullRequestStatusEnumType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListPullRequestsOutputTypeDef:
         """
         Returns a list of pull requests for a specified repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.list_pull_requests)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#list_pull_requests)
         """
@@ -1032,15 +1031,15 @@
 
     async def merge_branches_by_fast_forward(
         self,
         *,
         repositoryName: str,
         sourceCommitSpecifier: str,
         destinationCommitSpecifier: str,
-        targetBranch: str = ...
+        targetBranch: str = ...,
     ) -> MergeBranchesByFastForwardOutputTypeDef:
         """
         Merges two branches using the fast-forward merge strategy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.merge_branches_by_fast_forward)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#merge_branches_by_fast_forward)
         """
@@ -1054,15 +1053,15 @@
         targetBranch: str = ...,
         conflictDetailLevel: ConflictDetailLevelTypeEnumType = ...,
         conflictResolutionStrategy: ConflictResolutionStrategyTypeEnumType = ...,
         authorName: str = ...,
         email: str = ...,
         commitMessage: str = ...,
         keepEmptyFolders: bool = ...,
-        conflictResolution: ConflictResolutionTypeDef = ...
+        conflictResolution: ConflictResolutionTypeDef = ...,
     ) -> MergeBranchesBySquashOutputTypeDef:
         """
         Merges two branches using the squash merge strategy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.merge_branches_by_squash)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#merge_branches_by_squash)
         """
@@ -1076,15 +1075,15 @@
         targetBranch: str = ...,
         conflictDetailLevel: ConflictDetailLevelTypeEnumType = ...,
         conflictResolutionStrategy: ConflictResolutionStrategyTypeEnumType = ...,
         authorName: str = ...,
         email: str = ...,
         commitMessage: str = ...,
         keepEmptyFolders: bool = ...,
-        conflictResolution: ConflictResolutionTypeDef = ...
+        conflictResolution: ConflictResolutionTypeDef = ...,
     ) -> MergeBranchesByThreeWayOutputTypeDef:
         """
         Merges two specified branches using the three-way merge strategy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.merge_branches_by_three_way)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#merge_branches_by_three_way)
         """
@@ -1110,15 +1109,15 @@
         sourceCommitId: str = ...,
         conflictDetailLevel: ConflictDetailLevelTypeEnumType = ...,
         conflictResolutionStrategy: ConflictResolutionStrategyTypeEnumType = ...,
         commitMessage: str = ...,
         authorName: str = ...,
         email: str = ...,
         keepEmptyFolders: bool = ...,
-        conflictResolution: ConflictResolutionTypeDef = ...
+        conflictResolution: ConflictResolutionTypeDef = ...,
     ) -> MergePullRequestBySquashOutputTypeDef:
         """
         Attempts to merge the source commit of a pull request into the specified
         destination branch for that pull request at the specified commit using the
         squash merge
         strategy.
 
@@ -1134,15 +1133,15 @@
         sourceCommitId: str = ...,
         conflictDetailLevel: ConflictDetailLevelTypeEnumType = ...,
         conflictResolutionStrategy: ConflictResolutionStrategyTypeEnumType = ...,
         commitMessage: str = ...,
         authorName: str = ...,
         email: str = ...,
         keepEmptyFolders: bool = ...,
-        conflictResolution: ConflictResolutionTypeDef = ...
+        conflictResolution: ConflictResolutionTypeDef = ...,
     ) -> MergePullRequestByThreeWayOutputTypeDef:
         """
         Attempts to merge the source commit of a pull request into the specified
         destination branch for that pull request at the specified commit using the
         three-way merge
         strategy.
 
@@ -1165,15 +1164,15 @@
         self,
         *,
         repositoryName: str,
         afterCommitId: str,
         content: str,
         beforeCommitId: str = ...,
         location: LocationTypeDef = ...,
-        clientRequestToken: str = ...
+        clientRequestToken: str = ...,
     ) -> PostCommentForComparedCommitOutputTypeDef:
         """
         Posts a comment on the comparison between two commits.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.post_comment_for_compared_commit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#post_comment_for_compared_commit)
         """
@@ -1183,15 +1182,15 @@
         *,
         pullRequestId: str,
         repositoryName: str,
         beforeCommitId: str,
         afterCommitId: str,
         content: str,
         location: LocationTypeDef = ...,
-        clientRequestToken: str = ...
+        clientRequestToken: str = ...,
     ) -> PostCommentForPullRequestOutputTypeDef:
         """
         Posts a comment on a pull request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.post_comment_for_pull_request)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#post_comment_for_pull_request)
         """
@@ -1227,15 +1226,15 @@
         branchName: str,
         fileContent: BlobTypeDef,
         filePath: str,
         fileMode: FileModeTypeEnumType = ...,
         parentCommitId: str = ...,
         commitMessage: str = ...,
         name: str = ...,
-        email: str = ...
+        email: str = ...,
     ) -> PutFileOutputTypeDef:
         """
         Adds or updates a file in a branch in an CodeCommit repository, and generates a
         commit for the addition in the specified
         branch.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.put_file)
@@ -1285,15 +1284,15 @@
         """
 
     async def update_approval_rule_template_content(
         self,
         *,
         approvalRuleTemplateName: str,
         newRuleContent: str,
-        existingRuleContentSha256: str = ...
+        existingRuleContentSha256: str = ...,
     ) -> UpdateApprovalRuleTemplateContentOutputTypeDef:
         """
         Updates the content of an approval rule template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.update_approval_rule_template_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#update_approval_rule_template_content)
         """
@@ -1338,15 +1337,15 @@
 
     async def update_pull_request_approval_rule_content(
         self,
         *,
         pullRequestId: str,
         approvalRuleName: str,
         newRuleContent: str,
-        existingRuleContentSha256: str = ...
+        existingRuleContentSha256: str = ...,
     ) -> UpdatePullRequestApprovalRuleContentOutputTypeDef:
         """
         Updates the structure of an approval rule created specifically for a pull
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.update_pull_request_approval_rule_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#update_pull_request_approval_rule_content)
```

### Comparing `types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit/client.pyi` & `types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -371,15 +371,15 @@
         sourceCommitSpecifier: str,
         mergeOption: MergeOptionTypeEnumType,
         maxMergeHunks: int = ...,
         maxConflictFiles: int = ...,
         filePaths: Sequence[str] = ...,
         conflictDetailLevel: ConflictDetailLevelTypeEnumType = ...,
         conflictResolutionStrategy: ConflictResolutionStrategyTypeEnumType = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> BatchDescribeMergeConflictsOutputTypeDef:
         """
         Returns information about one or more merge conflicts in the attempted merge of
         two commit specifiers using the squash or three-way merge
         strategy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.batch_describe_merge_conflicts)
@@ -435,15 +435,15 @@
         """
 
     async def create_approval_rule_template(
         self,
         *,
         approvalRuleTemplateName: str,
         approvalRuleTemplateContent: str,
-        approvalRuleTemplateDescription: str = ...
+        approvalRuleTemplateDescription: str = ...,
     ) -> CreateApprovalRuleTemplateOutputTypeDef:
         """
         Creates a template for approval rules that can then be associated with one or
         more repositories in your Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.create_approval_rule_template)
@@ -468,30 +468,30 @@
         parentCommitId: str = ...,
         authorName: str = ...,
         email: str = ...,
         commitMessage: str = ...,
         keepEmptyFolders: bool = ...,
         putFiles: Sequence[PutFileEntryTypeDef] = ...,
         deleteFiles: Sequence[DeleteFileEntryTypeDef] = ...,
-        setFileModes: Sequence[SetFileModeEntryTypeDef] = ...
+        setFileModes: Sequence[SetFileModeEntryTypeDef] = ...,
     ) -> CreateCommitOutputTypeDef:
         """
         Creates a commit for a repository on the tip of a specified branch.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.create_commit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#create_commit)
         """
 
     async def create_pull_request(
         self,
         *,
         title: str,
         targets: Sequence[TargetTypeDef],
         description: str = ...,
-        clientRequestToken: str = ...
+        clientRequestToken: str = ...,
     ) -> CreatePullRequestOutputTypeDef:
         """
         Creates a pull request in the specified repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.create_pull_request)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#create_pull_request)
         """
@@ -507,15 +507,15 @@
         """
 
     async def create_repository(
         self,
         *,
         repositoryName: str,
         repositoryDescription: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateRepositoryOutputTypeDef:
         """
         Creates a new, empty repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.create_repository)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#create_repository)
         """
@@ -529,15 +529,15 @@
         mergeOption: MergeOptionTypeEnumType,
         conflictDetailLevel: ConflictDetailLevelTypeEnumType = ...,
         conflictResolutionStrategy: ConflictResolutionStrategyTypeEnumType = ...,
         authorName: str = ...,
         email: str = ...,
         commitMessage: str = ...,
         keepEmptyFolders: bool = ...,
-        conflictResolution: ConflictResolutionTypeDef = ...
+        conflictResolution: ConflictResolutionTypeDef = ...,
     ) -> CreateUnreferencedMergeCommitOutputTypeDef:
         """
         Creates an unreferenced commit that represents the result of merging two
         branches using a specified merge
         strategy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.create_unreferenced_merge_commit)
@@ -581,15 +581,15 @@
         repositoryName: str,
         branchName: str,
         filePath: str,
         parentCommitId: str,
         keepEmptyFolders: bool = ...,
         commitMessage: str = ...,
         name: str = ...,
-        email: str = ...
+        email: str = ...,
     ) -> DeleteFileOutputTypeDef:
         """
         Deletes a specified file from a specified branch.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.delete_file)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#delete_file)
         """
@@ -619,15 +619,15 @@
         destinationCommitSpecifier: str,
         sourceCommitSpecifier: str,
         mergeOption: MergeOptionTypeEnumType,
         filePath: str,
         maxMergeHunks: int = ...,
         conflictDetailLevel: ConflictDetailLevelTypeEnumType = ...,
         conflictResolutionStrategy: ConflictResolutionStrategyTypeEnumType = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeMergeConflictsOutputTypeDef:
         """
         Returns information about one or more merge conflicts in the attempted merge of
         two commit specifiers using the squash or three-way merge
         strategy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.describe_merge_conflicts)
@@ -637,15 +637,15 @@
     async def describe_pull_request_events(
         self,
         *,
         pullRequestId: str,
         pullRequestEventType: PullRequestEventTypeType = ...,
         actorArn: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribePullRequestEventsOutputTypeDef:
         """
         Returns information about one or more pull request events.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.describe_pull_request_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#describe_pull_request_events)
         """
@@ -730,15 +730,15 @@
 
     async def get_comment_reactions(
         self,
         *,
         commentId: str,
         reactionUserArn: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetCommentReactionsOutputTypeDef:
         """
         Returns information about reactions to a specified comment ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.get_comment_reactions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#get_comment_reactions)
         """
@@ -746,15 +746,15 @@
     async def get_comments_for_compared_commit(
         self,
         *,
         repositoryName: str,
         afterCommitId: str,
         beforeCommitId: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetCommentsForComparedCommitOutputTypeDef:
         """
         Returns information about comments made on the comparison between two commits.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.get_comments_for_compared_commit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#get_comments_for_compared_commit)
         """
@@ -763,15 +763,15 @@
         self,
         *,
         pullRequestId: str,
         repositoryName: str = ...,
         beforeCommitId: str = ...,
         afterCommitId: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetCommentsForPullRequestOutputTypeDef:
         """
         Returns comments made on a pull request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.get_comments_for_pull_request)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#get_comments_for_pull_request)
         """
@@ -790,15 +790,15 @@
         *,
         repositoryName: str,
         afterCommitSpecifier: str,
         beforeCommitSpecifier: str = ...,
         beforePath: str = ...,
         afterPath: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetDifferencesOutputTypeDef:
         """
         Returns information about the differences in a valid commit specifier (such as
         a branch, tag, HEAD, commit ID, or other fully qualified
         reference).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.get_differences)
@@ -828,15 +828,15 @@
     async def get_merge_commit(
         self,
         *,
         repositoryName: str,
         sourceCommitSpecifier: str,
         destinationCommitSpecifier: str,
         conflictDetailLevel: ConflictDetailLevelTypeEnumType = ...,
-        conflictResolutionStrategy: ConflictResolutionStrategyTypeEnumType = ...
+        conflictResolutionStrategy: ConflictResolutionStrategyTypeEnumType = ...,
     ) -> GetMergeCommitOutputTypeDef:
         """
         Returns information about a specified merge commit.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.get_merge_commit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#get_merge_commit)
         """
@@ -847,15 +847,15 @@
         repositoryName: str,
         destinationCommitSpecifier: str,
         sourceCommitSpecifier: str,
         mergeOption: MergeOptionTypeEnumType,
         conflictDetailLevel: ConflictDetailLevelTypeEnumType = ...,
         maxConflictFiles: int = ...,
         conflictResolutionStrategy: ConflictResolutionStrategyTypeEnumType = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> GetMergeConflictsOutputTypeDef:
         """
         Returns information about merge conflicts between the before and after commit
         IDs for a pull request in a
         repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.get_merge_conflicts)
@@ -865,15 +865,15 @@
     async def get_merge_options(
         self,
         *,
         repositoryName: str,
         sourceCommitSpecifier: str,
         destinationCommitSpecifier: str,
         conflictDetailLevel: ConflictDetailLevelTypeEnumType = ...,
-        conflictResolutionStrategy: ConflictResolutionStrategyTypeEnumType = ...
+        conflictResolutionStrategy: ConflictResolutionStrategyTypeEnumType = ...,
     ) -> GetMergeOptionsOutputTypeDef:
         """
         Returns information about the merge options available for merging two specified
         branches.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.get_merge_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#get_merge_options)
@@ -965,15 +965,15 @@
     async def list_file_commit_history(
         self,
         *,
         repositoryName: str,
         filePath: str,
         commitSpecifier: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListFileCommitHistoryResponseTypeDef:
         """
         Retrieves a list of commits and changes to a specified file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.list_file_commit_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#list_file_commit_history)
         """
@@ -981,15 +981,15 @@
     async def list_pull_requests(
         self,
         *,
         repositoryName: str,
         authorArn: str = ...,
         pullRequestStatus: PullRequestStatusEnumType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListPullRequestsOutputTypeDef:
         """
         Returns a list of pull requests for a specified repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.list_pull_requests)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#list_pull_requests)
         """
@@ -1028,15 +1028,15 @@
 
     async def merge_branches_by_fast_forward(
         self,
         *,
         repositoryName: str,
         sourceCommitSpecifier: str,
         destinationCommitSpecifier: str,
-        targetBranch: str = ...
+        targetBranch: str = ...,
     ) -> MergeBranchesByFastForwardOutputTypeDef:
         """
         Merges two branches using the fast-forward merge strategy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.merge_branches_by_fast_forward)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#merge_branches_by_fast_forward)
         """
@@ -1050,15 +1050,15 @@
         targetBranch: str = ...,
         conflictDetailLevel: ConflictDetailLevelTypeEnumType = ...,
         conflictResolutionStrategy: ConflictResolutionStrategyTypeEnumType = ...,
         authorName: str = ...,
         email: str = ...,
         commitMessage: str = ...,
         keepEmptyFolders: bool = ...,
-        conflictResolution: ConflictResolutionTypeDef = ...
+        conflictResolution: ConflictResolutionTypeDef = ...,
     ) -> MergeBranchesBySquashOutputTypeDef:
         """
         Merges two branches using the squash merge strategy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.merge_branches_by_squash)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#merge_branches_by_squash)
         """
@@ -1072,15 +1072,15 @@
         targetBranch: str = ...,
         conflictDetailLevel: ConflictDetailLevelTypeEnumType = ...,
         conflictResolutionStrategy: ConflictResolutionStrategyTypeEnumType = ...,
         authorName: str = ...,
         email: str = ...,
         commitMessage: str = ...,
         keepEmptyFolders: bool = ...,
-        conflictResolution: ConflictResolutionTypeDef = ...
+        conflictResolution: ConflictResolutionTypeDef = ...,
     ) -> MergeBranchesByThreeWayOutputTypeDef:
         """
         Merges two specified branches using the three-way merge strategy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.merge_branches_by_three_way)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#merge_branches_by_three_way)
         """
@@ -1106,15 +1106,15 @@
         sourceCommitId: str = ...,
         conflictDetailLevel: ConflictDetailLevelTypeEnumType = ...,
         conflictResolutionStrategy: ConflictResolutionStrategyTypeEnumType = ...,
         commitMessage: str = ...,
         authorName: str = ...,
         email: str = ...,
         keepEmptyFolders: bool = ...,
-        conflictResolution: ConflictResolutionTypeDef = ...
+        conflictResolution: ConflictResolutionTypeDef = ...,
     ) -> MergePullRequestBySquashOutputTypeDef:
         """
         Attempts to merge the source commit of a pull request into the specified
         destination branch for that pull request at the specified commit using the
         squash merge
         strategy.
 
@@ -1130,15 +1130,15 @@
         sourceCommitId: str = ...,
         conflictDetailLevel: ConflictDetailLevelTypeEnumType = ...,
         conflictResolutionStrategy: ConflictResolutionStrategyTypeEnumType = ...,
         commitMessage: str = ...,
         authorName: str = ...,
         email: str = ...,
         keepEmptyFolders: bool = ...,
-        conflictResolution: ConflictResolutionTypeDef = ...
+        conflictResolution: ConflictResolutionTypeDef = ...,
     ) -> MergePullRequestByThreeWayOutputTypeDef:
         """
         Attempts to merge the source commit of a pull request into the specified
         destination branch for that pull request at the specified commit using the
         three-way merge
         strategy.
 
@@ -1161,15 +1161,15 @@
         self,
         *,
         repositoryName: str,
         afterCommitId: str,
         content: str,
         beforeCommitId: str = ...,
         location: LocationTypeDef = ...,
-        clientRequestToken: str = ...
+        clientRequestToken: str = ...,
     ) -> PostCommentForComparedCommitOutputTypeDef:
         """
         Posts a comment on the comparison between two commits.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.post_comment_for_compared_commit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#post_comment_for_compared_commit)
         """
@@ -1179,15 +1179,15 @@
         *,
         pullRequestId: str,
         repositoryName: str,
         beforeCommitId: str,
         afterCommitId: str,
         content: str,
         location: LocationTypeDef = ...,
-        clientRequestToken: str = ...
+        clientRequestToken: str = ...,
     ) -> PostCommentForPullRequestOutputTypeDef:
         """
         Posts a comment on a pull request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.post_comment_for_pull_request)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#post_comment_for_pull_request)
         """
@@ -1223,15 +1223,15 @@
         branchName: str,
         fileContent: BlobTypeDef,
         filePath: str,
         fileMode: FileModeTypeEnumType = ...,
         parentCommitId: str = ...,
         commitMessage: str = ...,
         name: str = ...,
-        email: str = ...
+        email: str = ...,
     ) -> PutFileOutputTypeDef:
         """
         Adds or updates a file in a branch in an CodeCommit repository, and generates a
         commit for the addition in the specified
         branch.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.put_file)
@@ -1281,15 +1281,15 @@
         """
 
     async def update_approval_rule_template_content(
         self,
         *,
         approvalRuleTemplateName: str,
         newRuleContent: str,
-        existingRuleContentSha256: str = ...
+        existingRuleContentSha256: str = ...,
     ) -> UpdateApprovalRuleTemplateContentOutputTypeDef:
         """
         Updates the content of an approval rule template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.update_approval_rule_template_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#update_approval_rule_template_content)
         """
@@ -1334,15 +1334,15 @@
 
     async def update_pull_request_approval_rule_content(
         self,
         *,
         pullRequestId: str,
         approvalRuleName: str,
         newRuleContent: str,
-        existingRuleContentSha256: str = ...
+        existingRuleContentSha256: str = ...,
     ) -> UpdatePullRequestApprovalRuleContentOutputTypeDef:
         """
         Updates the structure of an approval rule created specifically for a pull
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.update_pull_request_approval_rule_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#update_pull_request_approval_rule_content)
```

### Comparing `types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit/literals.py` & `types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit/literals.py`

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
     "ApprovalStateType",
     "ChangeTypeEnumType",
     "ConflictDetailLevelTypeEnumType",
     "ConflictResolutionStrategyTypeEnumType",
     "DescribePullRequestEventsPaginatorName",
     "FileModeTypeEnumType",
@@ -46,15 +45,14 @@
     "CodeCommitServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ApprovalStateType = Literal["APPROVE", "REVOKE"]
 ChangeTypeEnumType = Literal["A", "D", "M"]
 ConflictDetailLevelTypeEnumType = Literal["FILE_LEVEL", "LINE_LEVEL"]
 ConflictResolutionStrategyTypeEnumType = Literal[
     "ACCEPT_DESTINATION", "ACCEPT_SOURCE", "AUTOMERGE", "NONE"
 ]
 DescribePullRequestEventsPaginatorName = Literal["describe_pull_request_events"]
```

### Comparing `types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit/literals.pyi` & `types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit/paginator.py` & `types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,14 @@
     "GetCommentsForPullRequestPaginator",
     "GetDifferencesPaginator",
     "ListBranchesPaginator",
     "ListPullRequestsPaginator",
     "ListRepositoriesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -84,15 +83,15 @@
 
     def paginate(
         self,
         *,
         pullRequestId: str,
         pullRequestEventType: PullRequestEventTypeType = ...,
         actorArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribePullRequestEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.DescribePullRequestEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/paginators/#describepullrequesteventspaginator)
         """
 
 
@@ -104,15 +103,15 @@
 
     def paginate(
         self,
         *,
         repositoryName: str,
         afterCommitId: str,
         beforeCommitId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetCommentsForComparedCommitOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetCommentsForComparedCommit.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/paginators/#getcommentsforcomparedcommitpaginator)
         """
 
 
@@ -125,15 +124,15 @@
     def paginate(
         self,
         *,
         pullRequestId: str,
         repositoryName: str = ...,
         beforeCommitId: str = ...,
         afterCommitId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetCommentsForPullRequestOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetCommentsForPullRequest.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/paginators/#getcommentsforpullrequestpaginator)
         """
 
 
@@ -147,15 +146,15 @@
         self,
         *,
         repositoryName: str,
         afterCommitSpecifier: str,
         beforeCommitSpecifier: str = ...,
         beforePath: str = ...,
         afterPath: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetDifferencesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetDifferences.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/paginators/#getdifferencespaginator)
         """
 
 
@@ -182,15 +181,15 @@
 
     def paginate(
         self,
         *,
         repositoryName: str,
         authorArn: str = ...,
         pullRequestStatus: PullRequestStatusEnumType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPullRequestsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListPullRequests.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/paginators/#listpullrequestspaginator)
         """
 
 
@@ -201,13 +200,13 @@
     """
 
     def paginate(
         self,
         *,
         sortBy: SortByEnumType = ...,
         order: OrderEnumType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRepositoriesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListRepositories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/paginators/#listrepositoriespaginator)
         """
```

### Comparing `types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit/paginator.pyi` & `types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
     def paginate(
         self,
         *,
         pullRequestId: str,
         pullRequestEventType: PullRequestEventTypeType = ...,
         actorArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribePullRequestEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.DescribePullRequestEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/paginators/#describepullrequesteventspaginator)
         """
 
 class GetCommentsForComparedCommitPaginator(AioPaginator):
@@ -100,15 +100,15 @@
 
     def paginate(
         self,
         *,
         repositoryName: str,
         afterCommitId: str,
         beforeCommitId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetCommentsForComparedCommitOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetCommentsForComparedCommit.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/paginators/#getcommentsforcomparedcommitpaginator)
         """
 
 class GetCommentsForPullRequestPaginator(AioPaginator):
@@ -120,15 +120,15 @@
     def paginate(
         self,
         *,
         pullRequestId: str,
         repositoryName: str = ...,
         beforeCommitId: str = ...,
         afterCommitId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetCommentsForPullRequestOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetCommentsForPullRequest.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/paginators/#getcommentsforpullrequestpaginator)
         """
 
 class GetDifferencesPaginator(AioPaginator):
@@ -141,15 +141,15 @@
         self,
         *,
         repositoryName: str,
         afterCommitSpecifier: str,
         beforeCommitSpecifier: str = ...,
         beforePath: str = ...,
         afterPath: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetDifferencesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetDifferences.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/paginators/#getdifferencespaginator)
         """
 
 class ListBranchesPaginator(AioPaginator):
@@ -174,15 +174,15 @@
 
     def paginate(
         self,
         *,
         repositoryName: str,
         authorArn: str = ...,
         pullRequestStatus: PullRequestStatusEnumType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPullRequestsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListPullRequests.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/paginators/#listpullrequestspaginator)
         """
 
 class ListRepositoriesPaginator(AioPaginator):
@@ -192,13 +192,13 @@
     """
 
     def paginate(
         self,
         *,
         sortBy: SortByEnumType = ...,
         order: OrderEnumType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRepositoriesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListRepositories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/paginators/#listrepositoriespaginator)
         """
```

### Comparing `types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit/type_defs.py` & `types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ApprovalRuleEventMetadataTypeDef",
     "ApprovalRuleOverriddenEventMetadataTypeDef",
     "ApprovalRuleTemplateTypeDef",
     "OriginApprovalRuleTemplateTypeDef",
     "ApprovalStateChangedEventMetadataTypeDef",
     "ApprovalTypeDef",
```

### Comparing `types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit/type_defs.pyi` & `types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit.egg-info/PKG-INFO` & `types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codecommit
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CodeCommit 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CodeCommit 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/
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
 
 <a id="types-aiobotocore-codecommit"></a>
 
 # types-aiobotocore-codecommit
 
 [![PyPI - types-aiobotocore-codecommit](https://img.shields.io/pypi/v/types-aiobotocore-codecommit.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codecommit)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codecommit.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codecommit)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codecommit)](https://pepy.tech/project/types-aiobotocore-codecommit)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeCommit 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
+[aiobotocore.CodeCommit 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
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
 [types-aiobotocore-codecommit docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codecommit-2.9.0/types_aiobotocore_codecommit.egg-info/SOURCES.txt` & `types-aiobotocore-codecommit-2.9.1/types_aiobotocore_codecommit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

