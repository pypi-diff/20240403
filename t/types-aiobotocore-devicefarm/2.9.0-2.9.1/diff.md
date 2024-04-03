# Comparing `tmp/types-aiobotocore-devicefarm-2.9.0.tar.gz` & `tmp/types-aiobotocore-devicefarm-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-devicefarm-2.9.0.tar", last modified: Wed Dec 13 19:59:05 2023, max compression
+gzip compressed data, was "types-aiobotocore-devicefarm-2.9.1.tar", last modified: Thu Jan 18 01:20:31 2024, max compression
```

## Comparing `types-aiobotocore-devicefarm-2.9.0.tar` & `types-aiobotocore-devicefarm-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:05.693841 types-aiobotocore-devicefarm-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:44:01.000000 types-aiobotocore-devicefarm-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15786 2023-12-13 19:59:05.693841 types-aiobotocore-devicefarm-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14211 2023-12-13 19:44:01.000000 types-aiobotocore-devicefarm-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:05.693841 types-aiobotocore-devicefarm-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2023-12-13 19:44:01.000000 types-aiobotocore-devicefarm-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:05.693841 types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm/
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2023-12-13 19:44:01.000000 types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2023-12-13 19:44:01.000000 types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      944 2023-12-13 19:44:01.000000 types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    61030 2023-12-13 19:44:01.000000 types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    61026 2023-12-13 19:44:01.000000 types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16287 2023-12-13 19:44:01.000000 types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    16285 2023-12-13 19:44:01.000000 types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    23439 2023-12-13 19:44:01.000000 types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    23417 2023-12-13 19:44:01.000000 types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:44:01.000000 types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    67302 2023-12-13 19:44:04.000000 types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    67301 2023-12-13 19:44:02.000000 types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:44:01.000000 types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:05.693841 types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15786 2023-12-13 19:59:05.000000 types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      870 2023-12-13 19:59:05.000000 types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:05.000000 types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:05.000000 types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:05.000000 types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-13 19:59:05.000000 types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:31.161390 types-aiobotocore-devicefarm-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:05:56.000000 types-aiobotocore-devicefarm-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15806 2024-01-18 01:20:31.161390 types-aiobotocore-devicefarm-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14211 2024-01-18 01:05:56.000000 types-aiobotocore-devicefarm-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:31.161390 types-aiobotocore-devicefarm-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-01-18 01:05:55.000000 types-aiobotocore-devicefarm-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:31.157390 types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm/
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-01-18 01:05:56.000000 types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-01-18 01:05:56.000000 types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-01-18 01:05:56.000000 types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61044 2024-01-18 01:05:56.000000 types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61041 2024-01-18 01:05:56.000000 types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-01-18 01:05:56.000000 types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-01-18 01:05:56.000000 types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    23443 2024-01-18 01:05:56.000000 types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23422 2024-01-18 01:05:56.000000 types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:05:56.000000 types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    67301 2024-01-18 01:05:59.000000 types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67301 2024-01-18 01:05:57.000000 types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:05:56.000000 types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:31.161390 types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15806 2024-01-18 01:20:31.000000 types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-01-18 01:20:31.000000 types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:31.000000 types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:31.000000 types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:31.000000 types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-18 01:20:31.000000 types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-devicefarm-2.9.0/LICENSE` & `types-aiobotocore-devicefarm-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-devicefarm-2.9.0/PKG-INFO` & `types-aiobotocore-devicefarm-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-devicefarm
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.DeviceFarm 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.DeviceFarm 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/
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
 
 <a id="types-aiobotocore-devicefarm"></a>
 
 # types-aiobotocore-devicefarm
 
 [![PyPI - types-aiobotocore-devicefarm](https://img.shields.io/pypi/v/types-aiobotocore-devicefarm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-devicefarm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-devicefarm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-devicefarm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-devicefarm)](https://pepy.tech/project/types-aiobotocore-devicefarm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DeviceFarm 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
+[aiobotocore.DeviceFarm 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
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
 [types-aiobotocore-devicefarm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-devicefarm-2.9.0/README.md` & `types-aiobotocore-devicefarm-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-devicefarm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-devicefarm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-devicefarm)](https://pepy.tech/project/types-aiobotocore-devicefarm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DeviceFarm 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
+[aiobotocore.DeviceFarm 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
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
 [types-aiobotocore-devicefarm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-devicefarm-2.9.0/setup.py` & `types-aiobotocore-devicefarm-2.9.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-devicefarm",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_devicefarm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.DeviceFarm 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.DeviceFarm 2.9.1 service generated with"
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
     keywords="aiobotocore devicefarm type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_devicefarm": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm/__init__.py` & `types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,14 @@
     ListUniqueProblemsPaginator,
     ListUploadsPaginator,
     ListVPCEConfigurationsPaginator,
 )
 
 Client = DeviceFarmClient
 
-
 __all__ = (
     "Client",
     "DeviceFarmClient",
     "GetOfferingStatusPaginator",
     "ListArtifactsPaginator",
     "ListDeviceInstancesPaginator",
     "ListDevicePoolsPaginator",
```

### Comparing `types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm/__init__.pyi` & `types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm/__main__.py` & `types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DeviceFarm 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.DeviceFarm 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm\nOther"
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

### Comparing `types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm/client.py` & `types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -134,26 +134,23 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("DeviceFarmClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ArgumentException: Type[BotocoreClientError]
     CannotDeleteException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     IdempotencyException: Type[BotocoreClientError]
     InternalServiceException: Type[BotocoreClientError]
     InvalidOperationException: Type[BotocoreClientError]
@@ -161,15 +158,14 @@
     NotEligibleException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     ServiceAccountException: Type[BotocoreClientError]
     TagOperationException: Type[BotocoreClientError]
     TagPolicyException: Type[BotocoreClientError]
     TooManyTagsException: Type[BotocoreClientError]
 
-
 class DeviceFarmClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/)
     """
 
     meta: ClientMeta
@@ -202,15 +198,15 @@
     async def create_device_pool(
         self,
         *,
         projectArn: str,
         name: str,
         rules: Sequence[RuleTypeDef],
         description: str = ...,
-        maxDevices: int = ...
+        maxDevices: int = ...,
     ) -> CreateDevicePoolResultTypeDef:
         """
         Creates a device pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.create_device_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#create_device_pool)
         """
@@ -218,15 +214,15 @@
     async def create_instance_profile(
         self,
         *,
         name: str,
         description: str = ...,
         packageCleanup: bool = ...,
         excludeAppPackagesFromCleanup: Sequence[str] = ...,
-        rebootAfterUse: bool = ...
+        rebootAfterUse: bool = ...,
     ) -> CreateInstanceProfileResultTypeDef:
         """
         Creates a profile that can be applied to one or more private fleet device
         instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.create_instance_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#create_instance_profile)
@@ -242,15 +238,15 @@
         uplinkBandwidthBits: int = ...,
         downlinkBandwidthBits: int = ...,
         uplinkDelayMs: int = ...,
         downlinkDelayMs: int = ...,
         uplinkJitterMs: int = ...,
         downlinkJitterMs: int = ...,
         uplinkLossPercent: int = ...,
-        downlinkLossPercent: int = ...
+        downlinkLossPercent: int = ...,
     ) -> CreateNetworkProfileResultTypeDef:
         """
         Creates a network profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.create_network_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#create_network_profile)
         """
@@ -275,15 +271,15 @@
         remoteDebugEnabled: bool = ...,
         remoteRecordEnabled: bool = ...,
         remoteRecordAppArn: str = ...,
         name: str = ...,
         clientId: str = ...,
         configuration: CreateRemoteAccessSessionConfigurationTypeDef = ...,
         interactionMode: InteractionModeType = ...,
-        skipAppResign: bool = ...
+        skipAppResign: bool = ...,
     ) -> CreateRemoteAccessSessionResultTypeDef:
         """
         Specifies and starts a remote access session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.create_remote_access_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#create_remote_access_session)
         """
@@ -322,15 +318,15 @@
 
     async def create_vpce_configuration(
         self,
         *,
         vpceConfigurationName: str,
         vpceServiceName: str,
         serviceDnsName: str,
-        vpceConfigurationDescription: str = ...
+        vpceConfigurationDescription: str = ...,
     ) -> CreateVPCEConfigurationResultTypeDef:
         """
         Creates a configuration record in Device Farm for your Amazon Virtual Private
         Cloud (VPC)
         endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.create_vpce_configuration)
@@ -461,15 +457,15 @@
     async def get_device_pool_compatibility(
         self,
         *,
         devicePoolArn: str,
         appArn: str = ...,
         testType: TestTypeType = ...,
         test: ScheduleRunTestTypeDef = ...,
-        configuration: ScheduleRunConfigurationTypeDef = ...
+        configuration: ScheduleRunConfigurationTypeDef = ...,
     ) -> GetDevicePoolCompatibilityResultTypeDef:
         """
         Gets information about compatibility with a device pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.get_device_pool_compatibility)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#get_device_pool_compatibility)
         """
@@ -772,15 +768,15 @@
 
     async def list_test_grid_session_artifacts(
         self,
         *,
         sessionArn: str,
         type: TestGridSessionArtifactCategoryType = ...,
         maxResult: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListTestGridSessionArtifactsResultTypeDef:
         """
         Retrieves a list of artifacts created during the session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.list_test_grid_session_artifacts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#list_test_grid_session_artifacts)
         """
@@ -791,15 +787,15 @@
         projectArn: str,
         status: TestGridSessionStatusType = ...,
         creationTimeAfter: TimestampTypeDef = ...,
         creationTimeBefore: TimestampTypeDef = ...,
         endTimeAfter: TimestampTypeDef = ...,
         endTimeBefore: TimestampTypeDef = ...,
         maxResult: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListTestGridSessionsResultTypeDef:
         """
         Retrieves a list of sessions for a  TestGridProject.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.list_test_grid_sessions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#list_test_grid_sessions)
         """
@@ -870,15 +866,15 @@
         projectArn: str,
         test: ScheduleRunTestTypeDef,
         appArn: str = ...,
         devicePoolArn: str = ...,
         deviceSelectionConfiguration: DeviceSelectionConfigurationTypeDef = ...,
         name: str = ...,
         configuration: ScheduleRunConfigurationTypeDef = ...,
-        executionConfiguration: ExecutionConfigurationTypeDef = ...
+        executionConfiguration: ExecutionConfigurationTypeDef = ...,
     ) -> ScheduleRunResultTypeDef:
         """
         Schedules a run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.schedule_run)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#schedule_run)
         """
@@ -937,15 +933,15 @@
         self,
         *,
         arn: str,
         name: str = ...,
         description: str = ...,
         rules: Sequence[RuleTypeDef] = ...,
         maxDevices: int = ...,
-        clearMaxDevices: bool = ...
+        clearMaxDevices: bool = ...,
     ) -> UpdateDevicePoolResultTypeDef:
         """
         Modifies the name, description, and rules in a device pool given the attributes
         and the pool
         ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.update_device_pool)
@@ -956,15 +952,15 @@
         self,
         *,
         arn: str,
         name: str = ...,
         description: str = ...,
         packageCleanup: bool = ...,
         excludeAppPackagesFromCleanup: Sequence[str] = ...,
-        rebootAfterUse: bool = ...
+        rebootAfterUse: bool = ...,
     ) -> UpdateInstanceProfileResultTypeDef:
         """
         Updates information about an existing private device instance profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.update_instance_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#update_instance_profile)
         """
@@ -979,45 +975,45 @@
         uplinkBandwidthBits: int = ...,
         downlinkBandwidthBits: int = ...,
         uplinkDelayMs: int = ...,
         downlinkDelayMs: int = ...,
         uplinkJitterMs: int = ...,
         downlinkJitterMs: int = ...,
         uplinkLossPercent: int = ...,
-        downlinkLossPercent: int = ...
+        downlinkLossPercent: int = ...,
     ) -> UpdateNetworkProfileResultTypeDef:
         """
         Updates the network profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.update_network_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#update_network_profile)
         """
 
     async def update_project(
         self,
         *,
         arn: str,
         name: str = ...,
         defaultJobTimeoutMinutes: int = ...,
-        vpcConfig: VpcConfigTypeDef = ...
+        vpcConfig: VpcConfigTypeDef = ...,
     ) -> UpdateProjectResultTypeDef:
         """
         Modifies the specified project name, given the project ARN and a new name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.update_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#update_project)
         """
 
     async def update_test_grid_project(
         self,
         *,
         projectArn: str,
         name: str = ...,
         description: str = ...,
-        vpcConfig: TestGridVpcConfigTypeDef = ...
+        vpcConfig: TestGridVpcConfigTypeDef = ...,
     ) -> UpdateTestGridProjectResultTypeDef:
         """
         Change details of a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.update_test_grid_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#update_test_grid_project)
         """
@@ -1035,15 +1031,15 @@
     async def update_vpce_configuration(
         self,
         *,
         arn: str,
         vpceConfigurationName: str = ...,
         vpceServiceName: str = ...,
         serviceDnsName: str = ...,
-        vpceConfigurationDescription: str = ...
+        vpceConfigurationDescription: str = ...,
     ) -> UpdateVPCEConfigurationResultTypeDef:
         """
         Updates information about an Amazon Virtual Private Cloud (VPC) endpoint
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.update_vpce_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#update_vpce_configuration)
```

### Comparing `types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm/client.pyi` & `types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,21 +136,23 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("DeviceFarmClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ArgumentException: Type[BotocoreClientError]
     CannotDeleteException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     IdempotencyException: Type[BotocoreClientError]
     InternalServiceException: Type[BotocoreClientError]
     InvalidOperationException: Type[BotocoreClientError]
@@ -158,14 +160,15 @@
     NotEligibleException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     ServiceAccountException: Type[BotocoreClientError]
     TagOperationException: Type[BotocoreClientError]
     TagPolicyException: Type[BotocoreClientError]
     TooManyTagsException: Type[BotocoreClientError]
 
+
 class DeviceFarmClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/)
     """
 
     meta: ClientMeta
@@ -198,15 +201,15 @@
     async def create_device_pool(
         self,
         *,
         projectArn: str,
         name: str,
         rules: Sequence[RuleTypeDef],
         description: str = ...,
-        maxDevices: int = ...
+        maxDevices: int = ...,
     ) -> CreateDevicePoolResultTypeDef:
         """
         Creates a device pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.create_device_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#create_device_pool)
         """
@@ -214,15 +217,15 @@
     async def create_instance_profile(
         self,
         *,
         name: str,
         description: str = ...,
         packageCleanup: bool = ...,
         excludeAppPackagesFromCleanup: Sequence[str] = ...,
-        rebootAfterUse: bool = ...
+        rebootAfterUse: bool = ...,
     ) -> CreateInstanceProfileResultTypeDef:
         """
         Creates a profile that can be applied to one or more private fleet device
         instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.create_instance_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#create_instance_profile)
@@ -238,15 +241,15 @@
         uplinkBandwidthBits: int = ...,
         downlinkBandwidthBits: int = ...,
         uplinkDelayMs: int = ...,
         downlinkDelayMs: int = ...,
         uplinkJitterMs: int = ...,
         downlinkJitterMs: int = ...,
         uplinkLossPercent: int = ...,
-        downlinkLossPercent: int = ...
+        downlinkLossPercent: int = ...,
     ) -> CreateNetworkProfileResultTypeDef:
         """
         Creates a network profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.create_network_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#create_network_profile)
         """
@@ -271,15 +274,15 @@
         remoteDebugEnabled: bool = ...,
         remoteRecordEnabled: bool = ...,
         remoteRecordAppArn: str = ...,
         name: str = ...,
         clientId: str = ...,
         configuration: CreateRemoteAccessSessionConfigurationTypeDef = ...,
         interactionMode: InteractionModeType = ...,
-        skipAppResign: bool = ...
+        skipAppResign: bool = ...,
     ) -> CreateRemoteAccessSessionResultTypeDef:
         """
         Specifies and starts a remote access session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.create_remote_access_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#create_remote_access_session)
         """
@@ -318,15 +321,15 @@
 
     async def create_vpce_configuration(
         self,
         *,
         vpceConfigurationName: str,
         vpceServiceName: str,
         serviceDnsName: str,
-        vpceConfigurationDescription: str = ...
+        vpceConfigurationDescription: str = ...,
     ) -> CreateVPCEConfigurationResultTypeDef:
         """
         Creates a configuration record in Device Farm for your Amazon Virtual Private
         Cloud (VPC)
         endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.create_vpce_configuration)
@@ -457,15 +460,15 @@
     async def get_device_pool_compatibility(
         self,
         *,
         devicePoolArn: str,
         appArn: str = ...,
         testType: TestTypeType = ...,
         test: ScheduleRunTestTypeDef = ...,
-        configuration: ScheduleRunConfigurationTypeDef = ...
+        configuration: ScheduleRunConfigurationTypeDef = ...,
     ) -> GetDevicePoolCompatibilityResultTypeDef:
         """
         Gets information about compatibility with a device pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.get_device_pool_compatibility)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#get_device_pool_compatibility)
         """
@@ -768,15 +771,15 @@
 
     async def list_test_grid_session_artifacts(
         self,
         *,
         sessionArn: str,
         type: TestGridSessionArtifactCategoryType = ...,
         maxResult: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListTestGridSessionArtifactsResultTypeDef:
         """
         Retrieves a list of artifacts created during the session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.list_test_grid_session_artifacts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#list_test_grid_session_artifacts)
         """
@@ -787,15 +790,15 @@
         projectArn: str,
         status: TestGridSessionStatusType = ...,
         creationTimeAfter: TimestampTypeDef = ...,
         creationTimeBefore: TimestampTypeDef = ...,
         endTimeAfter: TimestampTypeDef = ...,
         endTimeBefore: TimestampTypeDef = ...,
         maxResult: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListTestGridSessionsResultTypeDef:
         """
         Retrieves a list of sessions for a  TestGridProject.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.list_test_grid_sessions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#list_test_grid_sessions)
         """
@@ -866,15 +869,15 @@
         projectArn: str,
         test: ScheduleRunTestTypeDef,
         appArn: str = ...,
         devicePoolArn: str = ...,
         deviceSelectionConfiguration: DeviceSelectionConfigurationTypeDef = ...,
         name: str = ...,
         configuration: ScheduleRunConfigurationTypeDef = ...,
-        executionConfiguration: ExecutionConfigurationTypeDef = ...
+        executionConfiguration: ExecutionConfigurationTypeDef = ...,
     ) -> ScheduleRunResultTypeDef:
         """
         Schedules a run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.schedule_run)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#schedule_run)
         """
@@ -933,15 +936,15 @@
         self,
         *,
         arn: str,
         name: str = ...,
         description: str = ...,
         rules: Sequence[RuleTypeDef] = ...,
         maxDevices: int = ...,
-        clearMaxDevices: bool = ...
+        clearMaxDevices: bool = ...,
     ) -> UpdateDevicePoolResultTypeDef:
         """
         Modifies the name, description, and rules in a device pool given the attributes
         and the pool
         ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.update_device_pool)
@@ -952,15 +955,15 @@
         self,
         *,
         arn: str,
         name: str = ...,
         description: str = ...,
         packageCleanup: bool = ...,
         excludeAppPackagesFromCleanup: Sequence[str] = ...,
-        rebootAfterUse: bool = ...
+        rebootAfterUse: bool = ...,
     ) -> UpdateInstanceProfileResultTypeDef:
         """
         Updates information about an existing private device instance profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.update_instance_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#update_instance_profile)
         """
@@ -975,45 +978,45 @@
         uplinkBandwidthBits: int = ...,
         downlinkBandwidthBits: int = ...,
         uplinkDelayMs: int = ...,
         downlinkDelayMs: int = ...,
         uplinkJitterMs: int = ...,
         downlinkJitterMs: int = ...,
         uplinkLossPercent: int = ...,
-        downlinkLossPercent: int = ...
+        downlinkLossPercent: int = ...,
     ) -> UpdateNetworkProfileResultTypeDef:
         """
         Updates the network profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.update_network_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#update_network_profile)
         """
 
     async def update_project(
         self,
         *,
         arn: str,
         name: str = ...,
         defaultJobTimeoutMinutes: int = ...,
-        vpcConfig: VpcConfigTypeDef = ...
+        vpcConfig: VpcConfigTypeDef = ...,
     ) -> UpdateProjectResultTypeDef:
         """
         Modifies the specified project name, given the project ARN and a new name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.update_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#update_project)
         """
 
     async def update_test_grid_project(
         self,
         *,
         projectArn: str,
         name: str = ...,
         description: str = ...,
-        vpcConfig: TestGridVpcConfigTypeDef = ...
+        vpcConfig: TestGridVpcConfigTypeDef = ...,
     ) -> UpdateTestGridProjectResultTypeDef:
         """
         Change details of a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.update_test_grid_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#update_test_grid_project)
         """
@@ -1031,15 +1034,15 @@
     async def update_vpce_configuration(
         self,
         *,
         arn: str,
         vpceConfigurationName: str = ...,
         vpceServiceName: str = ...,
         serviceDnsName: str = ...,
-        vpceConfigurationDescription: str = ...
+        vpceConfigurationDescription: str = ...,
     ) -> UpdateVPCEConfigurationResultTypeDef:
         """
         Updates information about an Amazon Virtual Private Cloud (VPC) endpoint
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.update_vpce_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#update_vpce_configuration)
```

### Comparing `types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm/literals.py` & `types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm/literals.py`

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
     "ArtifactCategoryType",
     "ArtifactTypeType",
     "BillingMethodType",
     "CurrencyCodeType",
     "DeviceAttributeType",
     "DeviceAvailabilityType",
@@ -72,15 +71,14 @@
     "DeviceFarmServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ArtifactCategoryType = Literal["FILE", "LOG", "SCREENSHOT"]
 ArtifactTypeType = Literal[
     "APPIUM_JAVA_OUTPUT",
     "APPIUM_JAVA_XML_OUTPUT",
     "APPIUM_PYTHON_OUTPUT",
     "APPIUM_PYTHON_XML_OUTPUT",
     "APPIUM_SERVER_OUTPUT",
```

### Comparing `types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm/literals.pyi` & `types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm/paginator.py` & `types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,14 @@
     "ListSuitesPaginator",
     "ListTestsPaginator",
     "ListUniqueProblemsPaginator",
     "ListUploadsPaginator",
     "ListVPCEConfigurationsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -151,15 +150,15 @@
     """
 
     def paginate(
         self,
         *,
         arn: str,
         type: ArtifactCategoryType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListArtifactsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListArtifacts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/paginators/#listartifactspaginator)
         """
 
 
@@ -185,15 +184,15 @@
     """
 
     def paginate(
         self,
         *,
         arn: str,
         type: DevicePoolTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDevicePoolsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListDevicePools.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/paginators/#listdevicepoolspaginator)
         """
 
 
@@ -204,15 +203,15 @@
     """
 
     def paginate(
         self,
         *,
         arn: str = ...,
         filters: Sequence[DeviceFilterPaginatorTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDevicesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListDevices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/paginators/#listdevicespaginator)
         """
 
 
@@ -253,15 +252,15 @@
     """
 
     def paginate(
         self,
         *,
         arn: str,
         type: NetworkProfileTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListNetworkProfilesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListNetworkProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/paginators/#listnetworkprofilespaginator)
         """
 
 
@@ -422,15 +421,15 @@
     """
 
     def paginate(
         self,
         *,
         arn: str,
         type: UploadTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListUploadsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListUploads.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/paginators/#listuploadspaginator)
         """
```

### Comparing `types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm/paginator.pyi` & `types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
     """
 
     def paginate(
         self,
         *,
         arn: str,
         type: ArtifactCategoryType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListArtifactsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListArtifacts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/paginators/#listartifactspaginator)
         """
 
 class ListDeviceInstancesPaginator(AioPaginator):
@@ -179,15 +179,15 @@
     """
 
     def paginate(
         self,
         *,
         arn: str,
         type: DevicePoolTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDevicePoolsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListDevicePools.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/paginators/#listdevicepoolspaginator)
         """
 
 class ListDevicesPaginator(AioPaginator):
@@ -197,15 +197,15 @@
     """
 
     def paginate(
         self,
         *,
         arn: str = ...,
         filters: Sequence[DeviceFilterPaginatorTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDevicesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListDevices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/paginators/#listdevicespaginator)
         """
 
 class ListInstanceProfilesPaginator(AioPaginator):
@@ -243,15 +243,15 @@
     """
 
     def paginate(
         self,
         *,
         arn: str,
         type: NetworkProfileTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListNetworkProfilesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListNetworkProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/paginators/#listnetworkprofilespaginator)
         """
 
 class ListOfferingPromotionsPaginator(AioPaginator):
@@ -401,15 +401,15 @@
     """
 
     def paginate(
         self,
         *,
         arn: str,
         type: UploadTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListUploadsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListUploads.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/paginators/#listuploadspaginator)
         """
 
 class ListVPCEConfigurationsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm/type_defs.py` & `types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TrialMinutesTypeDef",
     "ArtifactTypeDef",
     "CPUTypeDef",
     "CountersTypeDef",
     "RuleTypeDef",
     "ResponseMetadataTypeDef",
```

### Comparing `types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm/type_defs.pyi` & `types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm.egg-info/PKG-INFO` & `types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-devicefarm
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.DeviceFarm 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.DeviceFarm 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/
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
 
 <a id="types-aiobotocore-devicefarm"></a>
 
 # types-aiobotocore-devicefarm
 
 [![PyPI - types-aiobotocore-devicefarm](https://img.shields.io/pypi/v/types-aiobotocore-devicefarm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-devicefarm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-devicefarm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-devicefarm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-devicefarm)](https://pepy.tech/project/types-aiobotocore-devicefarm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DeviceFarm 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
+[aiobotocore.DeviceFarm 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
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
 [types-aiobotocore-devicefarm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-devicefarm-2.9.0/types_aiobotocore_devicefarm.egg-info/SOURCES.txt` & `types-aiobotocore-devicefarm-2.9.1/types_aiobotocore_devicefarm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

