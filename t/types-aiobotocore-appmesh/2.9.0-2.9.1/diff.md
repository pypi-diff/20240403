# Comparing `tmp/types-aiobotocore-appmesh-2.9.0.tar.gz` & `tmp/types-aiobotocore-appmesh-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-appmesh-2.9.0.tar", last modified: Wed Dec 13 19:58:36 2023, max compression
+gzip compressed data, was "types-aiobotocore-appmesh-2.9.1.tar", last modified: Thu Jan 18 01:20:04 2024, max compression
```

## Comparing `types-aiobotocore-appmesh-2.9.0.tar` & `types-aiobotocore-appmesh-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:36.078083 types-aiobotocore-appmesh-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:41:09.000000 types-aiobotocore-appmesh-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14045 2023-12-13 19:58:36.078083 types-aiobotocore-appmesh-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12482 2023-12-13 19:41:09.000000 types-aiobotocore-appmesh-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:36.078083 types-aiobotocore-appmesh-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2023-12-13 19:41:09.000000 types-aiobotocore-appmesh-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:36.078083 types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh/
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2023-12-13 19:41:09.000000 types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-12-13 19:41:09.000000 types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      932 2023-12-13 19:41:09.000000 types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32312 2023-12-13 19:41:10.000000 types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    32308 2023-12-13 19:41:10.000000 types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11628 2023-12-13 19:41:10.000000 types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11626 2023-12-13 19:41:10.000000 types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9948 2023-12-13 19:41:10.000000 types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9938 2023-12-13 19:41:10.000000 types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:41:09.000000 types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    59831 2023-12-13 19:41:11.000000 types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    59830 2023-12-13 19:41:10.000000 types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:41:09.000000 types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:36.078083 types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14045 2023-12-13 19:58:36.000000 types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-12-13 19:58:36.000000 types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:36.000000 types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:36.000000 types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:36.000000 types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-13 19:58:36.000000 types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:04.061510 types-aiobotocore-appmesh-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:03:08.000000 types-aiobotocore-appmesh-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14065 2024-01-18 01:20:04.061510 types-aiobotocore-appmesh-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12482 2024-01-18 01:03:08.000000 types-aiobotocore-appmesh-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:04.061510 types-aiobotocore-appmesh-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-01-18 01:03:08.000000 types-aiobotocore-appmesh-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:04.061510 types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh/
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-01-18 01:03:08.000000 types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-01-18 01:03:08.000000 types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-01-18 01:03:08.000000 types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32326 2024-01-18 01:03:08.000000 types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32323 2024-01-18 01:03:08.000000 types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11626 2024-01-18 01:03:09.000000 types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11626 2024-01-18 01:03:09.000000 types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9949 2024-01-18 01:03:08.000000 types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9940 2024-01-18 01:03:08.000000 types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:03:08.000000 types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    59830 2024-01-18 01:03:10.000000 types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59830 2024-01-18 01:03:10.000000 types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:03:08.000000 types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:04.061510 types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14065 2024-01-18 01:20:04.000000 types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-01-18 01:20:04.000000 types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:04.000000 types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:04.000000 types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:04.000000 types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-18 01:20:04.000000 types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-appmesh-2.9.0/LICENSE` & `types-aiobotocore-appmesh-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-appmesh-2.9.0/PKG-INFO` & `types-aiobotocore-appmesh-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appmesh
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AppMesh 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AppMesh 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/
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
 
 <a id="types-aiobotocore-appmesh"></a>
 
 # types-aiobotocore-appmesh
 
 [![PyPI - types-aiobotocore-appmesh](https://img.shields.io/pypi/v/types-aiobotocore-appmesh.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appmesh)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appmesh.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appmesh)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appmesh)](https://pepy.tech/project/types-aiobotocore-appmesh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppMesh 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
+[aiobotocore.AppMesh 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
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
 [types-aiobotocore-appmesh docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-appmesh-2.9.0/README.md` & `types-aiobotocore-appmesh-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appmesh.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appmesh)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appmesh)](https://pepy.tech/project/types-aiobotocore-appmesh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppMesh 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
+[aiobotocore.AppMesh 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
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
 [types-aiobotocore-appmesh docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-appmesh-2.9.0/setup.py` & `types-aiobotocore-appmesh-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-appmesh",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_appmesh"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.AppMesh 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.AppMesh 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore appmesh type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_appmesh": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh/__init__.py` & `types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     ListVirtualNodesPaginator,
     ListVirtualRoutersPaginator,
     ListVirtualServicesPaginator,
 )
 
 Client = AppMeshClient
 
-
 __all__ = (
     "AppMeshClient",
     "Client",
     "ListGatewayRoutesPaginator",
     "ListMeshesPaginator",
     "ListRoutesPaginator",
     "ListTagsForResourcePaginator",
```

### Comparing `types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh/__init__.pyi` & `types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh/__main__.py` & `types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AppMesh 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.AppMesh 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh\nOther"
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

### Comparing `types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh/client.py` & `types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("AppMeshClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -147,30 +146,30 @@
         *,
         gatewayRouteName: str,
         meshName: str,
         spec: GatewayRouteSpecTypeDef,
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
-        tags: Sequence[TagRefTypeDef] = ...
+        tags: Sequence[TagRefTypeDef] = ...,
     ) -> CreateGatewayRouteOutputTypeDef:
         """
         Creates a gateway route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_gateway_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_gateway_route)
         """
 
     async def create_mesh(
         self,
         *,
         meshName: str,
         clientToken: str = ...,
         spec: MeshSpecTypeDef = ...,
-        tags: Sequence[TagRefTypeDef] = ...
+        tags: Sequence[TagRefTypeDef] = ...,
     ) -> CreateMeshOutputTypeDef:
         """
         Creates a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_mesh)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_mesh)
         """
@@ -180,15 +179,15 @@
         *,
         meshName: str,
         routeName: str,
         spec: RouteSpecTypeDef,
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
-        tags: Sequence[TagRefTypeDef] = ...
+        tags: Sequence[TagRefTypeDef] = ...,
     ) -> CreateRouteOutputTypeDef:
         """
         Creates a route that is associated with a virtual router.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_route)
         """
@@ -197,15 +196,15 @@
         self,
         *,
         meshName: str,
         spec: VirtualGatewaySpecTypeDef,
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
-        tags: Sequence[TagRefTypeDef] = ...
+        tags: Sequence[TagRefTypeDef] = ...,
     ) -> CreateVirtualGatewayOutputTypeDef:
         """
         Creates a virtual gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_virtual_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_virtual_gateway)
         """
@@ -214,15 +213,15 @@
         self,
         *,
         meshName: str,
         spec: VirtualNodeSpecTypeDef,
         virtualNodeName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
-        tags: Sequence[TagRefTypeDef] = ...
+        tags: Sequence[TagRefTypeDef] = ...,
     ) -> CreateVirtualNodeOutputTypeDef:
         """
         Creates a virtual node within a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_virtual_node)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_virtual_node)
         """
@@ -231,15 +230,15 @@
         self,
         *,
         meshName: str,
         spec: VirtualRouterSpecTypeDef,
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
-        tags: Sequence[TagRefTypeDef] = ...
+        tags: Sequence[TagRefTypeDef] = ...,
     ) -> CreateVirtualRouterOutputTypeDef:
         """
         Creates a virtual router within a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_virtual_router)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_virtual_router)
         """
@@ -248,15 +247,15 @@
         self,
         *,
         meshName: str,
         spec: VirtualServiceSpecTypeDef,
         virtualServiceName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
-        tags: Sequence[TagRefTypeDef] = ...
+        tags: Sequence[TagRefTypeDef] = ...,
     ) -> CreateVirtualServiceOutputTypeDef:
         """
         Creates a virtual service within a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_virtual_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_virtual_service)
         """
@@ -416,15 +415,15 @@
     async def list_gateway_routes(
         self,
         *,
         meshName: str,
         virtualGatewayName: str,
         limit: int = ...,
         meshOwner: str = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListGatewayRoutesOutputTypeDef:
         """
         Returns a list of existing gateway routes that are associated to a virtual
         gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_gateway_routes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#list_gateway_routes)
@@ -443,15 +442,15 @@
     async def list_routes(
         self,
         *,
         meshName: str,
         virtualRouterName: str,
         limit: int = ...,
         meshOwner: str = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListRoutesOutputTypeDef:
         """
         Returns a list of existing routes in a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_routes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#list_routes)
         """
@@ -528,15 +527,15 @@
         self,
         *,
         gatewayRouteName: str,
         meshName: str,
         spec: GatewayRouteSpecTypeDef,
         virtualGatewayName: str,
         clientToken: str = ...,
-        meshOwner: str = ...
+        meshOwner: str = ...,
     ) -> UpdateGatewayRouteOutputTypeDef:
         """
         Updates an existing gateway route that is associated to a specified virtual
         gateway in a service
         mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_gateway_route)
@@ -557,15 +556,15 @@
         self,
         *,
         meshName: str,
         routeName: str,
         spec: RouteSpecTypeDef,
         virtualRouterName: str,
         clientToken: str = ...,
-        meshOwner: str = ...
+        meshOwner: str = ...,
     ) -> UpdateRouteOutputTypeDef:
         """
         Updates an existing route for a specified service mesh and virtual router.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#update_route)
         """
@@ -573,15 +572,15 @@
     async def update_virtual_gateway(
         self,
         *,
         meshName: str,
         spec: VirtualGatewaySpecTypeDef,
         virtualGatewayName: str,
         clientToken: str = ...,
-        meshOwner: str = ...
+        meshOwner: str = ...,
     ) -> UpdateVirtualGatewayOutputTypeDef:
         """
         Updates an existing virtual gateway in a specified service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_virtual_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#update_virtual_gateway)
         """
@@ -589,15 +588,15 @@
     async def update_virtual_node(
         self,
         *,
         meshName: str,
         spec: VirtualNodeSpecTypeDef,
         virtualNodeName: str,
         clientToken: str = ...,
-        meshOwner: str = ...
+        meshOwner: str = ...,
     ) -> UpdateVirtualNodeOutputTypeDef:
         """
         Updates an existing virtual node in a specified service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_virtual_node)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#update_virtual_node)
         """
@@ -605,15 +604,15 @@
     async def update_virtual_router(
         self,
         *,
         meshName: str,
         spec: VirtualRouterSpecTypeDef,
         virtualRouterName: str,
         clientToken: str = ...,
-        meshOwner: str = ...
+        meshOwner: str = ...,
     ) -> UpdateVirtualRouterOutputTypeDef:
         """
         Updates an existing virtual router in a specified service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_virtual_router)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#update_virtual_router)
         """
@@ -621,15 +620,15 @@
     async def update_virtual_service(
         self,
         *,
         meshName: str,
         spec: VirtualServiceSpecTypeDef,
         virtualServiceName: str,
         clientToken: str = ...,
-        meshOwner: str = ...
+        meshOwner: str = ...,
     ) -> UpdateVirtualServiceOutputTypeDef:
         """
         Updates an existing virtual service in a specified service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_virtual_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#update_virtual_service)
         """
```

### Comparing `types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh/client.pyi` & `types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -143,30 +143,30 @@
         *,
         gatewayRouteName: str,
         meshName: str,
         spec: GatewayRouteSpecTypeDef,
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
-        tags: Sequence[TagRefTypeDef] = ...
+        tags: Sequence[TagRefTypeDef] = ...,
     ) -> CreateGatewayRouteOutputTypeDef:
         """
         Creates a gateway route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_gateway_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_gateway_route)
         """
 
     async def create_mesh(
         self,
         *,
         meshName: str,
         clientToken: str = ...,
         spec: MeshSpecTypeDef = ...,
-        tags: Sequence[TagRefTypeDef] = ...
+        tags: Sequence[TagRefTypeDef] = ...,
     ) -> CreateMeshOutputTypeDef:
         """
         Creates a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_mesh)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_mesh)
         """
@@ -176,15 +176,15 @@
         *,
         meshName: str,
         routeName: str,
         spec: RouteSpecTypeDef,
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
-        tags: Sequence[TagRefTypeDef] = ...
+        tags: Sequence[TagRefTypeDef] = ...,
     ) -> CreateRouteOutputTypeDef:
         """
         Creates a route that is associated with a virtual router.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_route)
         """
@@ -193,15 +193,15 @@
         self,
         *,
         meshName: str,
         spec: VirtualGatewaySpecTypeDef,
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
-        tags: Sequence[TagRefTypeDef] = ...
+        tags: Sequence[TagRefTypeDef] = ...,
     ) -> CreateVirtualGatewayOutputTypeDef:
         """
         Creates a virtual gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_virtual_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_virtual_gateway)
         """
@@ -210,15 +210,15 @@
         self,
         *,
         meshName: str,
         spec: VirtualNodeSpecTypeDef,
         virtualNodeName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
-        tags: Sequence[TagRefTypeDef] = ...
+        tags: Sequence[TagRefTypeDef] = ...,
     ) -> CreateVirtualNodeOutputTypeDef:
         """
         Creates a virtual node within a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_virtual_node)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_virtual_node)
         """
@@ -227,15 +227,15 @@
         self,
         *,
         meshName: str,
         spec: VirtualRouterSpecTypeDef,
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
-        tags: Sequence[TagRefTypeDef] = ...
+        tags: Sequence[TagRefTypeDef] = ...,
     ) -> CreateVirtualRouterOutputTypeDef:
         """
         Creates a virtual router within a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_virtual_router)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_virtual_router)
         """
@@ -244,15 +244,15 @@
         self,
         *,
         meshName: str,
         spec: VirtualServiceSpecTypeDef,
         virtualServiceName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
-        tags: Sequence[TagRefTypeDef] = ...
+        tags: Sequence[TagRefTypeDef] = ...,
     ) -> CreateVirtualServiceOutputTypeDef:
         """
         Creates a virtual service within a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_virtual_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_virtual_service)
         """
@@ -412,15 +412,15 @@
     async def list_gateway_routes(
         self,
         *,
         meshName: str,
         virtualGatewayName: str,
         limit: int = ...,
         meshOwner: str = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListGatewayRoutesOutputTypeDef:
         """
         Returns a list of existing gateway routes that are associated to a virtual
         gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_gateway_routes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#list_gateway_routes)
@@ -439,15 +439,15 @@
     async def list_routes(
         self,
         *,
         meshName: str,
         virtualRouterName: str,
         limit: int = ...,
         meshOwner: str = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListRoutesOutputTypeDef:
         """
         Returns a list of existing routes in a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_routes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#list_routes)
         """
@@ -524,15 +524,15 @@
         self,
         *,
         gatewayRouteName: str,
         meshName: str,
         spec: GatewayRouteSpecTypeDef,
         virtualGatewayName: str,
         clientToken: str = ...,
-        meshOwner: str = ...
+        meshOwner: str = ...,
     ) -> UpdateGatewayRouteOutputTypeDef:
         """
         Updates an existing gateway route that is associated to a specified virtual
         gateway in a service
         mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_gateway_route)
@@ -553,15 +553,15 @@
         self,
         *,
         meshName: str,
         routeName: str,
         spec: RouteSpecTypeDef,
         virtualRouterName: str,
         clientToken: str = ...,
-        meshOwner: str = ...
+        meshOwner: str = ...,
     ) -> UpdateRouteOutputTypeDef:
         """
         Updates an existing route for a specified service mesh and virtual router.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#update_route)
         """
@@ -569,15 +569,15 @@
     async def update_virtual_gateway(
         self,
         *,
         meshName: str,
         spec: VirtualGatewaySpecTypeDef,
         virtualGatewayName: str,
         clientToken: str = ...,
-        meshOwner: str = ...
+        meshOwner: str = ...,
     ) -> UpdateVirtualGatewayOutputTypeDef:
         """
         Updates an existing virtual gateway in a specified service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_virtual_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#update_virtual_gateway)
         """
@@ -585,15 +585,15 @@
     async def update_virtual_node(
         self,
         *,
         meshName: str,
         spec: VirtualNodeSpecTypeDef,
         virtualNodeName: str,
         clientToken: str = ...,
-        meshOwner: str = ...
+        meshOwner: str = ...,
     ) -> UpdateVirtualNodeOutputTypeDef:
         """
         Updates an existing virtual node in a specified service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_virtual_node)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#update_virtual_node)
         """
@@ -601,15 +601,15 @@
     async def update_virtual_router(
         self,
         *,
         meshName: str,
         spec: VirtualRouterSpecTypeDef,
         virtualRouterName: str,
         clientToken: str = ...,
-        meshOwner: str = ...
+        meshOwner: str = ...,
     ) -> UpdateVirtualRouterOutputTypeDef:
         """
         Updates an existing virtual router in a specified service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_virtual_router)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#update_virtual_router)
         """
@@ -617,15 +617,15 @@
     async def update_virtual_service(
         self,
         *,
         meshName: str,
         spec: VirtualServiceSpecTypeDef,
         virtualServiceName: str,
         clientToken: str = ...,
-        meshOwner: str = ...
+        meshOwner: str = ...,
     ) -> UpdateVirtualServiceOutputTypeDef:
         """
         Updates an existing virtual service in a specified service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_virtual_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#update_virtual_service)
         """
```

### Comparing `types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh/literals.py` & `types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh/literals.py`

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
     "DefaultGatewayRouteRewriteType",
     "DnsResponseTypeType",
     "DurationUnitType",
     "EgressFilterTypeType",
     "GatewayRouteStatusCodeType",
     "GrpcRetryPolicyEventType",
@@ -52,15 +51,14 @@
     "AppMeshServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DefaultGatewayRouteRewriteType = Literal["DISABLED", "ENABLED"]
 DnsResponseTypeType = Literal["ENDPOINTS", "LOADBALANCER"]
 DurationUnitType = Literal["ms", "s"]
 EgressFilterTypeType = Literal["ALLOW_ALL", "DROP_ALL"]
 GatewayRouteStatusCodeType = Literal["ACTIVE", "DELETED", "INACTIVE"]
 GrpcRetryPolicyEventType = Literal[
     "cancelled", "deadline-exceeded", "internal", "resource-exhausted", "unavailable"
```

### Comparing `types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh/literals.pyi` & `types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh/paginator.py` & `types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,14 @@
     "ListTagsForResourcePaginator",
     "ListVirtualGatewaysPaginator",
     "ListVirtualNodesPaginator",
     "ListVirtualRoutersPaginator",
     "ListVirtualServicesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -82,15 +81,15 @@
 
     def paginate(
         self,
         *,
         meshName: str,
         virtualGatewayName: str,
         meshOwner: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListGatewayRoutesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListGatewayRoutes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/paginators/#listgatewayroutespaginator)
         """
 
 
@@ -117,15 +116,15 @@
 
     def paginate(
         self,
         *,
         meshName: str,
         virtualRouterName: str,
         meshOwner: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRoutesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListRoutes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/paginators/#listroutespaginator)
         """
```

### Comparing `types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh/paginator.pyi` & `types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
     def paginate(
         self,
         *,
         meshName: str,
         virtualGatewayName: str,
         meshOwner: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListGatewayRoutesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListGatewayRoutes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/paginators/#listgatewayroutespaginator)
         """
 
 class ListMeshesPaginator(AioPaginator):
@@ -112,15 +112,15 @@
 
     def paginate(
         self,
         *,
         meshName: str,
         virtualRouterName: str,
         meshOwner: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRoutesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListRoutes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/paginators/#listroutespaginator)
         """
 
 class ListTagsForResourcePaginator(AioPaginator):
```

### Comparing `types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh/type_defs.py` & `types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh/type_defs.py`

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
     "AwsCloudMapInstanceAttributeTypeDef",
     "ListenerTlsFileCertificateTypeDef",
     "ListenerTlsSdsCertificateTypeDef",
     "TagRefTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteGatewayRouteInputRequestTypeDef",
```

### Comparing `types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh/type_defs.pyi` & `types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh.egg-info/PKG-INFO` & `types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appmesh
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AppMesh 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AppMesh 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/
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
 
 <a id="types-aiobotocore-appmesh"></a>
 
 # types-aiobotocore-appmesh
 
 [![PyPI - types-aiobotocore-appmesh](https://img.shields.io/pypi/v/types-aiobotocore-appmesh.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appmesh)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appmesh.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appmesh)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appmesh)](https://pepy.tech/project/types-aiobotocore-appmesh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppMesh 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
+[aiobotocore.AppMesh 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
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
 [types-aiobotocore-appmesh docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-appmesh-2.9.0/types_aiobotocore_appmesh.egg-info/SOURCES.txt` & `types-aiobotocore-appmesh-2.9.1/types_aiobotocore_appmesh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

