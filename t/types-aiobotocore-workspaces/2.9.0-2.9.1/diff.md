# Comparing `tmp/types-aiobotocore-workspaces-2.9.0.tar.gz` & `tmp/types-aiobotocore-workspaces-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-workspaces-2.9.0.tar", last modified: Wed Dec 13 20:00:47 2023, max compression
+gzip compressed data, was "types-aiobotocore-workspaces-2.9.1.tar", last modified: Thu Jan 18 01:22:04 2024, max compression
```

## Comparing `types-aiobotocore-workspaces-2.9.0.tar` & `types-aiobotocore-workspaces-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:47.864989 types-aiobotocore-workspaces-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:58:03.000000 types-aiobotocore-workspaces-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14536 2023-12-13 20:00:47.864989 types-aiobotocore-workspaces-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12961 2023-12-13 19:58:03.000000 types-aiobotocore-workspaces-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:47.864989 types-aiobotocore-workspaces-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2023-12-13 19:58:03.000000 types-aiobotocore-workspaces-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:47.864989 types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces/
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2023-12-13 19:58:03.000000 types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2023-12-13 19:58:03.000000 types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      944 2023-12-13 19:58:03.000000 types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    57405 2023-12-13 19:58:06.000000 types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    57401 2023-12-13 19:58:03.000000 types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16255 2023-12-13 19:58:07.000000 types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    16253 2023-12-13 19:58:07.000000 types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11239 2023-12-13 19:58:07.000000 types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11229 2023-12-13 19:58:07.000000 types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:03.000000 types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    60773 2023-12-13 19:58:08.000000 types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    60772 2023-12-13 19:58:07.000000 types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:58:03.000000 types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:47.864989 types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14536 2023-12-13 20:00:47.000000 types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      870 2023-12-13 20:00:47.000000 types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:47.000000 types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:47.000000 types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:47.000000 types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-13 20:00:47.000000 types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:04.660962 types-aiobotocore-workspaces-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:19:31.000000 types-aiobotocore-workspaces-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14556 2024-01-18 01:22:04.660962 types-aiobotocore-workspaces-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12961 2024-01-18 01:19:31.000000 types-aiobotocore-workspaces-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:22:04.660962 types-aiobotocore-workspaces-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-01-18 01:19:31.000000 types-aiobotocore-workspaces-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:04.660962 types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-01-18 01:19:31.000000 types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-01-18 01:19:31.000000 types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-01-18 01:19:31.000000 types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57419 2024-01-18 01:19:32.000000 types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57416 2024-01-18 01:19:32.000000 types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16253 2024-01-18 01:19:32.000000 types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16253 2024-01-18 01:19:32.000000 types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11242 2024-01-18 01:19:32.000000 types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11233 2024-01-18 01:19:32.000000 types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:31.000000 types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    60772 2024-01-18 01:19:33.000000 types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60772 2024-01-18 01:19:33.000000 types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:19:31.000000 types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:04.660962 types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14556 2024-01-18 01:22:04.000000 types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-01-18 01:22:04.000000 types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:22:04.000000 types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:22:04.000000 types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:22:04.000000 types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-18 01:22:04.000000 types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-workspaces-2.9.0/LICENSE` & `types-aiobotocore-workspaces-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-workspaces-2.9.0/PKG-INFO` & `types-aiobotocore-workspaces-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-workspaces
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.WorkSpaces 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.WorkSpaces 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/
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
 
 <a id="types-aiobotocore-workspaces"></a>
 
 # types-aiobotocore-workspaces
 
 [![PyPI - types-aiobotocore-workspaces](https://img.shields.io/pypi/v/types-aiobotocore-workspaces.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workspaces)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-workspaces.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workspaces)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-workspaces)](https://pepy.tech/project/types-aiobotocore-workspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WorkSpaces 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
+[aiobotocore.WorkSpaces 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
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
 [types-aiobotocore-workspaces docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-workspaces-2.9.0/README.md` & `types-aiobotocore-workspaces-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-workspaces.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workspaces)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-workspaces)](https://pepy.tech/project/types-aiobotocore-workspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WorkSpaces 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
+[aiobotocore.WorkSpaces 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
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
 [types-aiobotocore-workspaces docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-workspaces-2.9.0/setup.py` & `types-aiobotocore-workspaces-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-workspaces",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_workspaces"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.WorkSpaces 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.WorkSpaces 2.9.1 service generated with"
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
     keywords="aiobotocore workspaces type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_workspaces": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces/__init__.py` & `types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     DescribeWorkspacesConnectionStatusPaginator,
     DescribeWorkspacesPaginator,
     ListAvailableManagementCidrRangesPaginator,
 )
 
 Client = WorkSpacesClient
 
-
 __all__ = (
     "Client",
     "DescribeAccountModificationsPaginator",
     "DescribeIpGroupsPaginator",
     "DescribeWorkspaceBundlesPaginator",
     "DescribeWorkspaceDirectoriesPaginator",
     "DescribeWorkspaceImagesPaginator",
```

### Comparing `types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces/__init__.pyi` & `types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces/__main__.py` & `types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.WorkSpaces 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.WorkSpaces 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces\nOther"
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

### Comparing `types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces/client.py` & `types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("WorkSpacesClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -231,15 +230,15 @@
     async def copy_workspace_image(
         self,
         *,
         Name: str,
         SourceImageId: str,
         SourceRegion: str,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CopyWorkspaceImageResultTypeDef:
         """
         Copies the specified image from the specified Region to the current Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.copy_workspace_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#copy_workspace_image)
         """
@@ -266,15 +265,15 @@
 
     async def create_ip_group(
         self,
         *,
         GroupName: str,
         GroupDesc: str = ...,
         UserRules: Sequence[IpRuleItemTypeDef] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateIpGroupResultTypeDef:
         """
         Creates an IP access control group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_ip_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#create_ip_group)
         """
@@ -312,15 +311,15 @@
         *,
         BundleName: str,
         BundleDescription: str,
         ImageId: str,
         ComputeType: ComputeTypeTypeDef,
         UserStorage: UserStorageTypeDef,
         RootStorage: RootStorageTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateWorkspaceBundleResultTypeDef:
         """
         Creates the specified WorkSpace bundle.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_workspace_bundle)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#create_workspace_bundle)
         """
@@ -449,15 +448,15 @@
 
     async def describe_application_associations(
         self,
         *,
         ApplicationId: str,
         AssociatedResourceTypes: Sequence[ApplicationAssociatedResourceTypeType],
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeApplicationAssociationsResultTypeDef:
         """
         Describes the associations between the application and the specified associated
         resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.describe_application_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#describe_application_associations)
@@ -468,15 +467,15 @@
         *,
         ApplicationIds: Sequence[str] = ...,
         ComputeTypeNames: Sequence[ComputeType] = ...,
         LicenseType: WorkSpaceApplicationLicenseTypeType = ...,
         OperatingSystemNames: Sequence[OperatingSystemNameType] = ...,
         Owner: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeApplicationsResultTypeDef:
         """
         Describes the specified applications by filtering based on their compute types,
         license availability, operating systems, and
         owners.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.describe_applications)
@@ -537,15 +536,15 @@
 
     async def describe_connection_aliases(
         self,
         *,
         AliasIds: Sequence[str] = ...,
         ResourceId: str = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeConnectionAliasesResultTypeDef:
         """
         Retrieves a list that describes the connection aliases used for cross-Region
         redirection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.describe_connection_aliases)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#describe_connection_aliases)
@@ -623,15 +622,15 @@
 
     async def describe_workspace_images(
         self,
         *,
         ImageIds: Sequence[str] = ...,
         ImageType: ImageTypeType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeWorkspaceImagesResultTypeDef:
         """
         Retrieves a list that describes one or more specified images, if the image
         identifiers are
         provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.describe_workspace_images)
@@ -652,15 +651,15 @@
         self,
         *,
         WorkspaceIds: Sequence[str] = ...,
         DirectoryId: str = ...,
         UserName: str = ...,
         BundleId: str = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeWorkspacesResultTypeDef:
         """
         Describes the specified WorkSpaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.describe_workspaces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#describe_workspaces)
         """
@@ -723,15 +722,15 @@
         *,
         ResourceId: str,
         DeviceTypeWindows: DefaultImportClientBrandingAttributesTypeDef = ...,
         DeviceTypeOsx: DefaultImportClientBrandingAttributesTypeDef = ...,
         DeviceTypeAndroid: DefaultImportClientBrandingAttributesTypeDef = ...,
         DeviceTypeIos: IosImportClientBrandingAttributesTypeDef = ...,
         DeviceTypeLinux: DefaultImportClientBrandingAttributesTypeDef = ...,
-        DeviceTypeWeb: DefaultImportClientBrandingAttributesTypeDef = ...
+        DeviceTypeWeb: DefaultImportClientBrandingAttributesTypeDef = ...,
     ) -> ImportClientBrandingResultTypeDef:
         """
         Imports client branding.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.import_client_branding)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#import_client_branding)
         """
@@ -740,15 +739,15 @@
         self,
         *,
         Ec2ImageId: str,
         IngestionProcess: WorkspaceImageIngestionProcessType,
         ImageName: str,
         ImageDescription: str,
         Tags: Sequence[TagTypeDef] = ...,
-        Applications: Sequence[ApplicationType] = ...
+        Applications: Sequence[ApplicationType] = ...,
     ) -> ImportWorkspaceImageResultTypeDef:
         """
         Imports the specified Windows 10 or 11 Bring Your Own License (BYOL) image into
         Amazon
         WorkSpaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.import_workspace_image)
@@ -780,15 +779,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#migrate_workspace)
         """
 
     async def modify_account(
         self,
         *,
         DedicatedTenancySupport: Literal["ENABLED"] = ...,
-        DedicatedTenancyManagementCidrRange: str = ...
+        DedicatedTenancyManagementCidrRange: str = ...,
     ) -> Dict[str, Any]:
         """
         Modifies the configuration of Bring Your Own License (BYOL) for the specified
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.modify_account)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#modify_account)
@@ -797,15 +796,15 @@
     async def modify_certificate_based_auth_properties(
         self,
         *,
         ResourceId: str,
         CertificateBasedAuthProperties: CertificateBasedAuthPropertiesTypeDef = ...,
         PropertiesToDelete: Sequence[
             Literal["CERTIFICATE_BASED_AUTH_PROPERTIES_CERTIFICATE_AUTHORITY_ARN"]
-        ] = ...
+        ] = ...,
     ) -> Dict[str, Any]:
         """
         Modifies the properties of the certificate-based authentication you want to use
         with your
         WorkSpaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.modify_certificate_based_auth_properties)
@@ -823,15 +822,15 @@
         """
 
     async def modify_saml_properties(
         self,
         *,
         ResourceId: str,
         SamlProperties: SamlPropertiesTypeDef = ...,
-        PropertiesToDelete: Sequence[DeletableSamlPropertyType] = ...
+        PropertiesToDelete: Sequence[DeletableSamlPropertyType] = ...,
     ) -> Dict[str, Any]:
         """
         Modifies multiple properties related to SAML 2.0 authentication, including the
         enablement status, user access URL, and relay state parameter name that are
         used for configuring federation with an SAML 2.0 identity
         provider.
 
@@ -871,15 +870,15 @@
         """
 
     async def modify_workspace_properties(
         self,
         *,
         WorkspaceId: str,
         WorkspaceProperties: WorkspacePropertiesTypeDef = ...,
-        DataReplication: DataReplicationType = ...
+        DataReplication: DataReplicationType = ...,
     ) -> Dict[str, Any]:
         """
         Modifies the specified WorkSpace properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.modify_workspace_properties)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#modify_workspace_properties)
         """
@@ -918,15 +917,15 @@
         self,
         *,
         DirectoryId: str,
         EnableWorkDocs: bool,
         SubnetIds: Sequence[str] = ...,
         EnableSelfService: bool = ...,
         Tenancy: TenancyType = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Registers the specified directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.register_workspace_directory)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#register_workspace_directory)
         """
```

### Comparing `types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces/client.pyi` & `types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -227,15 +227,15 @@
     async def copy_workspace_image(
         self,
         *,
         Name: str,
         SourceImageId: str,
         SourceRegion: str,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CopyWorkspaceImageResultTypeDef:
         """
         Copies the specified image from the specified Region to the current Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.copy_workspace_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#copy_workspace_image)
         """
@@ -262,15 +262,15 @@
 
     async def create_ip_group(
         self,
         *,
         GroupName: str,
         GroupDesc: str = ...,
         UserRules: Sequence[IpRuleItemTypeDef] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateIpGroupResultTypeDef:
         """
         Creates an IP access control group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_ip_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#create_ip_group)
         """
@@ -308,15 +308,15 @@
         *,
         BundleName: str,
         BundleDescription: str,
         ImageId: str,
         ComputeType: ComputeTypeTypeDef,
         UserStorage: UserStorageTypeDef,
         RootStorage: RootStorageTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateWorkspaceBundleResultTypeDef:
         """
         Creates the specified WorkSpace bundle.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_workspace_bundle)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#create_workspace_bundle)
         """
@@ -445,15 +445,15 @@
 
     async def describe_application_associations(
         self,
         *,
         ApplicationId: str,
         AssociatedResourceTypes: Sequence[ApplicationAssociatedResourceTypeType],
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeApplicationAssociationsResultTypeDef:
         """
         Describes the associations between the application and the specified associated
         resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.describe_application_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#describe_application_associations)
@@ -464,15 +464,15 @@
         *,
         ApplicationIds: Sequence[str] = ...,
         ComputeTypeNames: Sequence[ComputeType] = ...,
         LicenseType: WorkSpaceApplicationLicenseTypeType = ...,
         OperatingSystemNames: Sequence[OperatingSystemNameType] = ...,
         Owner: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeApplicationsResultTypeDef:
         """
         Describes the specified applications by filtering based on their compute types,
         license availability, operating systems, and
         owners.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.describe_applications)
@@ -533,15 +533,15 @@
 
     async def describe_connection_aliases(
         self,
         *,
         AliasIds: Sequence[str] = ...,
         ResourceId: str = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeConnectionAliasesResultTypeDef:
         """
         Retrieves a list that describes the connection aliases used for cross-Region
         redirection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.describe_connection_aliases)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#describe_connection_aliases)
@@ -619,15 +619,15 @@
 
     async def describe_workspace_images(
         self,
         *,
         ImageIds: Sequence[str] = ...,
         ImageType: ImageTypeType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeWorkspaceImagesResultTypeDef:
         """
         Retrieves a list that describes one or more specified images, if the image
         identifiers are
         provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.describe_workspace_images)
@@ -648,15 +648,15 @@
         self,
         *,
         WorkspaceIds: Sequence[str] = ...,
         DirectoryId: str = ...,
         UserName: str = ...,
         BundleId: str = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeWorkspacesResultTypeDef:
         """
         Describes the specified WorkSpaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.describe_workspaces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#describe_workspaces)
         """
@@ -719,15 +719,15 @@
         *,
         ResourceId: str,
         DeviceTypeWindows: DefaultImportClientBrandingAttributesTypeDef = ...,
         DeviceTypeOsx: DefaultImportClientBrandingAttributesTypeDef = ...,
         DeviceTypeAndroid: DefaultImportClientBrandingAttributesTypeDef = ...,
         DeviceTypeIos: IosImportClientBrandingAttributesTypeDef = ...,
         DeviceTypeLinux: DefaultImportClientBrandingAttributesTypeDef = ...,
-        DeviceTypeWeb: DefaultImportClientBrandingAttributesTypeDef = ...
+        DeviceTypeWeb: DefaultImportClientBrandingAttributesTypeDef = ...,
     ) -> ImportClientBrandingResultTypeDef:
         """
         Imports client branding.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.import_client_branding)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#import_client_branding)
         """
@@ -736,15 +736,15 @@
         self,
         *,
         Ec2ImageId: str,
         IngestionProcess: WorkspaceImageIngestionProcessType,
         ImageName: str,
         ImageDescription: str,
         Tags: Sequence[TagTypeDef] = ...,
-        Applications: Sequence[ApplicationType] = ...
+        Applications: Sequence[ApplicationType] = ...,
     ) -> ImportWorkspaceImageResultTypeDef:
         """
         Imports the specified Windows 10 or 11 Bring Your Own License (BYOL) image into
         Amazon
         WorkSpaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.import_workspace_image)
@@ -776,15 +776,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#migrate_workspace)
         """
 
     async def modify_account(
         self,
         *,
         DedicatedTenancySupport: Literal["ENABLED"] = ...,
-        DedicatedTenancyManagementCidrRange: str = ...
+        DedicatedTenancyManagementCidrRange: str = ...,
     ) -> Dict[str, Any]:
         """
         Modifies the configuration of Bring Your Own License (BYOL) for the specified
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.modify_account)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#modify_account)
@@ -793,15 +793,15 @@
     async def modify_certificate_based_auth_properties(
         self,
         *,
         ResourceId: str,
         CertificateBasedAuthProperties: CertificateBasedAuthPropertiesTypeDef = ...,
         PropertiesToDelete: Sequence[
             Literal["CERTIFICATE_BASED_AUTH_PROPERTIES_CERTIFICATE_AUTHORITY_ARN"]
-        ] = ...
+        ] = ...,
     ) -> Dict[str, Any]:
         """
         Modifies the properties of the certificate-based authentication you want to use
         with your
         WorkSpaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.modify_certificate_based_auth_properties)
@@ -819,15 +819,15 @@
         """
 
     async def modify_saml_properties(
         self,
         *,
         ResourceId: str,
         SamlProperties: SamlPropertiesTypeDef = ...,
-        PropertiesToDelete: Sequence[DeletableSamlPropertyType] = ...
+        PropertiesToDelete: Sequence[DeletableSamlPropertyType] = ...,
     ) -> Dict[str, Any]:
         """
         Modifies multiple properties related to SAML 2.0 authentication, including the
         enablement status, user access URL, and relay state parameter name that are
         used for configuring federation with an SAML 2.0 identity
         provider.
 
@@ -867,15 +867,15 @@
         """
 
     async def modify_workspace_properties(
         self,
         *,
         WorkspaceId: str,
         WorkspaceProperties: WorkspacePropertiesTypeDef = ...,
-        DataReplication: DataReplicationType = ...
+        DataReplication: DataReplicationType = ...,
     ) -> Dict[str, Any]:
         """
         Modifies the specified WorkSpace properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.modify_workspace_properties)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#modify_workspace_properties)
         """
@@ -914,15 +914,15 @@
         self,
         *,
         DirectoryId: str,
         EnableWorkDocs: bool,
         SubnetIds: Sequence[str] = ...,
         EnableSelfService: bool = ...,
         Tenancy: TenancyType = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Registers the specified directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.register_workspace_directory)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#register_workspace_directory)
         """
```

### Comparing `types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces/literals.py` & `types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces/literals.py`

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
     "AccessPropertyValueType",
     "ApplicationAssociatedResourceTypeType",
     "ApplicationType",
     "AssociationErrorCodeType",
     "AssociationStateType",
     "AssociationStatusType",
@@ -76,15 +75,14 @@
     "WorkSpacesServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AccessPropertyValueType = Literal["ALLOW", "DENY"]
 ApplicationAssociatedResourceTypeType = Literal["BUNDLE", "IMAGE", "WORKSPACE"]
 ApplicationType = Literal["Microsoft_Office_2016", "Microsoft_Office_2019"]
 AssociationErrorCodeType = Literal[
     "DeploymentError.InternalServerError",
     "DeploymentError.WorkspaceUnreachable",
     "ValidationError.InsufficientDiskSpace",
```

### Comparing `types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces/literals.pyi` & `types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces/paginator.py` & `types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,14 @@
     "DescribeWorkspaceDirectoriesPaginator",
     "DescribeWorkspaceImagesPaginator",
     "DescribeWorkspacesPaginator",
     "DescribeWorkspacesConnectionStatusPaginator",
     "ListAvailableManagementCidrRangesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -112,15 +111,15 @@
     """
 
     def paginate(
         self,
         *,
         BundleIds: Sequence[str] = ...,
         Owner: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeWorkspaceBundlesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspaceBundles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/paginators/#describeworkspacebundlespaginator)
         """
 
 
@@ -131,15 +130,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryIds: Sequence[str] = ...,
         Limit: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeWorkspaceDirectoriesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspaceDirectories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/paginators/#describeworkspacedirectoriespaginator)
         """
 
 
@@ -150,15 +149,15 @@
     """
 
     def paginate(
         self,
         *,
         ImageIds: Sequence[str] = ...,
         ImageType: ImageTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeWorkspaceImagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspaceImages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/paginators/#describeworkspaceimagespaginator)
         """
 
 
@@ -171,15 +170,15 @@
     def paginate(
         self,
         *,
         WorkspaceIds: Sequence[str] = ...,
         DirectoryId: str = ...,
         UserName: str = ...,
         BundleId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeWorkspacesResultPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspaces.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/paginators/#describeworkspacespaginator)
         """
```

### Comparing `types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces/paginator.pyi` & `types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     """
 
     def paginate(
         self,
         *,
         BundleIds: Sequence[str] = ...,
         Owner: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeWorkspaceBundlesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspaceBundles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/paginators/#describeworkspacebundlespaginator)
         """
 
 class DescribeWorkspaceDirectoriesPaginator(AioPaginator):
@@ -125,15 +125,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryIds: Sequence[str] = ...,
         Limit: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeWorkspaceDirectoriesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspaceDirectories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/paginators/#describeworkspacedirectoriespaginator)
         """
 
 class DescribeWorkspaceImagesPaginator(AioPaginator):
@@ -143,15 +143,15 @@
     """
 
     def paginate(
         self,
         *,
         ImageIds: Sequence[str] = ...,
         ImageType: ImageTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeWorkspaceImagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspaceImages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/paginators/#describeworkspaceimagespaginator)
         """
 
 class DescribeWorkspacesPaginator(AioPaginator):
@@ -163,15 +163,15 @@
     def paginate(
         self,
         *,
         WorkspaceIds: Sequence[str] = ...,
         DirectoryId: str = ...,
         UserName: str = ...,
         BundleId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeWorkspacesResultPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspaces.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/paginators/#describeworkspacespaginator)
         """
 
 class DescribeWorkspacesConnectionStatusPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces/type_defs.py` & `types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountModificationTypeDef",
     "AssociationStateReasonTypeDef",
     "AssociateConnectionAliasRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociateIpGroupsRequestRequestTypeDef",
     "AssociateWorkspaceApplicationRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces/type_defs.pyi` & `types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces.egg-info/PKG-INFO` & `types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-workspaces
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.WorkSpaces 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.WorkSpaces 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/
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
 
 <a id="types-aiobotocore-workspaces"></a>
 
 # types-aiobotocore-workspaces
 
 [![PyPI - types-aiobotocore-workspaces](https://img.shields.io/pypi/v/types-aiobotocore-workspaces.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workspaces)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-workspaces.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workspaces)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-workspaces)](https://pepy.tech/project/types-aiobotocore-workspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WorkSpaces 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
+[aiobotocore.WorkSpaces 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
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
 [types-aiobotocore-workspaces docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-workspaces-2.9.0/types_aiobotocore_workspaces.egg-info/SOURCES.txt` & `types-aiobotocore-workspaces-2.9.1/types_aiobotocore_workspaces.egg-info/SOURCES.txt`

 * *Files identical despite different names*

