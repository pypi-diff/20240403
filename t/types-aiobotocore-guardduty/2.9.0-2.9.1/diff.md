# Comparing `tmp/types-aiobotocore-guardduty-2.9.0.tar.gz` & `tmp/types-aiobotocore-guardduty-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-guardduty-2.9.0.tar", last modified: Wed Dec 13 19:59:25 2023, max compression
+gzip compressed data, was "types-aiobotocore-guardduty-2.9.1.tar", last modified: Thu Jan 18 01:20:49 2024, max compression
```

## Comparing `types-aiobotocore-guardduty-2.9.0.tar` & `types-aiobotocore-guardduty-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:25.437711 types-aiobotocore-guardduty-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:47:06.000000 types-aiobotocore-guardduty-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14357 2023-12-13 19:59:25.437711 types-aiobotocore-guardduty-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12786 2023-12-13 19:47:06.000000 types-aiobotocore-guardduty-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:25.437711 types-aiobotocore-guardduty-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2023-12-13 19:47:06.000000 types-aiobotocore-guardduty-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:25.437711 types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty/
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2023-12-13 19:47:06.000000 types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2023-12-13 19:47:06.000000 types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-12-13 19:47:06.000000 types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52722 2023-12-13 19:47:07.000000 types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    52718 2023-12-13 19:47:07.000000 types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15389 2023-12-13 19:47:07.000000 types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    15387 2023-12-13 19:47:07.000000 types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12533 2023-12-13 19:47:07.000000 types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12521 2023-12-13 19:47:07.000000 types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:47:06.000000 types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    88316 2023-12-13 19:47:10.000000 types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    88315 2023-12-13 19:47:09.000000 types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:47:06.000000 types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:25.437711 types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14357 2023-12-13 19:59:25.000000 types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-12-13 19:59:25.000000 types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:25.000000 types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:25.000000 types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:25.000000 types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-13 19:59:25.000000 types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:49.397302 types-aiobotocore-guardduty-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:08:59.000000 types-aiobotocore-guardduty-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14377 2024-01-18 01:20:49.397302 types-aiobotocore-guardduty-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12786 2024-01-18 01:08:59.000000 types-aiobotocore-guardduty-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:49.397302 types-aiobotocore-guardduty-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-01-18 01:08:59.000000 types-aiobotocore-guardduty-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:49.397302 types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty/
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-01-18 01:08:59.000000 types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-01-18 01:08:59.000000 types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-01-18 01:08:59.000000 types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52743 2024-01-18 01:08:59.000000 types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52740 2024-01-18 01:08:59.000000 types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15387 2024-01-18 01:08:59.000000 types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15387 2024-01-18 01:08:59.000000 types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12536 2024-01-18 01:08:59.000000 types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12525 2024-01-18 01:08:59.000000 types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:08:59.000000 types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    88315 2024-01-18 01:09:02.000000 types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    88315 2024-01-18 01:09:02.000000 types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:08:59.000000 types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:49.397302 types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14377 2024-01-18 01:20:49.000000 types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-01-18 01:20:49.000000 types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:49.000000 types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:49.000000 types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:49.000000 types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-18 01:20:49.000000 types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-guardduty-2.9.0/LICENSE` & `types-aiobotocore-guardduty-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-guardduty-2.9.0/PKG-INFO` & `types-aiobotocore-guardduty-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-guardduty
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.GuardDuty 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.GuardDuty 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/
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
 
 <a id="types-aiobotocore-guardduty"></a>
 
 # types-aiobotocore-guardduty
 
 [![PyPI - types-aiobotocore-guardduty](https://img.shields.io/pypi/v/types-aiobotocore-guardduty.svg?color=blue)](https://pypi.org/project/types-aiobotocore-guardduty)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-guardduty.svg?color=blue)](https://pypi.org/project/types-aiobotocore-guardduty)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-guardduty)](https://pepy.tech/project/types-aiobotocore-guardduty)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GuardDuty 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
+[aiobotocore.GuardDuty 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
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
 [types-aiobotocore-guardduty docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-guardduty-2.9.0/README.md` & `types-aiobotocore-guardduty-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-guardduty.svg?color=blue)](https://pypi.org/project/types-aiobotocore-guardduty)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-guardduty)](https://pepy.tech/project/types-aiobotocore-guardduty)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GuardDuty 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
+[aiobotocore.GuardDuty 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
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
 [types-aiobotocore-guardduty docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-guardduty-2.9.0/setup.py` & `types-aiobotocore-guardduty-2.9.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-guardduty",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_guardduty"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.GuardDuty 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.GuardDuty 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore guardduty type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_guardduty": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty/__init__.py` & `types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     ListMembersPaginator,
     ListOrganizationAdminAccountsPaginator,
     ListThreatIntelSetsPaginator,
 )
 
 Client = GuardDutyClient
 
-
 __all__ = (
     "Client",
     "DescribeMalwareScansPaginator",
     "GuardDutyClient",
     "ListCoveragePaginator",
     "ListDetectorsPaginator",
     "ListFiltersPaginator",
```

### Comparing `types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty/__init__.pyi` & `types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty/__main__.py` & `types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.GuardDuty 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.GuardDuty 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty\nOther"
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

### Comparing `types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty/client.py` & `types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("GuardDutyClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -200,15 +199,15 @@
         self,
         *,
         Enable: bool,
         ClientToken: str = ...,
         FindingPublishingFrequency: FindingPublishingFrequencyType = ...,
         DataSources: DataSourceConfigurationsTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        Features: Sequence[DetectorFeatureConfigurationTypeDef] = ...
+        Features: Sequence[DetectorFeatureConfigurationTypeDef] = ...,
     ) -> CreateDetectorResponseTypeDef:
         """
         Creates a single Amazon GuardDuty detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.create_detector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#create_detector)
         """
@@ -219,15 +218,15 @@
         DetectorId: str,
         Name: str,
         FindingCriteria: FindingCriteriaTypeDef,
         Description: str = ...,
         Action: FilterActionType = ...,
         Rank: int = ...,
         ClientToken: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateFilterResponseTypeDef:
         """
         Creates a filter using the specified finding criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.create_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#create_filter)
         """
@@ -237,15 +236,15 @@
         *,
         DetectorId: str,
         Name: str,
         Format: IpSetFormatType,
         Location: str,
         Activate: bool,
         ClientToken: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateIPSetResponseTypeDef:
         """
         Creates a new IPSet, which is called a trusted IP list in the console user
         interface.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.create_ip_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#create_ip_set)
@@ -265,15 +264,15 @@
 
     async def create_publishing_destination(
         self,
         *,
         DetectorId: str,
         DestinationType: Literal["S3"],
         DestinationProperties: DestinationPropertiesTypeDef,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreatePublishingDestinationResponseTypeDef:
         """
         Creates a publishing destination to export findings to.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.create_publishing_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#create_publishing_destination)
         """
@@ -293,15 +292,15 @@
         *,
         DetectorId: str,
         Name: str,
         Format: ThreatIntelSetFormatType,
         Location: str,
         Activate: bool,
         ClientToken: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateThreatIntelSetResponseTypeDef:
         """
         Creates a new ThreatIntelSet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.create_threat_intel_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#create_threat_intel_set)
         """
@@ -389,15 +388,15 @@
     async def describe_malware_scans(
         self,
         *,
         DetectorId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         FilterCriteria: FilterCriteriaTypeDef = ...,
-        SortCriteria: SortCriteriaTypeDef = ...
+        SortCriteria: SortCriteriaTypeDef = ...,
     ) -> DescribeMalwareScansResponseTypeDef:
         """
         Returns a list of malware scans.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.describe_malware_scans)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#describe_malware_scans)
         """
@@ -500,15 +499,15 @@
         """
 
     async def get_coverage_statistics(
         self,
         *,
         DetectorId: str,
         StatisticsType: Sequence[CoverageStatisticsTypeType],
-        FilterCriteria: CoverageFilterCriteriaTypeDef = ...
+        FilterCriteria: CoverageFilterCriteriaTypeDef = ...,
     ) -> GetCoverageStatisticsResponseTypeDef:
         """
         Retrieves aggregated statistics for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_coverage_statistics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#get_coverage_statistics)
         """
@@ -540,15 +539,15 @@
         """
 
     async def get_findings_statistics(
         self,
         *,
         DetectorId: str,
         FindingStatisticTypes: Sequence[Literal["COUNT_BY_SEVERITY"]],
-        FindingCriteria: FindingCriteriaTypeDef = ...
+        FindingCriteria: FindingCriteriaTypeDef = ...,
     ) -> GetFindingsStatisticsResponseTypeDef:
         """
         Lists Amazon GuardDuty findings statistics for the specified detector ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_findings_statistics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#get_findings_statistics)
         """
@@ -638,15 +637,15 @@
         self,
         *,
         DetectorId: str,
         UsageStatisticType: UsageStatisticTypeType,
         UsageCriteria: UsageCriteriaTypeDef,
         Unit: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetUsageStatisticsResponseTypeDef:
         """
         Lists Amazon GuardDuty usage statistics over the last 30 days for the specified
         detector
         ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_usage_statistics)
@@ -655,15 +654,15 @@
 
     async def invite_members(
         self,
         *,
         DetectorId: str,
         AccountIds: Sequence[str],
         DisableEmailNotification: bool = ...,
-        Message: str = ...
+        Message: str = ...,
     ) -> InviteMembersResponseTypeDef:
         """
         Invites Amazon Web Services accounts to become members of an organization
         administered by the Amazon Web Services account that invokes this
         API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.invite_members)
@@ -673,15 +672,15 @@
     async def list_coverage(
         self,
         *,
         DetectorId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         FilterCriteria: CoverageFilterCriteriaTypeDef = ...,
-        SortCriteria: CoverageSortCriteriaTypeDef = ...
+        SortCriteria: CoverageSortCriteriaTypeDef = ...,
     ) -> ListCoverageResponseTypeDef:
         """
         Lists coverage details for your GuardDuty account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.list_coverage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#list_coverage)
         """
@@ -709,15 +708,15 @@
     async def list_findings(
         self,
         *,
         DetectorId: str,
         FindingCriteria: FindingCriteriaTypeDef = ...,
         SortCriteria: SortCriteriaTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListFindingsResponseTypeDef:
         """
         Lists Amazon GuardDuty findings for the specified detector ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.list_findings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#list_findings)
         """
@@ -746,15 +745,15 @@
 
     async def list_members(
         self,
         *,
         DetectorId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        OnlyAssociated: str = ...
+        OnlyAssociated: str = ...,
     ) -> ListMembersResponseTypeDef:
         """
         Lists details about all member accounts for the current GuardDuty administrator
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.list_members)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#list_members)
@@ -858,15 +857,15 @@
     async def update_detector(
         self,
         *,
         DetectorId: str,
         Enable: bool = ...,
         FindingPublishingFrequency: FindingPublishingFrequencyType = ...,
         DataSources: DataSourceConfigurationsTypeDef = ...,
-        Features: Sequence[DetectorFeatureConfigurationTypeDef] = ...
+        Features: Sequence[DetectorFeatureConfigurationTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Updates the Amazon GuardDuty detector specified by the detectorId.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_detector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#update_detector)
         """
@@ -875,30 +874,30 @@
         self,
         *,
         DetectorId: str,
         FilterName: str,
         Description: str = ...,
         Action: FilterActionType = ...,
         Rank: int = ...,
-        FindingCriteria: FindingCriteriaTypeDef = ...
+        FindingCriteria: FindingCriteriaTypeDef = ...,
     ) -> UpdateFilterResponseTypeDef:
         """
         Updates the filter specified by the filter name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#update_filter)
         """
 
     async def update_findings_feedback(
         self,
         *,
         DetectorId: str,
         FindingIds: Sequence[str],
         Feedback: FeedbackType,
-        Comments: str = ...
+        Comments: str = ...,
     ) -> Dict[str, Any]:
         """
         Marks the specified GuardDuty findings as useful or not useful.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_findings_feedback)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#update_findings_feedback)
         """
@@ -906,44 +905,44 @@
     async def update_ip_set(
         self,
         *,
         DetectorId: str,
         IpSetId: str,
         Name: str = ...,
         Location: str = ...,
-        Activate: bool = ...
+        Activate: bool = ...,
     ) -> Dict[str, Any]:
         """
         Updates the IPSet specified by the IPSet ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_ip_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#update_ip_set)
         """
 
     async def update_malware_scan_settings(
         self,
         *,
         DetectorId: str,
         ScanResourceCriteria: ScanResourceCriteriaTypeDef = ...,
-        EbsSnapshotPreservation: EbsSnapshotPreservationType = ...
+        EbsSnapshotPreservation: EbsSnapshotPreservationType = ...,
     ) -> Dict[str, Any]:
         """
         Updates the malware scan settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_malware_scan_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#update_malware_scan_settings)
         """
 
     async def update_member_detectors(
         self,
         *,
         DetectorId: str,
         AccountIds: Sequence[str],
         DataSources: DataSourceConfigurationsTypeDef = ...,
-        Features: Sequence[MemberFeaturesConfigurationTypeDef] = ...
+        Features: Sequence[MemberFeaturesConfigurationTypeDef] = ...,
     ) -> UpdateMemberDetectorsResponseTypeDef:
         """
         Contains information on member accounts to be updated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_member_detectors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#update_member_detectors)
         """
@@ -951,29 +950,29 @@
     async def update_organization_configuration(
         self,
         *,
         DetectorId: str,
         AutoEnable: bool = ...,
         DataSources: OrganizationDataSourceConfigurationsTypeDef = ...,
         Features: Sequence[OrganizationFeatureConfigurationTypeDef] = ...,
-        AutoEnableOrganizationMembers: AutoEnableMembersType = ...
+        AutoEnableOrganizationMembers: AutoEnableMembersType = ...,
     ) -> Dict[str, Any]:
         """
         Configures the delegated administrator account with the provided values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_organization_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#update_organization_configuration)
         """
 
     async def update_publishing_destination(
         self,
         *,
         DetectorId: str,
         DestinationId: str,
-        DestinationProperties: DestinationPropertiesTypeDef = ...
+        DestinationProperties: DestinationPropertiesTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates information about the publishing destination specified by the
         `destinationId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_publishing_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#update_publishing_destination)
@@ -982,15 +981,15 @@
     async def update_threat_intel_set(
         self,
         *,
         DetectorId: str,
         ThreatIntelSetId: str,
         Name: str = ...,
         Location: str = ...,
-        Activate: bool = ...
+        Activate: bool = ...,
     ) -> Dict[str, Any]:
         """
         Updates the ThreatIntelSet specified by the ThreatIntelSet ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_threat_intel_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#update_threat_intel_set)
         """
```

### Comparing `types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty/client.pyi` & `types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -196,15 +196,15 @@
         self,
         *,
         Enable: bool,
         ClientToken: str = ...,
         FindingPublishingFrequency: FindingPublishingFrequencyType = ...,
         DataSources: DataSourceConfigurationsTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        Features: Sequence[DetectorFeatureConfigurationTypeDef] = ...
+        Features: Sequence[DetectorFeatureConfigurationTypeDef] = ...,
     ) -> CreateDetectorResponseTypeDef:
         """
         Creates a single Amazon GuardDuty detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.create_detector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#create_detector)
         """
@@ -215,15 +215,15 @@
         DetectorId: str,
         Name: str,
         FindingCriteria: FindingCriteriaTypeDef,
         Description: str = ...,
         Action: FilterActionType = ...,
         Rank: int = ...,
         ClientToken: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateFilterResponseTypeDef:
         """
         Creates a filter using the specified finding criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.create_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#create_filter)
         """
@@ -233,15 +233,15 @@
         *,
         DetectorId: str,
         Name: str,
         Format: IpSetFormatType,
         Location: str,
         Activate: bool,
         ClientToken: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateIPSetResponseTypeDef:
         """
         Creates a new IPSet, which is called a trusted IP list in the console user
         interface.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.create_ip_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#create_ip_set)
@@ -261,15 +261,15 @@
 
     async def create_publishing_destination(
         self,
         *,
         DetectorId: str,
         DestinationType: Literal["S3"],
         DestinationProperties: DestinationPropertiesTypeDef,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreatePublishingDestinationResponseTypeDef:
         """
         Creates a publishing destination to export findings to.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.create_publishing_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#create_publishing_destination)
         """
@@ -289,15 +289,15 @@
         *,
         DetectorId: str,
         Name: str,
         Format: ThreatIntelSetFormatType,
         Location: str,
         Activate: bool,
         ClientToken: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateThreatIntelSetResponseTypeDef:
         """
         Creates a new ThreatIntelSet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.create_threat_intel_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#create_threat_intel_set)
         """
@@ -385,15 +385,15 @@
     async def describe_malware_scans(
         self,
         *,
         DetectorId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         FilterCriteria: FilterCriteriaTypeDef = ...,
-        SortCriteria: SortCriteriaTypeDef = ...
+        SortCriteria: SortCriteriaTypeDef = ...,
     ) -> DescribeMalwareScansResponseTypeDef:
         """
         Returns a list of malware scans.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.describe_malware_scans)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#describe_malware_scans)
         """
@@ -496,15 +496,15 @@
         """
 
     async def get_coverage_statistics(
         self,
         *,
         DetectorId: str,
         StatisticsType: Sequence[CoverageStatisticsTypeType],
-        FilterCriteria: CoverageFilterCriteriaTypeDef = ...
+        FilterCriteria: CoverageFilterCriteriaTypeDef = ...,
     ) -> GetCoverageStatisticsResponseTypeDef:
         """
         Retrieves aggregated statistics for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_coverage_statistics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#get_coverage_statistics)
         """
@@ -536,15 +536,15 @@
         """
 
     async def get_findings_statistics(
         self,
         *,
         DetectorId: str,
         FindingStatisticTypes: Sequence[Literal["COUNT_BY_SEVERITY"]],
-        FindingCriteria: FindingCriteriaTypeDef = ...
+        FindingCriteria: FindingCriteriaTypeDef = ...,
     ) -> GetFindingsStatisticsResponseTypeDef:
         """
         Lists Amazon GuardDuty findings statistics for the specified detector ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_findings_statistics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#get_findings_statistics)
         """
@@ -634,15 +634,15 @@
         self,
         *,
         DetectorId: str,
         UsageStatisticType: UsageStatisticTypeType,
         UsageCriteria: UsageCriteriaTypeDef,
         Unit: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetUsageStatisticsResponseTypeDef:
         """
         Lists Amazon GuardDuty usage statistics over the last 30 days for the specified
         detector
         ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_usage_statistics)
@@ -651,15 +651,15 @@
 
     async def invite_members(
         self,
         *,
         DetectorId: str,
         AccountIds: Sequence[str],
         DisableEmailNotification: bool = ...,
-        Message: str = ...
+        Message: str = ...,
     ) -> InviteMembersResponseTypeDef:
         """
         Invites Amazon Web Services accounts to become members of an organization
         administered by the Amazon Web Services account that invokes this
         API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.invite_members)
@@ -669,15 +669,15 @@
     async def list_coverage(
         self,
         *,
         DetectorId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         FilterCriteria: CoverageFilterCriteriaTypeDef = ...,
-        SortCriteria: CoverageSortCriteriaTypeDef = ...
+        SortCriteria: CoverageSortCriteriaTypeDef = ...,
     ) -> ListCoverageResponseTypeDef:
         """
         Lists coverage details for your GuardDuty account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.list_coverage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#list_coverage)
         """
@@ -705,15 +705,15 @@
     async def list_findings(
         self,
         *,
         DetectorId: str,
         FindingCriteria: FindingCriteriaTypeDef = ...,
         SortCriteria: SortCriteriaTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListFindingsResponseTypeDef:
         """
         Lists Amazon GuardDuty findings for the specified detector ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.list_findings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#list_findings)
         """
@@ -742,15 +742,15 @@
 
     async def list_members(
         self,
         *,
         DetectorId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        OnlyAssociated: str = ...
+        OnlyAssociated: str = ...,
     ) -> ListMembersResponseTypeDef:
         """
         Lists details about all member accounts for the current GuardDuty administrator
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.list_members)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#list_members)
@@ -854,15 +854,15 @@
     async def update_detector(
         self,
         *,
         DetectorId: str,
         Enable: bool = ...,
         FindingPublishingFrequency: FindingPublishingFrequencyType = ...,
         DataSources: DataSourceConfigurationsTypeDef = ...,
-        Features: Sequence[DetectorFeatureConfigurationTypeDef] = ...
+        Features: Sequence[DetectorFeatureConfigurationTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Updates the Amazon GuardDuty detector specified by the detectorId.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_detector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#update_detector)
         """
@@ -871,30 +871,30 @@
         self,
         *,
         DetectorId: str,
         FilterName: str,
         Description: str = ...,
         Action: FilterActionType = ...,
         Rank: int = ...,
-        FindingCriteria: FindingCriteriaTypeDef = ...
+        FindingCriteria: FindingCriteriaTypeDef = ...,
     ) -> UpdateFilterResponseTypeDef:
         """
         Updates the filter specified by the filter name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#update_filter)
         """
 
     async def update_findings_feedback(
         self,
         *,
         DetectorId: str,
         FindingIds: Sequence[str],
         Feedback: FeedbackType,
-        Comments: str = ...
+        Comments: str = ...,
     ) -> Dict[str, Any]:
         """
         Marks the specified GuardDuty findings as useful or not useful.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_findings_feedback)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#update_findings_feedback)
         """
@@ -902,44 +902,44 @@
     async def update_ip_set(
         self,
         *,
         DetectorId: str,
         IpSetId: str,
         Name: str = ...,
         Location: str = ...,
-        Activate: bool = ...
+        Activate: bool = ...,
     ) -> Dict[str, Any]:
         """
         Updates the IPSet specified by the IPSet ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_ip_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#update_ip_set)
         """
 
     async def update_malware_scan_settings(
         self,
         *,
         DetectorId: str,
         ScanResourceCriteria: ScanResourceCriteriaTypeDef = ...,
-        EbsSnapshotPreservation: EbsSnapshotPreservationType = ...
+        EbsSnapshotPreservation: EbsSnapshotPreservationType = ...,
     ) -> Dict[str, Any]:
         """
         Updates the malware scan settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_malware_scan_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#update_malware_scan_settings)
         """
 
     async def update_member_detectors(
         self,
         *,
         DetectorId: str,
         AccountIds: Sequence[str],
         DataSources: DataSourceConfigurationsTypeDef = ...,
-        Features: Sequence[MemberFeaturesConfigurationTypeDef] = ...
+        Features: Sequence[MemberFeaturesConfigurationTypeDef] = ...,
     ) -> UpdateMemberDetectorsResponseTypeDef:
         """
         Contains information on member accounts to be updated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_member_detectors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#update_member_detectors)
         """
@@ -947,29 +947,29 @@
     async def update_organization_configuration(
         self,
         *,
         DetectorId: str,
         AutoEnable: bool = ...,
         DataSources: OrganizationDataSourceConfigurationsTypeDef = ...,
         Features: Sequence[OrganizationFeatureConfigurationTypeDef] = ...,
-        AutoEnableOrganizationMembers: AutoEnableMembersType = ...
+        AutoEnableOrganizationMembers: AutoEnableMembersType = ...,
     ) -> Dict[str, Any]:
         """
         Configures the delegated administrator account with the provided values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_organization_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#update_organization_configuration)
         """
 
     async def update_publishing_destination(
         self,
         *,
         DetectorId: str,
         DestinationId: str,
-        DestinationProperties: DestinationPropertiesTypeDef = ...
+        DestinationProperties: DestinationPropertiesTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates information about the publishing destination specified by the
         `destinationId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_publishing_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#update_publishing_destination)
@@ -978,15 +978,15 @@
     async def update_threat_intel_set(
         self,
         *,
         DetectorId: str,
         ThreatIntelSetId: str,
         Name: str = ...,
         Location: str = ...,
-        Activate: bool = ...
+        Activate: bool = ...,
     ) -> Dict[str, Any]:
         """
         Updates the ThreatIntelSet specified by the ThreatIntelSet ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_threat_intel_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#update_threat_intel_set)
         """
```

### Comparing `types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty/literals.py` & `types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty/literals.py`

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
     "AdminStatusType",
     "AutoEnableMembersType",
     "CoverageFilterCriterionKeyType",
     "CoverageSortKeyType",
     "CoverageStatisticsTypeType",
     "CoverageStatusType",
@@ -74,15 +73,14 @@
     "GuardDutyServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AdminStatusType = Literal["DISABLE_IN_PROGRESS", "ENABLED"]
 AutoEnableMembersType = Literal["ALL", "NEW", "NONE"]
 CoverageFilterCriterionKeyType = Literal[
     "ACCOUNT_ID",
     "ADDON_VERSION",
     "AGENT_VERSION",
     "CLUSTER_ARN",
```

### Comparing `types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty/literals.pyi` & `types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty/paginator.py` & `types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,14 @@
     "ListIPSetsPaginator",
     "ListInvitationsPaginator",
     "ListMembersPaginator",
     "ListOrganizationAdminAccountsPaginator",
     "ListThreatIntelSetsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -95,15 +94,15 @@
 
     def paginate(
         self,
         *,
         DetectorId: str,
         FilterCriteria: FilterCriteriaTypeDef = ...,
         SortCriteria: SortCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeMalwareScansResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.DescribeMalwareScans.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#describemalwarescanspaginator)
         """
 
 
@@ -115,15 +114,15 @@
 
     def paginate(
         self,
         *,
         DetectorId: str,
         FilterCriteria: CoverageFilterCriteriaTypeDef = ...,
         SortCriteria: CoverageSortCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCoverageResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListCoverage.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listcoveragepaginator)
         """
 
 
@@ -165,15 +164,15 @@
 
     def paginate(
         self,
         *,
         DetectorId: str,
         FindingCriteria: FindingCriteriaTypeDef = ...,
         SortCriteria: SortCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listfindingspaginator)
         """
 
 
@@ -214,15 +213,15 @@
     """
 
     def paginate(
         self,
         *,
         DetectorId: str,
         OnlyAssociated: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListMembers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listmemberspaginator)
         """
```

### Comparing `types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty/paginator.pyi` & `types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
     def paginate(
         self,
         *,
         DetectorId: str,
         FilterCriteria: FilterCriteriaTypeDef = ...,
         SortCriteria: SortCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeMalwareScansResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.DescribeMalwareScans.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#describemalwarescanspaginator)
         """
 
 class ListCoveragePaginator(AioPaginator):
@@ -111,15 +111,15 @@
 
     def paginate(
         self,
         *,
         DetectorId: str,
         FilterCriteria: CoverageFilterCriteriaTypeDef = ...,
         SortCriteria: CoverageSortCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCoverageResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListCoverage.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listcoveragepaginator)
         """
 
 class ListDetectorsPaginator(AioPaginator):
@@ -158,15 +158,15 @@
 
     def paginate(
         self,
         *,
         DetectorId: str,
         FindingCriteria: FindingCriteriaTypeDef = ...,
         SortCriteria: SortCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listfindingspaginator)
         """
 
 class ListIPSetsPaginator(AioPaginator):
@@ -204,15 +204,15 @@
     """
 
     def paginate(
         self,
         *,
         DetectorId: str,
         OnlyAssociated: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListMembers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listmemberspaginator)
         """
 
 class ListOrganizationAdminAccountsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty/type_defs.py` & `types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceptAdministratorInvitationRequestRequestTypeDef",
     "AcceptInvitationRequestRequestTypeDef",
     "AccessControlListTypeDef",
     "AccessKeyDetailsTypeDef",
     "AccountDetailTypeDef",
     "FreeTrialFeatureConfigurationResultTypeDef",
```

### Comparing `types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty/type_defs.pyi` & `types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty.egg-info/PKG-INFO` & `types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-guardduty
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.GuardDuty 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.GuardDuty 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/
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
 
 <a id="types-aiobotocore-guardduty"></a>
 
 # types-aiobotocore-guardduty
 
 [![PyPI - types-aiobotocore-guardduty](https://img.shields.io/pypi/v/types-aiobotocore-guardduty.svg?color=blue)](https://pypi.org/project/types-aiobotocore-guardduty)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-guardduty.svg?color=blue)](https://pypi.org/project/types-aiobotocore-guardduty)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-guardduty)](https://pepy.tech/project/types-aiobotocore-guardduty)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GuardDuty 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
+[aiobotocore.GuardDuty 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
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
 [types-aiobotocore-guardduty docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-guardduty-2.9.0/types_aiobotocore_guardduty.egg-info/SOURCES.txt` & `types-aiobotocore-guardduty-2.9.1/types_aiobotocore_guardduty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

