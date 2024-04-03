# Comparing `tmp/types-aiobotocore-lightsail-2.9.0.tar.gz` & `tmp/types-aiobotocore-lightsail-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-lightsail-2.9.0.tar", last modified: Wed Dec 13 19:59:46 2023, max compression
+gzip compressed data, was "types-aiobotocore-lightsail-2.9.1.tar", last modified: Thu Jan 18 01:21:08 2024, max compression
```

## Comparing `types-aiobotocore-lightsail-2.9.0.tar` & `types-aiobotocore-lightsail-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:46.309522 types-aiobotocore-lightsail-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:49:14.000000 types-aiobotocore-lightsail-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16067 2023-12-13 19:59:46.309522 types-aiobotocore-lightsail-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14496 2023-12-13 19:49:14.000000 types-aiobotocore-lightsail-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:46.309522 types-aiobotocore-lightsail-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2023-12-13 19:49:14.000000 types-aiobotocore-lightsail-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:46.309522 types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail/
--rw-r--r--   0 runner    (1001) docker     (127)     4924 2023-12-13 19:49:14.000000 types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2023-12-13 19:49:14.000000 types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-12-13 19:49:14.000000 types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   119564 2023-12-13 19:49:17.000000 types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   119560 2023-12-13 19:49:16.000000 types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    25808 2023-12-13 19:49:17.000000 types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    25806 2023-12-13 19:49:17.000000 types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    24001 2023-12-13 19:49:17.000000 types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    23978 2023-12-13 19:49:17.000000 types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:49:14.000000 types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   138855 2023-12-13 19:49:21.000000 types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   138854 2023-12-13 19:49:18.000000 types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:49:14.000000 types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:46.309522 types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16067 2023-12-13 19:59:46.000000 types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-12-13 19:59:46.000000 types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:46.000000 types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:46.000000 types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:46.000000 types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-13 19:59:46.000000 types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:08.765215 types-aiobotocore-lightsail-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:11:02.000000 types-aiobotocore-lightsail-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16087 2024-01-18 01:21:08.765215 types-aiobotocore-lightsail-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14496 2024-01-18 01:11:02.000000 types-aiobotocore-lightsail-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:08.765215 types-aiobotocore-lightsail-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-01-18 01:11:02.000000 types-aiobotocore-lightsail-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:08.761215 types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail/
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-01-18 01:11:02.000000 types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-01-18 01:11:02.000000 types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-01-18 01:11:02.000000 types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119601 2024-01-18 01:11:03.000000 types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119598 2024-01-18 01:11:02.000000 types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    25806 2024-01-18 01:11:03.000000 types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25806 2024-01-18 01:11:03.000000 types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    24002 2024-01-18 01:11:03.000000 types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23981 2024-01-18 01:11:03.000000 types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:11:02.000000 types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   138854 2024-01-18 01:11:07.000000 types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   138854 2024-01-18 01:11:07.000000 types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:11:02.000000 types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:08.765215 types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16087 2024-01-18 01:21:08.000000 types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-01-18 01:21:08.000000 types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:08.000000 types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:08.000000 types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:08.000000 types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-18 01:21:08.000000 types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lightsail-2.9.0/LICENSE` & `types-aiobotocore-lightsail-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-lightsail-2.9.0/PKG-INFO` & `types-aiobotocore-lightsail-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lightsail
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Lightsail 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Lightsail 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/
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
 
 <a id="types-aiobotocore-lightsail"></a>
 
 # types-aiobotocore-lightsail
 
 [![PyPI - types-aiobotocore-lightsail](https://img.shields.io/pypi/v/types-aiobotocore-lightsail.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lightsail)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lightsail.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lightsail)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lightsail)](https://pepy.tech/project/types-aiobotocore-lightsail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Lightsail 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
+[aiobotocore.Lightsail 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
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
 [types-aiobotocore-lightsail docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-lightsail-2.9.0/README.md` & `types-aiobotocore-lightsail-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lightsail.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lightsail)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lightsail)](https://pepy.tech/project/types-aiobotocore-lightsail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Lightsail 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
+[aiobotocore.Lightsail 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
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
 [types-aiobotocore-lightsail docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-lightsail-2.9.0/setup.py` & `types-aiobotocore-lightsail-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-lightsail",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_lightsail"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Lightsail 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Lightsail 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore lightsail type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_lightsail": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail/__init__.py` & `types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,14 @@
     GetRelationalDatabaseSnapshotsPaginator,
     GetRelationalDatabasesPaginator,
     GetStaticIpsPaginator,
 )
 
 Client = LightsailClient
 
-
 __all__ = (
     "Client",
     "GetActiveNamesPaginator",
     "GetBlueprintsPaginator",
     "GetBundlesPaginator",
     "GetCloudFormationStackRecordsPaginator",
     "GetDiskSnapshotsPaginator",
```

### Comparing `types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail/__init__.pyi` & `types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail/__main__.py` & `types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Lightsail 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Lightsail 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail\nOther"
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

### Comparing `types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail/client.py` & `types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,15 +250,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("LightsailClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -386,15 +385,15 @@
         self,
         *,
         targetSnapshotName: str,
         sourceRegion: RegionNameType,
         sourceSnapshotName: str = ...,
         sourceResourceName: str = ...,
         restoreDate: str = ...,
-        useLatestRestorableAutoSnapshot: bool = ...
+        useLatestRestorableAutoSnapshot: bool = ...,
     ) -> CopySnapshotResultTypeDef:
         """
         Copies a manual snapshot of an instance or disk as another manual snapshot, or
         copies an automatic snapshot of an instance or disk as a manual
         snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.copy_snapshot)
@@ -403,15 +402,15 @@
 
     async def create_bucket(
         self,
         *,
         bucketName: str,
         bundleId: str,
         tags: Sequence[TagTypeDef] = ...,
-        enableObjectVersioning: bool = ...
+        enableObjectVersioning: bool = ...,
     ) -> CreateBucketResultTypeDef:
         """
         Creates an Amazon Lightsail bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#create_bucket)
         """
@@ -428,15 +427,15 @@
 
     async def create_certificate(
         self,
         *,
         certificateName: str,
         domainName: str,
         subjectAlternativeNames: Sequence[str] = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateCertificateResultTypeDef:
         """
         Creates an SSL/TLS certificate for an Amazon Lightsail content delivery network
         (CDN) distribution and a container
         service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_certificate)
@@ -470,29 +469,29 @@
         *,
         serviceName: str,
         power: ContainerServicePowerNameType,
         scale: int,
         tags: Sequence[TagTypeDef] = ...,
         publicDomainNames: Mapping[str, Sequence[str]] = ...,
         deployment: ContainerServiceDeploymentRequestTypeDef = ...,
-        privateRegistryAccess: PrivateRegistryAccessRequestTypeDef = ...
+        privateRegistryAccess: PrivateRegistryAccessRequestTypeDef = ...,
     ) -> CreateContainerServiceResultTypeDef:
         """
         Creates an Amazon Lightsail container service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_container_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#create_container_service)
         """
 
     async def create_container_service_deployment(
         self,
         *,
         serviceName: str,
         containers: Mapping[str, ContainerTypeDef] = ...,
-        publicEndpoint: EndpointRequestTypeDef = ...
+        publicEndpoint: EndpointRequestTypeDef = ...,
     ) -> CreateContainerServiceDeploymentResultTypeDef:
         """
         Creates a deployment for your Amazon Lightsail container service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_container_service_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#create_container_service_deployment)
         """
@@ -512,15 +511,15 @@
     async def create_disk(
         self,
         *,
         diskName: str,
         availabilityZone: str,
         sizeInGb: int,
         tags: Sequence[TagTypeDef] = ...,
-        addOns: Sequence[AddOnRequestTypeDef] = ...
+        addOns: Sequence[AddOnRequestTypeDef] = ...,
     ) -> CreateDiskResultTypeDef:
         """
         Creates a block storage disk that can be attached to an Amazon Lightsail
         instance in the same Availability Zone (e.g.,
         `us-east-2a`).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_disk)
@@ -534,30 +533,30 @@
         availabilityZone: str,
         sizeInGb: int,
         diskSnapshotName: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         addOns: Sequence[AddOnRequestTypeDef] = ...,
         sourceDiskName: str = ...,
         restoreDate: str = ...,
-        useLatestRestorableAutoSnapshot: bool = ...
+        useLatestRestorableAutoSnapshot: bool = ...,
     ) -> CreateDiskFromSnapshotResultTypeDef:
         """
         Creates a block storage disk from a manual or automatic snapshot of a disk.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_disk_from_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#create_disk_from_snapshot)
         """
 
     async def create_disk_snapshot(
         self,
         *,
         diskSnapshotName: str,
         diskName: str = ...,
         instanceName: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDiskSnapshotResultTypeDef:
         """
         Creates a snapshot of a block storage disk.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_disk_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#create_disk_snapshot)
         """
@@ -568,15 +567,15 @@
         distributionName: str,
         origin: InputOriginTypeDef,
         defaultCacheBehavior: CacheBehaviorTypeDef,
         bundleId: str,
         cacheBehaviorSettings: CacheSettingsTypeDef = ...,
         cacheBehaviors: Sequence[CacheBehaviorPerPathTypeDef] = ...,
         ipAddressType: IpAddressTypeType = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDistributionResultTypeDef:
         """
         Creates an Amazon Lightsail content delivery network (CDN) distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_distribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#create_distribution)
         """
@@ -634,15 +633,15 @@
         blueprintId: str,
         bundleId: str,
         customImageName: str = ...,
         userData: str = ...,
         keyPairName: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         addOns: Sequence[AddOnRequestTypeDef] = ...,
-        ipAddressType: IpAddressTypeType = ...
+        ipAddressType: IpAddressTypeType = ...,
     ) -> CreateInstancesResultTypeDef:
         """
         Creates one or more Amazon Lightsail instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#create_instances)
         """
@@ -658,15 +657,15 @@
         userData: str = ...,
         keyPairName: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         addOns: Sequence[AddOnRequestTypeDef] = ...,
         ipAddressType: IpAddressTypeType = ...,
         sourceInstanceName: str = ...,
         restoreDate: str = ...,
-        useLatestRestorableAutoSnapshot: bool = ...
+        useLatestRestorableAutoSnapshot: bool = ...,
     ) -> CreateInstancesFromSnapshotResultTypeDef:
         """
         Creates one or more new instances from a manual or automatic snapshot of an
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_instances_from_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#create_instances_from_snapshot)
@@ -690,15 +689,15 @@
         instancePort: int,
         healthCheckPath: str = ...,
         certificateName: str = ...,
         certificateDomainName: str = ...,
         certificateAlternativeNames: Sequence[str] = ...,
         tags: Sequence[TagTypeDef] = ...,
         ipAddressType: IpAddressTypeType = ...,
-        tlsPolicyName: str = ...
+        tlsPolicyName: str = ...,
     ) -> CreateLoadBalancerResultTypeDef:
         """
         Creates a Lightsail load balancer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_load_balancer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#create_load_balancer)
         """
@@ -706,15 +705,15 @@
     async def create_load_balancer_tls_certificate(
         self,
         *,
         loadBalancerName: str,
         certificateName: str,
         certificateDomainName: str,
         certificateAlternativeNames: Sequence[str] = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateLoadBalancerTlsCertificateResultTypeDef:
         """
         Creates an SSL/TLS certificate for an Amazon Lightsail load balancer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_load_balancer_tls_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#create_load_balancer_tls_certificate)
         """
@@ -728,15 +727,15 @@
         masterDatabaseName: str,
         masterUsername: str,
         availabilityZone: str = ...,
         masterUserPassword: str = ...,
         preferredBackupWindow: str = ...,
         preferredMaintenanceWindow: str = ...,
         publiclyAccessible: bool = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRelationalDatabaseResultTypeDef:
         """
         Creates a new database in Amazon Lightsail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_relational_database)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#create_relational_database)
         """
@@ -748,29 +747,29 @@
         availabilityZone: str = ...,
         publiclyAccessible: bool = ...,
         relationalDatabaseSnapshotName: str = ...,
         relationalDatabaseBundleId: str = ...,
         sourceRelationalDatabaseName: str = ...,
         restoreTime: TimestampTypeDef = ...,
         useLatestRestorableTime: bool = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRelationalDatabaseFromSnapshotResultTypeDef:
         """
         Creates a new database from an existing database snapshot in Amazon Lightsail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_relational_database_from_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#create_relational_database_from_snapshot)
         """
 
     async def create_relational_database_snapshot(
         self,
         *,
         relationalDatabaseName: str,
         relationalDatabaseSnapshotName: str,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRelationalDatabaseSnapshotResultTypeDef:
         """
         Creates a snapshot of your database in Amazon Lightsail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_relational_database_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#create_relational_database_snapshot)
         """
@@ -961,15 +960,15 @@
         """
 
     async def delete_relational_database(
         self,
         *,
         relationalDatabaseName: str,
         skipFinalSnapshot: bool = ...,
-        finalRelationalDatabaseSnapshotName: str = ...
+        finalRelationalDatabaseSnapshotName: str = ...,
     ) -> DeleteRelationalDatabaseResultTypeDef:
         """
         Deletes a database in Amazon Lightsail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.delete_relational_database)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#delete_relational_database)
         """
@@ -1101,15 +1100,15 @@
         """
 
     async def get_blueprints(
         self,
         *,
         includeInactive: bool = ...,
         pageToken: str = ...,
-        appCategory: Literal["LfR"] = ...
+        appCategory: Literal["LfR"] = ...,
     ) -> GetBlueprintsResultTypeDef:
         """
         Returns the list of available instance images, or *blueprints*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_blueprints)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#get_blueprints)
         """
@@ -1137,15 +1136,15 @@
         *,
         bucketName: str,
         metricName: BucketMetricNameType,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
         period: int,
         statistics: Sequence[MetricStatisticType],
-        unit: MetricUnitType
+        unit: MetricUnitType,
     ) -> GetBucketMetricDataResultTypeDef:
         """
         Returns the data points of a specific metric for an Amazon Lightsail bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_bucket_metric_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#get_bucket_metric_data)
         """
@@ -1161,15 +1160,15 @@
         """
 
     async def get_bundles(
         self,
         *,
         includeInactive: bool = ...,
         pageToken: str = ...,
-        appCategory: Literal["LfR"] = ...
+        appCategory: Literal["LfR"] = ...,
     ) -> GetBundlesResultTypeDef:
         """
         Returns the bundles that you can apply to an Amazon Lightsail instance when you
         create
         it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_bundles)
@@ -1178,15 +1177,15 @@
 
     async def get_certificates(
         self,
         *,
         certificateStatuses: Sequence[CertificateStatusType] = ...,
         includeCertificateDetails: bool = ...,
         certificateName: str = ...,
-        pageToken: str = ...
+        pageToken: str = ...,
     ) -> GetCertificatesResultTypeDef:
         """
         Returns information about one or more Amazon Lightsail SSL/TLS certificates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_certificates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#get_certificates)
         """
@@ -1237,15 +1236,15 @@
         self,
         *,
         serviceName: str,
         containerName: str,
         startTime: TimestampTypeDef = ...,
         endTime: TimestampTypeDef = ...,
         filterPattern: str = ...,
-        pageToken: str = ...
+        pageToken: str = ...,
     ) -> GetContainerLogResultTypeDef:
         """
         Returns the log events of a container of your Amazon Lightsail container
         service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_container_log)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#get_container_log)
@@ -1268,15 +1267,15 @@
         self,
         *,
         serviceName: str,
         metricName: ContainerServiceMetricNameType,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
         period: int,
-        statistics: Sequence[MetricStatisticType]
+        statistics: Sequence[MetricStatisticType],
     ) -> GetContainerServiceMetricDataResultTypeDef:
         """
         Returns the data points of a specific metric of your Amazon Lightsail container
         service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_container_service_metric_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#get_container_service_metric_data)
@@ -1375,15 +1374,15 @@
         *,
         distributionName: str,
         metricName: DistributionMetricNameType,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
         period: int,
         unit: MetricUnitType,
-        statistics: Sequence[MetricStatisticType]
+        statistics: Sequence[MetricStatisticType],
     ) -> GetDistributionMetricDataResultTypeDef:
         """
         Returns the data points of a specific metric for an Amazon Lightsail content
         delivery network (CDN)
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_distribution_metric_data)
@@ -1457,15 +1456,15 @@
         *,
         instanceName: str,
         metricName: InstanceMetricNameType,
         period: int,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
         unit: MetricUnitType,
-        statistics: Sequence[MetricStatisticType]
+        statistics: Sequence[MetricStatisticType],
     ) -> GetInstanceMetricDataResultTypeDef:
         """
         Returns the data points for the specified Amazon Lightsail instance metric,
         given an instance
         name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_instance_metric_data)
@@ -1552,15 +1551,15 @@
         *,
         loadBalancerName: str,
         metricName: LoadBalancerMetricNameType,
         period: int,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
         unit: MetricUnitType,
-        statistics: Sequence[MetricStatisticType]
+        statistics: Sequence[MetricStatisticType],
     ) -> GetLoadBalancerMetricDataResultTypeDef:
         """
         Returns information about health metrics for your Lightsail load balancer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_load_balancer_metric_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#get_load_balancer_metric_data)
         """
@@ -1622,15 +1621,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#get_operations_for_resource)
         """
 
     async def get_regions(
         self,
         *,
         includeAvailabilityZones: bool = ...,
-        includeRelationalDatabaseAvailabilityZones: bool = ...
+        includeRelationalDatabaseAvailabilityZones: bool = ...,
     ) -> GetRegionsResultTypeDef:
         """
         Returns a list of all valid regions for Amazon Lightsail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_regions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#get_regions)
         """
@@ -1679,15 +1678,15 @@
         self,
         *,
         relationalDatabaseName: str,
         logStreamName: str,
         startTime: TimestampTypeDef = ...,
         endTime: TimestampTypeDef = ...,
         startFromHead: bool = ...,
-        pageToken: str = ...
+        pageToken: str = ...,
     ) -> GetRelationalDatabaseLogEventsResultTypeDef:
         """
         Returns a list of log events for a database in Amazon Lightsail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_relational_database_log_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#get_relational_database_log_events)
         """
@@ -1703,15 +1702,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#get_relational_database_log_streams)
         """
 
     async def get_relational_database_master_user_password(
         self,
         *,
         relationalDatabaseName: str,
-        passwordVersion: RelationalDatabasePasswordVersionType = ...
+        passwordVersion: RelationalDatabasePasswordVersionType = ...,
     ) -> GetRelationalDatabaseMasterUserPasswordResultTypeDef:
         """
         Returns the current, previous, or pending versions of the master user password
         for a Lightsail
         database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_relational_database_master_user_password)
@@ -1723,15 +1722,15 @@
         *,
         relationalDatabaseName: str,
         metricName: RelationalDatabaseMetricNameType,
         period: int,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
         unit: MetricUnitType,
-        statistics: Sequence[MetricStatisticType]
+        statistics: Sequence[MetricStatisticType],
     ) -> GetRelationalDatabaseMetricDataResultTypeDef:
         """
         Returns the data points of the specified metric for a database in Amazon
         Lightsail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_relational_database_metric_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#get_relational_database_metric_data)
@@ -1842,15 +1841,15 @@
         comparisonOperator: ComparisonOperatorType,
         threshold: float,
         evaluationPeriods: int,
         datapointsToAlarm: int = ...,
         treatMissingData: TreatMissingDataType = ...,
         contactProtocols: Sequence[ContactProtocolType] = ...,
         notificationTriggers: Sequence[AlarmStateType] = ...,
-        notificationEnabled: bool = ...
+        notificationEnabled: bool = ...,
     ) -> PutAlarmResultTypeDef:
         """
         Creates or updates an alarm, and associates it with the specified metric.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.put_alarm)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#put_alarm)
         """
@@ -2047,15 +2046,15 @@
     async def update_bucket(
         self,
         *,
         bucketName: str,
         accessRules: AccessRulesTypeDef = ...,
         versioning: str = ...,
         readonlyAccessAccounts: Sequence[str] = ...,
-        accessLogConfig: BucketAccessLogConfigTypeDef = ...
+        accessLogConfig: BucketAccessLogConfigTypeDef = ...,
     ) -> UpdateBucketResultTypeDef:
         """
         Updates an existing Amazon Lightsail bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.update_bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#update_bucket)
         """
@@ -2074,15 +2073,15 @@
         self,
         *,
         serviceName: str,
         power: ContainerServicePowerNameType = ...,
         scale: int = ...,
         isDisabled: bool = ...,
         publicDomainNames: Mapping[str, Sequence[str]] = ...,
-        privateRegistryAccess: PrivateRegistryAccessRequestTypeDef = ...
+        privateRegistryAccess: PrivateRegistryAccessRequestTypeDef = ...,
     ) -> UpdateContainerServiceResultTypeDef:
         """
         Updates the configuration of your Amazon Lightsail container service, such as
         its power, scale, and public domain
         names.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.update_container_service)
@@ -2093,15 +2092,15 @@
         self,
         *,
         distributionName: str,
         origin: InputOriginTypeDef = ...,
         defaultCacheBehavior: CacheBehaviorTypeDef = ...,
         cacheBehaviorSettings: CacheSettingsTypeDef = ...,
         cacheBehaviors: Sequence[CacheBehaviorPerPathTypeDef] = ...,
-        isEnabled: bool = ...
+        isEnabled: bool = ...,
     ) -> UpdateDistributionResultTypeDef:
         """
         Updates an existing Amazon Lightsail content delivery network (CDN)
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.update_distribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#update_distribution)
@@ -2131,15 +2130,15 @@
     async def update_instance_metadata_options(
         self,
         *,
         instanceName: str,
         httpTokens: HttpTokensType = ...,
         httpEndpoint: HttpEndpointType = ...,
         httpPutResponseHopLimit: int = ...,
-        httpProtocolIpv6: HttpProtocolIpv6Type = ...
+        httpProtocolIpv6: HttpProtocolIpv6Type = ...,
     ) -> UpdateInstanceMetadataOptionsResultTypeDef:
         """
         Modifies the Amazon Lightsail instance metadata parameters on a running or
         stopped
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.update_instance_metadata_options)
@@ -2147,15 +2146,15 @@
         """
 
     async def update_load_balancer_attribute(
         self,
         *,
         loadBalancerName: str,
         attributeName: LoadBalancerAttributeNameType,
-        attributeValue: str
+        attributeValue: str,
     ) -> UpdateLoadBalancerAttributeResultTypeDef:
         """
         Updates the specified attribute for a load balancer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.update_load_balancer_attribute)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#update_load_balancer_attribute)
         """
@@ -2168,28 +2167,28 @@
         rotateMasterUserPassword: bool = ...,
         preferredBackupWindow: str = ...,
         preferredMaintenanceWindow: str = ...,
         enableBackupRetention: bool = ...,
         disableBackupRetention: bool = ...,
         publiclyAccessible: bool = ...,
         applyImmediately: bool = ...,
-        caCertificateIdentifier: str = ...
+        caCertificateIdentifier: str = ...,
     ) -> UpdateRelationalDatabaseResultTypeDef:
         """
         Allows the update of one or more attributes of a database in Amazon Lightsail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.update_relational_database)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#update_relational_database)
         """
 
     async def update_relational_database_parameters(
         self,
         *,
         relationalDatabaseName: str,
-        parameters: Sequence[RelationalDatabaseParameterTypeDef]
+        parameters: Sequence[RelationalDatabaseParameterTypeDef],
     ) -> UpdateRelationalDatabaseParametersResultTypeDef:
         """
         Allows the update of one or more parameters of a database in Amazon Lightsail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.update_relational_database_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#update_relational_database_parameters)
         """
```

### Comparing `types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail/client.pyi` & `types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -382,15 +382,15 @@
         self,
         *,
         targetSnapshotName: str,
         sourceRegion: RegionNameType,
         sourceSnapshotName: str = ...,
         sourceResourceName: str = ...,
         restoreDate: str = ...,
-        useLatestRestorableAutoSnapshot: bool = ...
+        useLatestRestorableAutoSnapshot: bool = ...,
     ) -> CopySnapshotResultTypeDef:
         """
         Copies a manual snapshot of an instance or disk as another manual snapshot, or
         copies an automatic snapshot of an instance or disk as a manual
         snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.copy_snapshot)
@@ -399,15 +399,15 @@
 
     async def create_bucket(
         self,
         *,
         bucketName: str,
         bundleId: str,
         tags: Sequence[TagTypeDef] = ...,
-        enableObjectVersioning: bool = ...
+        enableObjectVersioning: bool = ...,
     ) -> CreateBucketResultTypeDef:
         """
         Creates an Amazon Lightsail bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#create_bucket)
         """
@@ -424,15 +424,15 @@
 
     async def create_certificate(
         self,
         *,
         certificateName: str,
         domainName: str,
         subjectAlternativeNames: Sequence[str] = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateCertificateResultTypeDef:
         """
         Creates an SSL/TLS certificate for an Amazon Lightsail content delivery network
         (CDN) distribution and a container
         service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_certificate)
@@ -466,29 +466,29 @@
         *,
         serviceName: str,
         power: ContainerServicePowerNameType,
         scale: int,
         tags: Sequence[TagTypeDef] = ...,
         publicDomainNames: Mapping[str, Sequence[str]] = ...,
         deployment: ContainerServiceDeploymentRequestTypeDef = ...,
-        privateRegistryAccess: PrivateRegistryAccessRequestTypeDef = ...
+        privateRegistryAccess: PrivateRegistryAccessRequestTypeDef = ...,
     ) -> CreateContainerServiceResultTypeDef:
         """
         Creates an Amazon Lightsail container service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_container_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#create_container_service)
         """
 
     async def create_container_service_deployment(
         self,
         *,
         serviceName: str,
         containers: Mapping[str, ContainerTypeDef] = ...,
-        publicEndpoint: EndpointRequestTypeDef = ...
+        publicEndpoint: EndpointRequestTypeDef = ...,
     ) -> CreateContainerServiceDeploymentResultTypeDef:
         """
         Creates a deployment for your Amazon Lightsail container service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_container_service_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#create_container_service_deployment)
         """
@@ -508,15 +508,15 @@
     async def create_disk(
         self,
         *,
         diskName: str,
         availabilityZone: str,
         sizeInGb: int,
         tags: Sequence[TagTypeDef] = ...,
-        addOns: Sequence[AddOnRequestTypeDef] = ...
+        addOns: Sequence[AddOnRequestTypeDef] = ...,
     ) -> CreateDiskResultTypeDef:
         """
         Creates a block storage disk that can be attached to an Amazon Lightsail
         instance in the same Availability Zone (e.g.,
         `us-east-2a`).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_disk)
@@ -530,30 +530,30 @@
         availabilityZone: str,
         sizeInGb: int,
         diskSnapshotName: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         addOns: Sequence[AddOnRequestTypeDef] = ...,
         sourceDiskName: str = ...,
         restoreDate: str = ...,
-        useLatestRestorableAutoSnapshot: bool = ...
+        useLatestRestorableAutoSnapshot: bool = ...,
     ) -> CreateDiskFromSnapshotResultTypeDef:
         """
         Creates a block storage disk from a manual or automatic snapshot of a disk.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_disk_from_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#create_disk_from_snapshot)
         """
 
     async def create_disk_snapshot(
         self,
         *,
         diskSnapshotName: str,
         diskName: str = ...,
         instanceName: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDiskSnapshotResultTypeDef:
         """
         Creates a snapshot of a block storage disk.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_disk_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#create_disk_snapshot)
         """
@@ -564,15 +564,15 @@
         distributionName: str,
         origin: InputOriginTypeDef,
         defaultCacheBehavior: CacheBehaviorTypeDef,
         bundleId: str,
         cacheBehaviorSettings: CacheSettingsTypeDef = ...,
         cacheBehaviors: Sequence[CacheBehaviorPerPathTypeDef] = ...,
         ipAddressType: IpAddressTypeType = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDistributionResultTypeDef:
         """
         Creates an Amazon Lightsail content delivery network (CDN) distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_distribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#create_distribution)
         """
@@ -630,15 +630,15 @@
         blueprintId: str,
         bundleId: str,
         customImageName: str = ...,
         userData: str = ...,
         keyPairName: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         addOns: Sequence[AddOnRequestTypeDef] = ...,
-        ipAddressType: IpAddressTypeType = ...
+        ipAddressType: IpAddressTypeType = ...,
     ) -> CreateInstancesResultTypeDef:
         """
         Creates one or more Amazon Lightsail instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#create_instances)
         """
@@ -654,15 +654,15 @@
         userData: str = ...,
         keyPairName: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         addOns: Sequence[AddOnRequestTypeDef] = ...,
         ipAddressType: IpAddressTypeType = ...,
         sourceInstanceName: str = ...,
         restoreDate: str = ...,
-        useLatestRestorableAutoSnapshot: bool = ...
+        useLatestRestorableAutoSnapshot: bool = ...,
     ) -> CreateInstancesFromSnapshotResultTypeDef:
         """
         Creates one or more new instances from a manual or automatic snapshot of an
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_instances_from_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#create_instances_from_snapshot)
@@ -686,15 +686,15 @@
         instancePort: int,
         healthCheckPath: str = ...,
         certificateName: str = ...,
         certificateDomainName: str = ...,
         certificateAlternativeNames: Sequence[str] = ...,
         tags: Sequence[TagTypeDef] = ...,
         ipAddressType: IpAddressTypeType = ...,
-        tlsPolicyName: str = ...
+        tlsPolicyName: str = ...,
     ) -> CreateLoadBalancerResultTypeDef:
         """
         Creates a Lightsail load balancer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_load_balancer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#create_load_balancer)
         """
@@ -702,15 +702,15 @@
     async def create_load_balancer_tls_certificate(
         self,
         *,
         loadBalancerName: str,
         certificateName: str,
         certificateDomainName: str,
         certificateAlternativeNames: Sequence[str] = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateLoadBalancerTlsCertificateResultTypeDef:
         """
         Creates an SSL/TLS certificate for an Amazon Lightsail load balancer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_load_balancer_tls_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#create_load_balancer_tls_certificate)
         """
@@ -724,15 +724,15 @@
         masterDatabaseName: str,
         masterUsername: str,
         availabilityZone: str = ...,
         masterUserPassword: str = ...,
         preferredBackupWindow: str = ...,
         preferredMaintenanceWindow: str = ...,
         publiclyAccessible: bool = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRelationalDatabaseResultTypeDef:
         """
         Creates a new database in Amazon Lightsail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_relational_database)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#create_relational_database)
         """
@@ -744,29 +744,29 @@
         availabilityZone: str = ...,
         publiclyAccessible: bool = ...,
         relationalDatabaseSnapshotName: str = ...,
         relationalDatabaseBundleId: str = ...,
         sourceRelationalDatabaseName: str = ...,
         restoreTime: TimestampTypeDef = ...,
         useLatestRestorableTime: bool = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRelationalDatabaseFromSnapshotResultTypeDef:
         """
         Creates a new database from an existing database snapshot in Amazon Lightsail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_relational_database_from_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#create_relational_database_from_snapshot)
         """
 
     async def create_relational_database_snapshot(
         self,
         *,
         relationalDatabaseName: str,
         relationalDatabaseSnapshotName: str,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRelationalDatabaseSnapshotResultTypeDef:
         """
         Creates a snapshot of your database in Amazon Lightsail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_relational_database_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#create_relational_database_snapshot)
         """
@@ -957,15 +957,15 @@
         """
 
     async def delete_relational_database(
         self,
         *,
         relationalDatabaseName: str,
         skipFinalSnapshot: bool = ...,
-        finalRelationalDatabaseSnapshotName: str = ...
+        finalRelationalDatabaseSnapshotName: str = ...,
     ) -> DeleteRelationalDatabaseResultTypeDef:
         """
         Deletes a database in Amazon Lightsail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.delete_relational_database)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#delete_relational_database)
         """
@@ -1097,15 +1097,15 @@
         """
 
     async def get_blueprints(
         self,
         *,
         includeInactive: bool = ...,
         pageToken: str = ...,
-        appCategory: Literal["LfR"] = ...
+        appCategory: Literal["LfR"] = ...,
     ) -> GetBlueprintsResultTypeDef:
         """
         Returns the list of available instance images, or *blueprints*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_blueprints)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#get_blueprints)
         """
@@ -1133,15 +1133,15 @@
         *,
         bucketName: str,
         metricName: BucketMetricNameType,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
         period: int,
         statistics: Sequence[MetricStatisticType],
-        unit: MetricUnitType
+        unit: MetricUnitType,
     ) -> GetBucketMetricDataResultTypeDef:
         """
         Returns the data points of a specific metric for an Amazon Lightsail bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_bucket_metric_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#get_bucket_metric_data)
         """
@@ -1157,15 +1157,15 @@
         """
 
     async def get_bundles(
         self,
         *,
         includeInactive: bool = ...,
         pageToken: str = ...,
-        appCategory: Literal["LfR"] = ...
+        appCategory: Literal["LfR"] = ...,
     ) -> GetBundlesResultTypeDef:
         """
         Returns the bundles that you can apply to an Amazon Lightsail instance when you
         create
         it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_bundles)
@@ -1174,15 +1174,15 @@
 
     async def get_certificates(
         self,
         *,
         certificateStatuses: Sequence[CertificateStatusType] = ...,
         includeCertificateDetails: bool = ...,
         certificateName: str = ...,
-        pageToken: str = ...
+        pageToken: str = ...,
     ) -> GetCertificatesResultTypeDef:
         """
         Returns information about one or more Amazon Lightsail SSL/TLS certificates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_certificates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#get_certificates)
         """
@@ -1233,15 +1233,15 @@
         self,
         *,
         serviceName: str,
         containerName: str,
         startTime: TimestampTypeDef = ...,
         endTime: TimestampTypeDef = ...,
         filterPattern: str = ...,
-        pageToken: str = ...
+        pageToken: str = ...,
     ) -> GetContainerLogResultTypeDef:
         """
         Returns the log events of a container of your Amazon Lightsail container
         service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_container_log)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#get_container_log)
@@ -1264,15 +1264,15 @@
         self,
         *,
         serviceName: str,
         metricName: ContainerServiceMetricNameType,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
         period: int,
-        statistics: Sequence[MetricStatisticType]
+        statistics: Sequence[MetricStatisticType],
     ) -> GetContainerServiceMetricDataResultTypeDef:
         """
         Returns the data points of a specific metric of your Amazon Lightsail container
         service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_container_service_metric_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#get_container_service_metric_data)
@@ -1371,15 +1371,15 @@
         *,
         distributionName: str,
         metricName: DistributionMetricNameType,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
         period: int,
         unit: MetricUnitType,
-        statistics: Sequence[MetricStatisticType]
+        statistics: Sequence[MetricStatisticType],
     ) -> GetDistributionMetricDataResultTypeDef:
         """
         Returns the data points of a specific metric for an Amazon Lightsail content
         delivery network (CDN)
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_distribution_metric_data)
@@ -1453,15 +1453,15 @@
         *,
         instanceName: str,
         metricName: InstanceMetricNameType,
         period: int,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
         unit: MetricUnitType,
-        statistics: Sequence[MetricStatisticType]
+        statistics: Sequence[MetricStatisticType],
     ) -> GetInstanceMetricDataResultTypeDef:
         """
         Returns the data points for the specified Amazon Lightsail instance metric,
         given an instance
         name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_instance_metric_data)
@@ -1548,15 +1548,15 @@
         *,
         loadBalancerName: str,
         metricName: LoadBalancerMetricNameType,
         period: int,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
         unit: MetricUnitType,
-        statistics: Sequence[MetricStatisticType]
+        statistics: Sequence[MetricStatisticType],
     ) -> GetLoadBalancerMetricDataResultTypeDef:
         """
         Returns information about health metrics for your Lightsail load balancer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_load_balancer_metric_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#get_load_balancer_metric_data)
         """
@@ -1618,15 +1618,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#get_operations_for_resource)
         """
 
     async def get_regions(
         self,
         *,
         includeAvailabilityZones: bool = ...,
-        includeRelationalDatabaseAvailabilityZones: bool = ...
+        includeRelationalDatabaseAvailabilityZones: bool = ...,
     ) -> GetRegionsResultTypeDef:
         """
         Returns a list of all valid regions for Amazon Lightsail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_regions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#get_regions)
         """
@@ -1675,15 +1675,15 @@
         self,
         *,
         relationalDatabaseName: str,
         logStreamName: str,
         startTime: TimestampTypeDef = ...,
         endTime: TimestampTypeDef = ...,
         startFromHead: bool = ...,
-        pageToken: str = ...
+        pageToken: str = ...,
     ) -> GetRelationalDatabaseLogEventsResultTypeDef:
         """
         Returns a list of log events for a database in Amazon Lightsail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_relational_database_log_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#get_relational_database_log_events)
         """
@@ -1699,15 +1699,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#get_relational_database_log_streams)
         """
 
     async def get_relational_database_master_user_password(
         self,
         *,
         relationalDatabaseName: str,
-        passwordVersion: RelationalDatabasePasswordVersionType = ...
+        passwordVersion: RelationalDatabasePasswordVersionType = ...,
     ) -> GetRelationalDatabaseMasterUserPasswordResultTypeDef:
         """
         Returns the current, previous, or pending versions of the master user password
         for a Lightsail
         database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_relational_database_master_user_password)
@@ -1719,15 +1719,15 @@
         *,
         relationalDatabaseName: str,
         metricName: RelationalDatabaseMetricNameType,
         period: int,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
         unit: MetricUnitType,
-        statistics: Sequence[MetricStatisticType]
+        statistics: Sequence[MetricStatisticType],
     ) -> GetRelationalDatabaseMetricDataResultTypeDef:
         """
         Returns the data points of the specified metric for a database in Amazon
         Lightsail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_relational_database_metric_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#get_relational_database_metric_data)
@@ -1838,15 +1838,15 @@
         comparisonOperator: ComparisonOperatorType,
         threshold: float,
         evaluationPeriods: int,
         datapointsToAlarm: int = ...,
         treatMissingData: TreatMissingDataType = ...,
         contactProtocols: Sequence[ContactProtocolType] = ...,
         notificationTriggers: Sequence[AlarmStateType] = ...,
-        notificationEnabled: bool = ...
+        notificationEnabled: bool = ...,
     ) -> PutAlarmResultTypeDef:
         """
         Creates or updates an alarm, and associates it with the specified metric.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.put_alarm)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#put_alarm)
         """
@@ -2043,15 +2043,15 @@
     async def update_bucket(
         self,
         *,
         bucketName: str,
         accessRules: AccessRulesTypeDef = ...,
         versioning: str = ...,
         readonlyAccessAccounts: Sequence[str] = ...,
-        accessLogConfig: BucketAccessLogConfigTypeDef = ...
+        accessLogConfig: BucketAccessLogConfigTypeDef = ...,
     ) -> UpdateBucketResultTypeDef:
         """
         Updates an existing Amazon Lightsail bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.update_bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#update_bucket)
         """
@@ -2070,15 +2070,15 @@
         self,
         *,
         serviceName: str,
         power: ContainerServicePowerNameType = ...,
         scale: int = ...,
         isDisabled: bool = ...,
         publicDomainNames: Mapping[str, Sequence[str]] = ...,
-        privateRegistryAccess: PrivateRegistryAccessRequestTypeDef = ...
+        privateRegistryAccess: PrivateRegistryAccessRequestTypeDef = ...,
     ) -> UpdateContainerServiceResultTypeDef:
         """
         Updates the configuration of your Amazon Lightsail container service, such as
         its power, scale, and public domain
         names.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.update_container_service)
@@ -2089,15 +2089,15 @@
         self,
         *,
         distributionName: str,
         origin: InputOriginTypeDef = ...,
         defaultCacheBehavior: CacheBehaviorTypeDef = ...,
         cacheBehaviorSettings: CacheSettingsTypeDef = ...,
         cacheBehaviors: Sequence[CacheBehaviorPerPathTypeDef] = ...,
-        isEnabled: bool = ...
+        isEnabled: bool = ...,
     ) -> UpdateDistributionResultTypeDef:
         """
         Updates an existing Amazon Lightsail content delivery network (CDN)
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.update_distribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#update_distribution)
@@ -2127,15 +2127,15 @@
     async def update_instance_metadata_options(
         self,
         *,
         instanceName: str,
         httpTokens: HttpTokensType = ...,
         httpEndpoint: HttpEndpointType = ...,
         httpPutResponseHopLimit: int = ...,
-        httpProtocolIpv6: HttpProtocolIpv6Type = ...
+        httpProtocolIpv6: HttpProtocolIpv6Type = ...,
     ) -> UpdateInstanceMetadataOptionsResultTypeDef:
         """
         Modifies the Amazon Lightsail instance metadata parameters on a running or
         stopped
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.update_instance_metadata_options)
@@ -2143,15 +2143,15 @@
         """
 
     async def update_load_balancer_attribute(
         self,
         *,
         loadBalancerName: str,
         attributeName: LoadBalancerAttributeNameType,
-        attributeValue: str
+        attributeValue: str,
     ) -> UpdateLoadBalancerAttributeResultTypeDef:
         """
         Updates the specified attribute for a load balancer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.update_load_balancer_attribute)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#update_load_balancer_attribute)
         """
@@ -2164,28 +2164,28 @@
         rotateMasterUserPassword: bool = ...,
         preferredBackupWindow: str = ...,
         preferredMaintenanceWindow: str = ...,
         enableBackupRetention: bool = ...,
         disableBackupRetention: bool = ...,
         publiclyAccessible: bool = ...,
         applyImmediately: bool = ...,
-        caCertificateIdentifier: str = ...
+        caCertificateIdentifier: str = ...,
     ) -> UpdateRelationalDatabaseResultTypeDef:
         """
         Allows the update of one or more attributes of a database in Amazon Lightsail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.update_relational_database)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#update_relational_database)
         """
 
     async def update_relational_database_parameters(
         self,
         *,
         relationalDatabaseName: str,
-        parameters: Sequence[RelationalDatabaseParameterTypeDef]
+        parameters: Sequence[RelationalDatabaseParameterTypeDef],
     ) -> UpdateRelationalDatabaseParametersResultTypeDef:
         """
         Allows the update of one or more parameters of a database in Amazon Lightsail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.update_relational_database_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#update_relational_database_parameters)
         """
```

### Comparing `types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail/literals.py` & `types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail/literals.py`

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
     "AccessDirectionType",
     "AccessTypeType",
     "AccountLevelBpaSyncStatusType",
     "AddOnTypeType",
     "AlarmStateType",
     "AppCategoryType",
@@ -122,15 +121,14 @@
     "LightsailServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AccessDirectionType = Literal["inbound", "outbound"]
 AccessTypeType = Literal["private", "public"]
 AccountLevelBpaSyncStatusType = Literal["Defaulted", "Failed", "InSync", "NeverSynced"]
 AddOnTypeType = Literal["AutoSnapshot", "StopInstanceOnIdle"]
 AlarmStateType = Literal["ALARM", "INSUFFICIENT_DATA", "OK"]
 AppCategoryType = Literal["LfR"]
 AutoMountStatusType = Literal["Failed", "Mounted", "NotMounted", "Pending"]
```

### Comparing `types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail/literals.pyi` & `types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail/paginator.py` & `types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "GetActiveNamesPaginator",
     "GetBlueprintsPaginator",
     "GetBundlesPaginator",
     "GetCloudFormationStackRecordsPaginator",
     "GetDiskSnapshotsPaginator",
     "GetDisksPaginator",
@@ -114,15 +113,14 @@
     "GetRelationalDatabaseEventsPaginator",
     "GetRelationalDatabaseParametersPaginator",
     "GetRelationalDatabaseSnapshotsPaginator",
     "GetRelationalDatabasesPaginator",
     "GetStaticIpsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -151,15 +149,15 @@
     """
 
     def paginate(
         self,
         *,
         includeInactive: bool = ...,
         appCategory: Literal["LfR"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetBlueprintsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetBlueprints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/paginators/#getblueprintspaginator)
         """
 
 
@@ -170,15 +168,15 @@
     """
 
     def paginate(
         self,
         *,
         includeInactive: bool = ...,
         appCategory: Literal["LfR"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetBundlesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetBundles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/paginators/#getbundlespaginator)
         """
 
 
@@ -369,15 +367,15 @@
     """
 
     def paginate(
         self,
         *,
         relationalDatabaseName: str,
         durationInMinutes: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetRelationalDatabaseEventsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/paginators/#getrelationaldatabaseeventspaginator)
         """
```

### Comparing `types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail/paginator.pyi` & `types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -146,15 +146,15 @@
     """
 
     def paginate(
         self,
         *,
         includeInactive: bool = ...,
         appCategory: Literal["LfR"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetBlueprintsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetBlueprints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/paginators/#getblueprintspaginator)
         """
 
 class GetBundlesPaginator(AioPaginator):
@@ -164,15 +164,15 @@
     """
 
     def paginate(
         self,
         *,
         includeInactive: bool = ...,
         appCategory: Literal["LfR"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetBundlesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetBundles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/paginators/#getbundlespaginator)
         """
 
 class GetCloudFormationStackRecordsPaginator(AioPaginator):
@@ -350,15 +350,15 @@
     """
 
     def paginate(
         self,
         *,
         relationalDatabaseName: str,
         durationInMinutes: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetRelationalDatabaseEventsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/paginators/#getrelationaldatabaseeventspaginator)
         """
 
 class GetRelationalDatabaseParametersPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail/type_defs.py` & `types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccessKeyLastUsedTypeDef",
     "AccessRulesTypeDef",
     "AccountLevelBpaSyncTypeDef",
     "AutoSnapshotAddOnRequestTypeDef",
     "StopInstanceOnIdleRequestTypeDef",
     "AddOnTypeDef",
```

### Comparing `types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail/type_defs.pyi` & `types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail.egg-info/PKG-INFO` & `types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lightsail
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Lightsail 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Lightsail 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/
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
 
 <a id="types-aiobotocore-lightsail"></a>
 
 # types-aiobotocore-lightsail
 
 [![PyPI - types-aiobotocore-lightsail](https://img.shields.io/pypi/v/types-aiobotocore-lightsail.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lightsail)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lightsail.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lightsail)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lightsail)](https://pepy.tech/project/types-aiobotocore-lightsail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Lightsail 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
+[aiobotocore.Lightsail 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
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
 [types-aiobotocore-lightsail docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-lightsail-2.9.0/types_aiobotocore_lightsail.egg-info/SOURCES.txt` & `types-aiobotocore-lightsail-2.9.1/types_aiobotocore_lightsail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

