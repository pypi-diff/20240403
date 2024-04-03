# Comparing `tmp/types-aiobotocore-ecs-2.9.0.tar.gz` & `tmp/types-aiobotocore-ecs-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ecs-2.9.0.tar", last modified: Wed Dec 13 19:59:12 2023, max compression
+gzip compressed data, was "types-aiobotocore-ecs-2.9.1.tar", last modified: Thu Jan 18 01:20:37 2024, max compression
```

## Comparing `types-aiobotocore-ecs-2.9.0.tar` & `types-aiobotocore-ecs-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:12.305787 types-aiobotocore-ecs-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:45:28.000000 types-aiobotocore-ecs-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14949 2023-12-13 19:59:12.305787 types-aiobotocore-ecs-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13402 2023-12-13 19:45:28.000000 types-aiobotocore-ecs-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:12.305787 types-aiobotocore-ecs-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-12-13 19:45:27.000000 types-aiobotocore-ecs-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:12.305787 types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs/
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2023-12-13 19:45:28.000000 types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2023-12-13 19:45:28.000000 types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-13 19:45:28.000000 types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52640 2023-12-13 19:45:29.000000 types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    52636 2023-12-13 19:45:29.000000 types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16411 2023-12-13 19:45:30.000000 types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    16409 2023-12-13 19:45:29.000000 types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2023-12-13 19:45:29.000000 types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12034 2023-12-13 19:45:29.000000 types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:45:28.000000 types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    77122 2023-12-13 19:45:31.000000 types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    77121 2023-12-13 19:45:30.000000 types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:45:28.000000 types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4840 2023-12-13 19:45:29.000000 types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4835 2023-12-13 19:45:29.000000 types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:12.305787 types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14949 2023-12-13 19:59:12.000000 types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      802 2023-12-13 19:59:12.000000 types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:12.000000 types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:12.000000 types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:12.000000 types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 19:59:12.000000 types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:37.313358 types-aiobotocore-ecs-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:07:24.000000 types-aiobotocore-ecs-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14969 2024-01-18 01:20:37.313358 types-aiobotocore-ecs-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-01-18 01:07:24.000000 types-aiobotocore-ecs-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:37.313358 types-aiobotocore-ecs-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-01-18 01:07:24.000000 types-aiobotocore-ecs-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:37.309358 types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-01-18 01:07:24.000000 types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-01-18 01:07:24.000000 types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-18 01:07:24.000000 types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52666 2024-01-18 01:07:24.000000 types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52663 2024-01-18 01:07:24.000000 types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16409 2024-01-18 01:07:25.000000 types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16409 2024-01-18 01:07:25.000000 types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12051 2024-01-18 01:07:24.000000 types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12041 2024-01-18 01:07:24.000000 types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:07:24.000000 types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    77121 2024-01-18 01:07:27.000000 types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77121 2024-01-18 01:07:27.000000 types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:07:24.000000 types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-01-18 01:07:25.000000 types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-01-18 01:07:25.000000 types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:37.313358 types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14969 2024-01-18 01:20:37.000000 types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-01-18 01:20:37.000000 types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:37.000000 types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:37.000000 types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:37.000000 types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:20:37.000000 types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ecs-2.9.0/LICENSE` & `types-aiobotocore-ecs-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-ecs-2.9.0/PKG-INFO` & `types-aiobotocore-ecs-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ecs
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ECS 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ECS 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/
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
 
 <a id="types-aiobotocore-ecs"></a>
 
 # types-aiobotocore-ecs
 
 [![PyPI - types-aiobotocore-ecs](https://img.shields.io/pypi/v/types-aiobotocore-ecs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ecs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ecs)](https://pepy.tech/project/types-aiobotocore-ecs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ECS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
+[aiobotocore.ECS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
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
 [types-aiobotocore-ecs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ecs-2.9.0/README.md` & `types-aiobotocore-ecs-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ecs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ecs)](https://pepy.tech/project/types-aiobotocore-ecs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ECS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
+[aiobotocore.ECS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
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
 [types-aiobotocore-ecs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ecs-2.9.0/setup.py` & `types-aiobotocore-ecs-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ecs",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_ecs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ECS 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.ECS 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore ecs type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_ecs": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs/__init__.py` & `types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,14 @@
     ServicesStableWaiter,
     TasksRunningWaiter,
     TasksStoppedWaiter,
 )
 
 Client = ECSClient
 
-
 __all__ = (
     "Client",
     "ECSClient",
     "ListAccountSettingsPaginator",
     "ListAttributesPaginator",
     "ListClustersPaginator",
     "ListContainerInstancesPaginator",
```

### Comparing `types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs/__init__.pyi` & `types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs/__main__.py` & `types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ECS 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ECS 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS\nOther"
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

### Comparing `types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs/client.py` & `types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ECSClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -226,15 +225,15 @@
         """
 
     async def create_capacity_provider(
         self,
         *,
         name: str,
         autoScalingGroupProvider: AutoScalingGroupProviderTypeDef,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateCapacityProviderResponseTypeDef:
         """
         Creates a new capacity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.create_capacity_provider)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#create_capacity_provider)
         """
@@ -244,15 +243,15 @@
         *,
         clusterName: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         settings: Sequence[ClusterSettingTypeDef] = ...,
         configuration: ClusterConfigurationTypeDef = ...,
         capacityProviders: Sequence[str] = ...,
         defaultCapacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
-        serviceConnectDefaults: ClusterServiceConnectDefaultsRequestTypeDef = ...
+        serviceConnectDefaults: ClusterServiceConnectDefaultsRequestTypeDef = ...,
     ) -> CreateClusterResponseTypeDef:
         """
         Creates a new Amazon ECS cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.create_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#create_cluster)
         """
@@ -278,15 +277,15 @@
         healthCheckGracePeriodSeconds: int = ...,
         schedulingStrategy: SchedulingStrategyType = ...,
         deploymentController: DeploymentControllerTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         enableECSManagedTags: bool = ...,
         propagateTags: PropagateTagsType = ...,
         enableExecuteCommand: bool = ...,
-        serviceConnectConfiguration: ServiceConnectConfigurationTypeDef = ...
+        serviceConnectConfiguration: ServiceConnectConfigurationTypeDef = ...,
     ) -> CreateServiceResponseTypeDef:
         """
         Runs and maintains your desired number of tasks from a specified task
         definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.create_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#create_service)
@@ -303,15 +302,15 @@
         loadBalancers: Sequence[LoadBalancerTypeDef] = ...,
         serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...,
         launchType: LaunchTypeType = ...,
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
         platformVersion: str = ...,
         scale: ScaleTypeDef = ...,
         clientToken: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateTaskSetResponseTypeDef:
         """
         Create a task set in the specified cluster and service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.create_task_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#create_task_set)
         """
@@ -407,15 +406,15 @@
 
     async def describe_capacity_providers(
         self,
         *,
         capacityProviders: Sequence[str] = ...,
         include: Sequence[Literal["TAGS"]] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeCapacityProvidersResponseTypeDef:
         """
         Describes one or more of your capacity providers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.describe_capacity_providers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#describe_capacity_providers)
         """
@@ -431,29 +430,29 @@
         """
 
     async def describe_container_instances(
         self,
         *,
         containerInstances: Sequence[str],
         cluster: str = ...,
-        include: Sequence[ContainerInstanceFieldType] = ...
+        include: Sequence[ContainerInstanceFieldType] = ...,
     ) -> DescribeContainerInstancesResponseTypeDef:
         """
         Describes one or more container instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.describe_container_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#describe_container_instances)
         """
 
     async def describe_services(
         self,
         *,
         services: Sequence[str],
         cluster: str = ...,
-        include: Sequence[Literal["TAGS"]] = ...
+        include: Sequence[Literal["TAGS"]] = ...,
     ) -> DescribeServicesResponseTypeDef:
         """
         Describes the specified services running in your cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.describe_services)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#describe_services)
         """
@@ -470,15 +469,15 @@
 
     async def describe_task_sets(
         self,
         *,
         cluster: str,
         service: str,
         taskSets: Sequence[str] = ...,
-        include: Sequence[Literal["TAGS"]] = ...
+        include: Sequence[Literal["TAGS"]] = ...,
     ) -> DescribeTaskSetsResponseTypeDef:
         """
         Describes the task sets in the specified cluster and service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.describe_task_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#describe_task_sets)
         """
@@ -506,15 +505,15 @@
     async def execute_command(
         self,
         *,
         command: str,
         interactive: bool,
         task: str,
         cluster: str = ...,
-        container: str = ...
+        container: str = ...,
     ) -> ExecuteCommandResponseTypeDef:
         """
         Runs a command remotely on a container within a task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.execute_command)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#execute_command)
         """
@@ -547,15 +546,15 @@
         self,
         *,
         name: SettingNameType = ...,
         value: str = ...,
         principalArn: str = ...,
         effectiveSettings: bool = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListAccountSettingsResponseTypeDef:
         """
         Lists the account settings for a specified principal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_account_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#list_account_settings)
         """
@@ -564,15 +563,15 @@
         self,
         *,
         targetType: Literal["container-instance"],
         cluster: str = ...,
         attributeName: str = ...,
         attributeValue: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListAttributesResponseTypeDef:
         """
         Lists the attributes for Amazon ECS resources within a specified target type
         and
         cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_attributes)
@@ -592,15 +591,15 @@
     async def list_container_instances(
         self,
         *,
         cluster: str = ...,
         filter: str = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        status: ContainerInstanceStatusType = ...
+        status: ContainerInstanceStatusType = ...,
     ) -> ListContainerInstancesResponseTypeDef:
         """
         Returns a list of container instances in a specified cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_container_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#list_container_instances)
         """
@@ -608,15 +607,15 @@
     async def list_services(
         self,
         *,
         cluster: str = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         launchType: LaunchTypeType = ...,
-        schedulingStrategy: SchedulingStrategyType = ...
+        schedulingStrategy: SchedulingStrategyType = ...,
     ) -> ListServicesResponseTypeDef:
         """
         Returns a list of services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_services)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#list_services)
         """
@@ -644,15 +643,15 @@
 
     async def list_task_definition_families(
         self,
         *,
         familyPrefix: str = ...,
         status: TaskDefinitionFamilyStatusType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListTaskDefinitionFamiliesResponseTypeDef:
         """
         Returns a list of task definition families that are registered to your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_task_definition_families)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#list_task_definition_families)
         """
@@ -660,15 +659,15 @@
     async def list_task_definitions(
         self,
         *,
         familyPrefix: str = ...,
         status: TaskDefinitionStatusType = ...,
         sort: SortOrderType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListTaskDefinitionsResponseTypeDef:
         """
         Returns a list of task definitions that are registered to your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_task_definitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#list_task_definitions)
         """
@@ -680,15 +679,15 @@
         containerInstance: str = ...,
         family: str = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         startedBy: str = ...,
         serviceName: str = ...,
         desiredStatus: DesiredStatusType = ...,
-        launchType: LaunchTypeType = ...
+        launchType: LaunchTypeType = ...,
     ) -> ListTasksResponseTypeDef:
         """
         Returns a list of tasks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#list_tasks)
         """
@@ -726,15 +725,15 @@
         """
 
     async def put_cluster_capacity_providers(
         self,
         *,
         cluster: str,
         capacityProviders: Sequence[str],
-        defaultCapacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef]
+        defaultCapacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef],
     ) -> PutClusterCapacityProvidersResponseTypeDef:
         """
         Modifies the available capacity providers and the default capacity provider
         strategy for a
         cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.put_cluster_capacity_providers)
@@ -748,15 +747,15 @@
         instanceIdentityDocument: str = ...,
         instanceIdentityDocumentSignature: str = ...,
         totalResources: Sequence[ResourceTypeDef] = ...,
         versionInfo: VersionInfoTypeDef = ...,
         containerInstanceArn: str = ...,
         attributes: Sequence[AttributeTypeDef] = ...,
         platformDevices: Sequence[PlatformDeviceTypeDef] = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> RegisterContainerInstanceResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.register_container_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#register_container_instance)
         """
@@ -776,15 +775,15 @@
         memory: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         pidMode: PidModeType = ...,
         ipcMode: IpcModeType = ...,
         proxyConfiguration: ProxyConfigurationTypeDef = ...,
         inferenceAccelerators: Sequence[InferenceAcceleratorTypeDef] = ...,
         ephemeralStorage: EphemeralStorageTypeDef = ...,
-        runtimePlatform: RuntimePlatformTypeDef = ...
+        runtimePlatform: RuntimePlatformTypeDef = ...,
     ) -> RegisterTaskDefinitionResponseTypeDef:
         """
         Registers a new task definition from the supplied `family` and
         `containerDefinitions`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.register_task_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#register_task_definition)
@@ -806,15 +805,15 @@
         placementConstraints: Sequence[PlacementConstraintTypeDef] = ...,
         placementStrategy: Sequence[PlacementStrategyTypeDef] = ...,
         platformVersion: str = ...,
         propagateTags: PropagateTagsType = ...,
         referenceId: str = ...,
         startedBy: str = ...,
         tags: Sequence[TagTypeDef] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> RunTaskResponseTypeDef:
         """
         Starts a new task using the specified task definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.run_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#run_task)
         """
@@ -829,15 +828,15 @@
         enableExecuteCommand: bool = ...,
         group: str = ...,
         networkConfiguration: NetworkConfigurationTypeDef = ...,
         overrides: TaskOverrideTypeDef = ...,
         propagateTags: PropagateTagsType = ...,
         referenceId: str = ...,
         startedBy: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> StartTaskResponseTypeDef:
         """
         Starts a new task from the specified task definition on the specified container
         instance or
         instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.start_task)
@@ -870,15 +869,15 @@
         cluster: str = ...,
         task: str = ...,
         containerName: str = ...,
         runtimeId: str = ...,
         status: str = ...,
         exitCode: int = ...,
         reason: str = ...,
-        networkBindings: Sequence[NetworkBindingTypeDef] = ...
+        networkBindings: Sequence[NetworkBindingTypeDef] = ...,
     ) -> SubmitContainerStateChangeResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.submit_container_state_change)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#submit_container_state_change)
         """
@@ -891,15 +890,15 @@
         status: str = ...,
         reason: str = ...,
         containers: Sequence[ContainerStateChangeTypeDef] = ...,
         attachments: Sequence[AttachmentStateChangeTypeDef] = ...,
         managedAgents: Sequence[ManagedAgentStateChangeTypeDef] = ...,
         pullStartedAt: TimestampTypeDef = ...,
         pullStoppedAt: TimestampTypeDef = ...,
-        executionStoppedAt: TimestampTypeDef = ...
+        executionStoppedAt: TimestampTypeDef = ...,
     ) -> SubmitTaskStateChangeResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.submit_task_state_change)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#submit_task_state_change)
         """
@@ -932,15 +931,15 @@
 
     async def update_cluster(
         self,
         *,
         cluster: str,
         settings: Sequence[ClusterSettingTypeDef] = ...,
         configuration: ClusterConfigurationTypeDef = ...,
-        serviceConnectDefaults: ClusterServiceConnectDefaultsRequestTypeDef = ...
+        serviceConnectDefaults: ClusterServiceConnectDefaultsRequestTypeDef = ...,
     ) -> UpdateClusterResponseTypeDef:
         """
         Updates the cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#update_cluster)
         """
@@ -966,15 +965,15 @@
         """
 
     async def update_container_instances_state(
         self,
         *,
         containerInstances: Sequence[str],
         status: ContainerInstanceStatusType,
-        cluster: str = ...
+        cluster: str = ...,
     ) -> UpdateContainerInstancesStateResponseTypeDef:
         """
         Modifies the status of an Amazon ECS container instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_container_instances_state)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#update_container_instances_state)
         """
@@ -995,15 +994,15 @@
         forceNewDeployment: bool = ...,
         healthCheckGracePeriodSeconds: int = ...,
         enableExecuteCommand: bool = ...,
         enableECSManagedTags: bool = ...,
         loadBalancers: Sequence[LoadBalancerTypeDef] = ...,
         propagateTags: PropagateTagsType = ...,
         serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...,
-        serviceConnectConfiguration: ServiceConnectConfigurationTypeDef = ...
+        serviceConnectConfiguration: ServiceConnectConfigurationTypeDef = ...,
     ) -> UpdateServiceResponseTypeDef:
         """
         Modifies the parameters of a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#update_service)
         """
@@ -1020,15 +1019,15 @@
 
     async def update_task_protection(
         self,
         *,
         cluster: str,
         tasks: Sequence[str],
         protectionEnabled: bool,
-        expiresInMinutes: int = ...
+        expiresInMinutes: int = ...,
     ) -> UpdateTaskProtectionResponseTypeDef:
         """
         Updates the protection status of a task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_task_protection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#update_task_protection)
         """
```

### Comparing `types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs/client.pyi` & `types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -222,15 +222,15 @@
         """
 
     async def create_capacity_provider(
         self,
         *,
         name: str,
         autoScalingGroupProvider: AutoScalingGroupProviderTypeDef,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateCapacityProviderResponseTypeDef:
         """
         Creates a new capacity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.create_capacity_provider)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#create_capacity_provider)
         """
@@ -240,15 +240,15 @@
         *,
         clusterName: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         settings: Sequence[ClusterSettingTypeDef] = ...,
         configuration: ClusterConfigurationTypeDef = ...,
         capacityProviders: Sequence[str] = ...,
         defaultCapacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
-        serviceConnectDefaults: ClusterServiceConnectDefaultsRequestTypeDef = ...
+        serviceConnectDefaults: ClusterServiceConnectDefaultsRequestTypeDef = ...,
     ) -> CreateClusterResponseTypeDef:
         """
         Creates a new Amazon ECS cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.create_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#create_cluster)
         """
@@ -274,15 +274,15 @@
         healthCheckGracePeriodSeconds: int = ...,
         schedulingStrategy: SchedulingStrategyType = ...,
         deploymentController: DeploymentControllerTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         enableECSManagedTags: bool = ...,
         propagateTags: PropagateTagsType = ...,
         enableExecuteCommand: bool = ...,
-        serviceConnectConfiguration: ServiceConnectConfigurationTypeDef = ...
+        serviceConnectConfiguration: ServiceConnectConfigurationTypeDef = ...,
     ) -> CreateServiceResponseTypeDef:
         """
         Runs and maintains your desired number of tasks from a specified task
         definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.create_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#create_service)
@@ -299,15 +299,15 @@
         loadBalancers: Sequence[LoadBalancerTypeDef] = ...,
         serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...,
         launchType: LaunchTypeType = ...,
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
         platformVersion: str = ...,
         scale: ScaleTypeDef = ...,
         clientToken: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateTaskSetResponseTypeDef:
         """
         Create a task set in the specified cluster and service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.create_task_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#create_task_set)
         """
@@ -403,15 +403,15 @@
 
     async def describe_capacity_providers(
         self,
         *,
         capacityProviders: Sequence[str] = ...,
         include: Sequence[Literal["TAGS"]] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeCapacityProvidersResponseTypeDef:
         """
         Describes one or more of your capacity providers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.describe_capacity_providers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#describe_capacity_providers)
         """
@@ -427,29 +427,29 @@
         """
 
     async def describe_container_instances(
         self,
         *,
         containerInstances: Sequence[str],
         cluster: str = ...,
-        include: Sequence[ContainerInstanceFieldType] = ...
+        include: Sequence[ContainerInstanceFieldType] = ...,
     ) -> DescribeContainerInstancesResponseTypeDef:
         """
         Describes one or more container instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.describe_container_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#describe_container_instances)
         """
 
     async def describe_services(
         self,
         *,
         services: Sequence[str],
         cluster: str = ...,
-        include: Sequence[Literal["TAGS"]] = ...
+        include: Sequence[Literal["TAGS"]] = ...,
     ) -> DescribeServicesResponseTypeDef:
         """
         Describes the specified services running in your cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.describe_services)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#describe_services)
         """
@@ -466,15 +466,15 @@
 
     async def describe_task_sets(
         self,
         *,
         cluster: str,
         service: str,
         taskSets: Sequence[str] = ...,
-        include: Sequence[Literal["TAGS"]] = ...
+        include: Sequence[Literal["TAGS"]] = ...,
     ) -> DescribeTaskSetsResponseTypeDef:
         """
         Describes the task sets in the specified cluster and service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.describe_task_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#describe_task_sets)
         """
@@ -502,15 +502,15 @@
     async def execute_command(
         self,
         *,
         command: str,
         interactive: bool,
         task: str,
         cluster: str = ...,
-        container: str = ...
+        container: str = ...,
     ) -> ExecuteCommandResponseTypeDef:
         """
         Runs a command remotely on a container within a task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.execute_command)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#execute_command)
         """
@@ -543,15 +543,15 @@
         self,
         *,
         name: SettingNameType = ...,
         value: str = ...,
         principalArn: str = ...,
         effectiveSettings: bool = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListAccountSettingsResponseTypeDef:
         """
         Lists the account settings for a specified principal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_account_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#list_account_settings)
         """
@@ -560,15 +560,15 @@
         self,
         *,
         targetType: Literal["container-instance"],
         cluster: str = ...,
         attributeName: str = ...,
         attributeValue: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListAttributesResponseTypeDef:
         """
         Lists the attributes for Amazon ECS resources within a specified target type
         and
         cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_attributes)
@@ -588,15 +588,15 @@
     async def list_container_instances(
         self,
         *,
         cluster: str = ...,
         filter: str = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        status: ContainerInstanceStatusType = ...
+        status: ContainerInstanceStatusType = ...,
     ) -> ListContainerInstancesResponseTypeDef:
         """
         Returns a list of container instances in a specified cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_container_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#list_container_instances)
         """
@@ -604,15 +604,15 @@
     async def list_services(
         self,
         *,
         cluster: str = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         launchType: LaunchTypeType = ...,
-        schedulingStrategy: SchedulingStrategyType = ...
+        schedulingStrategy: SchedulingStrategyType = ...,
     ) -> ListServicesResponseTypeDef:
         """
         Returns a list of services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_services)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#list_services)
         """
@@ -640,15 +640,15 @@
 
     async def list_task_definition_families(
         self,
         *,
         familyPrefix: str = ...,
         status: TaskDefinitionFamilyStatusType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListTaskDefinitionFamiliesResponseTypeDef:
         """
         Returns a list of task definition families that are registered to your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_task_definition_families)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#list_task_definition_families)
         """
@@ -656,15 +656,15 @@
     async def list_task_definitions(
         self,
         *,
         familyPrefix: str = ...,
         status: TaskDefinitionStatusType = ...,
         sort: SortOrderType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListTaskDefinitionsResponseTypeDef:
         """
         Returns a list of task definitions that are registered to your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_task_definitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#list_task_definitions)
         """
@@ -676,15 +676,15 @@
         containerInstance: str = ...,
         family: str = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         startedBy: str = ...,
         serviceName: str = ...,
         desiredStatus: DesiredStatusType = ...,
-        launchType: LaunchTypeType = ...
+        launchType: LaunchTypeType = ...,
     ) -> ListTasksResponseTypeDef:
         """
         Returns a list of tasks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#list_tasks)
         """
@@ -722,15 +722,15 @@
         """
 
     async def put_cluster_capacity_providers(
         self,
         *,
         cluster: str,
         capacityProviders: Sequence[str],
-        defaultCapacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef]
+        defaultCapacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef],
     ) -> PutClusterCapacityProvidersResponseTypeDef:
         """
         Modifies the available capacity providers and the default capacity provider
         strategy for a
         cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.put_cluster_capacity_providers)
@@ -744,15 +744,15 @@
         instanceIdentityDocument: str = ...,
         instanceIdentityDocumentSignature: str = ...,
         totalResources: Sequence[ResourceTypeDef] = ...,
         versionInfo: VersionInfoTypeDef = ...,
         containerInstanceArn: str = ...,
         attributes: Sequence[AttributeTypeDef] = ...,
         platformDevices: Sequence[PlatformDeviceTypeDef] = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> RegisterContainerInstanceResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.register_container_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#register_container_instance)
         """
@@ -772,15 +772,15 @@
         memory: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         pidMode: PidModeType = ...,
         ipcMode: IpcModeType = ...,
         proxyConfiguration: ProxyConfigurationTypeDef = ...,
         inferenceAccelerators: Sequence[InferenceAcceleratorTypeDef] = ...,
         ephemeralStorage: EphemeralStorageTypeDef = ...,
-        runtimePlatform: RuntimePlatformTypeDef = ...
+        runtimePlatform: RuntimePlatformTypeDef = ...,
     ) -> RegisterTaskDefinitionResponseTypeDef:
         """
         Registers a new task definition from the supplied `family` and
         `containerDefinitions`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.register_task_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#register_task_definition)
@@ -802,15 +802,15 @@
         placementConstraints: Sequence[PlacementConstraintTypeDef] = ...,
         placementStrategy: Sequence[PlacementStrategyTypeDef] = ...,
         platformVersion: str = ...,
         propagateTags: PropagateTagsType = ...,
         referenceId: str = ...,
         startedBy: str = ...,
         tags: Sequence[TagTypeDef] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> RunTaskResponseTypeDef:
         """
         Starts a new task using the specified task definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.run_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#run_task)
         """
@@ -825,15 +825,15 @@
         enableExecuteCommand: bool = ...,
         group: str = ...,
         networkConfiguration: NetworkConfigurationTypeDef = ...,
         overrides: TaskOverrideTypeDef = ...,
         propagateTags: PropagateTagsType = ...,
         referenceId: str = ...,
         startedBy: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> StartTaskResponseTypeDef:
         """
         Starts a new task from the specified task definition on the specified container
         instance or
         instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.start_task)
@@ -866,15 +866,15 @@
         cluster: str = ...,
         task: str = ...,
         containerName: str = ...,
         runtimeId: str = ...,
         status: str = ...,
         exitCode: int = ...,
         reason: str = ...,
-        networkBindings: Sequence[NetworkBindingTypeDef] = ...
+        networkBindings: Sequence[NetworkBindingTypeDef] = ...,
     ) -> SubmitContainerStateChangeResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.submit_container_state_change)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#submit_container_state_change)
         """
@@ -887,15 +887,15 @@
         status: str = ...,
         reason: str = ...,
         containers: Sequence[ContainerStateChangeTypeDef] = ...,
         attachments: Sequence[AttachmentStateChangeTypeDef] = ...,
         managedAgents: Sequence[ManagedAgentStateChangeTypeDef] = ...,
         pullStartedAt: TimestampTypeDef = ...,
         pullStoppedAt: TimestampTypeDef = ...,
-        executionStoppedAt: TimestampTypeDef = ...
+        executionStoppedAt: TimestampTypeDef = ...,
     ) -> SubmitTaskStateChangeResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.submit_task_state_change)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#submit_task_state_change)
         """
@@ -928,15 +928,15 @@
 
     async def update_cluster(
         self,
         *,
         cluster: str,
         settings: Sequence[ClusterSettingTypeDef] = ...,
         configuration: ClusterConfigurationTypeDef = ...,
-        serviceConnectDefaults: ClusterServiceConnectDefaultsRequestTypeDef = ...
+        serviceConnectDefaults: ClusterServiceConnectDefaultsRequestTypeDef = ...,
     ) -> UpdateClusterResponseTypeDef:
         """
         Updates the cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#update_cluster)
         """
@@ -962,15 +962,15 @@
         """
 
     async def update_container_instances_state(
         self,
         *,
         containerInstances: Sequence[str],
         status: ContainerInstanceStatusType,
-        cluster: str = ...
+        cluster: str = ...,
     ) -> UpdateContainerInstancesStateResponseTypeDef:
         """
         Modifies the status of an Amazon ECS container instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_container_instances_state)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#update_container_instances_state)
         """
@@ -991,15 +991,15 @@
         forceNewDeployment: bool = ...,
         healthCheckGracePeriodSeconds: int = ...,
         enableExecuteCommand: bool = ...,
         enableECSManagedTags: bool = ...,
         loadBalancers: Sequence[LoadBalancerTypeDef] = ...,
         propagateTags: PropagateTagsType = ...,
         serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...,
-        serviceConnectConfiguration: ServiceConnectConfigurationTypeDef = ...
+        serviceConnectConfiguration: ServiceConnectConfigurationTypeDef = ...,
     ) -> UpdateServiceResponseTypeDef:
         """
         Modifies the parameters of a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#update_service)
         """
@@ -1016,15 +1016,15 @@
 
     async def update_task_protection(
         self,
         *,
         cluster: str,
         tasks: Sequence[str],
         protectionEnabled: bool,
-        expiresInMinutes: int = ...
+        expiresInMinutes: int = ...,
     ) -> UpdateTaskProtectionResponseTypeDef:
         """
         Updates the protection status of a task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_task_protection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#update_task_protection)
         """
```

### Comparing `types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs/literals.py` & `types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs/literals.py`

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
     "AgentUpdateStatusType",
     "ApplicationProtocolType",
     "AssignPublicIpType",
     "CPUArchitectureType",
     "CapacityProviderFieldType",
     "CapacityProviderStatusType",
@@ -97,15 +96,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AgentUpdateStatusType = Literal["FAILED", "PENDING", "STAGED", "STAGING", "UPDATED", "UPDATING"]
 ApplicationProtocolType = Literal["grpc", "http", "http2"]
 AssignPublicIpType = Literal["DISABLED", "ENABLED"]
 CPUArchitectureType = Literal["ARM64", "X86_64"]
 CapacityProviderFieldType = Literal["TAGS"]
 CapacityProviderStatusType = Literal["ACTIVE", "INACTIVE"]
 CapacityProviderUpdateStatusType = Literal[
```

### Comparing `types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs/literals.pyi` & `types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs/paginator.py` & `types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,28 +67,26 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListAccountSettingsPaginator",
     "ListAttributesPaginator",
     "ListClustersPaginator",
     "ListContainerInstancesPaginator",
     "ListServicesPaginator",
     "ListServicesByNamespacePaginator",
     "ListTaskDefinitionFamiliesPaginator",
     "ListTaskDefinitionsPaginator",
     "ListTasksPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -104,15 +102,15 @@
     def paginate(
         self,
         *,
         name: SettingNameType = ...,
         value: str = ...,
         principalArn: str = ...,
         effectiveSettings: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAccountSettingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAccountSettings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listaccountsettingspaginator)
         """
 
 
@@ -125,15 +123,15 @@
     def paginate(
         self,
         *,
         targetType: Literal["container-instance"],
         cluster: str = ...,
         attributeName: str = ...,
         attributeValue: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAttributesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAttributes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listattributespaginator)
         """
 
 
@@ -160,15 +158,15 @@
 
     def paginate(
         self,
         *,
         cluster: str = ...,
         filter: str = ...,
         status: ContainerInstanceStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListContainerInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListContainerInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listcontainerinstancespaginator)
         """
 
 
@@ -180,15 +178,15 @@
 
     def paginate(
         self,
         *,
         cluster: str = ...,
         launchType: LaunchTypeType = ...,
         schedulingStrategy: SchedulingStrategyType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListServices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listservicespaginator)
         """
 
 
@@ -214,15 +212,15 @@
     """
 
     def paginate(
         self,
         *,
         familyPrefix: str = ...,
         status: TaskDefinitionFamilyStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTaskDefinitionFamiliesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitionFamilies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listtaskdefinitionfamiliespaginator)
         """
 
 
@@ -234,15 +232,15 @@
 
     def paginate(
         self,
         *,
         familyPrefix: str = ...,
         status: TaskDefinitionStatusType = ...,
         sort: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTaskDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listtaskdefinitionspaginator)
         """
 
 
@@ -258,13 +256,13 @@
         cluster: str = ...,
         containerInstance: str = ...,
         family: str = ...,
         startedBy: str = ...,
         serviceName: str = ...,
         desiredStatus: DesiredStatusType = ...,
         launchType: LaunchTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listtaskspaginator)
         """
```

### Comparing `types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs/paginator.pyi` & `types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     def paginate(
         self,
         *,
         name: SettingNameType = ...,
         value: str = ...,
         principalArn: str = ...,
         effectiveSettings: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAccountSettingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAccountSettings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listaccountsettingspaginator)
         """
 
 class ListAttributesPaginator(AioPaginator):
@@ -120,15 +120,15 @@
     def paginate(
         self,
         *,
         targetType: Literal["container-instance"],
         cluster: str = ...,
         attributeName: str = ...,
         attributeValue: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAttributesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAttributes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listattributespaginator)
         """
 
 class ListClustersPaginator(AioPaginator):
@@ -153,15 +153,15 @@
 
     def paginate(
         self,
         *,
         cluster: str = ...,
         filter: str = ...,
         status: ContainerInstanceStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListContainerInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListContainerInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listcontainerinstancespaginator)
         """
 
 class ListServicesPaginator(AioPaginator):
@@ -172,15 +172,15 @@
 
     def paginate(
         self,
         *,
         cluster: str = ...,
         launchType: LaunchTypeType = ...,
         schedulingStrategy: SchedulingStrategyType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListServices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listservicespaginator)
         """
 
 class ListServicesByNamespacePaginator(AioPaginator):
@@ -204,15 +204,15 @@
     """
 
     def paginate(
         self,
         *,
         familyPrefix: str = ...,
         status: TaskDefinitionFamilyStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTaskDefinitionFamiliesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitionFamilies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listtaskdefinitionfamiliespaginator)
         """
 
 class ListTaskDefinitionsPaginator(AioPaginator):
@@ -223,15 +223,15 @@
 
     def paginate(
         self,
         *,
         familyPrefix: str = ...,
         status: TaskDefinitionStatusType = ...,
         sort: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTaskDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listtaskdefinitionspaginator)
         """
 
 class ListTasksPaginator(AioPaginator):
@@ -246,13 +246,13 @@
         cluster: str = ...,
         containerInstance: str = ...,
         family: str = ...,
         startedBy: str = ...,
         serviceName: str = ...,
         desiredStatus: DesiredStatusType = ...,
         launchType: LaunchTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listtaskspaginator)
         """
```

### Comparing `types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs/type_defs.py` & `types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AttachmentStateChangeTypeDef",
     "KeyValuePairTypeDef",
     "AttributeTypeDef",
     "ManagedScalingTypeDef",
     "AwsVpcConfigurationTypeDef",
     "CapacityProviderStrategyItemTypeDef",
```

### Comparing `types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs/type_defs.pyi` & `types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs/waiter.py` & `types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs/waiter.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 from .type_defs import WaiterConfigTypeDef
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ServicesInactiveWaiter",
     "ServicesStableWaiter",
     "TasksRunningWaiter",
     "TasksStoppedWaiter",
 )
 
@@ -56,15 +55,15 @@
 
     async def wait(
         self,
         *,
         services: Sequence[str],
         cluster: str = ...,
         include: Sequence[Literal["TAGS"]] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Waiter.ServicesInactive.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/waiters/#servicesinactivewaiter)
         """
 
 
@@ -76,15 +75,15 @@
 
     async def wait(
         self,
         *,
         services: Sequence[str],
         cluster: str = ...,
         include: Sequence[Literal["TAGS"]] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Waiter.ServicesStable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/waiters/#servicesstablewaiter)
         """
 
 
@@ -96,15 +95,15 @@
 
     async def wait(
         self,
         *,
         tasks: Sequence[str],
         cluster: str = ...,
         include: Sequence[Literal["TAGS"]] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Waiter.TasksRunning.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/waiters/#tasksrunningwaiter)
         """
 
 
@@ -116,13 +115,13 @@
 
     async def wait(
         self,
         *,
         tasks: Sequence[str],
         cluster: str = ...,
         include: Sequence[Literal["TAGS"]] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Waiter.TasksStopped.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/waiters/#tasksstoppedwaiter)
         """
```

### Comparing `types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs/waiter.pyi` & `types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs/waiter.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
     async def wait(
         self,
         *,
         services: Sequence[str],
         cluster: str = ...,
         include: Sequence[Literal["TAGS"]] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Waiter.ServicesInactive.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/waiters/#servicesinactivewaiter)
         """
 
 class ServicesStableWaiter(AIOWaiter):
@@ -73,15 +73,15 @@
 
     async def wait(
         self,
         *,
         services: Sequence[str],
         cluster: str = ...,
         include: Sequence[Literal["TAGS"]] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Waiter.ServicesStable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/waiters/#servicesstablewaiter)
         """
 
 class TasksRunningWaiter(AIOWaiter):
@@ -92,15 +92,15 @@
 
     async def wait(
         self,
         *,
         tasks: Sequence[str],
         cluster: str = ...,
         include: Sequence[Literal["TAGS"]] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Waiter.TasksRunning.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/waiters/#tasksrunningwaiter)
         """
 
 class TasksStoppedWaiter(AIOWaiter):
@@ -111,13 +111,13 @@
 
     async def wait(
         self,
         *,
         tasks: Sequence[str],
         cluster: str = ...,
         include: Sequence[Literal["TAGS"]] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Waiter.TasksStopped.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/waiters/#tasksstoppedwaiter)
         """
```

### Comparing `types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs.egg-info/PKG-INFO` & `types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ecs
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ECS 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ECS 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/
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
 
 <a id="types-aiobotocore-ecs"></a>
 
 # types-aiobotocore-ecs
 
 [![PyPI - types-aiobotocore-ecs](https://img.shields.io/pypi/v/types-aiobotocore-ecs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ecs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ecs)](https://pepy.tech/project/types-aiobotocore-ecs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ECS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
+[aiobotocore.ECS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
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
 [types-aiobotocore-ecs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ecs-2.9.0/types_aiobotocore_ecs.egg-info/SOURCES.txt` & `types-aiobotocore-ecs-2.9.1/types_aiobotocore_ecs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

