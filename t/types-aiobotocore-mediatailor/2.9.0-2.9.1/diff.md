# Comparing `tmp/types-aiobotocore-mediatailor-2.9.0.tar.gz` & `tmp/types-aiobotocore-mediatailor-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mediatailor-2.9.0.tar", last modified: Wed Dec 13 19:59:55 2023, max compression
+gzip compressed data, was "types-aiobotocore-mediatailor-2.9.1.tar", last modified: Thu Jan 18 01:21:17 2024, max compression
```

## Comparing `types-aiobotocore-mediatailor-2.9.0.tar` & `types-aiobotocore-mediatailor-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:55.337443 types-aiobotocore-mediatailor-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:50:20.000000 types-aiobotocore-mediatailor-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14283 2023-12-13 19:59:55.337443 types-aiobotocore-mediatailor-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12704 2023-12-13 19:50:20.000000 types-aiobotocore-mediatailor-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:55.337443 types-aiobotocore-mediatailor-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2023-12-13 19:50:20.000000 types-aiobotocore-mediatailor-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:55.333443 types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor/
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2023-12-13 19:50:20.000000 types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2023-12-13 19:50:20.000000 types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      948 2023-12-13 19:50:20.000000 types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35840 2023-12-13 19:50:20.000000 types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    35836 2023-12-13 19:50:20.000000 types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10725 2023-12-13 19:50:21.000000 types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10723 2023-12-13 19:50:21.000000 types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10180 2023-12-13 19:50:21.000000 types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10170 2023-12-13 19:50:20.000000 types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:50:20.000000 types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    47249 2023-12-13 19:50:21.000000 types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    47248 2023-12-13 19:50:21.000000 types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:50:20.000000 types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:55.337443 types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14283 2023-12-13 19:59:55.000000 types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      889 2023-12-13 19:59:55.000000 types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:55.000000 types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:55.000000 types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:55.000000 types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 19:59:55.000000 types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:17.089177 types-aiobotocore-mediatailor-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:12:04.000000 types-aiobotocore-mediatailor-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14303 2024-01-18 01:21:17.089177 types-aiobotocore-mediatailor-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12704 2024-01-18 01:12:04.000000 types-aiobotocore-mediatailor-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:17.089177 types-aiobotocore-mediatailor-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-01-18 01:12:04.000000 types-aiobotocore-mediatailor-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:17.085177 types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor/
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-01-18 01:12:04.000000 types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-01-18 01:12:04.000000 types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-01-18 01:12:04.000000 types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35853 2024-01-18 01:12:04.000000 types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35850 2024-01-18 01:12:04.000000 types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10723 2024-01-18 01:12:04.000000 types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10723 2024-01-18 01:12:04.000000 types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10181 2024-01-18 01:12:04.000000 types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-01-18 01:12:04.000000 types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:12:04.000000 types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    47248 2024-01-18 01:12:05.000000 types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47248 2024-01-18 01:12:05.000000 types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:12:04.000000 types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:17.089177 types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14303 2024-01-18 01:21:17.000000 types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-01-18 01:21:17.000000 types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:17.000000 types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:17.000000 types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:17.000000 types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-18 01:21:17.000000 types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mediatailor-2.9.0/LICENSE` & `types-aiobotocore-mediatailor-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-mediatailor-2.9.0/PKG-INFO` & `types-aiobotocore-mediatailor-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mediatailor
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MediaTailor 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MediaTailor 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/
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
 
 <a id="types-aiobotocore-mediatailor"></a>
 
 # types-aiobotocore-mediatailor
 
 [![PyPI - types-aiobotocore-mediatailor](https://img.shields.io/pypi/v/types-aiobotocore-mediatailor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediatailor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediatailor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediatailor)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediatailor)](https://pepy.tech/project/types-aiobotocore-mediatailor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaTailor 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor)
+[aiobotocore.MediaTailor 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor)
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
 [types-aiobotocore-mediatailor docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mediatailor-2.9.0/README.md` & `types-aiobotocore-mediatailor-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediatailor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediatailor)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediatailor)](https://pepy.tech/project/types-aiobotocore-mediatailor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaTailor 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor)
+[aiobotocore.MediaTailor 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor)
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
 [types-aiobotocore-mediatailor docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mediatailor-2.9.0/setup.py` & `types-aiobotocore-mediatailor-2.9.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mediatailor",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_mediatailor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MediaTailor 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.MediaTailor 2.9.1 service generated with"
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
     keywords="aiobotocore mediatailor type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_mediatailor": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor/__init__.py` & `types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     ListPrefetchSchedulesPaginator,
     ListSourceLocationsPaginator,
     ListVodSourcesPaginator,
 )
 
 Client = MediaTailorClient
 
-
 __all__ = (
     "Client",
     "GetChannelSchedulePaginator",
     "ListAlertsPaginator",
     "ListChannelsPaginator",
     "ListLiveSourcesPaginator",
     "ListPlaybackConfigurationsPaginator",
```

### Comparing `types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor/__init__.pyi` & `types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor/__main__.py` & `types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MediaTailor 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.MediaTailor 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor\nOther"
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

### Comparing `types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor/client.py` & `types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -86,31 +86,27 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("MediaTailorClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
 
-
 class MediaTailorClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/)
     """
 
     meta: ClientMeta
@@ -164,30 +160,30 @@
         self,
         *,
         ChannelName: str,
         Outputs: Sequence[RequestOutputItemTypeDef],
         PlaybackMode: PlaybackModeType,
         FillerSlate: SlateSourceTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        Tier: TierType = ...
+        Tier: TierType = ...,
     ) -> CreateChannelResponseTypeDef:
         """
         Creates a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#create_channel)
         """
 
     async def create_live_source(
         self,
         *,
         HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],
         LiveSourceName: str,
         SourceLocationName: str,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateLiveSourceResponseTypeDef:
         """
         The live source configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_live_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#create_live_source)
         """
@@ -195,15 +191,15 @@
     async def create_prefetch_schedule(
         self,
         *,
         Consumption: PrefetchConsumptionTypeDef,
         Name: str,
         PlaybackConfigurationName: str,
         Retrieval: PrefetchRetrievalTypeDef,
-        StreamId: str = ...
+        StreamId: str = ...,
     ) -> CreatePrefetchScheduleResponseTypeDef:
         """
         Creates a prefetch schedule for a playback configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_prefetch_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#create_prefetch_schedule)
         """
@@ -213,15 +209,15 @@
         *,
         ChannelName: str,
         ProgramName: str,
         ScheduleConfiguration: ScheduleConfigurationTypeDef,
         SourceLocationName: str,
         AdBreaks: Sequence[AdBreakTypeDef] = ...,
         LiveSourceName: str = ...,
-        VodSourceName: str = ...
+        VodSourceName: str = ...,
     ) -> CreateProgramResponseTypeDef:
         """
         Creates a program within a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_program)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#create_program)
         """
@@ -230,30 +226,30 @@
         self,
         *,
         HttpConfiguration: HttpConfigurationTypeDef,
         SourceLocationName: str,
         AccessConfiguration: AccessConfigurationTypeDef = ...,
         DefaultSegmentDeliveryConfiguration: DefaultSegmentDeliveryConfigurationTypeDef = ...,
         SegmentDeliveryConfigurations: Sequence[SegmentDeliveryConfigurationTypeDef] = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateSourceLocationResponseTypeDef:
         """
         Creates a source location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_source_location)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#create_source_location)
         """
 
     async def create_vod_source(
         self,
         *,
         HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],
         SourceLocationName: str,
         VodSourceName: str,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateVodSourceResponseTypeDef:
         """
         The VOD source configuration parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_vod_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#create_vod_source)
         """
@@ -402,15 +398,15 @@
 
     async def get_channel_schedule(
         self,
         *,
         ChannelName: str,
         DurationMinutes: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetChannelScheduleResponseTypeDef:
         """
         Retrieves information about your channel's schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.get_channel_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#get_channel_schedule)
         """
@@ -480,15 +476,15 @@
 
     async def list_prefetch_schedules(
         self,
         *,
         PlaybackConfigurationName: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        StreamId: str = ...
+        StreamId: str = ...,
     ) -> ListPrefetchSchedulesResponseTypeDef:
         """
         Lists the prefetch schedules for a playback configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_prefetch_schedules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#list_prefetch_schedules)
         """
@@ -543,15 +539,15 @@
         DashConfiguration: DashConfigurationForPutTypeDef = ...,
         LivePreRollConfiguration: LivePreRollConfigurationTypeDef = ...,
         ManifestProcessingRules: ManifestProcessingRulesTypeDef = ...,
         PersonalizationThresholdSeconds: int = ...,
         SlateAdUrl: str = ...,
         Tags: Mapping[str, str] = ...,
         TranscodeProfileName: str = ...,
-        VideoContentSourceUrl: str = ...
+        VideoContentSourceUrl: str = ...,
     ) -> PutPlaybackConfigurationResponseTypeDef:
         """
         Creates a playback configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.put_playback_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#put_playback_configuration)
         """
@@ -593,44 +589,44 @@
         """
 
     async def update_channel(
         self,
         *,
         ChannelName: str,
         Outputs: Sequence[RequestOutputItemTypeDef],
-        FillerSlate: SlateSourceTypeDef = ...
+        FillerSlate: SlateSourceTypeDef = ...,
     ) -> UpdateChannelResponseTypeDef:
         """
         Updates a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#update_channel)
         """
 
     async def update_live_source(
         self,
         *,
         HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],
         LiveSourceName: str,
-        SourceLocationName: str
+        SourceLocationName: str,
     ) -> UpdateLiveSourceResponseTypeDef:
         """
         Updates a live source's configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_live_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#update_live_source)
         """
 
     async def update_program(
         self,
         *,
         ChannelName: str,
         ProgramName: str,
         ScheduleConfiguration: UpdateProgramScheduleConfigurationTypeDef,
-        AdBreaks: Sequence[AdBreakTypeDef] = ...
+        AdBreaks: Sequence[AdBreakTypeDef] = ...,
     ) -> UpdateProgramResponseTypeDef:
         """
         Updates a program within a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_program)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#update_program)
         """
@@ -638,29 +634,29 @@
     async def update_source_location(
         self,
         *,
         HttpConfiguration: HttpConfigurationTypeDef,
         SourceLocationName: str,
         AccessConfiguration: AccessConfigurationTypeDef = ...,
         DefaultSegmentDeliveryConfiguration: DefaultSegmentDeliveryConfigurationTypeDef = ...,
-        SegmentDeliveryConfigurations: Sequence[SegmentDeliveryConfigurationTypeDef] = ...
+        SegmentDeliveryConfigurations: Sequence[SegmentDeliveryConfigurationTypeDef] = ...,
     ) -> UpdateSourceLocationResponseTypeDef:
         """
         Updates a source location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_source_location)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#update_source_location)
         """
 
     async def update_vod_source(
         self,
         *,
         HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],
         SourceLocationName: str,
-        VodSourceName: str
+        VodSourceName: str,
     ) -> UpdateVodSourceResponseTypeDef:
         """
         Updates a VOD source's configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_vod_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#update_vod_source)
         """
```

### Comparing `types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor/client.pyi` & `types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,25 +88,28 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("MediaTailorClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
 
+
 class MediaTailorClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/)
     """
 
     meta: ClientMeta
@@ -160,30 +163,30 @@
         self,
         *,
         ChannelName: str,
         Outputs: Sequence[RequestOutputItemTypeDef],
         PlaybackMode: PlaybackModeType,
         FillerSlate: SlateSourceTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        Tier: TierType = ...
+        Tier: TierType = ...,
     ) -> CreateChannelResponseTypeDef:
         """
         Creates a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#create_channel)
         """
 
     async def create_live_source(
         self,
         *,
         HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],
         LiveSourceName: str,
         SourceLocationName: str,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateLiveSourceResponseTypeDef:
         """
         The live source configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_live_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#create_live_source)
         """
@@ -191,15 +194,15 @@
     async def create_prefetch_schedule(
         self,
         *,
         Consumption: PrefetchConsumptionTypeDef,
         Name: str,
         PlaybackConfigurationName: str,
         Retrieval: PrefetchRetrievalTypeDef,
-        StreamId: str = ...
+        StreamId: str = ...,
     ) -> CreatePrefetchScheduleResponseTypeDef:
         """
         Creates a prefetch schedule for a playback configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_prefetch_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#create_prefetch_schedule)
         """
@@ -209,15 +212,15 @@
         *,
         ChannelName: str,
         ProgramName: str,
         ScheduleConfiguration: ScheduleConfigurationTypeDef,
         SourceLocationName: str,
         AdBreaks: Sequence[AdBreakTypeDef] = ...,
         LiveSourceName: str = ...,
-        VodSourceName: str = ...
+        VodSourceName: str = ...,
     ) -> CreateProgramResponseTypeDef:
         """
         Creates a program within a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_program)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#create_program)
         """
@@ -226,30 +229,30 @@
         self,
         *,
         HttpConfiguration: HttpConfigurationTypeDef,
         SourceLocationName: str,
         AccessConfiguration: AccessConfigurationTypeDef = ...,
         DefaultSegmentDeliveryConfiguration: DefaultSegmentDeliveryConfigurationTypeDef = ...,
         SegmentDeliveryConfigurations: Sequence[SegmentDeliveryConfigurationTypeDef] = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateSourceLocationResponseTypeDef:
         """
         Creates a source location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_source_location)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#create_source_location)
         """
 
     async def create_vod_source(
         self,
         *,
         HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],
         SourceLocationName: str,
         VodSourceName: str,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateVodSourceResponseTypeDef:
         """
         The VOD source configuration parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_vod_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#create_vod_source)
         """
@@ -398,15 +401,15 @@
 
     async def get_channel_schedule(
         self,
         *,
         ChannelName: str,
         DurationMinutes: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetChannelScheduleResponseTypeDef:
         """
         Retrieves information about your channel's schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.get_channel_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#get_channel_schedule)
         """
@@ -476,15 +479,15 @@
 
     async def list_prefetch_schedules(
         self,
         *,
         PlaybackConfigurationName: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        StreamId: str = ...
+        StreamId: str = ...,
     ) -> ListPrefetchSchedulesResponseTypeDef:
         """
         Lists the prefetch schedules for a playback configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_prefetch_schedules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#list_prefetch_schedules)
         """
@@ -539,15 +542,15 @@
         DashConfiguration: DashConfigurationForPutTypeDef = ...,
         LivePreRollConfiguration: LivePreRollConfigurationTypeDef = ...,
         ManifestProcessingRules: ManifestProcessingRulesTypeDef = ...,
         PersonalizationThresholdSeconds: int = ...,
         SlateAdUrl: str = ...,
         Tags: Mapping[str, str] = ...,
         TranscodeProfileName: str = ...,
-        VideoContentSourceUrl: str = ...
+        VideoContentSourceUrl: str = ...,
     ) -> PutPlaybackConfigurationResponseTypeDef:
         """
         Creates a playback configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.put_playback_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#put_playback_configuration)
         """
@@ -589,44 +592,44 @@
         """
 
     async def update_channel(
         self,
         *,
         ChannelName: str,
         Outputs: Sequence[RequestOutputItemTypeDef],
-        FillerSlate: SlateSourceTypeDef = ...
+        FillerSlate: SlateSourceTypeDef = ...,
     ) -> UpdateChannelResponseTypeDef:
         """
         Updates a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#update_channel)
         """
 
     async def update_live_source(
         self,
         *,
         HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],
         LiveSourceName: str,
-        SourceLocationName: str
+        SourceLocationName: str,
     ) -> UpdateLiveSourceResponseTypeDef:
         """
         Updates a live source's configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_live_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#update_live_source)
         """
 
     async def update_program(
         self,
         *,
         ChannelName: str,
         ProgramName: str,
         ScheduleConfiguration: UpdateProgramScheduleConfigurationTypeDef,
-        AdBreaks: Sequence[AdBreakTypeDef] = ...
+        AdBreaks: Sequence[AdBreakTypeDef] = ...,
     ) -> UpdateProgramResponseTypeDef:
         """
         Updates a program within a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_program)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#update_program)
         """
@@ -634,29 +637,29 @@
     async def update_source_location(
         self,
         *,
         HttpConfiguration: HttpConfigurationTypeDef,
         SourceLocationName: str,
         AccessConfiguration: AccessConfigurationTypeDef = ...,
         DefaultSegmentDeliveryConfiguration: DefaultSegmentDeliveryConfigurationTypeDef = ...,
-        SegmentDeliveryConfigurations: Sequence[SegmentDeliveryConfigurationTypeDef] = ...
+        SegmentDeliveryConfigurations: Sequence[SegmentDeliveryConfigurationTypeDef] = ...,
     ) -> UpdateSourceLocationResponseTypeDef:
         """
         Updates a source location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_source_location)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#update_source_location)
         """
 
     async def update_vod_source(
         self,
         *,
         HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],
         SourceLocationName: str,
-        VodSourceName: str
+        VodSourceName: str,
     ) -> UpdateVodSourceResponseTypeDef:
         """
         Updates a VOD source's configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_vod_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#update_vod_source)
         """
```

### Comparing `types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor/literals.py` & `types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor/literals.py`

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
     "AccessTypeType",
     "AdMarkupTypeType",
     "AlertCategoryType",
     "ChannelStateType",
     "FillPolicyType",
     "GetChannelSchedulePaginatorName",
@@ -47,15 +46,14 @@
     "MediaTailorServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AccessTypeType = Literal["AUTODETECT_SIGV4", "S3_SIGV4", "SECRETS_MANAGER_ACCESS_TOKEN"]
 AdMarkupTypeType = Literal["DATERANGE", "SCTE35_ENHANCED"]
 AlertCategoryType = Literal["INFO", "PLAYBACK_WARNING", "SCHEDULING_ERROR"]
 ChannelStateType = Literal["RUNNING", "STOPPED"]
 FillPolicyType = Literal["FULL_AVAIL_ONLY", "PARTIAL_AVAIL"]
 GetChannelSchedulePaginatorName = Literal["get_channel_schedule"]
 ListAlertsPaginatorName = Literal["list_alerts"]
```

### Comparing `types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor/literals.pyi` & `types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor/paginator.py` & `types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,14 @@
     "ListLiveSourcesPaginator",
     "ListPlaybackConfigurationsPaginator",
     "ListPrefetchSchedulesPaginator",
     "ListSourceLocationsPaginator",
     "ListVodSourcesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -81,15 +80,15 @@
     """
 
     def paginate(
         self,
         *,
         ChannelName: str,
         DurationMinutes: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetChannelScheduleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.GetChannelSchedule.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/paginators/#getchannelschedulepaginator)
         """
 
 
@@ -160,15 +159,15 @@
     """
 
     def paginate(
         self,
         *,
         PlaybackConfigurationName: str,
         StreamId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPrefetchSchedulesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListPrefetchSchedules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/paginators/#listprefetchschedulespaginator)
         """
```

### Comparing `types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor/paginator.pyi` & `types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     """
 
     def paginate(
         self,
         *,
         ChannelName: str,
         DurationMinutes: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetChannelScheduleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.GetChannelSchedule.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/paginators/#getchannelschedulepaginator)
         """
 
 class ListAlertsPaginator(AioPaginator):
@@ -152,15 +152,15 @@
     """
 
     def paginate(
         self,
         *,
         PlaybackConfigurationName: str,
         StreamId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPrefetchSchedulesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListPrefetchSchedules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/paginators/#listprefetchschedulespaginator)
         """
 
 class ListSourceLocationsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor/type_defs.py` & `types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor/type_defs.py`

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
     "SecretsManagerAccessTokenConfigurationTypeDef",
     "AdBreakOpportunityTypeDef",
     "KeyValuePairTypeDef",
     "SlateSourceTypeDef",
     "SpliceInsertMessageTypeDef",
     "AdMarkerPassthroughTypeDef",
```

### Comparing `types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor/type_defs.pyi` & `types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor.egg-info/PKG-INFO` & `types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mediatailor
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MediaTailor 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MediaTailor 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/
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
 
 <a id="types-aiobotocore-mediatailor"></a>
 
 # types-aiobotocore-mediatailor
 
 [![PyPI - types-aiobotocore-mediatailor](https://img.shields.io/pypi/v/types-aiobotocore-mediatailor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediatailor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediatailor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediatailor)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediatailor)](https://pepy.tech/project/types-aiobotocore-mediatailor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaTailor 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor)
+[aiobotocore.MediaTailor 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor)
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
 [types-aiobotocore-mediatailor docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mediatailor-2.9.0/types_aiobotocore_mediatailor.egg-info/SOURCES.txt` & `types-aiobotocore-mediatailor-2.9.1/types_aiobotocore_mediatailor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

