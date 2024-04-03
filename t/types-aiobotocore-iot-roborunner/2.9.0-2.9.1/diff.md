# Comparing `tmp/types-aiobotocore-iot-roborunner-2.9.0.tar.gz` & `tmp/types-aiobotocore-iot-roborunner-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iot-roborunner-2.9.0.tar", last modified: Wed Dec 13 19:59:31 2023, max compression
+gzip compressed data, was "types-aiobotocore-iot-roborunner-2.9.1.tar", last modified: Thu Jan 18 01:20:55 2024, max compression
```

## Comparing `types-aiobotocore-iot-roborunner-2.9.0.tar` & `types-aiobotocore-iot-roborunner-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:31.813657 types-aiobotocore-iot-roborunner-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:47:48.000000 types-aiobotocore-iot-roborunner-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13759 2023-12-13 19:59:31.813657 types-aiobotocore-iot-roborunner-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12169 2023-12-13 19:47:48.000000 types-aiobotocore-iot-roborunner-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:31.813657 types-aiobotocore-iot-roborunner-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2023-12-13 19:47:48.000000 types-aiobotocore-iot-roborunner-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:31.809657 types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2023-12-13 19:47:48.000000 types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2023-12-13 19:47:48.000000 types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      958 2023-12-13 19:47:48.000000 types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20665 2023-12-13 19:47:48.000000 types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    20661 2023-12-13 19:47:48.000000 types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8782 2023-12-13 19:47:48.000000 types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8780 2023-12-13 19:47:48.000000 types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2023-12-13 19:47:48.000000 types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2023-12-13 19:47:48.000000 types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:47:48.000000 types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    15190 2023-12-13 19:47:48.000000 types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15189 2023-12-13 19:47:48.000000 types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:47:48.000000 types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:31.809657 types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13759 2023-12-13 19:59:31.000000 types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-12-13 19:59:31.000000 types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:31.000000 types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:31.000000 types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:31.000000 types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-13 19:59:31.000000 types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:55.349275 types-aiobotocore-iot-roborunner-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:09:39.000000 types-aiobotocore-iot-roborunner-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13779 2024-01-18 01:20:55.349275 types-aiobotocore-iot-roborunner-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12169 2024-01-18 01:09:39.000000 types-aiobotocore-iot-roborunner-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:55.349275 types-aiobotocore-iot-roborunner-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-01-18 01:09:38.000000 types-aiobotocore-iot-roborunner-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:55.345275 types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner/
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-01-18 01:09:39.000000 types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-01-18 01:09:39.000000 types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-01-18 01:09:39.000000 types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20669 2024-01-18 01:09:39.000000 types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20666 2024-01-18 01:09:39.000000 types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8780 2024-01-18 01:09:39.000000 types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8780 2024-01-18 01:09:39.000000 types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-01-18 01:09:39.000000 types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-01-18 01:09:39.000000 types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:09:39.000000 types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    15189 2024-01-18 01:09:39.000000 types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15189 2024-01-18 01:09:39.000000 types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:09:39.000000 types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:55.345275 types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13779 2024-01-18 01:20:55.000000 types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-01-18 01:20:55.000000 types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:55.000000 types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:55.000000 types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:55.000000 types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-18 01:20:55.000000 types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iot-roborunner-2.9.0/LICENSE` & `types-aiobotocore-iot-roborunner-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-iot-roborunner-2.9.0/PKG-INFO` & `types-aiobotocore-iot-roborunner-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iot-roborunner
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IoTRoboRunner 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IoTRoboRunner 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/
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
 
 <a id="types-aiobotocore-iot-roborunner"></a>
 
 # types-aiobotocore-iot-roborunner
 
 [![PyPI - types-aiobotocore-iot-roborunner](https://img.shields.io/pypi/v/types-aiobotocore-iot-roborunner.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot-roborunner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot-roborunner.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot-roborunner)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot-roborunner)](https://pepy.tech/project/types-aiobotocore-iot-roborunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTRoboRunner 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
+[aiobotocore.IoTRoboRunner 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
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
 [types-aiobotocore-iot-roborunner docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iot-roborunner-2.9.0/README.md` & `types-aiobotocore-iot-roborunner-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot-roborunner.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot-roborunner)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot-roborunner)](https://pepy.tech/project/types-aiobotocore-iot-roborunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTRoboRunner 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
+[aiobotocore.IoTRoboRunner 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
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
 [types-aiobotocore-iot-roborunner docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iot-roborunner-2.9.0/setup.py` & `types-aiobotocore-iot-roborunner-2.9.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iot-roborunner",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_iot_roborunner"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.IoTRoboRunner 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.IoTRoboRunner 2.9.1 service generated with"
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
     keywords="aiobotocore iot-roborunner type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_iot_roborunner": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner/__init__.py` & `types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     ListSitesPaginator,
     ListWorkerFleetsPaginator,
     ListWorkersPaginator,
 )
 
 Client = IoTRoboRunnerClient
 
-
 __all__ = (
     "Client",
     "IoTRoboRunnerClient",
     "ListDestinationsPaginator",
     "ListSitesPaginator",
     "ListWorkerFleetsPaginator",
     "ListWorkersPaginator",
```

### Comparing `types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner/__init__.pyi` & `types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner/__main__.py` & `types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTRoboRunner 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.IoTRoboRunner 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner\nOther"
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

### Comparing `types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner/client.py` & `types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("IoTRoboRunnerClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -114,15 +113,15 @@
     async def create_destination(
         self,
         *,
         name: str,
         site: str,
         clientToken: str = ...,
         state: DestinationStateType = ...,
-        additionalFixedProperties: str = ...
+        additionalFixedProperties: str = ...,
     ) -> CreateDestinationResponseTypeDef:
         """
         Grants permission to create a destination See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/iot-roborunner-2018-05-10/CreateDestination).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.create_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/client/#create_destination)
@@ -145,15 +144,15 @@
         name: str,
         fleet: str,
         clientToken: str = ...,
         additionalTransientProperties: str = ...,
         additionalFixedProperties: str = ...,
         vendorProperties: VendorPropertiesTypeDef = ...,
         position: PositionCoordinatesTypeDef = ...,
-        orientation: OrientationTypeDef = ...
+        orientation: OrientationTypeDef = ...,
     ) -> CreateWorkerResponseTypeDef:
         """
         Grants permission to create a worker See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/iot-roborunner-2018-05-10/CreateWorker).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.create_worker)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/client/#create_worker)
@@ -258,15 +257,15 @@
 
     async def list_destinations(
         self,
         *,
         site: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        state: DestinationStateType = ...
+        state: DestinationStateType = ...,
     ) -> ListDestinationsResponseTypeDef:
         """
         Grants permission to list destinations See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/iot-roborunner-2018-05-10/ListDestinations).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.list_destinations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/client/#list_destinations)
@@ -307,15 +306,15 @@
 
     async def update_destination(
         self,
         *,
         id: str,
         name: str = ...,
         state: DestinationStateType = ...,
-        additionalFixedProperties: str = ...
+        additionalFixedProperties: str = ...,
     ) -> UpdateDestinationResponseTypeDef:
         """
         Grants permission to update a destination See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/iot-roborunner-2018-05-10/UpdateDestination).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.update_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/client/#update_destination)
@@ -337,15 +336,15 @@
         *,
         id: str,
         name: str = ...,
         additionalTransientProperties: str = ...,
         additionalFixedProperties: str = ...,
         vendorProperties: VendorPropertiesTypeDef = ...,
         position: PositionCoordinatesTypeDef = ...,
-        orientation: OrientationTypeDef = ...
+        orientation: OrientationTypeDef = ...,
     ) -> UpdateWorkerResponseTypeDef:
         """
         Grants permission to update a worker See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/iot-roborunner-2018-05-10/UpdateWorker).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.update_worker)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/client/#update_worker)
```

### Comparing `types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner/client.pyi` & `types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     async def create_destination(
         self,
         *,
         name: str,
         site: str,
         clientToken: str = ...,
         state: DestinationStateType = ...,
-        additionalFixedProperties: str = ...
+        additionalFixedProperties: str = ...,
     ) -> CreateDestinationResponseTypeDef:
         """
         Grants permission to create a destination See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/iot-roborunner-2018-05-10/CreateDestination).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.create_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/client/#create_destination)
@@ -141,15 +141,15 @@
         name: str,
         fleet: str,
         clientToken: str = ...,
         additionalTransientProperties: str = ...,
         additionalFixedProperties: str = ...,
         vendorProperties: VendorPropertiesTypeDef = ...,
         position: PositionCoordinatesTypeDef = ...,
-        orientation: OrientationTypeDef = ...
+        orientation: OrientationTypeDef = ...,
     ) -> CreateWorkerResponseTypeDef:
         """
         Grants permission to create a worker See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/iot-roborunner-2018-05-10/CreateWorker).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.create_worker)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/client/#create_worker)
@@ -254,15 +254,15 @@
 
     async def list_destinations(
         self,
         *,
         site: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        state: DestinationStateType = ...
+        state: DestinationStateType = ...,
     ) -> ListDestinationsResponseTypeDef:
         """
         Grants permission to list destinations See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/iot-roborunner-2018-05-10/ListDestinations).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.list_destinations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/client/#list_destinations)
@@ -303,15 +303,15 @@
 
     async def update_destination(
         self,
         *,
         id: str,
         name: str = ...,
         state: DestinationStateType = ...,
-        additionalFixedProperties: str = ...
+        additionalFixedProperties: str = ...,
     ) -> UpdateDestinationResponseTypeDef:
         """
         Grants permission to update a destination See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/iot-roborunner-2018-05-10/UpdateDestination).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.update_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/client/#update_destination)
@@ -333,15 +333,15 @@
         *,
         id: str,
         name: str = ...,
         additionalTransientProperties: str = ...,
         additionalFixedProperties: str = ...,
         vendorProperties: VendorPropertiesTypeDef = ...,
         position: PositionCoordinatesTypeDef = ...,
-        orientation: OrientationTypeDef = ...
+        orientation: OrientationTypeDef = ...,
     ) -> UpdateWorkerResponseTypeDef:
         """
         Grants permission to update a worker See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/iot-roborunner-2018-05-10/UpdateWorker).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.update_worker)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/client/#update_worker)
```

### Comparing `types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner/literals.py` & `types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner/literals.py`

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
     "DestinationStateType",
     "ListDestinationsPaginatorName",
     "ListSitesPaginatorName",
     "ListWorkerFleetsPaginatorName",
     "ListWorkersPaginatorName",
     "IoTRoboRunnerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DestinationStateType = Literal["DECOMMISSIONED", "DISABLED", "ENABLED"]
 ListDestinationsPaginatorName = Literal["list_destinations"]
 ListSitesPaginatorName = Literal["list_sites"]
 ListWorkerFleetsPaginatorName = Literal["list_worker_fleets"]
 ListWorkersPaginatorName = Literal["list_workers"]
 IoTRoboRunnerServiceName = Literal["iot-roborunner"]
 ServiceName = Literal[
```

### Comparing `types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner/literals.pyi` & `types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner/paginator.py` & `types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 __all__ = (
     "ListDestinationsPaginator",
     "ListSitesPaginator",
     "ListWorkerFleetsPaginator",
     "ListWorkersPaginator",
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
         site: str,
         state: DestinationStateType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDestinationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListDestinations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/paginators/#listdestinationspaginator)
         """
```

### Comparing `types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner/paginator.pyi` & `types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     """
 
     def paginate(
         self,
         *,
         site: str,
         state: DestinationStateType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDestinationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListDestinations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/paginators/#listdestinationspaginator)
         """
 
 class ListSitesPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner/type_defs.py` & `types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner/type_defs.py`

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
     "CartesianCoordinatesTypeDef",
     "CreateDestinationRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateSiteRequestRequestTypeDef",
     "CreateWorkerFleetRequestRequestTypeDef",
     "OrientationTypeDef",
```

### Comparing `types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner/type_defs.pyi` & `types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner.egg-info/PKG-INFO` & `types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iot-roborunner
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IoTRoboRunner 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IoTRoboRunner 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/
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
 
 <a id="types-aiobotocore-iot-roborunner"></a>
 
 # types-aiobotocore-iot-roborunner
 
 [![PyPI - types-aiobotocore-iot-roborunner](https://img.shields.io/pypi/v/types-aiobotocore-iot-roborunner.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot-roborunner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot-roborunner.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot-roborunner)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot-roborunner)](https://pepy.tech/project/types-aiobotocore-iot-roborunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTRoboRunner 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
+[aiobotocore.IoTRoboRunner 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
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
 [types-aiobotocore-iot-roborunner docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iot-roborunner-2.9.0/types_aiobotocore_iot_roborunner.egg-info/SOURCES.txt` & `types-aiobotocore-iot-roborunner-2.9.1/types_aiobotocore_iot_roborunner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

