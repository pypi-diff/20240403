# Comparing `tmp/types-aiobotocore-workspaces-thin-client-2.9.0.tar.gz` & `tmp/types-aiobotocore-workspaces-thin-client-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-workspaces-thin-client-2.9.0.tar", last modified: Wed Dec 13 20:00:48 2023, max compression
+gzip compressed data, was "types-aiobotocore-workspaces-thin-client-2.9.1.tar", last modified: Thu Jan 18 01:22:05 2024, max compression
```

## Comparing `types-aiobotocore-workspaces-thin-client-2.9.0.tar` & `types-aiobotocore-workspaces-thin-client-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:48.256986 types-aiobotocore-workspaces-thin-client-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:58:08.000000 types-aiobotocore-workspaces-thin-client-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14098 2023-12-13 20:00:48.256986 types-aiobotocore-workspaces-thin-client-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12477 2023-12-13 19:58:08.000000 types-aiobotocore-workspaces-thin-client-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:48.256986 types-aiobotocore-workspaces-thin-client-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2023-12-13 19:58:08.000000 types-aiobotocore-workspaces-thin-client-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:48.256986 types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2023-12-13 19:58:08.000000 types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2023-12-13 19:58:08.000000 types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      988 2023-12-13 19:58:08.000000 types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16274 2023-12-13 19:58:08.000000 types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16270 2023-12-13 19:58:08.000000 types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10016 2023-12-13 19:58:08.000000 types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10014 2023-12-13 19:58:08.000000 types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2023-12-13 19:58:08.000000 types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2023-12-13 19:58:08.000000 types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:08.000000 types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    16337 2023-12-13 19:58:09.000000 types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16336 2023-12-13 19:58:08.000000 types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:58:08.000000 types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:48.256986 types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14098 2023-12-13 20:00:48.000000 types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2023-12-13 20:00:48.000000 types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:48.000000 types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:48.000000 types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:48.000000 types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-13 20:00:48.000000 types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:05.012961 types-aiobotocore-workspaces-thin-client-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:19:33.000000 types-aiobotocore-workspaces-thin-client-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14118 2024-01-18 01:22:05.012961 types-aiobotocore-workspaces-thin-client-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12477 2024-01-18 01:19:33.000000 types-aiobotocore-workspaces-thin-client-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:22:05.012961 types-aiobotocore-workspaces-thin-client-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-01-18 01:19:33.000000 types-aiobotocore-workspaces-thin-client-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:05.012961 types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-01-18 01:19:33.000000 types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-01-18 01:19:33.000000 types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-01-18 01:19:33.000000 types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16276 2024-01-18 01:19:33.000000 types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16273 2024-01-18 01:19:33.000000 types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10014 2024-01-18 01:19:34.000000 types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10014 2024-01-18 01:19:34.000000 types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-01-18 01:19:34.000000 types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-01-18 01:19:33.000000 types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:33.000000 types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16336 2024-01-18 01:19:34.000000 types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16336 2024-01-18 01:19:34.000000 types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:19:33.000000 types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:05.012961 types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14118 2024-01-18 01:22:04.000000 types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-01-18 01:22:04.000000 types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:22:04.000000 types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:22:04.000000 types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:22:04.000000 types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-18 01:22:04.000000 types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-workspaces-thin-client-2.9.0/LICENSE` & `types-aiobotocore-workspaces-thin-client-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-workspaces-thin-client-2.9.0/PKG-INFO` & `types-aiobotocore-workspaces-thin-client-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-workspaces-thin-client
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.WorkSpacesThinClient 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.WorkSpacesThinClient 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_thin_client/
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
 
 <a id="types-aiobotocore-workspaces-thin-client"></a>
 
 # types-aiobotocore-workspaces-thin-client
 
 [![PyPI - types-aiobotocore-workspaces-thin-client](https://img.shields.io/pypi/v/types-aiobotocore-workspaces-thin-client.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workspaces-thin-client)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-workspaces-thin-client.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workspaces-thin-client)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_thin_client/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-workspaces-thin-client)](https://pepy.tech/project/types-aiobotocore-workspaces-thin-client)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WorkSpacesThinClient 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#WorkSpacesThinClient)
+[aiobotocore.WorkSpacesThinClient 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#WorkSpacesThinClient)
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
 [types-aiobotocore-workspaces-thin-client docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_thin_client/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-workspaces-thin-client-2.9.0/README.md` & `types-aiobotocore-workspaces-thin-client-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-workspaces-thin-client.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workspaces-thin-client)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_thin_client/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-workspaces-thin-client)](https://pepy.tech/project/types-aiobotocore-workspaces-thin-client)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WorkSpacesThinClient 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#WorkSpacesThinClient)
+[aiobotocore.WorkSpacesThinClient 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#WorkSpacesThinClient)
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
 [types-aiobotocore-workspaces-thin-client docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_thin_client/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-workspaces-thin-client-2.9.0/setup.py` & `types-aiobotocore-workspaces-thin-client-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,50 +7,49 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-workspaces-thin-client",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_workspaces_thin_client"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.WorkSpacesThinClient 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.WorkSpacesThinClient 2.9.1 service generated with"
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
     keywords=(
         "aiobotocore workspaces-thin-client type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_workspaces_thin_client": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_thin_client/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client/__init__.py` & `types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 """
 
 from .client import WorkSpacesThinClientClient
 from .paginator import ListDevicesPaginator, ListEnvironmentsPaginator, ListSoftwareSetsPaginator
 
 Client = WorkSpacesThinClientClient
 
-
 __all__ = (
     "Client",
     "ListDevicesPaginator",
     "ListEnvironmentsPaginator",
     "ListSoftwareSetsPaginator",
     "WorkSpacesThinClientClient",
 )
```

### Comparing `types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client/__init__.pyi` & `types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client/__main__.py` & `types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.WorkSpacesThinClient 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.WorkSpacesThinClient 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_thin_client//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#WorkSpacesThinClient\nOther"
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

### Comparing `types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client/client.py` & `types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -43,38 +43,34 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("WorkSpacesThinClientClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     InternalServiceException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class WorkSpacesThinClientClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#WorkSpacesThinClient.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_thin_client/client/)
     """
 
     meta: ClientMeta
@@ -112,15 +108,15 @@
         desktopEndpoint: str = ...,
         softwareSetUpdateSchedule: SoftwareSetUpdateScheduleType = ...,
         maintenanceWindow: MaintenanceWindowTypeDef = ...,
         softwareSetUpdateMode: SoftwareSetUpdateModeType = ...,
         desiredSoftwareSetId: str = ...,
         kmsKeyArn: str = ...,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateEnvironmentResponseTypeDef:
         """
         Creates an environment for your thin client devices.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#WorkSpacesThinClient.Client.create_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_thin_client/client/#create_environment)
         """
@@ -248,15 +244,15 @@
     async def update_device(
         self,
         *,
         id: str,
         name: str = ...,
         desiredSoftwareSetId: str = ...,
         softwareSetUpdateSchedule: SoftwareSetUpdateScheduleType = ...,
-        kmsKeyArn: str = ...
+        kmsKeyArn: str = ...,
     ) -> UpdateDeviceResponseTypeDef:
         """
         Updates a thin client device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#WorkSpacesThinClient.Client.update_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_thin_client/client/#update_device)
         """
@@ -267,15 +263,15 @@
         id: str,
         name: str = ...,
         desktopArn: str = ...,
         desktopEndpoint: str = ...,
         softwareSetUpdateSchedule: SoftwareSetUpdateScheduleType = ...,
         maintenanceWindow: MaintenanceWindowTypeDef = ...,
         softwareSetUpdateMode: SoftwareSetUpdateModeType = ...,
-        desiredSoftwareSetId: str = ...
+        desiredSoftwareSetId: str = ...,
     ) -> UpdateEnvironmentResponseTypeDef:
         """
         Updates an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#WorkSpacesThinClient.Client.update_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_thin_client/client/#update_environment)
         """
```

### Comparing `types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client/client.pyi` & `types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,32 +45,35 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("WorkSpacesThinClientClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     InternalServiceException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class WorkSpacesThinClientClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#WorkSpacesThinClient.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_thin_client/client/)
     """
 
     meta: ClientMeta
@@ -108,15 +111,15 @@
         desktopEndpoint: str = ...,
         softwareSetUpdateSchedule: SoftwareSetUpdateScheduleType = ...,
         maintenanceWindow: MaintenanceWindowTypeDef = ...,
         softwareSetUpdateMode: SoftwareSetUpdateModeType = ...,
         desiredSoftwareSetId: str = ...,
         kmsKeyArn: str = ...,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateEnvironmentResponseTypeDef:
         """
         Creates an environment for your thin client devices.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#WorkSpacesThinClient.Client.create_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_thin_client/client/#create_environment)
         """
@@ -244,15 +247,15 @@
     async def update_device(
         self,
         *,
         id: str,
         name: str = ...,
         desiredSoftwareSetId: str = ...,
         softwareSetUpdateSchedule: SoftwareSetUpdateScheduleType = ...,
-        kmsKeyArn: str = ...
+        kmsKeyArn: str = ...,
     ) -> UpdateDeviceResponseTypeDef:
         """
         Updates a thin client device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#WorkSpacesThinClient.Client.update_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_thin_client/client/#update_device)
         """
@@ -263,15 +266,15 @@
         id: str,
         name: str = ...,
         desktopArn: str = ...,
         desktopEndpoint: str = ...,
         softwareSetUpdateSchedule: SoftwareSetUpdateScheduleType = ...,
         maintenanceWindow: MaintenanceWindowTypeDef = ...,
         softwareSetUpdateMode: SoftwareSetUpdateModeType = ...,
-        desiredSoftwareSetId: str = ...
+        desiredSoftwareSetId: str = ...,
     ) -> UpdateEnvironmentResponseTypeDef:
         """
         Updates an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#WorkSpacesThinClient.Client.update_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_thin_client/client/#update_environment)
         """
```

### Comparing `types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client/literals.py` & `types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client/literals.py`

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
     "ApplyTimeOfType",
     "DayOfWeekType",
     "DesktopTypeType",
     "DeviceSoftwareSetComplianceStatusType",
     "DeviceStatusType",
     "EnvironmentSoftwareSetComplianceStatusType",
@@ -39,15 +38,14 @@
     "WorkSpacesThinClientServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ApplyTimeOfType = Literal["DEVICE", "UTC"]
 DayOfWeekType = Literal[
     "FRIDAY", "MONDAY", "SATURDAY", "SUNDAY", "THURSDAY", "TUESDAY", "WEDNESDAY"
 ]
 DesktopTypeType = Literal["appstream", "workspaces", "workspaces-web"]
 DeviceSoftwareSetComplianceStatusType = Literal["COMPLIANT", "NONE", "NOT_COMPLIANT"]
 DeviceStatusType = Literal["ARCHIVED", "DEREGISTERED", "DEREGISTERING", "REGISTERED"]
```

### Comparing `types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client/literals.pyi` & `types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client/paginator.py` & `types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     ListEnvironmentsResponsePaginatorTypeDef,
     ListSoftwareSetsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListDevicesPaginator", "ListEnvironmentsPaginator", "ListSoftwareSetsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client/paginator.pyi` & `types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client/type_defs.py` & `types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "MaintenanceWindowTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteDeviceRequestRequestTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
     "DeregisterDeviceRequestRequestTypeDef",
     "EmbeddedTagTypeDef",
```

### Comparing `types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client/type_defs.pyi` & `types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client.egg-info/PKG-INFO` & `types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-workspaces-thin-client
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.WorkSpacesThinClient 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.WorkSpacesThinClient 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_thin_client/
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
 
 <a id="types-aiobotocore-workspaces-thin-client"></a>
 
 # types-aiobotocore-workspaces-thin-client
 
 [![PyPI - types-aiobotocore-workspaces-thin-client](https://img.shields.io/pypi/v/types-aiobotocore-workspaces-thin-client.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workspaces-thin-client)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-workspaces-thin-client.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workspaces-thin-client)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_thin_client/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-workspaces-thin-client)](https://pepy.tech/project/types-aiobotocore-workspaces-thin-client)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WorkSpacesThinClient 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#WorkSpacesThinClient)
+[aiobotocore.WorkSpacesThinClient 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#WorkSpacesThinClient)
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
 [types-aiobotocore-workspaces-thin-client docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces_thin_client/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-workspaces-thin-client-2.9.0/types_aiobotocore_workspaces_thin_client.egg-info/SOURCES.txt` & `types-aiobotocore-workspaces-thin-client-2.9.1/types_aiobotocore_workspaces_thin_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

