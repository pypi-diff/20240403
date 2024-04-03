# Comparing `tmp/types-aiobotocore-iotsecuretunneling-2.9.0.tar.gz` & `tmp/types-aiobotocore-iotsecuretunneling-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotsecuretunneling-2.9.0.tar", last modified: Wed Dec 13 19:59:34 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotsecuretunneling-2.9.1.tar", last modified: Thu Jan 18 01:20:57 2024, max compression
```

## Comparing `types-aiobotocore-iotsecuretunneling-2.9.0.tar` & `types-aiobotocore-iotsecuretunneling-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:34.377624 types-aiobotocore-iotsecuretunneling-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:48:00.000000 types-aiobotocore-iotsecuretunneling-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12826 2023-12-13 19:59:34.377624 types-aiobotocore-iotsecuretunneling-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11219 2023-12-13 19:48:00.000000 types-aiobotocore-iotsecuretunneling-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:34.377624 types-aiobotocore-iotsecuretunneling-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2023-12-13 19:48:00.000000 types-aiobotocore-iotsecuretunneling-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:34.377624 types-aiobotocore-iotsecuretunneling-2.9.0/types_aiobotocore_iotsecuretunneling/
--rw-r--r--   0 runner    (1001) docker     (127)      531 2023-12-13 19:48:00.000000 types-aiobotocore-iotsecuretunneling-2.9.0/types_aiobotocore_iotsecuretunneling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2023-12-13 19:48:00.000000 types-aiobotocore-iotsecuretunneling-2.9.0/types_aiobotocore_iotsecuretunneling/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      976 2023-12-13 19:48:00.000000 types-aiobotocore-iotsecuretunneling-2.9.0/types_aiobotocore_iotsecuretunneling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9226 2023-12-13 19:48:00.000000 types-aiobotocore-iotsecuretunneling-2.9.0/types_aiobotocore_iotsecuretunneling/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9223 2023-12-13 19:48:00.000000 types-aiobotocore-iotsecuretunneling-2.9.0/types_aiobotocore_iotsecuretunneling/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8775 2023-12-13 19:48:00.000000 types-aiobotocore-iotsecuretunneling-2.9.0/types_aiobotocore_iotsecuretunneling/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8773 2023-12-13 19:48:00.000000 types-aiobotocore-iotsecuretunneling-2.9.0/types_aiobotocore_iotsecuretunneling/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:48:00.000000 types-aiobotocore-iotsecuretunneling-2.9.0/types_aiobotocore_iotsecuretunneling/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5979 2023-12-13 19:48:01.000000 types-aiobotocore-iotsecuretunneling-2.9.0/types_aiobotocore_iotsecuretunneling/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5978 2023-12-13 19:48:00.000000 types-aiobotocore-iotsecuretunneling-2.9.0/types_aiobotocore_iotsecuretunneling/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:48:00.000000 types-aiobotocore-iotsecuretunneling-2.9.0/types_aiobotocore_iotsecuretunneling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:34.377624 types-aiobotocore-iotsecuretunneling-2.9.0/types_aiobotocore_iotsecuretunneling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12826 2023-12-13 19:59:34.000000 types-aiobotocore-iotsecuretunneling-2.9.0/types_aiobotocore_iotsecuretunneling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      921 2023-12-13 19:59:34.000000 types-aiobotocore-iotsecuretunneling-2.9.0/types_aiobotocore_iotsecuretunneling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:34.000000 types-aiobotocore-iotsecuretunneling-2.9.0/types_aiobotocore_iotsecuretunneling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:34.000000 types-aiobotocore-iotsecuretunneling-2.9.0/types_aiobotocore_iotsecuretunneling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:34.000000 types-aiobotocore-iotsecuretunneling-2.9.0/types_aiobotocore_iotsecuretunneling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-13 19:59:34.000000 types-aiobotocore-iotsecuretunneling-2.9.0/types_aiobotocore_iotsecuretunneling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:57.745264 types-aiobotocore-iotsecuretunneling-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:09:51.000000 types-aiobotocore-iotsecuretunneling-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12846 2024-01-18 01:20:57.745264 types-aiobotocore-iotsecuretunneling-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11219 2024-01-18 01:09:51.000000 types-aiobotocore-iotsecuretunneling-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:57.745264 types-aiobotocore-iotsecuretunneling-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-01-18 01:09:51.000000 types-aiobotocore-iotsecuretunneling-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:57.745264 types-aiobotocore-iotsecuretunneling-2.9.1/types_aiobotocore_iotsecuretunneling/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-01-18 01:09:51.000000 types-aiobotocore-iotsecuretunneling-2.9.1/types_aiobotocore_iotsecuretunneling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-01-18 01:09:51.000000 types-aiobotocore-iotsecuretunneling-2.9.1/types_aiobotocore_iotsecuretunneling/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-01-18 01:09:51.000000 types-aiobotocore-iotsecuretunneling-2.9.1/types_aiobotocore_iotsecuretunneling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9228 2024-01-18 01:09:51.000000 types-aiobotocore-iotsecuretunneling-2.9.1/types_aiobotocore_iotsecuretunneling/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9225 2024-01-18 01:09:51.000000 types-aiobotocore-iotsecuretunneling-2.9.1/types_aiobotocore_iotsecuretunneling/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8773 2024-01-18 01:09:51.000000 types-aiobotocore-iotsecuretunneling-2.9.1/types_aiobotocore_iotsecuretunneling/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8773 2024-01-18 01:09:51.000000 types-aiobotocore-iotsecuretunneling-2.9.1/types_aiobotocore_iotsecuretunneling/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:09:51.000000 types-aiobotocore-iotsecuretunneling-2.9.1/types_aiobotocore_iotsecuretunneling/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-01-18 01:09:51.000000 types-aiobotocore-iotsecuretunneling-2.9.1/types_aiobotocore_iotsecuretunneling/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-01-18 01:09:51.000000 types-aiobotocore-iotsecuretunneling-2.9.1/types_aiobotocore_iotsecuretunneling/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:09:51.000000 types-aiobotocore-iotsecuretunneling-2.9.1/types_aiobotocore_iotsecuretunneling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:57.745264 types-aiobotocore-iotsecuretunneling-2.9.1/types_aiobotocore_iotsecuretunneling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12846 2024-01-18 01:20:57.000000 types-aiobotocore-iotsecuretunneling-2.9.1/types_aiobotocore_iotsecuretunneling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-01-18 01:20:57.000000 types-aiobotocore-iotsecuretunneling-2.9.1/types_aiobotocore_iotsecuretunneling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:57.000000 types-aiobotocore-iotsecuretunneling-2.9.1/types_aiobotocore_iotsecuretunneling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:57.000000 types-aiobotocore-iotsecuretunneling-2.9.1/types_aiobotocore_iotsecuretunneling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:57.000000 types-aiobotocore-iotsecuretunneling-2.9.1/types_aiobotocore_iotsecuretunneling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-01-18 01:20:57.000000 types-aiobotocore-iotsecuretunneling-2.9.1/types_aiobotocore_iotsecuretunneling.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotsecuretunneling-2.9.0/LICENSE` & `types-aiobotocore-iotsecuretunneling-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-iotsecuretunneling-2.9.0/PKG-INFO` & `types-aiobotocore-iotsecuretunneling-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotsecuretunneling
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IoTSecureTunneling 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IoTSecureTunneling 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/
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
 
 <a id="types-aiobotocore-iotsecuretunneling"></a>
 
 # types-aiobotocore-iotsecuretunneling
 
 [![PyPI - types-aiobotocore-iotsecuretunneling](https://img.shields.io/pypi/v/types-aiobotocore-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotsecuretunneling)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotsecuretunneling)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotsecuretunneling)](https://pepy.tech/project/types-aiobotocore-iotsecuretunneling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTSecureTunneling 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
+[aiobotocore.IoTSecureTunneling 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
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
 [types-aiobotocore-iotsecuretunneling docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iotsecuretunneling-2.9.0/README.md` & `types-aiobotocore-iotsecuretunneling-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotsecuretunneling)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotsecuretunneling)](https://pepy.tech/project/types-aiobotocore-iotsecuretunneling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTSecureTunneling 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
+[aiobotocore.IoTSecureTunneling 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
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
 [types-aiobotocore-iotsecuretunneling docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iotsecuretunneling-2.9.0/setup.py` & `types-aiobotocore-iotsecuretunneling-2.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotsecuretunneling",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_iotsecuretunneling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.IoTSecureTunneling 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.IoTSecureTunneling 2.9.1 service generated with"
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
     keywords="aiobotocore iotsecuretunneling type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_iotsecuretunneling": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-iotsecuretunneling-2.9.0/types_aiobotocore_iotsecuretunneling/__init__.py` & `types-aiobotocore-iotsecuretunneling-2.9.1/types_aiobotocore_iotsecuretunneling/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,9 +18,8 @@
     ```
 """
 
 from .client import IoTSecureTunnelingClient
 
 Client = IoTSecureTunnelingClient
 
-
 __all__ = ("Client", "IoTSecureTunnelingClient")
```

### Comparing `types-aiobotocore-iotsecuretunneling-2.9.0/types_aiobotocore_iotsecuretunneling/__init__.pyi` & `types-aiobotocore-iotsecuretunneling-2.9.1/types_aiobotocore_iotsecuretunneling/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsecuretunneling-2.9.0/types_aiobotocore_iotsecuretunneling/__main__.py` & `types-aiobotocore-iotsecuretunneling-2.9.1/types_aiobotocore_iotsecuretunneling/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTSecureTunneling 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.IoTSecureTunneling 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling\nOther"
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

### Comparing `types-aiobotocore-iotsecuretunneling-2.9.0/types_aiobotocore_iotsecuretunneling/client.py` & `types-aiobotocore-iotsecuretunneling-2.9.1/types_aiobotocore_iotsecuretunneling/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 
     async def open_tunnel(
         self,
         *,
         description: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         destinationConfig: DestinationConfigTypeDef = ...,
-        timeoutConfig: TimeoutConfigTypeDef = ...
+        timeoutConfig: TimeoutConfigTypeDef = ...,
     ) -> OpenTunnelResponseTypeDef:
         """
         Creates a new tunnel, and returns two client access tokens for clients to use
         to connect to the IoT Secure Tunneling proxy
         server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.open_tunnel)
@@ -150,15 +150,15 @@
         """
 
     async def rotate_tunnel_access_token(
         self,
         *,
         tunnelId: str,
         clientMode: ClientModeType,
-        destinationConfig: DestinationConfigTypeDef = ...
+        destinationConfig: DestinationConfigTypeDef = ...,
     ) -> RotateTunnelAccessTokenResponseTypeDef:
         """
         Revokes the current client access token (CAT) and returns new CAT for clients
         to use when reconnecting to secure tunneling to access the same
         tunnel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.rotate_tunnel_access_token)
```

### Comparing `types-aiobotocore-iotsecuretunneling-2.9.0/types_aiobotocore_iotsecuretunneling/client.pyi` & `types-aiobotocore-iotsecuretunneling-2.9.1/types_aiobotocore_iotsecuretunneling/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 
     async def open_tunnel(
         self,
         *,
         description: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         destinationConfig: DestinationConfigTypeDef = ...,
-        timeoutConfig: TimeoutConfigTypeDef = ...
+        timeoutConfig: TimeoutConfigTypeDef = ...,
     ) -> OpenTunnelResponseTypeDef:
         """
         Creates a new tunnel, and returns two client access tokens for clients to use
         to connect to the IoT Secure Tunneling proxy
         server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.open_tunnel)
@@ -147,15 +147,15 @@
         """
 
     async def rotate_tunnel_access_token(
         self,
         *,
         tunnelId: str,
         clientMode: ClientModeType,
-        destinationConfig: DestinationConfigTypeDef = ...
+        destinationConfig: DestinationConfigTypeDef = ...,
     ) -> RotateTunnelAccessTokenResponseTypeDef:
         """
         Revokes the current client access token (CAT) and returns new CAT for clients
         to use when reconnecting to secure tunneling to access the same
         tunnel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.rotate_tunnel_access_token)
```

### Comparing `types-aiobotocore-iotsecuretunneling-2.9.0/types_aiobotocore_iotsecuretunneling/literals.py` & `types-aiobotocore-iotsecuretunneling-2.9.1/types_aiobotocore_iotsecuretunneling/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,26 +15,24 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ClientModeType",
     "ConnectionStatusType",
     "TunnelStatusType",
     "IoTSecureTunnelingServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 ClientModeType = Literal["ALL", "DESTINATION", "SOURCE"]
 ConnectionStatusType = Literal["CONNECTED", "DISCONNECTED"]
 TunnelStatusType = Literal["CLOSED", "OPEN"]
 IoTSecureTunnelingServiceName = Literal["iotsecuretunneling"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
```

### Comparing `types-aiobotocore-iotsecuretunneling-2.9.0/types_aiobotocore_iotsecuretunneling/literals.pyi` & `types-aiobotocore-iotsecuretunneling-2.9.1/types_aiobotocore_iotsecuretunneling/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsecuretunneling-2.9.0/types_aiobotocore_iotsecuretunneling/type_defs.py` & `types-aiobotocore-iotsecuretunneling-2.9.1/types_aiobotocore_iotsecuretunneling/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CloseTunnelRequestRequestTypeDef",
     "ConnectionStateTypeDef",
     "DescribeTunnelRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DestinationConfigTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-iotsecuretunneling-2.9.0/types_aiobotocore_iotsecuretunneling/type_defs.pyi` & `types-aiobotocore-iotsecuretunneling-2.9.1/types_aiobotocore_iotsecuretunneling/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsecuretunneling-2.9.0/types_aiobotocore_iotsecuretunneling.egg-info/PKG-INFO` & `types-aiobotocore-iotsecuretunneling-2.9.1/types_aiobotocore_iotsecuretunneling.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotsecuretunneling
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IoTSecureTunneling 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IoTSecureTunneling 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/
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
 
 <a id="types-aiobotocore-iotsecuretunneling"></a>
 
 # types-aiobotocore-iotsecuretunneling
 
 [![PyPI - types-aiobotocore-iotsecuretunneling](https://img.shields.io/pypi/v/types-aiobotocore-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotsecuretunneling)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotsecuretunneling)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotsecuretunneling)](https://pepy.tech/project/types-aiobotocore-iotsecuretunneling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTSecureTunneling 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
+[aiobotocore.IoTSecureTunneling 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
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
 [types-aiobotocore-iotsecuretunneling docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iotsecuretunneling-2.9.0/types_aiobotocore_iotsecuretunneling.egg-info/SOURCES.txt` & `types-aiobotocore-iotsecuretunneling-2.9.1/types_aiobotocore_iotsecuretunneling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

