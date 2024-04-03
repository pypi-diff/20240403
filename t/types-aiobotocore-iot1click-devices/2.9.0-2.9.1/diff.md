# Comparing `tmp/types-aiobotocore-iot1click-devices-2.9.0.tar.gz` & `tmp/types-aiobotocore-iot1click-devices-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iot1click-devices-2.9.0.tar", last modified: Wed Dec 13 19:59:29 2023, max compression
+gzip compressed data, was "types-aiobotocore-iot1click-devices-2.9.1.tar", last modified: Thu Jan 18 01:20:53 2024, max compression
```

## Comparing `types-aiobotocore-iot1click-devices-2.9.0.tar` & `types-aiobotocore-iot1click-devices-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:29.917673 types-aiobotocore-iot1click-devices-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:47:49.000000 types-aiobotocore-iot1click-devices-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13820 2023-12-13 19:59:29.917673 types-aiobotocore-iot1click-devices-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12211 2023-12-13 19:47:49.000000 types-aiobotocore-iot1click-devices-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:29.917673 types-aiobotocore-iot1click-devices-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2023-12-13 19:47:49.000000 types-aiobotocore-iot1click-devices-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:29.917673 types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices/
--rw-r--r--   0 runner    (1001) docker     (127)      955 2023-12-13 19:47:49.000000 types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2023-12-13 19:47:49.000000 types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      984 2023-12-13 19:47:49.000000 types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14046 2023-12-13 19:47:49.000000 types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14042 2023-12-13 19:47:49.000000 types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8458 2023-12-13 19:47:49.000000 types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8456 2023-12-13 19:47:49.000000 types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2023-12-13 19:47:49.000000 types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2023-12-13 19:47:49.000000 types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:47:49.000000 types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8382 2023-12-13 19:47:49.000000 types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8381 2023-12-13 19:47:49.000000 types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:47:49.000000 types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:29.917673 types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13820 2023-12-13 19:59:29.000000 types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2023-12-13 19:59:29.000000 types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:29.000000 types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:29.000000 types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:29.000000 types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-13 19:59:29.000000 types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:53.597283 types-aiobotocore-iot1click-devices-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:09:39.000000 types-aiobotocore-iot1click-devices-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13840 2024-01-18 01:20:53.597283 types-aiobotocore-iot1click-devices-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12211 2024-01-18 01:09:39.000000 types-aiobotocore-iot1click-devices-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:53.597283 types-aiobotocore-iot1click-devices-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-01-18 01:09:39.000000 types-aiobotocore-iot1click-devices-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:53.593283 types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices/
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-01-18 01:09:39.000000 types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-01-18 01:09:39.000000 types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-18 01:09:39.000000 types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14047 2024-01-18 01:09:39.000000 types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14044 2024-01-18 01:09:39.000000 types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8456 2024-01-18 01:09:40.000000 types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8456 2024-01-18 01:09:40.000000 types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-01-18 01:09:39.000000 types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-01-18 01:09:39.000000 types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:09:39.000000 types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-01-18 01:09:40.000000 types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-01-18 01:09:40.000000 types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:09:39.000000 types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:53.597283 types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13840 2024-01-18 01:20:53.000000 types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-01-18 01:20:53.000000 types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:53.000000 types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:53.000000 types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:53.000000 types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-18 01:20:53.000000 types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iot1click-devices-2.9.0/LICENSE` & `types-aiobotocore-iot1click-devices-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-iot1click-devices-2.9.0/PKG-INFO` & `types-aiobotocore-iot1click-devices-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iot1click-devices
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IoT1ClickDevicesService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IoT1ClickDevicesService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/
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
 
 <a id="types-aiobotocore-iot1click-devices"></a>
 
 # types-aiobotocore-iot1click-devices
 
 [![PyPI - types-aiobotocore-iot1click-devices](https://img.shields.io/pypi/v/types-aiobotocore-iot1click-devices.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot1click-devices)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot1click-devices.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot1click-devices)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot1click-devices)](https://pepy.tech/project/types-aiobotocore-iot1click-devices)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoT1ClickDevicesService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
+[aiobotocore.IoT1ClickDevicesService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
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
 [types-aiobotocore-iot1click-devices docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iot1click-devices-2.9.0/README.md` & `types-aiobotocore-iot1click-devices-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot1click-devices.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot1click-devices)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot1click-devices)](https://pepy.tech/project/types-aiobotocore-iot1click-devices)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoT1ClickDevicesService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
+[aiobotocore.IoT1ClickDevicesService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
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
 [types-aiobotocore-iot1click-devices docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iot1click-devices-2.9.0/setup.py` & `types-aiobotocore-iot1click-devices-2.9.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iot1click-devices",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_iot1click_devices"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.IoT1ClickDevicesService 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.IoT1ClickDevicesService 2.9.1 service generated with"
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
     keywords="aiobotocore iot1click-devices type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_iot1click_devices": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices/__init__.py` & `types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,13 @@
 """
 
 from .client import IoT1ClickDevicesServiceClient
 from .paginator import ListDeviceEventsPaginator, ListDevicesPaginator
 
 Client = IoT1ClickDevicesServiceClient
 
-
 __all__ = (
     "Client",
     "IoT1ClickDevicesServiceClient",
     "ListDeviceEventsPaginator",
     "ListDevicesPaginator",
 )
```

### Comparing `types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices/__init__.pyi` & `types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices/__main__.py` & `types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoT1ClickDevicesService 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.IoT1ClickDevicesService 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService\nOther"
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

### Comparing `types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices/client.py` & `types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("IoT1ClickDevicesServiceClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -162,15 +161,15 @@
         """
 
     async def invoke_device_method(
         self,
         *,
         DeviceId: str,
         DeviceMethod: DeviceMethodTypeDef = ...,
-        DeviceMethodParameters: str = ...
+        DeviceMethodParameters: str = ...,
     ) -> InvokeDeviceMethodResponseTypeDef:
         """
         Given a device ID, issues a request to invoke a named device method (with
         possible
         parameters).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Client.invoke_device_method)
@@ -180,15 +179,15 @@
     async def list_device_events(
         self,
         *,
         DeviceId: str,
         FromTimeStamp: TimestampTypeDef,
         ToTimeStamp: TimestampTypeDef,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListDeviceEventsResponseTypeDef:
         """
         Using a device ID, returns a DeviceEventsResponse object containing an array of
         events for the
         device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Client.list_device_events)
```

### Comparing `types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices/client.pyi` & `types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         """
 
     async def invoke_device_method(
         self,
         *,
         DeviceId: str,
         DeviceMethod: DeviceMethodTypeDef = ...,
-        DeviceMethodParameters: str = ...
+        DeviceMethodParameters: str = ...,
     ) -> InvokeDeviceMethodResponseTypeDef:
         """
         Given a device ID, issues a request to invoke a named device method (with
         possible
         parameters).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Client.invoke_device_method)
@@ -176,15 +176,15 @@
     async def list_device_events(
         self,
         *,
         DeviceId: str,
         FromTimeStamp: TimestampTypeDef,
         ToTimeStamp: TimestampTypeDef,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListDeviceEventsResponseTypeDef:
         """
         Using a device ID, returns a DeviceEventsResponse object containing an array of
         events for the
         device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Client.list_device_events)
```

### Comparing `types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices/literals.py` & `types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,25 +15,23 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListDeviceEventsPaginatorName",
     "ListDevicesPaginatorName",
     "IoT1ClickDevicesServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 ListDeviceEventsPaginatorName = Literal["list_device_events"]
 ListDevicesPaginatorName = Literal["list_devices"]
 IoT1ClickDevicesServiceServiceName = Literal["iot1click-devices"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
```

### Comparing `types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices/literals.pyi` & `types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices/paginator.py` & `types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     ListDevicesResponseTypeDef,
     PaginatorConfigTypeDef,
     TimestampTypeDef,
 )
 
 __all__ = ("ListDeviceEventsPaginator", "ListDevicesPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -56,15 +55,15 @@
 
     def paginate(
         self,
         *,
         DeviceId: str,
         FromTimeStamp: TimestampTypeDef,
         ToTimeStamp: TimestampTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDeviceEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Paginator.ListDeviceEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/paginators/#listdeviceeventspaginator)
         """
```

### Comparing `types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices/paginator.pyi` & `types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
     def paginate(
         self,
         *,
         DeviceId: str,
         FromTimeStamp: TimestampTypeDef,
         ToTimeStamp: TimestampTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDeviceEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Paginator.ListDeviceEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/paginators/#listdeviceeventspaginator)
         """
 
 class ListDevicesPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices/type_defs.py` & `types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ClaimDevicesByClaimCodeRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DescribeDeviceRequestRequestTypeDef",
     "DeviceDescriptionTypeDef",
     "DeviceTypeDef",
     "DeviceMethodTypeDef",
```

### Comparing `types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices/type_defs.pyi` & `types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices.egg-info/PKG-INFO` & `types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iot1click-devices
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IoT1ClickDevicesService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IoT1ClickDevicesService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/
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
 
 <a id="types-aiobotocore-iot1click-devices"></a>
 
 # types-aiobotocore-iot1click-devices
 
 [![PyPI - types-aiobotocore-iot1click-devices](https://img.shields.io/pypi/v/types-aiobotocore-iot1click-devices.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot1click-devices)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot1click-devices.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot1click-devices)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot1click-devices)](https://pepy.tech/project/types-aiobotocore-iot1click-devices)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoT1ClickDevicesService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
+[aiobotocore.IoT1ClickDevicesService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
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
 [types-aiobotocore-iot1click-devices docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iot1click-devices-2.9.0/types_aiobotocore_iot1click_devices.egg-info/SOURCES.txt` & `types-aiobotocore-iot1click-devices-2.9.1/types_aiobotocore_iot1click_devices.egg-info/SOURCES.txt`

 * *Files identical despite different names*

