# Comparing `tmp/types-aiobotocore-snow-device-management-2.9.0.tar.gz` & `tmp/types-aiobotocore-snow-device-management-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-snow-device-management-2.9.0.tar", last modified: Wed Dec 13 20:00:33 2023, max compression
+gzip compressed data, was "types-aiobotocore-snow-device-management-2.9.1.tar", last modified: Thu Jan 18 01:21:51 2024, max compression
```

## Comparing `types-aiobotocore-snow-device-management-2.9.0.tar` & `types-aiobotocore-snow-device-management-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:33.601111 types-aiobotocore-snow-device-management-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:56:36.000000 types-aiobotocore-snow-device-management-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14214 2023-12-13 20:00:33.601111 types-aiobotocore-snow-device-management-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12593 2023-12-13 19:56:36.000000 types-aiobotocore-snow-device-management-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:33.601111 types-aiobotocore-snow-device-management-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2023-12-13 19:56:36.000000 types-aiobotocore-snow-device-management-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:33.597111 types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management/
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2023-12-13 19:56:36.000000 types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2023-12-13 19:56:36.000000 types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      988 2023-12-13 19:56:36.000000 types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14967 2023-12-13 19:56:37.000000 types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14963 2023-12-13 19:56:37.000000 types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9423 2023-12-13 19:56:37.000000 types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9421 2023-12-13 19:56:37.000000 types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5819 2023-12-13 19:56:37.000000 types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5813 2023-12-13 19:56:37.000000 types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:56:36.000000 types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13410 2023-12-13 19:56:37.000000 types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13409 2023-12-13 19:56:37.000000 types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:56:36.000000 types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:33.601111 types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14214 2023-12-13 20:00:33.000000 types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2023-12-13 20:00:33.000000 types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:33.000000 types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:33.000000 types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:33.000000 types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-13 20:00:33.000000 types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:51.713021 types-aiobotocore-snow-device-management-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:18:08.000000 types-aiobotocore-snow-device-management-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14234 2024-01-18 01:21:51.713021 types-aiobotocore-snow-device-management-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12593 2024-01-18 01:18:08.000000 types-aiobotocore-snow-device-management-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:51.713021 types-aiobotocore-snow-device-management-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-01-18 01:18:08.000000 types-aiobotocore-snow-device-management-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:51.709021 types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management/
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-01-18 01:18:08.000000 types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-01-18 01:18:08.000000 types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-01-18 01:18:08.000000 types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14968 2024-01-18 01:18:08.000000 types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14965 2024-01-18 01:18:08.000000 types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9421 2024-01-18 01:18:08.000000 types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9421 2024-01-18 01:18:08.000000 types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-01-18 01:18:08.000000 types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-01-18 01:18:08.000000 types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:18:08.000000 types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13409 2024-01-18 01:18:09.000000 types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13409 2024-01-18 01:18:09.000000 types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:18:08.000000 types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:51.713021 types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14234 2024-01-18 01:21:51.000000 types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-01-18 01:21:51.000000 types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:51.000000 types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:51.000000 types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:51.000000 types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-18 01:21:51.000000 types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-snow-device-management-2.9.0/LICENSE` & `types-aiobotocore-snow-device-management-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-snow-device-management-2.9.0/PKG-INFO` & `types-aiobotocore-snow-device-management-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-snow-device-management
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SnowDeviceManagement 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SnowDeviceManagement 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snow_device_management/
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
 
 <a id="types-aiobotocore-snow-device-management"></a>
 
 # types-aiobotocore-snow-device-management
 
 [![PyPI - types-aiobotocore-snow-device-management](https://img.shields.io/pypi/v/types-aiobotocore-snow-device-management.svg?color=blue)](https://pypi.org/project/types-aiobotocore-snow-device-management)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-snow-device-management.svg?color=blue)](https://pypi.org/project/types-aiobotocore-snow-device-management)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snow_device_management/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-snow-device-management)](https://pepy.tech/project/types-aiobotocore-snow-device-management)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SnowDeviceManagement 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement)
+[aiobotocore.SnowDeviceManagement 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement)
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
 [types-aiobotocore-snow-device-management docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snow_device_management/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-snow-device-management-2.9.0/README.md` & `types-aiobotocore-snow-device-management-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-snow-device-management.svg?color=blue)](https://pypi.org/project/types-aiobotocore-snow-device-management)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snow_device_management/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-snow-device-management)](https://pepy.tech/project/types-aiobotocore-snow-device-management)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SnowDeviceManagement 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement)
+[aiobotocore.SnowDeviceManagement 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement)
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
 [types-aiobotocore-snow-device-management docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snow_device_management/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-snow-device-management-2.9.0/setup.py` & `types-aiobotocore-snow-device-management-2.9.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,50 +7,49 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-snow-device-management",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_snow_device_management"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SnowDeviceManagement 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.SnowDeviceManagement 2.9.1 service generated with"
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
         "aiobotocore snow-device-management type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_snow_device_management": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snow_device_management/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management/__init__.py` & `types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     ListDevicesPaginator,
     ListExecutionsPaginator,
     ListTasksPaginator,
 )
 
 Client = SnowDeviceManagementClient
 
-
 __all__ = (
     "Client",
     "ListDeviceResourcesPaginator",
     "ListDevicesPaginator",
     "ListExecutionsPaginator",
     "ListTasksPaginator",
     "SnowDeviceManagementClient",
```

### Comparing `types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management/__init__.pyi` & `types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management/__main__.py` & `types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SnowDeviceManagement 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.SnowDeviceManagement 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snow_device_management//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement\nOther"
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

### Comparing `types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management/client.py` & `types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SnowDeviceManagementClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -115,15 +114,15 @@
     async def create_task(
         self,
         *,
         command: CommandTypeDef,
         targets: Sequence[str],
         clientToken: str = ...,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateTaskOutputTypeDef:
         """
         Instructs one or more devices to start a task, such as unlocking or rebooting.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Client.create_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snow_device_management/client/#create_task)
         """
@@ -205,15 +204,15 @@
 
     async def list_executions(
         self,
         *,
         taskId: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        state: ExecutionStateType = ...
+        state: ExecutionStateType = ...,
     ) -> ListExecutionsOutputTypeDef:
         """
         Returns the status of tasks for one or more target devices.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Client.list_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snow_device_management/client/#list_executions)
         """
```

### Comparing `types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management/client.pyi` & `types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     async def create_task(
         self,
         *,
         command: CommandTypeDef,
         targets: Sequence[str],
         clientToken: str = ...,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateTaskOutputTypeDef:
         """
         Instructs one or more devices to start a task, such as unlocking or rebooting.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Client.create_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snow_device_management/client/#create_task)
         """
@@ -201,15 +201,15 @@
 
     async def list_executions(
         self,
         *,
         taskId: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        state: ExecutionStateType = ...
+        state: ExecutionStateType = ...,
     ) -> ListExecutionsOutputTypeDef:
         """
         Returns the status of tasks for one or more target devices.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Client.list_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snow_device_management/client/#list_executions)
         """
```

### Comparing `types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management/literals.py` & `types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management/literals.py`

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
     "AttachmentStatusType",
     "ExecutionStateType",
     "InstanceStateNameType",
     "IpAddressAssignmentType",
     "ListDeviceResourcesPaginatorName",
     "ListDevicesPaginatorName",
@@ -34,15 +33,14 @@
     "UnlockStateType",
     "SnowDeviceManagementServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 AttachmentStatusType = Literal["ATTACHED", "ATTACHING", "DETACHED", "DETACHING"]
 ExecutionStateType = Literal[
     "CANCELED", "FAILED", "IN_PROGRESS", "QUEUED", "REJECTED", "SUCCEEDED", "TIMED_OUT"
 ]
 InstanceStateNameType = Literal[
     "PENDING", "RUNNING", "SHUTTING_DOWN", "STOPPED", "STOPPING", "TERMINATED"
 ]
```

### Comparing `types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management/literals.pyi` & `types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management/paginator.py` & `types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 __all__ = (
     "ListDeviceResourcesPaginator",
     "ListDevicesPaginator",
     "ListExecutionsPaginator",
     "ListTasksPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -66,15 +65,15 @@
     """
 
     def paginate(
         self,
         *,
         managedDeviceId: str,
         type: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDeviceResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListDeviceResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snow_device_management/paginators/#listdeviceresourcespaginator)
         """
 
 
@@ -100,15 +99,15 @@
     """
 
     def paginate(
         self,
         *,
         taskId: str,
         state: ExecutionStateType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snow_device_management/paginators/#listexecutionspaginator)
         """
```

### Comparing `types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management/paginator.pyi` & `types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     """
 
     def paginate(
         self,
         *,
         managedDeviceId: str,
         type: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDeviceResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListDeviceResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snow_device_management/paginators/#listdeviceresourcespaginator)
         """
 
 class ListDevicesPaginator(AioPaginator):
@@ -95,15 +95,15 @@
     """
 
     def paginate(
         self,
         *,
         taskId: str,
         state: ExecutionStateType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snow_device_management/paginators/#listexecutionspaginator)
         """
 
 class ListTasksPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management/type_defs.py` & `types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CancelTaskInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CapacityTypeDef",
     "CommandTypeDef",
     "CpuOptionsTypeDef",
     "DescribeDeviceEc2InputRequestTypeDef",
```

### Comparing `types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management/type_defs.pyi` & `types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management.egg-info/PKG-INFO` & `types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-snow-device-management
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SnowDeviceManagement 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SnowDeviceManagement 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snow_device_management/
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
 
 <a id="types-aiobotocore-snow-device-management"></a>
 
 # types-aiobotocore-snow-device-management
 
 [![PyPI - types-aiobotocore-snow-device-management](https://img.shields.io/pypi/v/types-aiobotocore-snow-device-management.svg?color=blue)](https://pypi.org/project/types-aiobotocore-snow-device-management)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-snow-device-management.svg?color=blue)](https://pypi.org/project/types-aiobotocore-snow-device-management)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snow_device_management/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-snow-device-management)](https://pepy.tech/project/types-aiobotocore-snow-device-management)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SnowDeviceManagement 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement)
+[aiobotocore.SnowDeviceManagement 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement)
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
 [types-aiobotocore-snow-device-management docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snow_device_management/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-snow-device-management-2.9.0/types_aiobotocore_snow_device_management.egg-info/SOURCES.txt` & `types-aiobotocore-snow-device-management-2.9.1/types_aiobotocore_snow_device_management.egg-info/SOURCES.txt`

 * *Files identical despite different names*

