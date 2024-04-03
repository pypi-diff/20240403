# Comparing `tmp/types-aiobotocore-cloudhsm-2.9.0.tar.gz` & `tmp/types-aiobotocore-cloudhsm-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudhsm-2.9.0.tar", last modified: Wed Dec 13 19:58:50 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudhsm-2.9.1.tar", last modified: Thu Jan 18 01:20:16 2024, max compression
```

## Comparing `types-aiobotocore-cloudhsm-2.9.0.tar` & `types-aiobotocore-cloudhsm-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:49.997969 types-aiobotocore-cloudhsm-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:42:29.000000 types-aiobotocore-cloudhsm-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13212 2023-12-13 19:58:49.993970 types-aiobotocore-cloudhsm-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11645 2023-12-13 19:42:29.000000 types-aiobotocore-cloudhsm-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:49.997969 types-aiobotocore-cloudhsm-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-12-13 19:42:29.000000 types-aiobotocore-cloudhsm-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:49.993970 types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm/
--rw-r--r--   0 runner    (1001) docker     (127)      985 2023-12-13 19:42:29.000000 types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2023-12-13 19:42:29.000000 types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-12-13 19:42:29.000000 types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16662 2023-12-13 19:42:30.000000 types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16658 2023-12-13 19:42:30.000000 types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8857 2023-12-13 19:42:30.000000 types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8855 2023-12-13 19:42:30.000000 types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2023-12-13 19:42:30.000000 types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2023-12-13 19:42:30.000000 types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:42:29.000000 types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    11661 2023-12-13 19:42:30.000000 types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11660 2023-12-13 19:42:30.000000 types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:42:29.000000 types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:49.993970 types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13212 2023-12-13 19:58:49.000000 types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-12-13 19:58:49.000000 types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:49.000000 types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:49.000000 types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:49.000000 types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-13 19:58:49.000000 types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:16.709460 types-aiobotocore-cloudhsm-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:04:26.000000 types-aiobotocore-cloudhsm-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13232 2024-01-18 01:20:16.709460 types-aiobotocore-cloudhsm-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11645 2024-01-18 01:04:26.000000 types-aiobotocore-cloudhsm-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:16.709460 types-aiobotocore-cloudhsm-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-18 01:04:26.000000 types-aiobotocore-cloudhsm-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:16.709460 types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm/
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-18 01:04:26.000000 types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-18 01:04:26.000000 types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-01-18 01:04:26.000000 types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16663 2024-01-18 01:04:26.000000 types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16660 2024-01-18 01:04:26.000000 types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-01-18 01:04:26.000000 types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-01-18 01:04:26.000000 types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-01-18 01:04:26.000000 types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-01-18 01:04:26.000000 types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:04:26.000000 types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    11660 2024-01-18 01:04:26.000000 types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11660 2024-01-18 01:04:26.000000 types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:04:26.000000 types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:16.709460 types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13232 2024-01-18 01:20:16.000000 types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-01-18 01:20:16.000000 types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:16.000000 types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:16.000000 types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:16.000000 types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-18 01:20:16.000000 types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudhsm-2.9.0/LICENSE` & `types-aiobotocore-cloudhsm-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-cloudhsm-2.9.0/PKG-INFO` & `types-aiobotocore-cloudhsm-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudhsm
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CloudHSM 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CloudHSM 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/
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
 
 <a id="types-aiobotocore-cloudhsm"></a>
 
 # types-aiobotocore-cloudhsm
 
 [![PyPI - types-aiobotocore-cloudhsm](https://img.shields.io/pypi/v/types-aiobotocore-cloudhsm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudhsm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudhsm)](https://pepy.tech/project/types-aiobotocore-cloudhsm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudHSM 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
+[aiobotocore.CloudHSM 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
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
 [types-aiobotocore-cloudhsm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cloudhsm-2.9.0/README.md` & `types-aiobotocore-cloudhsm-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudhsm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudhsm)](https://pepy.tech/project/types-aiobotocore-cloudhsm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudHSM 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
+[aiobotocore.CloudHSM 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
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
 [types-aiobotocore-cloudhsm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cloudhsm-2.9.0/setup.py` & `types-aiobotocore-cloudhsm-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudhsm",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_cloudhsm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CloudHSM 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.CloudHSM 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore cloudhsm type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_cloudhsm": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm/__init__.py` & `types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 """
 
 from .client import CloudHSMClient
 from .paginator import ListHapgsPaginator, ListHsmsPaginator, ListLunaClientsPaginator
 
 Client = CloudHSMClient
 
-
 __all__ = (
     "Client",
     "CloudHSMClient",
     "ListHapgsPaginator",
     "ListHsmsPaginator",
     "ListLunaClientsPaginator",
 )
```

### Comparing `types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm/__init__.pyi` & `types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm/__main__.py` & `types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudHSM 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CloudHSM 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM\nOther"
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

### Comparing `types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm/client.py` & `types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CloudHSMClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -128,15 +127,15 @@
         SubnetId: str,
         SshKey: str,
         IamRoleArn: str,
         SubscriptionType: Literal["PRODUCTION"],
         EniIp: str = ...,
         ExternalId: str = ...,
         ClientToken: str = ...,
-        SyslogIp: str = ...
+        SyslogIp: str = ...,
     ) -> CreateHsmResponseTypeDef:
         """
         This is documentation for **AWS CloudHSM Classic**.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.create_hsm)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/client/#create_hsm)
         """
@@ -283,15 +282,15 @@
         self,
         *,
         HsmArn: str,
         SubnetId: str = ...,
         EniIp: str = ...,
         IamRoleArn: str = ...,
         ExternalId: str = ...,
-        SyslogIp: str = ...
+        SyslogIp: str = ...,
     ) -> ModifyHsmResponseTypeDef:
         """
         This is documentation for **AWS CloudHSM Classic**.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.modify_hsm)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/client/#modify_hsm)
         """
```

### Comparing `types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm/client.pyi` & `types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         SubnetId: str,
         SshKey: str,
         IamRoleArn: str,
         SubscriptionType: Literal["PRODUCTION"],
         EniIp: str = ...,
         ExternalId: str = ...,
         ClientToken: str = ...,
-        SyslogIp: str = ...
+        SyslogIp: str = ...,
     ) -> CreateHsmResponseTypeDef:
         """
         This is documentation for **AWS CloudHSM Classic**.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.create_hsm)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/client/#create_hsm)
         """
@@ -279,15 +279,15 @@
         self,
         *,
         HsmArn: str,
         SubnetId: str = ...,
         EniIp: str = ...,
         IamRoleArn: str = ...,
         ExternalId: str = ...,
-        SyslogIp: str = ...
+        SyslogIp: str = ...,
     ) -> ModifyHsmResponseTypeDef:
         """
         This is documentation for **AWS CloudHSM Classic**.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.modify_hsm)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/client/#modify_hsm)
         """
```

### Comparing `types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm/literals.py` & `types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm/literals.py`

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
     "ClientVersionType",
     "CloudHsmObjectStateType",
     "HsmStatusType",
     "ListHapgsPaginatorName",
     "ListHsmsPaginatorName",
     "ListLunaClientsPaginatorName",
@@ -31,15 +30,14 @@
     "CloudHSMServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ClientVersionType = Literal["5.1", "5.3"]
 CloudHsmObjectStateType = Literal["DEGRADED", "READY", "UPDATING"]
 HsmStatusType = Literal[
     "DEGRADED", "PENDING", "RUNNING", "SUSPENDED", "TERMINATED", "TERMINATING", "UPDATING"
 ]
 ListHapgsPaginatorName = Literal["list_hapgs"]
 ListHsmsPaginatorName = Literal["list_hsms"]
```

### Comparing `types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm/literals.pyi` & `types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm/paginator.py` & `types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     ListHsmsResponseTypeDef,
     ListLunaClientsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListHapgsPaginator", "ListHsmsPaginator", "ListLunaClientsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm/paginator.pyi` & `types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm/type_defs.py` & `types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "CreateHapgRequestRequestTypeDef",
     "CreateHsmRequestRequestTypeDef",
     "CreateLunaClientRequestRequestTypeDef",
     "DeleteHapgRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm/type_defs.pyi` & `types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm.egg-info/PKG-INFO` & `types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudhsm
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CloudHSM 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CloudHSM 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/
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
 
 <a id="types-aiobotocore-cloudhsm"></a>
 
 # types-aiobotocore-cloudhsm
 
 [![PyPI - types-aiobotocore-cloudhsm](https://img.shields.io/pypi/v/types-aiobotocore-cloudhsm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudhsm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudhsm)](https://pepy.tech/project/types-aiobotocore-cloudhsm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudHSM 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
+[aiobotocore.CloudHSM 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
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
 [types-aiobotocore-cloudhsm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cloudhsm-2.9.0/types_aiobotocore_cloudhsm.egg-info/SOURCES.txt` & `types-aiobotocore-cloudhsm-2.9.1/types_aiobotocore_cloudhsm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

