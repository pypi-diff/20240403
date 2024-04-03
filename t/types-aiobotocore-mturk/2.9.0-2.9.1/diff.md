# Comparing `tmp/types-aiobotocore-mturk-2.9.0.tar.gz` & `tmp/types-aiobotocore-mturk-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mturk-2.9.0.tar", last modified: Wed Dec 13 19:59:59 2023, max compression
+gzip compressed data, was "types-aiobotocore-mturk-2.9.1.tar", last modified: Thu Jan 18 01:21:21 2024, max compression
```

## Comparing `types-aiobotocore-mturk-2.9.0.tar` & `types-aiobotocore-mturk-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:59.825403 types-aiobotocore-mturk-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:50:40.000000 types-aiobotocore-mturk-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14281 2023-12-13 19:59:59.825403 types-aiobotocore-mturk-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12726 2023-12-13 19:50:40.000000 types-aiobotocore-mturk-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:59.825403 types-aiobotocore-mturk-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2023-12-13 19:50:40.000000 types-aiobotocore-mturk-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:59.821403 types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk/
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2023-12-13 19:50:40.000000 types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2023-12-13 19:50:40.000000 types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      913 2023-12-13 19:50:40.000000 types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35558 2023-12-13 19:50:41.000000 types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    35554 2023-12-13 19:50:41.000000 types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11163 2023-12-13 19:50:41.000000 types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11161 2023-12-13 19:50:41.000000 types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11797 2023-12-13 19:50:41.000000 types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11786 2023-12-13 19:50:41.000000 types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:50:40.000000 types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    32325 2023-12-13 19:50:41.000000 types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    32324 2023-12-13 19:50:41.000000 types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:50:40.000000 types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:59.825403 types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14281 2023-12-13 19:59:59.000000 types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      775 2023-12-13 19:59:59.000000 types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:59.000000 types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:59.000000 types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:59.000000 types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-13 19:59:59.000000 types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:21.141159 types-aiobotocore-mturk-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:12:22.000000 types-aiobotocore-mturk-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14301 2024-01-18 01:21:21.141159 types-aiobotocore-mturk-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12726 2024-01-18 01:12:22.000000 types-aiobotocore-mturk-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:21.141159 types-aiobotocore-mturk-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-01-18 01:12:22.000000 types-aiobotocore-mturk-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:21.141159 types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk/
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-01-18 01:12:22.000000 types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-01-18 01:12:22.000000 types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-01-18 01:12:22.000000 types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35571 2024-01-18 01:12:22.000000 types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35568 2024-01-18 01:12:22.000000 types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11161 2024-01-18 01:12:23.000000 types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11161 2024-01-18 01:12:23.000000 types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11801 2024-01-18 01:12:22.000000 types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11791 2024-01-18 01:12:22.000000 types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:12:22.000000 types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    32324 2024-01-18 01:12:23.000000 types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32324 2024-01-18 01:12:23.000000 types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:12:22.000000 types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:21.141159 types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14301 2024-01-18 01:21:21.000000 types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-01-18 01:21:21.000000 types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:21.000000 types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:21.000000 types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:21.000000 types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-18 01:21:21.000000 types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mturk-2.9.0/LICENSE` & `types-aiobotocore-mturk-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-mturk-2.9.0/PKG-INFO` & `types-aiobotocore-mturk-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mturk
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MTurk 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MTurk 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/
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
 
 <a id="types-aiobotocore-mturk"></a>
 
 # types-aiobotocore-mturk
 
 [![PyPI - types-aiobotocore-mturk](https://img.shields.io/pypi/v/types-aiobotocore-mturk.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mturk)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mturk.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mturk)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mturk)](https://pepy.tech/project/types-aiobotocore-mturk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MTurk 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
+[aiobotocore.MTurk 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
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
 [types-aiobotocore-mturk docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mturk-2.9.0/README.md` & `types-aiobotocore-mturk-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mturk.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mturk)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mturk)](https://pepy.tech/project/types-aiobotocore-mturk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MTurk 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
+[aiobotocore.MTurk 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
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
 [types-aiobotocore-mturk docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mturk-2.9.0/setup.py` & `types-aiobotocore-mturk-2.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mturk",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_mturk"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MTurk 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.MTurk 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore mturk type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_mturk": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk/__init__.py` & `types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
     ListReviewableHITsPaginator,
     ListWorkerBlocksPaginator,
     ListWorkersWithQualificationTypePaginator,
 )
 
 Client = MTurkClient
 
-
 __all__ = (
     "Client",
     "ListAssignmentsForHITPaginator",
     "ListBonusPaymentsPaginator",
     "ListHITsForQualificationTypePaginator",
     "ListHITsPaginator",
     "ListQualificationRequestsPaginator",
```

### Comparing `types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk/__init__.pyi` & `types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk/__main__.py` & `types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MTurk 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.MTurk 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk\nOther"
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

### Comparing `types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk/client.py` & `types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -71,15 +71,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("MTurkClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -134,15 +133,15 @@
 
     async def associate_qualification_with_worker(
         self,
         *,
         QualificationTypeId: str,
         WorkerId: str,
         IntegerValue: int = ...,
-        SendNotification: bool = ...
+        SendNotification: bool = ...,
     ) -> Dict[str, Any]:
         """
         The `AssociateQualificationWithWorker` operation gives a Worker a Qualification.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.associate_qualification_with_worker)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/client/#associate_qualification_with_worker)
         """
@@ -189,15 +188,15 @@
         Question: str = ...,
         RequesterAnnotation: str = ...,
         QualificationRequirements: Sequence[QualificationRequirementTypeDef] = ...,
         UniqueRequestToken: str = ...,
         AssignmentReviewPolicy: ReviewPolicyTypeDef = ...,
         HITReviewPolicy: ReviewPolicyTypeDef = ...,
         HITLayoutId: str = ...,
-        HITLayoutParameters: Sequence[HITLayoutParameterTypeDef] = ...
+        HITLayoutParameters: Sequence[HITLayoutParameterTypeDef] = ...,
     ) -> CreateHITResponseTypeDef:
         """
         The `CreateHIT` operation creates a new Human Intelligence Task (HIT).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.create_hit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/client/#create_hit)
         """
@@ -207,15 +206,15 @@
         *,
         AssignmentDurationInSeconds: int,
         Reward: str,
         Title: str,
         Description: str,
         AutoApprovalDelayInSeconds: int = ...,
         Keywords: str = ...,
-        QualificationRequirements: Sequence[QualificationRequirementTypeDef] = ...
+        QualificationRequirements: Sequence[QualificationRequirementTypeDef] = ...,
     ) -> CreateHITTypeResponseTypeDef:
         """
         The `CreateHITType` operation creates a new HIT type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.create_hit_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/client/#create_hit_type)
         """
@@ -228,15 +227,15 @@
         MaxAssignments: int = ...,
         Question: str = ...,
         RequesterAnnotation: str = ...,
         UniqueRequestToken: str = ...,
         AssignmentReviewPolicy: ReviewPolicyTypeDef = ...,
         HITReviewPolicy: ReviewPolicyTypeDef = ...,
         HITLayoutId: str = ...,
-        HITLayoutParameters: Sequence[HITLayoutParameterTypeDef] = ...
+        HITLayoutParameters: Sequence[HITLayoutParameterTypeDef] = ...,
     ) -> CreateHITWithHITTypeResponseTypeDef:
         """
         The `CreateHITWithHITType` operation creates a new Human Intelligence Task
         (HIT) using an existing HITTypeID generated by the `CreateHITType`
         operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.create_hit_with_hit_type)
@@ -251,15 +250,15 @@
         QualificationTypeStatus: QualificationTypeStatusType,
         Keywords: str = ...,
         RetryDelayInSeconds: int = ...,
         Test: str = ...,
         AnswerKey: str = ...,
         TestDurationInSeconds: int = ...,
         AutoGranted: bool = ...,
-        AutoGrantedValue: int = ...
+        AutoGrantedValue: int = ...,
     ) -> CreateQualificationTypeResponseTypeDef:
         """
         The `CreateQualificationType` operation creates a new Qualification type, which
         is represented by a `QualificationType` data
         structure.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.create_qualification_type)
@@ -392,30 +391,30 @@
 
     async def list_assignments_for_hit(
         self,
         *,
         HITId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        AssignmentStatuses: Sequence[AssignmentStatusType] = ...
+        AssignmentStatuses: Sequence[AssignmentStatusType] = ...,
     ) -> ListAssignmentsForHITResponseTypeDef:
         """
         The `ListAssignmentsForHIT` operation retrieves completed assignments for a HIT.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.list_assignments_for_hit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/client/#list_assignments_for_hit)
         """
 
     async def list_bonus_payments(
         self,
         *,
         HITId: str = ...,
         AssignmentId: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListBonusPaymentsResponseTypeDef:
         """
         The `ListBonusPayments` operation retrieves the amounts of bonuses you have
         paid to Workers for a given HIT or
         assignment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.list_bonus_payments)
@@ -459,15 +458,15 @@
     async def list_qualification_types(
         self,
         *,
         MustBeRequestable: bool,
         Query: str = ...,
         MustBeOwnedByCaller: bool = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListQualificationTypesResponseTypeDef:
         """
         The `ListQualificationTypes` operation returns a list of Qualification types,
         filtered by an optional search
         term.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.list_qualification_types)
@@ -478,15 +477,15 @@
         self,
         *,
         HITId: str,
         PolicyLevels: Sequence[ReviewPolicyLevelType] = ...,
         RetrieveActions: bool = ...,
         RetrieveResults: bool = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListReviewPolicyResultsForHITResponseTypeDef:
         """
         The `ListReviewPolicyResultsForHIT` operation retrieves the computed results
         and the actions taken in the course of executing your Review Policies for a
         given
         HIT.
 
@@ -496,15 +495,15 @@
 
     async def list_reviewable_hits(
         self,
         *,
         HITTypeId: str = ...,
         Status: ReviewableHITStatusType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListReviewableHITsResponseTypeDef:
         """
         The `ListReviewableHITs` operation retrieves the HITs with Status equal to
         Reviewable or Status equal to Reviewing that belong to the Requester calling
         the
         operation.
 
@@ -526,15 +525,15 @@
 
     async def list_workers_with_qualification_type(
         self,
         *,
         QualificationTypeId: str,
         Status: QualificationStatusType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListWorkersWithQualificationTypeResponseTypeDef:
         """
         The `ListWorkersWithQualificationType` operation returns all of the Workers
         that have been associated with a given Qualification
         type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.list_workers_with_qualification_type)
@@ -577,15 +576,15 @@
     async def send_bonus(
         self,
         *,
         WorkerId: str,
         BonusAmount: str,
         AssignmentId: str,
         Reason: str,
-        UniqueRequestToken: str = ...
+        UniqueRequestToken: str = ...,
     ) -> Dict[str, Any]:
         """
         The `SendBonus` operation issues a payment of money from your account to a
         Worker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.send_bonus)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/client/#send_bonus)
@@ -635,15 +634,15 @@
         """
 
     async def update_notification_settings(
         self,
         *,
         HITTypeId: str,
         Notification: NotificationSpecificationTypeDef = ...,
-        Active: bool = ...
+        Active: bool = ...,
     ) -> Dict[str, Any]:
         """
         The `UpdateNotificationSettings` operation creates, updates, disables or
         re-enables notifications for a HIT
         type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.update_notification_settings)
@@ -657,15 +656,15 @@
         Description: str = ...,
         QualificationTypeStatus: QualificationTypeStatusType = ...,
         Test: str = ...,
         AnswerKey: str = ...,
         TestDurationInSeconds: int = ...,
         RetryDelayInSeconds: int = ...,
         AutoGranted: bool = ...,
-        AutoGrantedValue: int = ...
+        AutoGrantedValue: int = ...,
     ) -> UpdateQualificationTypeResponseTypeDef:
         """
         The `UpdateQualificationType` operation modifies the attributes of an existing
         Qualification type, which is represented by a QualificationType data
         structure.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.update_qualification_type)
```

### Comparing `types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk/client.pyi` & `types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk/client.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -130,15 +130,15 @@
 
     async def associate_qualification_with_worker(
         self,
         *,
         QualificationTypeId: str,
         WorkerId: str,
         IntegerValue: int = ...,
-        SendNotification: bool = ...
+        SendNotification: bool = ...,
     ) -> Dict[str, Any]:
         """
         The `AssociateQualificationWithWorker` operation gives a Worker a Qualification.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.associate_qualification_with_worker)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/client/#associate_qualification_with_worker)
         """
@@ -185,15 +185,15 @@
         Question: str = ...,
         RequesterAnnotation: str = ...,
         QualificationRequirements: Sequence[QualificationRequirementTypeDef] = ...,
         UniqueRequestToken: str = ...,
         AssignmentReviewPolicy: ReviewPolicyTypeDef = ...,
         HITReviewPolicy: ReviewPolicyTypeDef = ...,
         HITLayoutId: str = ...,
-        HITLayoutParameters: Sequence[HITLayoutParameterTypeDef] = ...
+        HITLayoutParameters: Sequence[HITLayoutParameterTypeDef] = ...,
     ) -> CreateHITResponseTypeDef:
         """
         The `CreateHIT` operation creates a new Human Intelligence Task (HIT).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.create_hit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/client/#create_hit)
         """
@@ -203,15 +203,15 @@
         *,
         AssignmentDurationInSeconds: int,
         Reward: str,
         Title: str,
         Description: str,
         AutoApprovalDelayInSeconds: int = ...,
         Keywords: str = ...,
-        QualificationRequirements: Sequence[QualificationRequirementTypeDef] = ...
+        QualificationRequirements: Sequence[QualificationRequirementTypeDef] = ...,
     ) -> CreateHITTypeResponseTypeDef:
         """
         The `CreateHITType` operation creates a new HIT type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.create_hit_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/client/#create_hit_type)
         """
@@ -224,15 +224,15 @@
         MaxAssignments: int = ...,
         Question: str = ...,
         RequesterAnnotation: str = ...,
         UniqueRequestToken: str = ...,
         AssignmentReviewPolicy: ReviewPolicyTypeDef = ...,
         HITReviewPolicy: ReviewPolicyTypeDef = ...,
         HITLayoutId: str = ...,
-        HITLayoutParameters: Sequence[HITLayoutParameterTypeDef] = ...
+        HITLayoutParameters: Sequence[HITLayoutParameterTypeDef] = ...,
     ) -> CreateHITWithHITTypeResponseTypeDef:
         """
         The `CreateHITWithHITType` operation creates a new Human Intelligence Task
         (HIT) using an existing HITTypeID generated by the `CreateHITType`
         operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.create_hit_with_hit_type)
@@ -247,15 +247,15 @@
         QualificationTypeStatus: QualificationTypeStatusType,
         Keywords: str = ...,
         RetryDelayInSeconds: int = ...,
         Test: str = ...,
         AnswerKey: str = ...,
         TestDurationInSeconds: int = ...,
         AutoGranted: bool = ...,
-        AutoGrantedValue: int = ...
+        AutoGrantedValue: int = ...,
     ) -> CreateQualificationTypeResponseTypeDef:
         """
         The `CreateQualificationType` operation creates a new Qualification type, which
         is represented by a `QualificationType` data
         structure.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.create_qualification_type)
@@ -388,30 +388,30 @@
 
     async def list_assignments_for_hit(
         self,
         *,
         HITId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        AssignmentStatuses: Sequence[AssignmentStatusType] = ...
+        AssignmentStatuses: Sequence[AssignmentStatusType] = ...,
     ) -> ListAssignmentsForHITResponseTypeDef:
         """
         The `ListAssignmentsForHIT` operation retrieves completed assignments for a HIT.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.list_assignments_for_hit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/client/#list_assignments_for_hit)
         """
 
     async def list_bonus_payments(
         self,
         *,
         HITId: str = ...,
         AssignmentId: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListBonusPaymentsResponseTypeDef:
         """
         The `ListBonusPayments` operation retrieves the amounts of bonuses you have
         paid to Workers for a given HIT or
         assignment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.list_bonus_payments)
@@ -455,15 +455,15 @@
     async def list_qualification_types(
         self,
         *,
         MustBeRequestable: bool,
         Query: str = ...,
         MustBeOwnedByCaller: bool = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListQualificationTypesResponseTypeDef:
         """
         The `ListQualificationTypes` operation returns a list of Qualification types,
         filtered by an optional search
         term.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.list_qualification_types)
@@ -474,15 +474,15 @@
         self,
         *,
         HITId: str,
         PolicyLevels: Sequence[ReviewPolicyLevelType] = ...,
         RetrieveActions: bool = ...,
         RetrieveResults: bool = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListReviewPolicyResultsForHITResponseTypeDef:
         """
         The `ListReviewPolicyResultsForHIT` operation retrieves the computed results
         and the actions taken in the course of executing your Review Policies for a
         given
         HIT.
 
@@ -492,15 +492,15 @@
 
     async def list_reviewable_hits(
         self,
         *,
         HITTypeId: str = ...,
         Status: ReviewableHITStatusType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListReviewableHITsResponseTypeDef:
         """
         The `ListReviewableHITs` operation retrieves the HITs with Status equal to
         Reviewable or Status equal to Reviewing that belong to the Requester calling
         the
         operation.
 
@@ -522,15 +522,15 @@
 
     async def list_workers_with_qualification_type(
         self,
         *,
         QualificationTypeId: str,
         Status: QualificationStatusType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListWorkersWithQualificationTypeResponseTypeDef:
         """
         The `ListWorkersWithQualificationType` operation returns all of the Workers
         that have been associated with a given Qualification
         type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.list_workers_with_qualification_type)
@@ -573,15 +573,15 @@
     async def send_bonus(
         self,
         *,
         WorkerId: str,
         BonusAmount: str,
         AssignmentId: str,
         Reason: str,
-        UniqueRequestToken: str = ...
+        UniqueRequestToken: str = ...,
     ) -> Dict[str, Any]:
         """
         The `SendBonus` operation issues a payment of money from your account to a
         Worker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.send_bonus)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/client/#send_bonus)
@@ -631,15 +631,15 @@
         """
 
     async def update_notification_settings(
         self,
         *,
         HITTypeId: str,
         Notification: NotificationSpecificationTypeDef = ...,
-        Active: bool = ...
+        Active: bool = ...,
     ) -> Dict[str, Any]:
         """
         The `UpdateNotificationSettings` operation creates, updates, disables or
         re-enables notifications for a HIT
         type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.update_notification_settings)
@@ -653,15 +653,15 @@
         Description: str = ...,
         QualificationTypeStatus: QualificationTypeStatusType = ...,
         Test: str = ...,
         AnswerKey: str = ...,
         TestDurationInSeconds: int = ...,
         RetryDelayInSeconds: int = ...,
         AutoGranted: bool = ...,
-        AutoGrantedValue: int = ...
+        AutoGrantedValue: int = ...,
     ) -> UpdateQualificationTypeResponseTypeDef:
         """
         The `UpdateQualificationType` operation modifies the attributes of an existing
         Qualification type, which is represented by a QualificationType data
         structure.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.update_qualification_type)
```

### Comparing `types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk/literals.py` & `types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk/literals.py`

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
     "AssignmentStatusType",
     "ComparatorType",
     "EventTypeType",
     "HITAccessActionsType",
     "HITReviewStatusType",
     "HITStatusType",
@@ -46,15 +45,14 @@
     "MTurkServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AssignmentStatusType = Literal["Approved", "Rejected", "Submitted"]
 ComparatorType = Literal[
     "DoesNotExist",
     "EqualTo",
     "Exists",
     "GreaterThan",
     "GreaterThanOrEqualTo",
```

### Comparing `types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk/literals.pyi` & `types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk/paginator.py` & `types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,14 @@
     "ListQualificationRequestsPaginator",
     "ListQualificationTypesPaginator",
     "ListReviewableHITsPaginator",
     "ListWorkerBlocksPaginator",
     "ListWorkersWithQualificationTypePaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -86,15 +85,15 @@
     """
 
     def paginate(
         self,
         *,
         HITId: str,
         AssignmentStatuses: Sequence[AssignmentStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAssignmentsForHITResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListAssignmentsForHIT.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listassignmentsforhitpaginator)
         """
 
 
@@ -105,15 +104,15 @@
     """
 
     def paginate(
         self,
         *,
         HITId: str = ...,
         AssignmentId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListBonusPaymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListBonusPayments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listbonuspaymentspaginator)
         """
 
 
@@ -170,15 +169,15 @@
 
     def paginate(
         self,
         *,
         MustBeRequestable: bool,
         Query: str = ...,
         MustBeOwnedByCaller: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListQualificationTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListQualificationTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listqualificationtypespaginator)
         """
 
 
@@ -189,15 +188,15 @@
     """
 
     def paginate(
         self,
         *,
         HITTypeId: str = ...,
         Status: ReviewableHITStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListReviewableHITsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListReviewableHITs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listreviewablehitspaginator)
         """
 
 
@@ -223,13 +222,13 @@
     """
 
     def paginate(
         self,
         *,
         QualificationTypeId: str,
         Status: QualificationStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListWorkersWithQualificationTypeResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListWorkersWithQualificationType.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listworkerswithqualificationtypepaginator)
         """
```

### Comparing `types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk/paginator.pyi` & `types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     """
 
     def paginate(
         self,
         *,
         HITId: str,
         AssignmentStatuses: Sequence[AssignmentStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAssignmentsForHITResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListAssignmentsForHIT.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listassignmentsforhitpaginator)
         """
 
 class ListBonusPaymentsPaginator(AioPaginator):
@@ -101,15 +101,15 @@
     """
 
     def paginate(
         self,
         *,
         HITId: str = ...,
         AssignmentId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListBonusPaymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListBonusPayments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listbonuspaymentspaginator)
         """
 
 class ListHITsPaginator(AioPaginator):
@@ -162,15 +162,15 @@
 
     def paginate(
         self,
         *,
         MustBeRequestable: bool,
         Query: str = ...,
         MustBeOwnedByCaller: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListQualificationTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListQualificationTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listqualificationtypespaginator)
         """
 
 class ListReviewableHITsPaginator(AioPaginator):
@@ -180,15 +180,15 @@
     """
 
     def paginate(
         self,
         *,
         HITTypeId: str = ...,
         Status: ReviewableHITStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListReviewableHITsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListReviewableHITs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listreviewablehitspaginator)
         """
 
 class ListWorkerBlocksPaginator(AioPaginator):
@@ -212,13 +212,13 @@
     """
 
     def paginate(
         self,
         *,
         QualificationTypeId: str,
         Status: QualificationStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListWorkersWithQualificationTypeResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListWorkersWithQualificationType.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/paginators/#listworkerswithqualificationtypepaginator)
         """
```

### Comparing `types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk/type_defs.py` & `types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceptQualificationRequestRequestRequestTypeDef",
     "ApproveAssignmentRequestRequestTypeDef",
     "AssignmentTypeDef",
     "AssociateQualificationWithWorkerRequestRequestTypeDef",
     "BonusPaymentTypeDef",
     "CreateAdditionalAssignmentsForHITRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk/type_defs.pyi` & `types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk.egg-info/PKG-INFO` & `types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mturk
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MTurk 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MTurk 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/
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
 
 <a id="types-aiobotocore-mturk"></a>
 
 # types-aiobotocore-mturk
 
 [![PyPI - types-aiobotocore-mturk](https://img.shields.io/pypi/v/types-aiobotocore-mturk.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mturk)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mturk.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mturk)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mturk)](https://pepy.tech/project/types-aiobotocore-mturk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MTurk 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
+[aiobotocore.MTurk 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
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
 [types-aiobotocore-mturk docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mturk-2.9.0/types_aiobotocore_mturk.egg-info/SOURCES.txt` & `types-aiobotocore-mturk-2.9.1/types_aiobotocore_mturk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

