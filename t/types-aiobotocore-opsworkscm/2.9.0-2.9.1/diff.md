# Comparing `tmp/types-aiobotocore-opsworkscm-2.9.0.tar.gz` & `tmp/types-aiobotocore-opsworkscm-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-opsworkscm-2.9.0.tar", last modified: Wed Dec 13 20:00:04 2023, max compression
+gzip compressed data, was "types-aiobotocore-opsworkscm-2.9.1.tar", last modified: Thu Jan 18 01:21:25 2024, max compression
```

## Comparing `types-aiobotocore-opsworkscm-2.9.0.tar` & `types-aiobotocore-opsworkscm-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:04.425363 types-aiobotocore-opsworkscm-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:51:16.000000 types-aiobotocore-opsworkscm-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14253 2023-12-13 20:00:04.425363 types-aiobotocore-opsworkscm-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12678 2023-12-13 19:51:16.000000 types-aiobotocore-opsworkscm-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:04.425363 types-aiobotocore-opsworkscm-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2023-12-13 19:51:16.000000 types-aiobotocore-opsworkscm-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:04.425363 types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm/
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2023-12-13 19:51:16.000000 types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2023-12-13 19:51:16.000000 types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      944 2023-12-13 19:51:16.000000 types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19219 2023-12-13 19:51:16.000000 types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    19215 2023-12-13 19:51:16.000000 types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9616 2023-12-13 19:51:16.000000 types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9614 2023-12-13 19:51:16.000000 types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5488 2023-12-13 19:51:16.000000 types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2023-12-13 19:51:16.000000 types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:51:16.000000 types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    15507 2023-12-13 19:51:16.000000 types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15506 2023-12-13 19:51:16.000000 types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:51:16.000000 types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2023-12-13 19:51:16.000000 types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2023-12-13 19:51:16.000000 types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:04.425363 types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14253 2023-12-13 20:00:04.000000 types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      949 2023-12-13 20:00:04.000000 types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:04.000000 types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:04.000000 types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:04.000000 types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-13 20:00:04.000000 types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:25.321139 types-aiobotocore-opsworkscm-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:12:56.000000 types-aiobotocore-opsworkscm-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14273 2024-01-18 01:21:25.321139 types-aiobotocore-opsworkscm-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12678 2024-01-18 01:12:56.000000 types-aiobotocore-opsworkscm-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:25.321139 types-aiobotocore-opsworkscm-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-01-18 01:12:55.000000 types-aiobotocore-opsworkscm-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:25.317139 types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-01-18 01:12:56.000000 types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-01-18 01:12:56.000000 types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-01-18 01:12:56.000000 types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19223 2024-01-18 01:12:56.000000 types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19220 2024-01-18 01:12:56.000000 types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9614 2024-01-18 01:12:56.000000 types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9614 2024-01-18 01:12:56.000000 types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-01-18 01:12:56.000000 types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5483 2024-01-18 01:12:56.000000 types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:12:56.000000 types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    15506 2024-01-18 01:12:56.000000 types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15506 2024-01-18 01:12:56.000000 types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:12:56.000000 types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-01-18 01:12:56.000000 types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-01-18 01:12:56.000000 types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:25.321139 types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14273 2024-01-18 01:21:25.000000 types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-01-18 01:21:25.000000 types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:25.000000 types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:25.000000 types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:25.000000 types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-18 01:21:25.000000 types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-opsworkscm-2.9.0/LICENSE` & `types-aiobotocore-opsworkscm-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-opsworkscm-2.9.0/PKG-INFO` & `types-aiobotocore-opsworkscm-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-opsworkscm
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.OpsWorksCM 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.OpsWorksCM 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/
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
 
 <a id="types-aiobotocore-opsworkscm"></a>
 
 # types-aiobotocore-opsworkscm
 
 [![PyPI - types-aiobotocore-opsworkscm](https://img.shields.io/pypi/v/types-aiobotocore-opsworkscm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opsworkscm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-opsworkscm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opsworkscm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-opsworkscm)](https://pepy.tech/project/types-aiobotocore-opsworkscm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.OpsWorksCM 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
+[aiobotocore.OpsWorksCM 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
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
 [types-aiobotocore-opsworkscm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-opsworkscm-2.9.0/README.md` & `types-aiobotocore-opsworkscm-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-opsworkscm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opsworkscm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-opsworkscm)](https://pepy.tech/project/types-aiobotocore-opsworkscm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.OpsWorksCM 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
+[aiobotocore.OpsWorksCM 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
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
 [types-aiobotocore-opsworkscm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-opsworkscm-2.9.0/setup.py` & `types-aiobotocore-opsworkscm-2.9.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-opsworkscm",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_opsworkscm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.OpsWorksCM 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.OpsWorksCM 2.9.1 service generated with"
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
     keywords="aiobotocore opsworkscm type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_opsworkscm": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm/__init__.py` & `types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
     DescribeServersPaginator,
     ListTagsForResourcePaginator,
 )
 from .waiter import NodeAssociatedWaiter
 
 Client = OpsWorksCMClient
 
-
 __all__ = (
     "Client",
     "DescribeBackupsPaginator",
     "DescribeEventsPaginator",
     "DescribeServersPaginator",
     "ListTagsForResourcePaginator",
     "NodeAssociatedWaiter",
```

### Comparing `types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm/__init__.pyi` & `types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm/__main__.py` & `types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.OpsWorksCM 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.OpsWorksCM 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM\nOther"
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

### Comparing `types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm/client.py` & `types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 from .waiter import NodeAssociatedWaiter
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("OpsWorksCMClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -147,15 +146,15 @@
         BackupRetentionCount: int = ...,
         KeyPair: str = ...,
         PreferredMaintenanceWindow: str = ...,
         PreferredBackupWindow: str = ...,
         SecurityGroupIds: Sequence[str] = ...,
         SubnetIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        BackupId: str = ...
+        BackupId: str = ...,
     ) -> CreateServerResponseTypeDef:
         """
         Creates and immedately starts a new server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.create_server)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/client/#create_server)
         """
@@ -188,15 +187,15 @@
 
     async def describe_backups(
         self,
         *,
         BackupId: str = ...,
         ServerName: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeBackupsResponseTypeDef:
         """
         Describes backups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.describe_backups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/client/#describe_backups)
         """
@@ -233,15 +232,15 @@
         """
 
     async def disassociate_node(
         self,
         *,
         ServerName: str,
         NodeName: str,
-        EngineAttributes: Sequence[EngineAttributeTypeDef] = ...
+        EngineAttributes: Sequence[EngineAttributeTypeDef] = ...,
     ) -> DisassociateNodeResponseTypeDef:
         """
         Disassociates a node from an AWS OpsWorks CM server, and removes the node from
         the server's managed
         nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.disassociate_node)
@@ -249,15 +248,15 @@
         """
 
     async def export_server_engine_attribute(
         self,
         *,
         ExportAttributeName: str,
         ServerName: str,
-        InputAttributes: Sequence[EngineAttributeTypeDef] = ...
+        InputAttributes: Sequence[EngineAttributeTypeDef] = ...,
     ) -> ExportServerEngineAttributeResponseTypeDef:
         """
         Exports a specified server engine attribute as a base64-encoded string.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.export_server_engine_attribute)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/client/#export_server_engine_attribute)
         """
@@ -331,15 +330,15 @@
     async def update_server(
         self,
         *,
         ServerName: str,
         DisableAutomatedBackup: bool = ...,
         BackupRetentionCount: int = ...,
         PreferredMaintenanceWindow: str = ...,
-        PreferredBackupWindow: str = ...
+        PreferredBackupWindow: str = ...,
     ) -> UpdateServerResponseTypeDef:
         """
         Updates settings for a server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.update_server)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/client/#update_server)
         """
```

### Comparing `types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm/client.pyi` & `types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         BackupRetentionCount: int = ...,
         KeyPair: str = ...,
         PreferredMaintenanceWindow: str = ...,
         PreferredBackupWindow: str = ...,
         SecurityGroupIds: Sequence[str] = ...,
         SubnetIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        BackupId: str = ...
+        BackupId: str = ...,
     ) -> CreateServerResponseTypeDef:
         """
         Creates and immedately starts a new server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.create_server)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/client/#create_server)
         """
@@ -184,15 +184,15 @@
 
     async def describe_backups(
         self,
         *,
         BackupId: str = ...,
         ServerName: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeBackupsResponseTypeDef:
         """
         Describes backups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.describe_backups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/client/#describe_backups)
         """
@@ -229,15 +229,15 @@
         """
 
     async def disassociate_node(
         self,
         *,
         ServerName: str,
         NodeName: str,
-        EngineAttributes: Sequence[EngineAttributeTypeDef] = ...
+        EngineAttributes: Sequence[EngineAttributeTypeDef] = ...,
     ) -> DisassociateNodeResponseTypeDef:
         """
         Disassociates a node from an AWS OpsWorks CM server, and removes the node from
         the server's managed
         nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.disassociate_node)
@@ -245,15 +245,15 @@
         """
 
     async def export_server_engine_attribute(
         self,
         *,
         ExportAttributeName: str,
         ServerName: str,
-        InputAttributes: Sequence[EngineAttributeTypeDef] = ...
+        InputAttributes: Sequence[EngineAttributeTypeDef] = ...,
     ) -> ExportServerEngineAttributeResponseTypeDef:
         """
         Exports a specified server engine attribute as a base64-encoded string.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.export_server_engine_attribute)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/client/#export_server_engine_attribute)
         """
@@ -327,15 +327,15 @@
     async def update_server(
         self,
         *,
         ServerName: str,
         DisableAutomatedBackup: bool = ...,
         BackupRetentionCount: int = ...,
         PreferredMaintenanceWindow: str = ...,
-        PreferredBackupWindow: str = ...
+        PreferredBackupWindow: str = ...,
     ) -> UpdateServerResponseTypeDef:
         """
         Updates settings for a server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.update_server)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/client/#update_server)
         """
```

### Comparing `types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm/literals.py` & `types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm/literals.py`

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
     "BackupStatusType",
     "BackupTypeType",
     "DescribeBackupsPaginatorName",
     "DescribeEventsPaginatorName",
     "DescribeServersPaginatorName",
     "ListTagsForResourcePaginatorName",
@@ -35,15 +34,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 BackupStatusType = Literal["DELETING", "FAILED", "IN_PROGRESS", "OK"]
 BackupTypeType = Literal["AUTOMATED", "MANUAL"]
 DescribeBackupsPaginatorName = Literal["describe_backups"]
 DescribeEventsPaginatorName = Literal["describe_events"]
 DescribeServersPaginatorName = Literal["describe_servers"]
 ListTagsForResourcePaginatorName = Literal["list_tags_for_resource"]
 MaintenanceStatusType = Literal["FAILED", "SUCCESS"]
```

### Comparing `types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm/literals.pyi` & `types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm/paginator.py` & `types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 __all__ = (
     "DescribeBackupsPaginator",
     "DescribeEventsPaginator",
     "DescribeServersPaginator",
     "ListTagsForResourcePaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -65,15 +64,15 @@
     """
 
     def paginate(
         self,
         *,
         BackupId: str = ...,
         ServerName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeBackupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeBackups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/paginators/#describebackupspaginator)
         """
```

### Comparing `types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm/paginator.pyi` & `types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     """
 
     def paginate(
         self,
         *,
         BackupId: str = ...,
         ServerName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeBackupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeBackups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/paginators/#describebackupspaginator)
         """
 
 class DescribeEventsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm/type_defs.py` & `types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountAttributeTypeDef",
     "EngineAttributeTypeDef",
     "ResponseMetadataTypeDef",
     "BackupTypeDef",
     "TagTypeDef",
     "DeleteBackupRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm/type_defs.pyi` & `types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm/waiter.py` & `types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm/waiter.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,13 +35,13 @@
     """
 
     async def wait(
         self,
         *,
         NodeAssociationStatusToken: str,
         ServerName: str,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Waiter.NodeAssociated.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/waiters/#nodeassociatedwaiter)
         """
```

### Comparing `types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm/waiter.pyi` & `types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm/waiter.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -34,13 +34,13 @@
     """
 
     async def wait(
         self,
         *,
         NodeAssociationStatusToken: str,
         ServerName: str,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Waiter.NodeAssociated.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/waiters/#nodeassociatedwaiter)
         """
```

### Comparing `types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm.egg-info/PKG-INFO` & `types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-opsworkscm
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.OpsWorksCM 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.OpsWorksCM 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/
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
 
 <a id="types-aiobotocore-opsworkscm"></a>
 
 # types-aiobotocore-opsworkscm
 
 [![PyPI - types-aiobotocore-opsworkscm](https://img.shields.io/pypi/v/types-aiobotocore-opsworkscm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opsworkscm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-opsworkscm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opsworkscm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-opsworkscm)](https://pepy.tech/project/types-aiobotocore-opsworkscm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.OpsWorksCM 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
+[aiobotocore.OpsWorksCM 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
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
 [types-aiobotocore-opsworkscm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-opsworkscm-2.9.0/types_aiobotocore_opsworkscm.egg-info/SOURCES.txt` & `types-aiobotocore-opsworkscm-2.9.1/types_aiobotocore_opsworkscm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

