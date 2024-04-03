# Comparing `tmp/types-aiobotocore-iotdeviceadvisor-2.9.0.tar.gz` & `tmp/types-aiobotocore-iotdeviceadvisor-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotdeviceadvisor-2.9.0.tar", last modified: Wed Dec 13 19:59:32 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotdeviceadvisor-2.9.1.tar", last modified: Thu Jan 18 01:20:56 2024, max compression
```

## Comparing `types-aiobotocore-iotdeviceadvisor-2.9.0.tar` & `types-aiobotocore-iotdeviceadvisor-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:32.541651 types-aiobotocore-iotdeviceadvisor-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:47:53.000000 types-aiobotocore-iotdeviceadvisor-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12722 2023-12-13 19:59:32.541651 types-aiobotocore-iotdeviceadvisor-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11123 2023-12-13 19:47:53.000000 types-aiobotocore-iotdeviceadvisor-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:32.541651 types-aiobotocore-iotdeviceadvisor-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2023-12-13 19:47:53.000000 types-aiobotocore-iotdeviceadvisor-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:32.541651 types-aiobotocore-iotdeviceadvisor-2.9.0/types_aiobotocore_iotdeviceadvisor/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2023-12-13 19:47:53.000000 types-aiobotocore-iotdeviceadvisor-2.9.0/types_aiobotocore_iotdeviceadvisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2023-12-13 19:47:53.000000 types-aiobotocore-iotdeviceadvisor-2.9.0/types_aiobotocore_iotdeviceadvisor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      968 2023-12-13 19:47:53.000000 types-aiobotocore-iotdeviceadvisor-2.9.0/types_aiobotocore_iotdeviceadvisor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12968 2023-12-13 19:47:53.000000 types-aiobotocore-iotdeviceadvisor-2.9.0/types_aiobotocore_iotdeviceadvisor/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12965 2023-12-13 19:47:53.000000 types-aiobotocore-iotdeviceadvisor-2.9.0/types_aiobotocore_iotdeviceadvisor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9174 2023-12-13 19:47:53.000000 types-aiobotocore-iotdeviceadvisor-2.9.0/types_aiobotocore_iotdeviceadvisor/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9172 2023-12-13 19:47:53.000000 types-aiobotocore-iotdeviceadvisor-2.9.0/types_aiobotocore_iotdeviceadvisor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:47:53.000000 types-aiobotocore-iotdeviceadvisor-2.9.0/types_aiobotocore_iotdeviceadvisor/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    11381 2023-12-13 19:47:54.000000 types-aiobotocore-iotdeviceadvisor-2.9.0/types_aiobotocore_iotdeviceadvisor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11380 2023-12-13 19:47:53.000000 types-aiobotocore-iotdeviceadvisor-2.9.0/types_aiobotocore_iotdeviceadvisor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:47:53.000000 types-aiobotocore-iotdeviceadvisor-2.9.0/types_aiobotocore_iotdeviceadvisor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:32.541651 types-aiobotocore-iotdeviceadvisor-2.9.0/types_aiobotocore_iotdeviceadvisor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12722 2023-12-13 19:59:32.000000 types-aiobotocore-iotdeviceadvisor-2.9.0/types_aiobotocore_iotdeviceadvisor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      887 2023-12-13 19:59:32.000000 types-aiobotocore-iotdeviceadvisor-2.9.0/types_aiobotocore_iotdeviceadvisor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:32.000000 types-aiobotocore-iotdeviceadvisor-2.9.0/types_aiobotocore_iotdeviceadvisor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:32.000000 types-aiobotocore-iotdeviceadvisor-2.9.0/types_aiobotocore_iotdeviceadvisor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:32.000000 types-aiobotocore-iotdeviceadvisor-2.9.0/types_aiobotocore_iotdeviceadvisor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-13 19:59:32.000000 types-aiobotocore-iotdeviceadvisor-2.9.0/types_aiobotocore_iotdeviceadvisor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:56.041272 types-aiobotocore-iotdeviceadvisor-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:09:44.000000 types-aiobotocore-iotdeviceadvisor-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12742 2024-01-18 01:20:56.037272 types-aiobotocore-iotdeviceadvisor-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11123 2024-01-18 01:09:44.000000 types-aiobotocore-iotdeviceadvisor-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:56.041272 types-aiobotocore-iotdeviceadvisor-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-01-18 01:09:44.000000 types-aiobotocore-iotdeviceadvisor-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:56.037272 types-aiobotocore-iotdeviceadvisor-2.9.1/types_aiobotocore_iotdeviceadvisor/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-01-18 01:09:44.000000 types-aiobotocore-iotdeviceadvisor-2.9.1/types_aiobotocore_iotdeviceadvisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-01-18 01:09:44.000000 types-aiobotocore-iotdeviceadvisor-2.9.1/types_aiobotocore_iotdeviceadvisor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-01-18 01:09:44.000000 types-aiobotocore-iotdeviceadvisor-2.9.1/types_aiobotocore_iotdeviceadvisor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12973 2024-01-18 01:09:44.000000 types-aiobotocore-iotdeviceadvisor-2.9.1/types_aiobotocore_iotdeviceadvisor/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12970 2024-01-18 01:09:44.000000 types-aiobotocore-iotdeviceadvisor-2.9.1/types_aiobotocore_iotdeviceadvisor/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9172 2024-01-18 01:09:44.000000 types-aiobotocore-iotdeviceadvisor-2.9.1/types_aiobotocore_iotdeviceadvisor/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9172 2024-01-18 01:09:44.000000 types-aiobotocore-iotdeviceadvisor-2.9.1/types_aiobotocore_iotdeviceadvisor/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:09:44.000000 types-aiobotocore-iotdeviceadvisor-2.9.1/types_aiobotocore_iotdeviceadvisor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    11380 2024-01-18 01:09:44.000000 types-aiobotocore-iotdeviceadvisor-2.9.1/types_aiobotocore_iotdeviceadvisor/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11380 2024-01-18 01:09:44.000000 types-aiobotocore-iotdeviceadvisor-2.9.1/types_aiobotocore_iotdeviceadvisor/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:09:44.000000 types-aiobotocore-iotdeviceadvisor-2.9.1/types_aiobotocore_iotdeviceadvisor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:56.037272 types-aiobotocore-iotdeviceadvisor-2.9.1/types_aiobotocore_iotdeviceadvisor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12742 2024-01-18 01:20:56.000000 types-aiobotocore-iotdeviceadvisor-2.9.1/types_aiobotocore_iotdeviceadvisor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-01-18 01:20:56.000000 types-aiobotocore-iotdeviceadvisor-2.9.1/types_aiobotocore_iotdeviceadvisor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:56.000000 types-aiobotocore-iotdeviceadvisor-2.9.1/types_aiobotocore_iotdeviceadvisor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:56.000000 types-aiobotocore-iotdeviceadvisor-2.9.1/types_aiobotocore_iotdeviceadvisor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:56.000000 types-aiobotocore-iotdeviceadvisor-2.9.1/types_aiobotocore_iotdeviceadvisor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-18 01:20:56.000000 types-aiobotocore-iotdeviceadvisor-2.9.1/types_aiobotocore_iotdeviceadvisor.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotdeviceadvisor-2.9.0/LICENSE` & `types-aiobotocore-iotdeviceadvisor-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-iotdeviceadvisor-2.9.0/PKG-INFO` & `types-aiobotocore-iotdeviceadvisor-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotdeviceadvisor
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IoTDeviceAdvisor 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IoTDeviceAdvisor 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/
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
 
 <a id="types-aiobotocore-iotdeviceadvisor"></a>
 
 # types-aiobotocore-iotdeviceadvisor
 
 [![PyPI - types-aiobotocore-iotdeviceadvisor](https://img.shields.io/pypi/v/types-aiobotocore-iotdeviceadvisor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotdeviceadvisor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotdeviceadvisor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotdeviceadvisor)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotdeviceadvisor)](https://pepy.tech/project/types-aiobotocore-iotdeviceadvisor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTDeviceAdvisor 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
+[aiobotocore.IoTDeviceAdvisor 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
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
 [types-aiobotocore-iotdeviceadvisor docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iotdeviceadvisor-2.9.0/README.md` & `types-aiobotocore-iotdeviceadvisor-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotdeviceadvisor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotdeviceadvisor)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotdeviceadvisor)](https://pepy.tech/project/types-aiobotocore-iotdeviceadvisor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTDeviceAdvisor 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
+[aiobotocore.IoTDeviceAdvisor 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
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
 [types-aiobotocore-iotdeviceadvisor docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iotdeviceadvisor-2.9.0/setup.py` & `types-aiobotocore-iotdeviceadvisor-2.9.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotdeviceadvisor",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_iotdeviceadvisor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.IoTDeviceAdvisor 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.IoTDeviceAdvisor 2.9.1 service generated with"
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
     keywords="aiobotocore iotdeviceadvisor type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_iotdeviceadvisor": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-iotdeviceadvisor-2.9.0/types_aiobotocore_iotdeviceadvisor/__init__.py` & `types-aiobotocore-iotdeviceadvisor-2.9.1/types_aiobotocore_iotdeviceadvisor/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,9 +18,8 @@
     ```
 """
 
 from .client import IoTDeviceAdvisorClient
 
 Client = IoTDeviceAdvisorClient
 
-
 __all__ = ("Client", "IoTDeviceAdvisorClient")
```

### Comparing `types-aiobotocore-iotdeviceadvisor-2.9.0/types_aiobotocore_iotdeviceadvisor/__init__.pyi` & `types-aiobotocore-iotdeviceadvisor-2.9.1/types_aiobotocore_iotdeviceadvisor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotdeviceadvisor-2.9.0/types_aiobotocore_iotdeviceadvisor/__main__.py` & `types-aiobotocore-iotdeviceadvisor-2.9.1/types_aiobotocore_iotdeviceadvisor/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTDeviceAdvisor 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.IoTDeviceAdvisor 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor\nOther"
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

### Comparing `types-aiobotocore-iotdeviceadvisor-2.9.0/types_aiobotocore_iotdeviceadvisor/client.py` & `types-aiobotocore-iotdeviceadvisor-2.9.1/types_aiobotocore_iotdeviceadvisor/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#close)
         """
 
     async def create_suite_definition(
         self,
         *,
         suiteDefinitionConfiguration: SuiteDefinitionConfigurationTypeDef,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateSuiteDefinitionResponseTypeDef:
         """
         Creates a Device Advisor test suite.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.create_suite_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#create_suite_definition)
         """
@@ -125,15 +125,15 @@
 
     async def get_endpoint(
         self,
         *,
         thingArn: str = ...,
         certificateArn: str = ...,
         deviceRoleArn: str = ...,
-        authenticationMethod: AuthenticationMethodType = ...
+        authenticationMethod: AuthenticationMethodType = ...,
     ) -> GetEndpointResponseTypeDef:
         """
         Gets information about an Device Advisor endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.get_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#get_endpoint)
         """
@@ -182,15 +182,15 @@
 
     async def list_suite_runs(
         self,
         *,
         suiteDefinitionId: str = ...,
         suiteDefinitionVersion: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListSuiteRunsResponseTypeDef:
         """
         Lists runs of the specified Device Advisor test suite.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.list_suite_runs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#list_suite_runs)
         """
@@ -207,15 +207,15 @@
 
     async def start_suite_run(
         self,
         *,
         suiteDefinitionId: str,
         suiteRunConfiguration: SuiteRunConfigurationTypeDef,
         suiteDefinitionVersion: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> StartSuiteRunResponseTypeDef:
         """
         Starts a Device Advisor test suite run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.start_suite_run)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#start_suite_run)
         """
@@ -244,15 +244,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#untag_resource)
         """
 
     async def update_suite_definition(
         self,
         *,
         suiteDefinitionId: str,
-        suiteDefinitionConfiguration: SuiteDefinitionConfigurationTypeDef
+        suiteDefinitionConfiguration: SuiteDefinitionConfigurationTypeDef,
     ) -> UpdateSuiteDefinitionResponseTypeDef:
         """
         Updates a Device Advisor test suite.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.update_suite_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#update_suite_definition)
         """
```

### Comparing `types-aiobotocore-iotdeviceadvisor-2.9.0/types_aiobotocore_iotdeviceadvisor/client.pyi` & `types-aiobotocore-iotdeviceadvisor-2.9.1/types_aiobotocore_iotdeviceadvisor/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#close)
         """
 
     async def create_suite_definition(
         self,
         *,
         suiteDefinitionConfiguration: SuiteDefinitionConfigurationTypeDef,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateSuiteDefinitionResponseTypeDef:
         """
         Creates a Device Advisor test suite.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.create_suite_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#create_suite_definition)
         """
@@ -122,15 +122,15 @@
 
     async def get_endpoint(
         self,
         *,
         thingArn: str = ...,
         certificateArn: str = ...,
         deviceRoleArn: str = ...,
-        authenticationMethod: AuthenticationMethodType = ...
+        authenticationMethod: AuthenticationMethodType = ...,
     ) -> GetEndpointResponseTypeDef:
         """
         Gets information about an Device Advisor endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.get_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#get_endpoint)
         """
@@ -179,15 +179,15 @@
 
     async def list_suite_runs(
         self,
         *,
         suiteDefinitionId: str = ...,
         suiteDefinitionVersion: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListSuiteRunsResponseTypeDef:
         """
         Lists runs of the specified Device Advisor test suite.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.list_suite_runs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#list_suite_runs)
         """
@@ -204,15 +204,15 @@
 
     async def start_suite_run(
         self,
         *,
         suiteDefinitionId: str,
         suiteRunConfiguration: SuiteRunConfigurationTypeDef,
         suiteDefinitionVersion: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> StartSuiteRunResponseTypeDef:
         """
         Starts a Device Advisor test suite run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.start_suite_run)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#start_suite_run)
         """
@@ -241,15 +241,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#untag_resource)
         """
 
     async def update_suite_definition(
         self,
         *,
         suiteDefinitionId: str,
-        suiteDefinitionConfiguration: SuiteDefinitionConfigurationTypeDef
+        suiteDefinitionConfiguration: SuiteDefinitionConfigurationTypeDef,
     ) -> UpdateSuiteDefinitionResponseTypeDef:
         """
         Updates a Device Advisor test suite.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.update_suite_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#update_suite_definition)
         """
```

### Comparing `types-aiobotocore-iotdeviceadvisor-2.9.0/types_aiobotocore_iotdeviceadvisor/literals.py` & `types-aiobotocore-iotdeviceadvisor-2.9.1/types_aiobotocore_iotdeviceadvisor/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,29 +15,27 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AuthenticationMethodType",
     "ProtocolType",
     "StatusType",
     "SuiteRunStatusType",
     "TestCaseScenarioStatusType",
     "TestCaseScenarioTypeType",
     "IoTDeviceAdvisorServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AuthenticationMethodType = Literal["SignatureVersion4", "X509ClientCertificate"]
 ProtocolType = Literal["MqttV3_1_1", "MqttV3_1_1_OverWebSocket", "MqttV5", "MqttV5_OverWebSocket"]
 StatusType = Literal[
     "CANCELED",
     "ERROR",
     "FAIL",
     "PASS",
```

### Comparing `types-aiobotocore-iotdeviceadvisor-2.9.0/types_aiobotocore_iotdeviceadvisor/literals.pyi` & `types-aiobotocore-iotdeviceadvisor-2.9.1/types_aiobotocore_iotdeviceadvisor/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotdeviceadvisor-2.9.0/types_aiobotocore_iotdeviceadvisor/type_defs.py` & `types-aiobotocore-iotdeviceadvisor-2.9.1/types_aiobotocore_iotdeviceadvisor/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ResponseMetadataTypeDef",
     "DeleteSuiteDefinitionRequestRequestTypeDef",
     "DeviceUnderTestTypeDef",
     "GetEndpointRequestRequestTypeDef",
     "GetSuiteDefinitionRequestRequestTypeDef",
     "GetSuiteRunReportRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-iotdeviceadvisor-2.9.0/types_aiobotocore_iotdeviceadvisor/type_defs.pyi` & `types-aiobotocore-iotdeviceadvisor-2.9.1/types_aiobotocore_iotdeviceadvisor/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotdeviceadvisor-2.9.0/types_aiobotocore_iotdeviceadvisor.egg-info/PKG-INFO` & `types-aiobotocore-iotdeviceadvisor-2.9.1/types_aiobotocore_iotdeviceadvisor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotdeviceadvisor
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IoTDeviceAdvisor 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IoTDeviceAdvisor 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/
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
 
 <a id="types-aiobotocore-iotdeviceadvisor"></a>
 
 # types-aiobotocore-iotdeviceadvisor
 
 [![PyPI - types-aiobotocore-iotdeviceadvisor](https://img.shields.io/pypi/v/types-aiobotocore-iotdeviceadvisor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotdeviceadvisor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotdeviceadvisor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotdeviceadvisor)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotdeviceadvisor)](https://pepy.tech/project/types-aiobotocore-iotdeviceadvisor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTDeviceAdvisor 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
+[aiobotocore.IoTDeviceAdvisor 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
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
 [types-aiobotocore-iotdeviceadvisor docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iotdeviceadvisor-2.9.0/types_aiobotocore_iotdeviceadvisor.egg-info/SOURCES.txt` & `types-aiobotocore-iotdeviceadvisor-2.9.1/types_aiobotocore_iotdeviceadvisor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

