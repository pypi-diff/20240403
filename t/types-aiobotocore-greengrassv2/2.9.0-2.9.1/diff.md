# Comparing `tmp/types-aiobotocore-greengrassv2-2.9.0.tar.gz` & `tmp/types-aiobotocore-greengrassv2-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-greengrassv2-2.9.0.tar", last modified: Wed Dec 13 19:59:24 2023, max compression
+gzip compressed data, was "types-aiobotocore-greengrassv2-2.9.1.tar", last modified: Thu Jan 18 01:20:48 2024, max compression
```

## Comparing `types-aiobotocore-greengrassv2-2.9.0.tar` & `types-aiobotocore-greengrassv2-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:24.689717 types-aiobotocore-greengrassv2-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:47:02.000000 types-aiobotocore-greengrassv2-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14372 2023-12-13 19:59:24.689717 types-aiobotocore-greengrassv2-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12789 2023-12-13 19:47:02.000000 types-aiobotocore-greengrassv2-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:24.689717 types-aiobotocore-greengrassv2-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2023-12-13 19:47:02.000000 types-aiobotocore-greengrassv2-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:24.689717 types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2/
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2023-12-13 19:47:02.000000 types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2023-12-13 19:47:02.000000 types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      952 2023-12-13 19:47:02.000000 types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27484 2023-12-13 19:47:02.000000 types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    27480 2023-12-13 19:47:02.000000 types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11616 2023-12-13 19:47:02.000000 types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11614 2023-12-13 19:47:02.000000 types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9930 2023-12-13 19:47:02.000000 types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9921 2023-12-13 19:47:02.000000 types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:47:02.000000 types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    33820 2023-12-13 19:47:04.000000 types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    33819 2023-12-13 19:47:02.000000 types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:47:02.000000 types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:24.689717 types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14372 2023-12-13 19:59:24.000000 types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      908 2023-12-13 19:59:24.000000 types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:24.000000 types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:24.000000 types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:24.000000 types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-13 19:59:24.000000 types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:48.713305 types-aiobotocore-greengrassv2-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:08:54.000000 types-aiobotocore-greengrassv2-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14392 2024-01-18 01:20:48.713305 types-aiobotocore-greengrassv2-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12789 2024-01-18 01:08:54.000000 types-aiobotocore-greengrassv2-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:48.713305 types-aiobotocore-greengrassv2-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-01-18 01:08:54.000000 types-aiobotocore-greengrassv2-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:48.713305 types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-01-18 01:08:54.000000 types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-01-18 01:08:54.000000 types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-01-18 01:08:54.000000 types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27492 2024-01-18 01:08:56.000000 types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27489 2024-01-18 01:08:56.000000 types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11614 2024-01-18 01:08:56.000000 types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11614 2024-01-18 01:08:56.000000 types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-01-18 01:08:56.000000 types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9925 2024-01-18 01:08:56.000000 types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:08:54.000000 types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    33819 2024-01-18 01:08:57.000000 types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33819 2024-01-18 01:08:56.000000 types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:08:54.000000 types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:48.713305 types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14392 2024-01-18 01:20:48.000000 types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-01-18 01:20:48.000000 types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:48.000000 types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:48.000000 types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:48.000000 types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-18 01:20:48.000000 types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-greengrassv2-2.9.0/LICENSE` & `types-aiobotocore-greengrassv2-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-greengrassv2-2.9.0/PKG-INFO` & `types-aiobotocore-greengrassv2-2.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-greengrassv2
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.GreengrassV2 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.GreengrassV2 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/
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
 
 <a id="types-aiobotocore-greengrassv2"></a>
 
 # types-aiobotocore-greengrassv2
 
 [![PyPI - types-aiobotocore-greengrassv2](https://img.shields.io/pypi/v/types-aiobotocore-greengrassv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-greengrassv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-greengrassv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-greengrassv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-greengrassv2)](https://pepy.tech/project/types-aiobotocore-greengrassv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GreengrassV2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
+[aiobotocore.GreengrassV2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
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
 [types-aiobotocore-greengrassv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-greengrassv2-2.9.0/README.md` & `types-aiobotocore-greengrassv2-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-greengrassv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-greengrassv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-greengrassv2)](https://pepy.tech/project/types-aiobotocore-greengrassv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GreengrassV2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
+[aiobotocore.GreengrassV2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
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
 [types-aiobotocore-greengrassv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-greengrassv2-2.9.0/setup.py` & `types-aiobotocore-greengrassv2-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-greengrassv2",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_greengrassv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.GreengrassV2 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.GreengrassV2 2.9.1 service generated with"
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
     keywords="aiobotocore greengrassv2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_greengrassv2": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2/__init__.py` & `types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     ListDeploymentsPaginator,
     ListEffectiveDeploymentsPaginator,
     ListInstalledComponentsPaginator,
 )
 
 Client = GreengrassV2Client
 
-
 __all__ = (
     "Client",
     "GreengrassV2Client",
     "ListClientDevicesAssociatedWithCoreDevicePaginator",
     "ListComponentVersionsPaginator",
     "ListComponentsPaginator",
     "ListCoreDevicesPaginator",
```

### Comparing `types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2/__init__.pyi` & `types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2/__main__.py` & `types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.GreengrassV2 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.GreengrassV2 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2\nOther"
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

### Comparing `types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2/client.py` & `types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("GreengrassV2Client",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -133,28 +132,28 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/client/#associate_service_role_to_account)
         """
 
     async def batch_associate_client_device_with_core_device(
         self,
         *,
         coreDeviceThingName: str,
-        entries: Sequence[AssociateClientDeviceWithCoreDeviceEntryTypeDef] = ...
+        entries: Sequence[AssociateClientDeviceWithCoreDeviceEntryTypeDef] = ...,
     ) -> BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef:
         """
         Associates a list of client devices with a core device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.batch_associate_client_device_with_core_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/client/#batch_associate_client_device_with_core_device)
         """
 
     async def batch_disassociate_client_device_from_core_device(
         self,
         *,
         coreDeviceThingName: str,
-        entries: Sequence[DisassociateClientDeviceFromCoreDeviceEntryTypeDef] = ...
+        entries: Sequence[DisassociateClientDeviceFromCoreDeviceEntryTypeDef] = ...,
     ) -> BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef:
         """
         Disassociates a list of client devices from a core device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.batch_disassociate_client_device_from_core_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/client/#batch_disassociate_client_device_from_core_device)
         """
@@ -185,15 +184,15 @@
 
     async def create_component_version(
         self,
         *,
         inlineRecipe: BlobTypeDef = ...,
         lambdaFunction: LambdaFunctionRecipeSourceTypeDef = ...,
         tags: Mapping[str, str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateComponentVersionResponseTypeDef:
         """
         Creates a component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.create_component_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/client/#create_component_version)
         """
@@ -204,15 +203,15 @@
         targetArn: str,
         deploymentName: str = ...,
         components: Mapping[str, ComponentDeploymentSpecificationTypeDef] = ...,
         iotJobConfiguration: DeploymentIoTJobConfigurationTypeDef = ...,
         deploymentPolicies: DeploymentPoliciesTypeDef = ...,
         parentTargetArn: str = ...,
         tags: Mapping[str, str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateDeploymentResponseTypeDef:
         """
         Creates a continuous deployment for a target, which is a Greengrass core device
         or group of core
         devices.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.create_deployment)
@@ -353,30 +352,30 @@
         """
 
     async def list_components(
         self,
         *,
         scope: ComponentVisibilityScopeType = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListComponentsResponseTypeDef:
         """
         Retrieves a paginated list of component summaries.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.list_components)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/client/#list_components)
         """
 
     async def list_core_devices(
         self,
         *,
         thingGroupArn: str = ...,
         status: CoreDeviceStatusType = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListCoreDevicesResponseTypeDef:
         """
         Retrieves a paginated list of Greengrass core devices.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.list_core_devices)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/client/#list_core_devices)
         """
@@ -384,15 +383,15 @@
     async def list_deployments(
         self,
         *,
         targetArn: str = ...,
         historyFilter: DeploymentHistoryFilterType = ...,
         parentTargetArn: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListDeploymentsResponseTypeDef:
         """
         Retrieves a paginated list of deployments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.list_deployments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/client/#list_deployments)
         """
@@ -411,15 +410,15 @@
 
     async def list_installed_components(
         self,
         *,
         coreDeviceThingName: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        topologyFilter: InstalledComponentTopologyFilterType = ...
+        topologyFilter: InstalledComponentTopologyFilterType = ...,
     ) -> ListInstalledComponentsResponseTypeDef:
         """
         Retrieves a paginated list of the components that a Greengrass core device runs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.list_installed_components)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/client/#list_installed_components)
         """
@@ -434,15 +433,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/client/#list_tags_for_resource)
         """
 
     async def resolve_component_candidates(
         self,
         *,
         platform: ComponentPlatformTypeDef = ...,
-        componentCandidates: Sequence[ComponentCandidateTypeDef] = ...
+        componentCandidates: Sequence[ComponentCandidateTypeDef] = ...,
     ) -> ResolveComponentCandidatesResponseTypeDef:
         """
         Retrieves a list of components that meet the component, version, and platform
         requirements of a
         deployment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.resolve_component_candidates)
```

### Comparing `types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2/client.pyi` & `types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -129,28 +129,28 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/client/#associate_service_role_to_account)
         """
 
     async def batch_associate_client_device_with_core_device(
         self,
         *,
         coreDeviceThingName: str,
-        entries: Sequence[AssociateClientDeviceWithCoreDeviceEntryTypeDef] = ...
+        entries: Sequence[AssociateClientDeviceWithCoreDeviceEntryTypeDef] = ...,
     ) -> BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef:
         """
         Associates a list of client devices with a core device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.batch_associate_client_device_with_core_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/client/#batch_associate_client_device_with_core_device)
         """
 
     async def batch_disassociate_client_device_from_core_device(
         self,
         *,
         coreDeviceThingName: str,
-        entries: Sequence[DisassociateClientDeviceFromCoreDeviceEntryTypeDef] = ...
+        entries: Sequence[DisassociateClientDeviceFromCoreDeviceEntryTypeDef] = ...,
     ) -> BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef:
         """
         Disassociates a list of client devices from a core device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.batch_disassociate_client_device_from_core_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/client/#batch_disassociate_client_device_from_core_device)
         """
@@ -181,15 +181,15 @@
 
     async def create_component_version(
         self,
         *,
         inlineRecipe: BlobTypeDef = ...,
         lambdaFunction: LambdaFunctionRecipeSourceTypeDef = ...,
         tags: Mapping[str, str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateComponentVersionResponseTypeDef:
         """
         Creates a component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.create_component_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/client/#create_component_version)
         """
@@ -200,15 +200,15 @@
         targetArn: str,
         deploymentName: str = ...,
         components: Mapping[str, ComponentDeploymentSpecificationTypeDef] = ...,
         iotJobConfiguration: DeploymentIoTJobConfigurationTypeDef = ...,
         deploymentPolicies: DeploymentPoliciesTypeDef = ...,
         parentTargetArn: str = ...,
         tags: Mapping[str, str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateDeploymentResponseTypeDef:
         """
         Creates a continuous deployment for a target, which is a Greengrass core device
         or group of core
         devices.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.create_deployment)
@@ -349,30 +349,30 @@
         """
 
     async def list_components(
         self,
         *,
         scope: ComponentVisibilityScopeType = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListComponentsResponseTypeDef:
         """
         Retrieves a paginated list of component summaries.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.list_components)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/client/#list_components)
         """
 
     async def list_core_devices(
         self,
         *,
         thingGroupArn: str = ...,
         status: CoreDeviceStatusType = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListCoreDevicesResponseTypeDef:
         """
         Retrieves a paginated list of Greengrass core devices.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.list_core_devices)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/client/#list_core_devices)
         """
@@ -380,15 +380,15 @@
     async def list_deployments(
         self,
         *,
         targetArn: str = ...,
         historyFilter: DeploymentHistoryFilterType = ...,
         parentTargetArn: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListDeploymentsResponseTypeDef:
         """
         Retrieves a paginated list of deployments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.list_deployments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/client/#list_deployments)
         """
@@ -407,15 +407,15 @@
 
     async def list_installed_components(
         self,
         *,
         coreDeviceThingName: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        topologyFilter: InstalledComponentTopologyFilterType = ...
+        topologyFilter: InstalledComponentTopologyFilterType = ...,
     ) -> ListInstalledComponentsResponseTypeDef:
         """
         Retrieves a paginated list of the components that a Greengrass core device runs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.list_installed_components)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/client/#list_installed_components)
         """
@@ -430,15 +430,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/client/#list_tags_for_resource)
         """
 
     async def resolve_component_candidates(
         self,
         *,
         platform: ComponentPlatformTypeDef = ...,
-        componentCandidates: Sequence[ComponentCandidateTypeDef] = ...
+        componentCandidates: Sequence[ComponentCandidateTypeDef] = ...,
     ) -> ResolveComponentCandidatesResponseTypeDef:
         """
         Retrieves a list of components that meet the component, version, and platform
         requirements of a
         deployment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.resolve_component_candidates)
```

### Comparing `types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2/literals.py` & `types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2/literals.py`

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
     "CloudComponentStateType",
     "ComponentDependencyTypeType",
     "ComponentVisibilityScopeType",
     "CoreDeviceStatusType",
     "DeploymentComponentUpdatePolicyActionType",
     "DeploymentFailureHandlingPolicyType",
@@ -50,15 +49,14 @@
     "GreengrassV2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 CloudComponentStateType = Literal["DEPLOYABLE", "DEPRECATED", "FAILED", "INITIATED", "REQUESTED"]
 ComponentDependencyTypeType = Literal["HARD", "SOFT"]
 ComponentVisibilityScopeType = Literal["PRIVATE", "PUBLIC"]
 CoreDeviceStatusType = Literal["HEALTHY", "UNHEALTHY"]
 DeploymentComponentUpdatePolicyActionType = Literal["NOTIFY_COMPONENTS", "SKIP_NOTIFY_COMPONENTS"]
 DeploymentFailureHandlingPolicyType = Literal["DO_NOTHING", "ROLLBACK"]
 DeploymentHistoryFilterType = Literal["ALL", "LATEST_ONLY"]
```

### Comparing `types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2/literals.pyi` & `types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2/paginator.py` & `types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,14 @@
     "ListComponentsPaginator",
     "ListCoreDevicesPaginator",
     "ListDeploymentsPaginator",
     "ListEffectiveDeploymentsPaginator",
     "ListInstalledComponentsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -112,15 +111,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/paginators/#listcomponentspaginator)
     """
 
     def paginate(
         self,
         *,
         scope: ComponentVisibilityScopeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListComponentsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListComponents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/paginators/#listcomponentspaginator)
         """
 
 
@@ -131,15 +130,15 @@
     """
 
     def paginate(
         self,
         *,
         thingGroupArn: str = ...,
         status: CoreDeviceStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCoreDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListCoreDevices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/paginators/#listcoredevicespaginator)
         """
 
 
@@ -151,15 +150,15 @@
 
     def paginate(
         self,
         *,
         targetArn: str = ...,
         historyFilter: DeploymentHistoryFilterType = ...,
         parentTargetArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListDeployments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/paginators/#listdeploymentspaginator)
         """
 
 
@@ -185,13 +184,13 @@
     """
 
     def paginate(
         self,
         *,
         coreDeviceThingName: str,
         topologyFilter: InstalledComponentTopologyFilterType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListInstalledComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListInstalledComponents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/paginators/#listinstalledcomponentspaginator)
         """
```

### Comparing `types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2/paginator.pyi` & `types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/paginators/#listcomponentspaginator)
     """
 
     def paginate(
         self,
         *,
         scope: ComponentVisibilityScopeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListComponentsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListComponents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/paginators/#listcomponentspaginator)
         """
 
 class ListCoreDevicesPaginator(AioPaginator):
@@ -125,15 +125,15 @@
     """
 
     def paginate(
         self,
         *,
         thingGroupArn: str = ...,
         status: CoreDeviceStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCoreDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListCoreDevices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/paginators/#listcoredevicespaginator)
         """
 
 class ListDeploymentsPaginator(AioPaginator):
@@ -144,15 +144,15 @@
 
     def paginate(
         self,
         *,
         targetArn: str = ...,
         historyFilter: DeploymentHistoryFilterType = ...,
         parentTargetArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListDeployments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/paginators/#listdeploymentspaginator)
         """
 
 class ListEffectiveDeploymentsPaginator(AioPaginator):
@@ -176,13 +176,13 @@
     """
 
     def paginate(
         self,
         *,
         coreDeviceThingName: str,
         topologyFilter: InstalledComponentTopologyFilterType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListInstalledComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListInstalledComponents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/paginators/#listinstalledcomponentspaginator)
         """
```

### Comparing `types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2/type_defs.py` & `types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssociateClientDeviceWithCoreDeviceEntryTypeDef",
     "AssociateClientDeviceWithCoreDeviceErrorEntryTypeDef",
     "AssociateServiceRoleToAccountRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociatedClientDeviceTypeDef",
     "DisassociateClientDeviceFromCoreDeviceEntryTypeDef",
```

### Comparing `types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2/type_defs.pyi` & `types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2.egg-info/PKG-INFO` & `types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-greengrassv2
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.GreengrassV2 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.GreengrassV2 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/
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
 
 <a id="types-aiobotocore-greengrassv2"></a>
 
 # types-aiobotocore-greengrassv2
 
 [![PyPI - types-aiobotocore-greengrassv2](https://img.shields.io/pypi/v/types-aiobotocore-greengrassv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-greengrassv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-greengrassv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-greengrassv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-greengrassv2)](https://pepy.tech/project/types-aiobotocore-greengrassv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GreengrassV2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
+[aiobotocore.GreengrassV2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
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
 [types-aiobotocore-greengrassv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-greengrassv2-2.9.0/types_aiobotocore_greengrassv2.egg-info/SOURCES.txt` & `types-aiobotocore-greengrassv2-2.9.1/types_aiobotocore_greengrassv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

