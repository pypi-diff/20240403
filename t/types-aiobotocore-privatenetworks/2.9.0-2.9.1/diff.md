# Comparing `tmp/types-aiobotocore-privatenetworks-2.9.0.tar.gz` & `tmp/types-aiobotocore-privatenetworks-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-privatenetworks-2.9.0.tar", last modified: Wed Dec 13 20:00:11 2023, max compression
+gzip compressed data, was "types-aiobotocore-privatenetworks-2.9.1.tar", last modified: Thu Jan 18 01:21:31 2024, max compression
```

## Comparing `types-aiobotocore-privatenetworks-2.9.0.tar` & `types-aiobotocore-privatenetworks-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:11.609301 types-aiobotocore-privatenetworks-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:51:56.000000 types-aiobotocore-privatenetworks-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14001 2023-12-13 20:00:11.609301 types-aiobotocore-privatenetworks-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12412 2023-12-13 19:51:56.000000 types-aiobotocore-privatenetworks-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:11.609301 types-aiobotocore-privatenetworks-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2023-12-13 19:51:56.000000 types-aiobotocore-privatenetworks-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:11.609301 types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks/
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2023-12-13 19:51:56.000000 types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2023-12-13 19:51:56.000000 types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      952 2023-12-13 19:51:56.000000 types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23106 2023-12-13 19:51:56.000000 types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    23102 2023-12-13 19:51:56.000000 types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10561 2023-12-13 19:51:56.000000 types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10559 2023-12-13 19:51:56.000000 types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7371 2023-12-13 19:51:56.000000 types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7363 2023-12-13 19:51:56.000000 types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:51:56.000000 types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    21916 2023-12-13 19:51:57.000000 types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21915 2023-12-13 19:51:56.000000 types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:51:56.000000 types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:11.609301 types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14001 2023-12-13 20:00:11.000000 types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      965 2023-12-13 20:00:11.000000 types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:11.000000 types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:11.000000 types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:11.000000 types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-13 20:00:11.000000 types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:31.733110 types-aiobotocore-privatenetworks-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:13:33.000000 types-aiobotocore-privatenetworks-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14021 2024-01-18 01:21:31.733110 types-aiobotocore-privatenetworks-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12412 2024-01-18 01:13:33.000000 types-aiobotocore-privatenetworks-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:31.733110 types-aiobotocore-privatenetworks-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-01-18 01:13:33.000000 types-aiobotocore-privatenetworks-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:31.733110 types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-01-18 01:13:33.000000 types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-01-18 01:13:33.000000 types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-01-18 01:13:33.000000 types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23115 2024-01-18 01:13:33.000000 types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23112 2024-01-18 01:13:33.000000 types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10559 2024-01-18 01:13:33.000000 types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10559 2024-01-18 01:13:33.000000 types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-01-18 01:13:33.000000 types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-01-18 01:13:33.000000 types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:13:33.000000 types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    21915 2024-01-18 01:13:33.000000 types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21915 2024-01-18 01:13:33.000000 types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:13:33.000000 types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:31.733110 types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14021 2024-01-18 01:21:31.000000 types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-01-18 01:21:31.000000 types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:31.000000 types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:31.000000 types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:31.000000 types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-01-18 01:21:31.000000 types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-privatenetworks-2.9.0/LICENSE` & `types-aiobotocore-privatenetworks-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-privatenetworks-2.9.0/PKG-INFO` & `types-aiobotocore-privatenetworks-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-privatenetworks
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Private5G 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Private5G 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/
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
 
 <a id="types-aiobotocore-privatenetworks"></a>
 
 # types-aiobotocore-privatenetworks
 
 [![PyPI - types-aiobotocore-privatenetworks](https://img.shields.io/pypi/v/types-aiobotocore-privatenetworks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-privatenetworks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-privatenetworks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-privatenetworks)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-privatenetworks)](https://pepy.tech/project/types-aiobotocore-privatenetworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Private5G 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
+[aiobotocore.Private5G 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
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
 [types-aiobotocore-privatenetworks docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-privatenetworks-2.9.0/README.md` & `types-aiobotocore-privatenetworks-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-privatenetworks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-privatenetworks)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-privatenetworks)](https://pepy.tech/project/types-aiobotocore-privatenetworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Private5G 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
+[aiobotocore.Private5G 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
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
 [types-aiobotocore-privatenetworks docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-privatenetworks-2.9.0/setup.py` & `types-aiobotocore-privatenetworks-2.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-privatenetworks",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_privatenetworks"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Private5G 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Private5G 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore privatenetworks type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_privatenetworks": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks/__init__.py` & `types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     ListNetworkSitesPaginator,
     ListNetworksPaginator,
     ListOrdersPaginator,
 )
 
 Client = Private5GClient
 
-
 __all__ = (
     "Client",
     "ListDeviceIdentifiersPaginator",
     "ListNetworkResourcesPaginator",
     "ListNetworkSitesPaginator",
     "ListNetworksPaginator",
     "ListOrdersPaginator",
```

### Comparing `types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks/__init__.pyi` & `types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks/__main__.py` & `types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Private5G 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Private5G 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G\nOther"
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

### Comparing `types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks/client.py` & `types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("Private5GClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -130,15 +129,15 @@
 
     async def activate_network_site(
         self,
         *,
         networkSiteArn: str,
         shippingAddress: AddressTypeDef,
         clientToken: str = ...,
-        commitmentConfiguration: CommitmentConfigurationTypeDef = ...
+        commitmentConfiguration: CommitmentConfigurationTypeDef = ...,
     ) -> ActivateNetworkSiteResponseTypeDef:
         """
         Activates the specified network site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.activate_network_site)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#activate_network_site)
         """
@@ -163,30 +162,30 @@
         self,
         *,
         accessPointArn: str,
         cpiSecretKey: str = ...,
         cpiUserId: str = ...,
         cpiUserPassword: str = ...,
         cpiUsername: str = ...,
-        position: PositionTypeDef = ...
+        position: PositionTypeDef = ...,
     ) -> ConfigureAccessPointResponseTypeDef:
         """
         Configures the specified network resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.configure_access_point)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#configure_access_point)
         """
 
     async def create_network(
         self,
         *,
         networkName: str,
         clientToken: str = ...,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateNetworkResponseTypeDef:
         """
         Creates a network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.create_network)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#create_network)
         """
@@ -197,15 +196,15 @@
         networkArn: str,
         networkSiteName: str,
         availabilityZone: str = ...,
         availabilityZoneId: str = ...,
         clientToken: str = ...,
         description: str = ...,
         pendingPlan: SitePlanTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateNetworkSiteResponseTypeDef:
         """
         Creates a network site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.create_network_site)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#create_network_site)
         """
@@ -300,74 +299,74 @@
 
     async def list_device_identifiers(
         self,
         *,
         networkArn: str,
         filters: Mapping[DeviceIdentifierFilterKeysType, Sequence[str]] = ...,
         maxResults: int = ...,
-        startToken: str = ...
+        startToken: str = ...,
     ) -> ListDeviceIdentifiersResponseTypeDef:
         """
         Lists device identifiers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_device_identifiers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#list_device_identifiers)
         """
 
     async def list_network_resources(
         self,
         *,
         networkArn: str,
         filters: Mapping[NetworkResourceFilterKeysType, Sequence[str]] = ...,
         maxResults: int = ...,
-        startToken: str = ...
+        startToken: str = ...,
     ) -> ListNetworkResourcesResponseTypeDef:
         """
         Lists network resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_network_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#list_network_resources)
         """
 
     async def list_network_sites(
         self,
         *,
         networkArn: str,
         filters: Mapping[Literal["STATUS"], Sequence[str]] = ...,
         maxResults: int = ...,
-        startToken: str = ...
+        startToken: str = ...,
     ) -> ListNetworkSitesResponseTypeDef:
         """
         Lists network sites.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_network_sites)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#list_network_sites)
         """
 
     async def list_networks(
         self,
         *,
         filters: Mapping[Literal["STATUS"], Sequence[str]] = ...,
         maxResults: int = ...,
-        startToken: str = ...
+        startToken: str = ...,
     ) -> ListNetworksResponseTypeDef:
         """
         Lists networks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_networks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#list_networks)
         """
 
     async def list_orders(
         self,
         *,
         networkArn: str,
         filters: Mapping[OrderFilterKeysType, Sequence[str]] = ...,
         maxResults: int = ...,
-        startToken: str = ...
+        startToken: str = ...,
     ) -> ListOrdersResponseTypeDef:
         """
         Lists orders.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_orders)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#list_orders)
         """
@@ -393,15 +392,15 @@
     async def start_network_resource_update(
         self,
         *,
         networkResourceArn: str,
         updateType: UpdateTypeType,
         commitmentConfiguration: CommitmentConfigurationTypeDef = ...,
         returnReason: str = ...,
-        shippingAddress: AddressTypeDef = ...
+        shippingAddress: AddressTypeDef = ...,
     ) -> StartNetworkResourceUpdateResponseTypeDef:
         """
         Use this action to do the following tasks: * Update the duration and renewal
         status of the commitment period for a radio
         unit.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.start_network_resource_update)
```

### Comparing `types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks/client.pyi` & `types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 
     async def activate_network_site(
         self,
         *,
         networkSiteArn: str,
         shippingAddress: AddressTypeDef,
         clientToken: str = ...,
-        commitmentConfiguration: CommitmentConfigurationTypeDef = ...
+        commitmentConfiguration: CommitmentConfigurationTypeDef = ...,
     ) -> ActivateNetworkSiteResponseTypeDef:
         """
         Activates the specified network site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.activate_network_site)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#activate_network_site)
         """
@@ -159,30 +159,30 @@
         self,
         *,
         accessPointArn: str,
         cpiSecretKey: str = ...,
         cpiUserId: str = ...,
         cpiUserPassword: str = ...,
         cpiUsername: str = ...,
-        position: PositionTypeDef = ...
+        position: PositionTypeDef = ...,
     ) -> ConfigureAccessPointResponseTypeDef:
         """
         Configures the specified network resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.configure_access_point)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#configure_access_point)
         """
 
     async def create_network(
         self,
         *,
         networkName: str,
         clientToken: str = ...,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateNetworkResponseTypeDef:
         """
         Creates a network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.create_network)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#create_network)
         """
@@ -193,15 +193,15 @@
         networkArn: str,
         networkSiteName: str,
         availabilityZone: str = ...,
         availabilityZoneId: str = ...,
         clientToken: str = ...,
         description: str = ...,
         pendingPlan: SitePlanTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateNetworkSiteResponseTypeDef:
         """
         Creates a network site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.create_network_site)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#create_network_site)
         """
@@ -296,74 +296,74 @@
 
     async def list_device_identifiers(
         self,
         *,
         networkArn: str,
         filters: Mapping[DeviceIdentifierFilterKeysType, Sequence[str]] = ...,
         maxResults: int = ...,
-        startToken: str = ...
+        startToken: str = ...,
     ) -> ListDeviceIdentifiersResponseTypeDef:
         """
         Lists device identifiers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_device_identifiers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#list_device_identifiers)
         """
 
     async def list_network_resources(
         self,
         *,
         networkArn: str,
         filters: Mapping[NetworkResourceFilterKeysType, Sequence[str]] = ...,
         maxResults: int = ...,
-        startToken: str = ...
+        startToken: str = ...,
     ) -> ListNetworkResourcesResponseTypeDef:
         """
         Lists network resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_network_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#list_network_resources)
         """
 
     async def list_network_sites(
         self,
         *,
         networkArn: str,
         filters: Mapping[Literal["STATUS"], Sequence[str]] = ...,
         maxResults: int = ...,
-        startToken: str = ...
+        startToken: str = ...,
     ) -> ListNetworkSitesResponseTypeDef:
         """
         Lists network sites.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_network_sites)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#list_network_sites)
         """
 
     async def list_networks(
         self,
         *,
         filters: Mapping[Literal["STATUS"], Sequence[str]] = ...,
         maxResults: int = ...,
-        startToken: str = ...
+        startToken: str = ...,
     ) -> ListNetworksResponseTypeDef:
         """
         Lists networks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_networks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#list_networks)
         """
 
     async def list_orders(
         self,
         *,
         networkArn: str,
         filters: Mapping[OrderFilterKeysType, Sequence[str]] = ...,
         maxResults: int = ...,
-        startToken: str = ...
+        startToken: str = ...,
     ) -> ListOrdersResponseTypeDef:
         """
         Lists orders.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_orders)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#list_orders)
         """
@@ -389,15 +389,15 @@
     async def start_network_resource_update(
         self,
         *,
         networkResourceArn: str,
         updateType: UpdateTypeType,
         commitmentConfiguration: CommitmentConfigurationTypeDef = ...,
         returnReason: str = ...,
-        shippingAddress: AddressTypeDef = ...
+        shippingAddress: AddressTypeDef = ...,
     ) -> StartNetworkResourceUpdateResponseTypeDef:
         """
         Use this action to do the following tasks: * Update the duration and renewal
         status of the commitment period for a radio
         unit.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.start_network_resource_update)
```

### Comparing `types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks/literals.py` & `types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks/literals.py`

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
     "AcknowledgmentStatusType",
     "CommitmentLengthType",
     "DeviceIdentifierFilterKeysType",
     "DeviceIdentifierStatusType",
     "ElevationReferenceType",
     "ElevationUnitType",
@@ -45,15 +44,14 @@
     "UpdateTypeType",
     "Private5GServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 AcknowledgmentStatusType = Literal["ACKNOWLEDGED", "ACKNOWLEDGING", "UNACKNOWLEDGED"]
 CommitmentLengthType = Literal["ONE_YEAR", "SIXTY_DAYS", "THREE_YEARS"]
 DeviceIdentifierFilterKeysType = Literal["ORDER", "STATUS", "TRAFFIC_GROUP"]
 DeviceIdentifierStatusType = Literal["ACTIVE", "INACTIVE"]
 ElevationReferenceType = Literal["AGL", "AMSL"]
 ElevationUnitType = Literal["FEET"]
 HealthStatusType = Literal["HEALTHY", "INITIAL", "UNHEALTHY"]
```

### Comparing `types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks/literals.pyi` & `types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks/paginator.py` & `types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,24 +50,22 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListDeviceIdentifiersPaginator",
     "ListNetworkResourcesPaginator",
     "ListNetworkSitesPaginator",
     "ListNetworksPaginator",
     "ListOrdersPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -81,15 +79,15 @@
     """
 
     def paginate(
         self,
         *,
         networkArn: str,
         filters: Mapping[DeviceIdentifierFilterKeysType, Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDeviceIdentifiersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Paginator.ListDeviceIdentifiers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/paginators/#listdeviceidentifierspaginator)
         """
 
 
@@ -100,15 +98,15 @@
     """
 
     def paginate(
         self,
         *,
         networkArn: str,
         filters: Mapping[NetworkResourceFilterKeysType, Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListNetworkResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Paginator.ListNetworkResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/paginators/#listnetworkresourcespaginator)
         """
 
 
@@ -119,15 +117,15 @@
     """
 
     def paginate(
         self,
         *,
         networkArn: str,
         filters: Mapping[Literal["STATUS"], Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListNetworkSitesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Paginator.ListNetworkSites.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/paginators/#listnetworksitespaginator)
         """
 
 
@@ -137,15 +135,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/paginators/#listnetworkspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Mapping[Literal["STATUS"], Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListNetworksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Paginator.ListNetworks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/paginators/#listnetworkspaginator)
         """
 
 
@@ -156,13 +154,13 @@
     """
 
     def paginate(
         self,
         *,
         networkArn: str,
         filters: Mapping[OrderFilterKeysType, Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOrdersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Paginator.ListOrders.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/paginators/#listorderspaginator)
         """
```

### Comparing `types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks/paginator.pyi` & `types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     """
 
     def paginate(
         self,
         *,
         networkArn: str,
         filters: Mapping[DeviceIdentifierFilterKeysType, Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDeviceIdentifiersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Paginator.ListDeviceIdentifiers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/paginators/#listdeviceidentifierspaginator)
         """
 
 class ListNetworkResourcesPaginator(AioPaginator):
@@ -95,15 +95,15 @@
     """
 
     def paginate(
         self,
         *,
         networkArn: str,
         filters: Mapping[NetworkResourceFilterKeysType, Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListNetworkResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Paginator.ListNetworkResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/paginators/#listnetworkresourcespaginator)
         """
 
 class ListNetworkSitesPaginator(AioPaginator):
@@ -113,15 +113,15 @@
     """
 
     def paginate(
         self,
         *,
         networkArn: str,
         filters: Mapping[Literal["STATUS"], Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListNetworkSitesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Paginator.ListNetworkSites.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/paginators/#listnetworksitespaginator)
         """
 
 class ListNetworksPaginator(AioPaginator):
@@ -130,15 +130,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/paginators/#listnetworkspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Mapping[Literal["STATUS"], Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListNetworksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Paginator.ListNetworks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/paginators/#listnetworkspaginator)
         """
 
 class ListOrdersPaginator(AioPaginator):
@@ -148,13 +148,13 @@
     """
 
     def paginate(
         self,
         *,
         networkArn: str,
         filters: Mapping[OrderFilterKeysType, Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOrdersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Paginator.ListOrders.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/paginators/#listorderspaginator)
         """
```

### Comparing `types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks/type_defs.py` & `types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks/type_defs.py`

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
     "AcknowledgeOrderReceiptRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ActivateDeviceIdentifierRequestRequestTypeDef",
     "DeviceIdentifierTypeDef",
     "AddressTypeDef",
     "CommitmentConfigurationTypeDef",
```

### Comparing `types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks/type_defs.pyi` & `types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks.egg-info/PKG-INFO` & `types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-privatenetworks
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Private5G 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Private5G 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/
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
 
 <a id="types-aiobotocore-privatenetworks"></a>
 
 # types-aiobotocore-privatenetworks
 
 [![PyPI - types-aiobotocore-privatenetworks](https://img.shields.io/pypi/v/types-aiobotocore-privatenetworks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-privatenetworks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-privatenetworks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-privatenetworks)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-privatenetworks)](https://pepy.tech/project/types-aiobotocore-privatenetworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Private5G 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
+[aiobotocore.Private5G 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
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
 [types-aiobotocore-privatenetworks docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-privatenetworks-2.9.0/types_aiobotocore_privatenetworks.egg-info/SOURCES.txt` & `types-aiobotocore-privatenetworks-2.9.1/types_aiobotocore_privatenetworks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

