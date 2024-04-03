# Comparing `tmp/types-aiobotocore-arc-zonal-shift-2.9.0.tar.gz` & `tmp/types-aiobotocore-arc-zonal-shift-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-arc-zonal-shift-2.9.0.tar", last modified: Wed Dec 13 19:58:37 2023, max compression
+gzip compressed data, was "types-aiobotocore-arc-zonal-shift-2.9.1.tar", last modified: Thu Jan 18 01:20:05 2024, max compression
```

## Comparing `types-aiobotocore-arc-zonal-shift-2.9.0.tar` & `types-aiobotocore-arc-zonal-shift-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:37.594070 types-aiobotocore-arc-zonal-shift-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:41:19.000000 types-aiobotocore-arc-zonal-shift-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13719 2023-12-13 19:58:37.594070 types-aiobotocore-arc-zonal-shift-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12126 2023-12-13 19:41:19.000000 types-aiobotocore-arc-zonal-shift-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:37.594070 types-aiobotocore-arc-zonal-shift-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2023-12-13 19:41:19.000000 types-aiobotocore-arc-zonal-shift-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:37.594070 types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift/
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2023-12-13 19:41:19.000000 types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2023-12-13 19:41:19.000000 types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      960 2023-12-13 19:41:19.000000 types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14539 2023-12-13 19:41:19.000000 types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14535 2023-12-13 19:41:19.000000 types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9764 2023-12-13 19:41:20.000000 types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9762 2023-12-13 19:41:19.000000 types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2023-12-13 19:41:19.000000 types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4607 2023-12-13 19:41:19.000000 types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:41:19.000000 types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    11317 2023-12-13 19:41:20.000000 types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11316 2023-12-13 19:41:20.000000 types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:41:19.000000 types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:37.594070 types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13719 2023-12-13 19:58:37.000000 types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      965 2023-12-13 19:58:37.000000 types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:37.000000 types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:37.000000 types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:37.000000 types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-13 19:58:37.000000 types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:05.465505 types-aiobotocore-arc-zonal-shift-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:03:18.000000 types-aiobotocore-arc-zonal-shift-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13739 2024-01-18 01:20:05.465505 types-aiobotocore-arc-zonal-shift-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12126 2024-01-18 01:03:18.000000 types-aiobotocore-arc-zonal-shift-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:05.465505 types-aiobotocore-arc-zonal-shift-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-01-18 01:03:18.000000 types-aiobotocore-arc-zonal-shift-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:05.465505 types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift/
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-01-18 01:03:18.000000 types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-01-18 01:03:18.000000 types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-01-18 01:03:18.000000 types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14542 2024-01-18 01:03:18.000000 types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14539 2024-01-18 01:03:18.000000 types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9762 2024-01-18 01:03:19.000000 types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9762 2024-01-18 01:03:19.000000 types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-01-18 01:03:19.000000 types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-01-18 01:03:19.000000 types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:03:18.000000 types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-01-18 01:03:19.000000 types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-01-18 01:03:19.000000 types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:03:18.000000 types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:05.465505 types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13739 2024-01-18 01:20:05.000000 types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-01-18 01:20:05.000000 types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:05.000000 types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:05.000000 types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:05.000000 types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-01-18 01:20:05.000000 types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-arc-zonal-shift-2.9.0/LICENSE` & `types-aiobotocore-arc-zonal-shift-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-arc-zonal-shift-2.9.0/PKG-INFO` & `types-aiobotocore-arc-zonal-shift-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-arc-zonal-shift
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ARCZonalShift 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ARCZonalShift 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/
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
 
 <a id="types-aiobotocore-arc-zonal-shift"></a>
 
 # types-aiobotocore-arc-zonal-shift
 
 [![PyPI - types-aiobotocore-arc-zonal-shift](https://img.shields.io/pypi/v/types-aiobotocore-arc-zonal-shift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-arc-zonal-shift)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-arc-zonal-shift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-arc-zonal-shift)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-arc-zonal-shift)](https://pepy.tech/project/types-aiobotocore-arc-zonal-shift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ARCZonalShift 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
+[aiobotocore.ARCZonalShift 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
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
 [types-aiobotocore-arc-zonal-shift docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-arc-zonal-shift-2.9.0/README.md` & `types-aiobotocore-arc-zonal-shift-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-arc-zonal-shift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-arc-zonal-shift)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-arc-zonal-shift)](https://pepy.tech/project/types-aiobotocore-arc-zonal-shift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ARCZonalShift 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
+[aiobotocore.ARCZonalShift 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
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
 [types-aiobotocore-arc-zonal-shift docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-arc-zonal-shift-2.9.0/setup.py` & `types-aiobotocore-arc-zonal-shift-2.9.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-arc-zonal-shift",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_arc_zonal_shift"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ARCZonalShift 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ARCZonalShift 2.9.1 service generated with"
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
     keywords="aiobotocore arc-zonal-shift type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_arc_zonal_shift": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift/__init__.py` & `types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     ListAutoshiftsPaginator,
     ListManagedResourcesPaginator,
     ListZonalShiftsPaginator,
 )
 
 Client = ARCZonalShiftClient
 
-
 __all__ = (
     "ARCZonalShiftClient",
     "Client",
     "ListAutoshiftsPaginator",
     "ListManagedResourcesPaginator",
     "ListZonalShiftsPaginator",
 )
```

### Comparing `types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift/__init__.pyi` & `types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift/__main__.py` & `types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ARCZonalShift 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ARCZonalShift 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift\nOther"
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

### Comparing `types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift/client.py` & `types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ARCZonalShiftClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -111,15 +110,15 @@
     async def create_practice_run_configuration(
         self,
         *,
         outcomeAlarms: Sequence[ControlConditionTypeDef],
         resourceIdentifier: str,
         blockedDates: Sequence[str] = ...,
         blockedWindows: Sequence[str] = ...,
-        blockingAlarms: Sequence[ControlConditionTypeDef] = ...
+        blockingAlarms: Sequence[ControlConditionTypeDef] = ...,
     ) -> CreatePracticeRunConfigurationResponseTypeDef:
         """
         A practice run configuration for zonal autoshift is required when you enable
         zonal
         autoshift.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Client.create_practice_run_configuration)
@@ -163,15 +162,15 @@
         """
 
     async def list_autoshifts(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
-        status: AutoshiftExecutionStatusType = ...
+        status: AutoshiftExecutionStatusType = ...,
     ) -> ListAutoshiftsResponseTypeDef:
         """
         Returns the active autoshifts for a specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Client.list_autoshifts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/client/#list_autoshifts)
         """
@@ -191,15 +190,15 @@
 
     async def list_zonal_shifts(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
         resourceIdentifier: str = ...,
-        status: ZonalShiftStatusType = ...
+        status: ZonalShiftStatusType = ...,
     ) -> ListZonalShiftsResponseTypeDef:
         """
         Lists all active and completed zonal shifts in Amazon Route 53 Application
         Recovery Controller in your Amazon Web Services account in this Amazon Web
         Services
         Region.
 
@@ -224,15 +223,15 @@
     async def update_practice_run_configuration(
         self,
         *,
         resourceIdentifier: str,
         blockedDates: Sequence[str] = ...,
         blockedWindows: Sequence[str] = ...,
         blockingAlarms: Sequence[ControlConditionTypeDef] = ...,
-        outcomeAlarms: Sequence[ControlConditionTypeDef] = ...
+        outcomeAlarms: Sequence[ControlConditionTypeDef] = ...,
     ) -> UpdatePracticeRunConfigurationResponseTypeDef:
         """
         Update a practice run configuration to change one or more of the following:
         add, change, or remove the blocking alarm; change the outcome alarm; or add,
         change, or remove blocking dates or time
         windows.
```

### Comparing `types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift/client.pyi` & `types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     async def create_practice_run_configuration(
         self,
         *,
         outcomeAlarms: Sequence[ControlConditionTypeDef],
         resourceIdentifier: str,
         blockedDates: Sequence[str] = ...,
         blockedWindows: Sequence[str] = ...,
-        blockingAlarms: Sequence[ControlConditionTypeDef] = ...
+        blockingAlarms: Sequence[ControlConditionTypeDef] = ...,
     ) -> CreatePracticeRunConfigurationResponseTypeDef:
         """
         A practice run configuration for zonal autoshift is required when you enable
         zonal
         autoshift.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Client.create_practice_run_configuration)
@@ -159,15 +159,15 @@
         """
 
     async def list_autoshifts(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
-        status: AutoshiftExecutionStatusType = ...
+        status: AutoshiftExecutionStatusType = ...,
     ) -> ListAutoshiftsResponseTypeDef:
         """
         Returns the active autoshifts for a specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Client.list_autoshifts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/client/#list_autoshifts)
         """
@@ -187,15 +187,15 @@
 
     async def list_zonal_shifts(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
         resourceIdentifier: str = ...,
-        status: ZonalShiftStatusType = ...
+        status: ZonalShiftStatusType = ...,
     ) -> ListZonalShiftsResponseTypeDef:
         """
         Lists all active and completed zonal shifts in Amazon Route 53 Application
         Recovery Controller in your Amazon Web Services account in this Amazon Web
         Services
         Region.
 
@@ -220,15 +220,15 @@
     async def update_practice_run_configuration(
         self,
         *,
         resourceIdentifier: str,
         blockedDates: Sequence[str] = ...,
         blockedWindows: Sequence[str] = ...,
         blockingAlarms: Sequence[ControlConditionTypeDef] = ...,
-        outcomeAlarms: Sequence[ControlConditionTypeDef] = ...
+        outcomeAlarms: Sequence[ControlConditionTypeDef] = ...,
     ) -> UpdatePracticeRunConfigurationResponseTypeDef:
         """
         Update a practice run configuration to change one or more of the following:
         add, change, or remove the blocking alarm; change the outcome alarm; or add,
         change, or remove blocking dates or time
         windows.
```

### Comparing `types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift/literals.py` & `types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift/literals.py`

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
     "AppliedStatusType",
     "AutoshiftAppliedStatusType",
     "AutoshiftExecutionStatusType",
     "ControlConditionTypeType",
     "ListAutoshiftsPaginatorName",
     "ListManagedResourcesPaginatorName",
@@ -34,15 +33,14 @@
     "ARCZonalShiftServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AppliedStatusType = Literal["APPLIED", "NOT_APPLIED"]
 AutoshiftAppliedStatusType = Literal["APPLIED", "NOT_APPLIED"]
 AutoshiftExecutionStatusType = Literal["ACTIVE", "COMPLETED"]
 ControlConditionTypeType = Literal["CLOUDWATCH"]
 ListAutoshiftsPaginatorName = Literal["list_autoshifts"]
 ListManagedResourcesPaginatorName = Literal["list_managed_resources"]
 ListZonalShiftsPaginatorName = Literal["list_zonal_shifts"]
```

### Comparing `types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift/literals.pyi` & `types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift/paginator.py` & `types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     ListManagedResourcesResponseTypeDef,
     ListZonalShiftsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListAutoshiftsPaginator", "ListManagedResourcesPaginator", "ListZonalShiftsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -57,15 +56,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/paginators/#listautoshiftspaginator)
     """
 
     def paginate(
         self,
         *,
         status: AutoshiftExecutionStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAutoshiftsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Paginator.ListAutoshifts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/paginators/#listautoshiftspaginator)
         """
 
 
@@ -91,13 +90,13 @@
     """
 
     def paginate(
         self,
         *,
         resourceIdentifier: str = ...,
         status: ZonalShiftStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListZonalShiftsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Paginator.ListZonalShifts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/paginators/#listzonalshiftspaginator)
         """
```

### Comparing `types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift/paginator.pyi` & `types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift/paginator.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/paginators/#listautoshiftspaginator)
     """
 
     def paginate(
         self,
         *,
         status: AutoshiftExecutionStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAutoshiftsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Paginator.ListAutoshifts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/paginators/#listautoshiftspaginator)
         """
 
 class ListManagedResourcesPaginator(AioPaginator):
@@ -86,13 +86,13 @@
     """
 
     def paginate(
         self,
         *,
         resourceIdentifier: str = ...,
         status: ZonalShiftStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListZonalShiftsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Paginator.ListZonalShifts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/paginators/#listzonalshiftspaginator)
         """
```

### Comparing `types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift/type_defs.py` & `types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AutoshiftInResourceTypeDef",
     "AutoshiftSummaryTypeDef",
     "CancelZonalShiftRequestRequestTypeDef",
     "ControlConditionTypeDef",
     "ResponseMetadataTypeDef",
     "DeletePracticeRunConfigurationRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift/type_defs.pyi` & `types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift.egg-info/PKG-INFO` & `types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-arc-zonal-shift
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ARCZonalShift 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ARCZonalShift 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/
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
 
 <a id="types-aiobotocore-arc-zonal-shift"></a>
 
 # types-aiobotocore-arc-zonal-shift
 
 [![PyPI - types-aiobotocore-arc-zonal-shift](https://img.shields.io/pypi/v/types-aiobotocore-arc-zonal-shift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-arc-zonal-shift)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-arc-zonal-shift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-arc-zonal-shift)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-arc-zonal-shift)](https://pepy.tech/project/types-aiobotocore-arc-zonal-shift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ARCZonalShift 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
+[aiobotocore.ARCZonalShift 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
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
 [types-aiobotocore-arc-zonal-shift docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-arc-zonal-shift-2.9.0/types_aiobotocore_arc_zonal_shift.egg-info/SOURCES.txt` & `types-aiobotocore-arc-zonal-shift-2.9.1/types_aiobotocore_arc_zonal_shift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

