# Comparing `tmp/types-aiobotocore-groundstation-2.9.0.tar.gz` & `tmp/types-aiobotocore-groundstation-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-groundstation-2.9.0.tar", last modified: Wed Dec 13 19:59:25 2023, max compression
+gzip compressed data, was "types-aiobotocore-groundstation-2.9.1.tar", last modified: Thu Jan 18 01:20:49 2024, max compression
```

## Comparing `types-aiobotocore-groundstation-2.9.0.tar` & `types-aiobotocore-groundstation-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:25.061714 types-aiobotocore-groundstation-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:47:05.000000 types-aiobotocore-groundstation-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14906 2023-12-13 19:59:25.061714 types-aiobotocore-groundstation-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13319 2023-12-13 19:47:05.000000 types-aiobotocore-groundstation-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:25.061714 types-aiobotocore-groundstation-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2023-12-13 19:47:05.000000 types-aiobotocore-groundstation-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:25.061714 types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation/
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2023-12-13 19:47:05.000000 types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2023-12-13 19:47:05.000000 types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      956 2023-12-13 19:47:05.000000 types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28819 2023-12-13 19:47:05.000000 types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    28815 2023-12-13 19:47:05.000000 types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11470 2023-12-13 19:47:05.000000 types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11468 2023-12-13 19:47:05.000000 types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9383 2023-12-13 19:47:05.000000 types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9374 2023-12-13 19:47:05.000000 types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:47:05.000000 types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    34482 2023-12-13 19:47:06.000000 types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    34481 2023-12-13 19:47:05.000000 types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:47:05.000000 types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2023-12-13 19:47:05.000000 types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2023-12-13 19:47:05.000000 types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:25.061714 types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14906 2023-12-13 19:59:25.000000 types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2023-12-13 19:59:25.000000 types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:25.000000 types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:25.000000 types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:25.000000 types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-13 19:59:25.000000 types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:49.053304 types-aiobotocore-groundstation-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:08:57.000000 types-aiobotocore-groundstation-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14926 2024-01-18 01:20:49.053304 types-aiobotocore-groundstation-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13319 2024-01-18 01:08:57.000000 types-aiobotocore-groundstation-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:49.053304 types-aiobotocore-groundstation-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-01-18 01:08:57.000000 types-aiobotocore-groundstation-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:49.049304 types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-01-18 01:08:57.000000 types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-01-18 01:08:57.000000 types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-01-18 01:08:57.000000 types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28827 2024-01-18 01:08:57.000000 types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28824 2024-01-18 01:08:57.000000 types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11468 2024-01-18 01:08:57.000000 types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11468 2024-01-18 01:08:57.000000 types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9384 2024-01-18 01:08:57.000000 types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9376 2024-01-18 01:08:57.000000 types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:08:57.000000 types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    34481 2024-01-18 01:08:58.000000 types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34481 2024-01-18 01:08:58.000000 types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:08:57.000000 types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-01-18 01:08:57.000000 types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-01-18 01:08:57.000000 types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:49.053304 types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14926 2024-01-18 01:20:49.000000 types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-01-18 01:20:49.000000 types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:49.000000 types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:49.000000 types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:49.000000 types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-18 01:20:49.000000 types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-groundstation-2.9.0/LICENSE` & `types-aiobotocore-groundstation-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-groundstation-2.9.0/PKG-INFO` & `types-aiobotocore-groundstation-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-groundstation
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.GroundStation 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.GroundStation 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/
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
 
 <a id="types-aiobotocore-groundstation"></a>
 
 # types-aiobotocore-groundstation
 
 [![PyPI - types-aiobotocore-groundstation](https://img.shields.io/pypi/v/types-aiobotocore-groundstation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-groundstation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-groundstation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-groundstation)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-groundstation)](https://pepy.tech/project/types-aiobotocore-groundstation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GroundStation 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
+[aiobotocore.GroundStation 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
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
 [types-aiobotocore-groundstation docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-groundstation-2.9.0/README.md` & `types-aiobotocore-groundstation-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-groundstation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-groundstation)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-groundstation)](https://pepy.tech/project/types-aiobotocore-groundstation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GroundStation 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
+[aiobotocore.GroundStation 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
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
 [types-aiobotocore-groundstation docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-groundstation-2.9.0/setup.py` & `types-aiobotocore-groundstation-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-groundstation",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_groundstation"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.GroundStation 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.GroundStation 2.9.1 service generated with"
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
     keywords="aiobotocore groundstation type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_groundstation": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation/__init__.py` & `types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     ListMissionProfilesPaginator,
     ListSatellitesPaginator,
 )
 from .waiter import ContactScheduledWaiter
 
 Client = GroundStationClient
 
-
 __all__ = (
     "Client",
     "ContactScheduledWaiter",
     "GroundStationClient",
     "ListConfigsPaginator",
     "ListContactsPaginator",
     "ListDataflowEndpointGroupsPaginator",
```

### Comparing `types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation/__init__.pyi` & `types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation/__main__.py` & `types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.GroundStation 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.GroundStation 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation\nOther"
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

### Comparing `types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation/client.py` & `types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -68,34 +68,30 @@
 from .waiter import ContactScheduledWaiter
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("GroundStationClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     DependencyException: Type[BotocoreClientError]
     InvalidParameterException: Type[BotocoreClientError]
     ResourceLimitExceededException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
 
-
 class GroundStationClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/client/)
     """
 
     meta: ClientMeta
@@ -145,15 +141,15 @@
 
     async def create_dataflow_endpoint_group(
         self,
         *,
         endpointDetails: Sequence[EndpointDetailsTypeDef],
         contactPostPassDurationSeconds: int = ...,
         contactPrePassDurationSeconds: int = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> DataflowEndpointGroupIdResponseTypeDef:
         """
         Creates a `DataflowEndpoint` group containing the specified list of
         `DataflowEndpoint`
         objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.create_dataflow_endpoint_group)
@@ -166,15 +162,15 @@
         name: str,
         satelliteId: str,
         enabled: bool = ...,
         ephemeris: EphemerisDataTypeDef = ...,
         expirationTime: TimestampTypeDef = ...,
         kmsKeyArn: str = ...,
         priority: int = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> EphemerisIdResponseTypeDef:
         """
         Creates an Ephemeris with the specified `EphemerisData`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.create_ephemeris)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/client/#create_ephemeris)
         """
@@ -186,15 +182,15 @@
         minimumViableContactDurationSeconds: int,
         name: str,
         trackingConfigArn: str,
         contactPostPassDurationSeconds: int = ...,
         contactPrePassDurationSeconds: int = ...,
         streamsKmsKey: KmsKeyTypeDef = ...,
         streamsKmsRole: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> MissionProfileIdResponseTypeDef:
         """
         Creates a mission profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.create_mission_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/client/#create_mission_profile)
         """
@@ -340,15 +336,15 @@
         endTime: TimestampTypeDef,
         startTime: TimestampTypeDef,
         statusList: Sequence[ContactStatusType],
         groundStation: str = ...,
         maxResults: int = ...,
         missionProfileArn: str = ...,
         nextToken: str = ...,
-        satelliteArn: str = ...
+        satelliteArn: str = ...,
     ) -> ListContactsResponseTypeDef:
         """
         Returns a list of contacts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.list_contacts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/client/#list_contacts)
         """
@@ -367,15 +363,15 @@
         self,
         *,
         endTime: TimestampTypeDef,
         satelliteId: str,
         startTime: TimestampTypeDef,
         maxResults: int = ...,
         nextToken: str = ...,
-        statusList: Sequence[EphemerisStatusType] = ...
+        statusList: Sequence[EphemerisStatusType] = ...,
     ) -> ListEphemeridesResponseTypeDef:
         """
         List existing ephemerides.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.list_ephemerides)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/client/#list_ephemerides)
         """
@@ -434,15 +430,15 @@
         self,
         *,
         endTime: TimestampTypeDef,
         groundStation: str,
         missionProfileArn: str,
         satelliteArn: str,
         startTime: TimestampTypeDef,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> ContactIdResponseTypeDef:
         """
         Reserves a contact using specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.reserve_contact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/client/#reserve_contact)
         """
@@ -465,30 +461,30 @@
 
     async def update_agent_status(
         self,
         *,
         agentId: str,
         aggregateStatus: AggregateStatusTypeDef,
         componentStatuses: Sequence[ComponentStatusDataTypeDef],
-        taskId: str
+        taskId: str,
     ) -> UpdateAgentStatusResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.update_agent_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/client/#update_agent_status)
         """
 
     async def update_config(
         self,
         *,
         configData: ConfigTypeDataTypeDef,
         configId: str,
         configType: ConfigCapabilityTypeType,
-        name: str
+        name: str,
     ) -> ConfigIdResponseTypeDef:
         """
         Updates the `Config` used when scheduling contacts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.update_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/client/#update_config)
         """
@@ -511,15 +507,15 @@
         contactPostPassDurationSeconds: int = ...,
         contactPrePassDurationSeconds: int = ...,
         dataflowEdges: Sequence[Sequence[str]] = ...,
         minimumViableContactDurationSeconds: int = ...,
         name: str = ...,
         streamsKmsKey: KmsKeyTypeDef = ...,
         streamsKmsRole: str = ...,
-        trackingConfigArn: str = ...
+        trackingConfigArn: str = ...,
     ) -> MissionProfileIdResponseTypeDef:
         """
         Updates a mission profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.update_mission_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/client/#update_mission_profile)
         """
```

### Comparing `types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation/client.pyi` & `types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,28 +70,31 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("GroundStationClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     DependencyException: Type[BotocoreClientError]
     InvalidParameterException: Type[BotocoreClientError]
     ResourceLimitExceededException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
 
+
 class GroundStationClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/client/)
     """
 
     meta: ClientMeta
@@ -141,15 +144,15 @@
 
     async def create_dataflow_endpoint_group(
         self,
         *,
         endpointDetails: Sequence[EndpointDetailsTypeDef],
         contactPostPassDurationSeconds: int = ...,
         contactPrePassDurationSeconds: int = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> DataflowEndpointGroupIdResponseTypeDef:
         """
         Creates a `DataflowEndpoint` group containing the specified list of
         `DataflowEndpoint`
         objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.create_dataflow_endpoint_group)
@@ -162,15 +165,15 @@
         name: str,
         satelliteId: str,
         enabled: bool = ...,
         ephemeris: EphemerisDataTypeDef = ...,
         expirationTime: TimestampTypeDef = ...,
         kmsKeyArn: str = ...,
         priority: int = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> EphemerisIdResponseTypeDef:
         """
         Creates an Ephemeris with the specified `EphemerisData`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.create_ephemeris)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/client/#create_ephemeris)
         """
@@ -182,15 +185,15 @@
         minimumViableContactDurationSeconds: int,
         name: str,
         trackingConfigArn: str,
         contactPostPassDurationSeconds: int = ...,
         contactPrePassDurationSeconds: int = ...,
         streamsKmsKey: KmsKeyTypeDef = ...,
         streamsKmsRole: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> MissionProfileIdResponseTypeDef:
         """
         Creates a mission profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.create_mission_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/client/#create_mission_profile)
         """
@@ -336,15 +339,15 @@
         endTime: TimestampTypeDef,
         startTime: TimestampTypeDef,
         statusList: Sequence[ContactStatusType],
         groundStation: str = ...,
         maxResults: int = ...,
         missionProfileArn: str = ...,
         nextToken: str = ...,
-        satelliteArn: str = ...
+        satelliteArn: str = ...,
     ) -> ListContactsResponseTypeDef:
         """
         Returns a list of contacts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.list_contacts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/client/#list_contacts)
         """
@@ -363,15 +366,15 @@
         self,
         *,
         endTime: TimestampTypeDef,
         satelliteId: str,
         startTime: TimestampTypeDef,
         maxResults: int = ...,
         nextToken: str = ...,
-        statusList: Sequence[EphemerisStatusType] = ...
+        statusList: Sequence[EphemerisStatusType] = ...,
     ) -> ListEphemeridesResponseTypeDef:
         """
         List existing ephemerides.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.list_ephemerides)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/client/#list_ephemerides)
         """
@@ -430,15 +433,15 @@
         self,
         *,
         endTime: TimestampTypeDef,
         groundStation: str,
         missionProfileArn: str,
         satelliteArn: str,
         startTime: TimestampTypeDef,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> ContactIdResponseTypeDef:
         """
         Reserves a contact using specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.reserve_contact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/client/#reserve_contact)
         """
@@ -461,30 +464,30 @@
 
     async def update_agent_status(
         self,
         *,
         agentId: str,
         aggregateStatus: AggregateStatusTypeDef,
         componentStatuses: Sequence[ComponentStatusDataTypeDef],
-        taskId: str
+        taskId: str,
     ) -> UpdateAgentStatusResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.update_agent_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/client/#update_agent_status)
         """
 
     async def update_config(
         self,
         *,
         configData: ConfigTypeDataTypeDef,
         configId: str,
         configType: ConfigCapabilityTypeType,
-        name: str
+        name: str,
     ) -> ConfigIdResponseTypeDef:
         """
         Updates the `Config` used when scheduling contacts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.update_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/client/#update_config)
         """
@@ -507,15 +510,15 @@
         contactPostPassDurationSeconds: int = ...,
         contactPrePassDurationSeconds: int = ...,
         dataflowEdges: Sequence[Sequence[str]] = ...,
         minimumViableContactDurationSeconds: int = ...,
         name: str = ...,
         streamsKmsKey: KmsKeyTypeDef = ...,
         streamsKmsRole: str = ...,
-        trackingConfigArn: str = ...
+        trackingConfigArn: str = ...,
     ) -> MissionProfileIdResponseTypeDef:
         """
         Updates a mission profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.update_mission_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/client/#update_mission_profile)
         """
```

### Comparing `types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation/literals.py` & `types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation/literals.py`

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
     "AgentStatusType",
     "AngleUnitsType",
     "AuditResultsType",
     "BandwidthUnitsType",
     "CapabilityHealthReasonType",
     "CapabilityHealthType",
@@ -49,15 +48,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AgentStatusType = Literal["ACTIVE", "FAILED", "INACTIVE", "SUCCESS"]
 AngleUnitsType = Literal["DEGREE_ANGLE", "RADIAN"]
 AuditResultsType = Literal["HEALTHY", "UNHEALTHY"]
 BandwidthUnitsType = Literal["GHz", "MHz", "kHz"]
 CapabilityHealthReasonType = Literal[
     "DATAPLANE_FAILURE",
     "HEALTHY",
```

### Comparing `types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation/literals.pyi` & `types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation/paginator.py` & `types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,14 @@
     "ListDataflowEndpointGroupsPaginator",
     "ListEphemeridesPaginator",
     "ListGroundStationsPaginator",
     "ListMissionProfilesPaginator",
     "ListSatellitesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -98,15 +97,15 @@
         *,
         endTime: TimestampTypeDef,
         startTime: TimestampTypeDef,
         statusList: Sequence[ContactStatusType],
         groundStation: str = ...,
         missionProfileArn: str = ...,
         satelliteArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListContactsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListContacts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/paginators/#listcontactspaginator)
         """
 
 
@@ -134,15 +133,15 @@
     def paginate(
         self,
         *,
         endTime: TimestampTypeDef,
         satelliteId: str,
         startTime: TimestampTypeDef,
         statusList: Sequence[EphemerisStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEphemeridesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListEphemerides.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/paginators/#listephemeridespaginator)
         """
```

### Comparing `types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation/paginator.pyi` & `types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         *,
         endTime: TimestampTypeDef,
         startTime: TimestampTypeDef,
         statusList: Sequence[ContactStatusType],
         groundStation: str = ...,
         missionProfileArn: str = ...,
         satelliteArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListContactsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListContacts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/paginators/#listcontactspaginator)
         """
 
 class ListDataflowEndpointGroupsPaginator(AioPaginator):
@@ -128,15 +128,15 @@
     def paginate(
         self,
         *,
         endTime: TimestampTypeDef,
         satelliteId: str,
         startTime: TimestampTypeDef,
         statusList: Sequence[EphemerisStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEphemeridesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListEphemerides.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/paginators/#listephemeridespaginator)
         """
 
 class ListGroundStationsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation/type_defs.py` & `types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ComponentVersionTypeDef",
     "AggregateStatusTypeDef",
     "AntennaDemodDecodeDetailsTypeDef",
     "DecodeConfigTypeDef",
     "DemodulationConfigTypeDef",
     "EirpTypeDef",
```

### Comparing `types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation/type_defs.pyi` & `types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation/waiter.py` & `types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation/waiter.pyi` & `types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation.egg-info/PKG-INFO` & `types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-groundstation
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.GroundStation 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.GroundStation 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/
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
 
 <a id="types-aiobotocore-groundstation"></a>
 
 # types-aiobotocore-groundstation
 
 [![PyPI - types-aiobotocore-groundstation](https://img.shields.io/pypi/v/types-aiobotocore-groundstation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-groundstation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-groundstation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-groundstation)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-groundstation)](https://pepy.tech/project/types-aiobotocore-groundstation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GroundStation 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
+[aiobotocore.GroundStation 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
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
 [types-aiobotocore-groundstation docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-groundstation-2.9.0/types_aiobotocore_groundstation.egg-info/SOURCES.txt` & `types-aiobotocore-groundstation-2.9.1/types_aiobotocore_groundstation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

