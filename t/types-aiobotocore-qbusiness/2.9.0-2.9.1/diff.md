# Comparing `tmp/types-aiobotocore-qbusiness-2.9.0.tar.gz` & `tmp/types-aiobotocore-qbusiness-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-qbusiness-2.9.0.tar", last modified: Wed Dec 13 20:00:12 2023, max compression
+gzip compressed data, was "types-aiobotocore-qbusiness-2.9.1.tar", last modified: Thu Jan 18 01:21:32 2024, max compression
```

## Comparing `types-aiobotocore-qbusiness-2.9.0.tar` & `types-aiobotocore-qbusiness-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:12.369295 types-aiobotocore-qbusiness-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:52:02.000000 types-aiobotocore-qbusiness-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14689 2023-12-13 20:00:12.369295 types-aiobotocore-qbusiness-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13118 2023-12-13 19:52:02.000000 types-aiobotocore-qbusiness-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:12.369295 types-aiobotocore-qbusiness-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2023-12-13 19:52:02.000000 types-aiobotocore-qbusiness-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:12.369295 types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness/
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2023-12-13 19:52:02.000000 types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2023-12-13 19:52:02.000000 types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-12-13 19:52:02.000000 types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46330 2023-12-13 19:52:02.000000 types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    46326 2023-12-13 19:52:02.000000 types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13727 2023-12-13 19:52:03.000000 types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13725 2023-12-13 19:52:03.000000 types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14887 2023-12-13 19:52:02.000000 types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    14873 2023-12-13 19:52:02.000000 types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:52:02.000000 types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    55227 2023-12-13 19:52:04.000000 types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    55226 2023-12-13 19:52:03.000000 types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:52:02.000000 types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:12.369295 types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14689 2023-12-13 20:00:12.000000 types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-12-13 20:00:12.000000 types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:12.000000 types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:12.000000 types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:12.000000 types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-13 20:00:12.000000 types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:32.425107 types-aiobotocore-qbusiness-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:13:40.000000 types-aiobotocore-qbusiness-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14709 2024-01-18 01:21:32.425107 types-aiobotocore-qbusiness-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13118 2024-01-18 01:13:40.000000 types-aiobotocore-qbusiness-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:32.425107 types-aiobotocore-qbusiness-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-01-18 01:13:39.000000 types-aiobotocore-qbusiness-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:32.425107 types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness/
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-01-18 01:13:40.000000 types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-01-18 01:13:40.000000 types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-01-18 01:13:40.000000 types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46353 2024-01-18 01:13:40.000000 types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46350 2024-01-18 01:13:40.000000 types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13725 2024-01-18 01:13:40.000000 types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13725 2024-01-18 01:13:40.000000 types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14890 2024-01-18 01:13:40.000000 types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14877 2024-01-18 01:13:40.000000 types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:13:40.000000 types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    55226 2024-01-18 01:13:41.000000 types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55226 2024-01-18 01:13:41.000000 types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:13:40.000000 types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:32.425107 types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14709 2024-01-18 01:21:32.000000 types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-01-18 01:21:32.000000 types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:32.000000 types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:32.000000 types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:32.000000 types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-18 01:21:32.000000 types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-qbusiness-2.9.0/LICENSE` & `types-aiobotocore-qbusiness-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-qbusiness-2.9.0/PKG-INFO` & `types-aiobotocore-qbusiness-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-qbusiness
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.QBusiness 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.QBusiness 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/
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
 
 <a id="types-aiobotocore-qbusiness"></a>
 
 # types-aiobotocore-qbusiness
 
 [![PyPI - types-aiobotocore-qbusiness](https://img.shields.io/pypi/v/types-aiobotocore-qbusiness.svg?color=blue)](https://pypi.org/project/types-aiobotocore-qbusiness)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-qbusiness.svg?color=blue)](https://pypi.org/project/types-aiobotocore-qbusiness)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-qbusiness)](https://pepy.tech/project/types-aiobotocore-qbusiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.QBusiness 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness)
+[aiobotocore.QBusiness 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness)
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
 [types-aiobotocore-qbusiness docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-qbusiness-2.9.0/README.md` & `types-aiobotocore-qbusiness-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-qbusiness.svg?color=blue)](https://pypi.org/project/types-aiobotocore-qbusiness)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-qbusiness)](https://pepy.tech/project/types-aiobotocore-qbusiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.QBusiness 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness)
+[aiobotocore.QBusiness 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness)
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
 [types-aiobotocore-qbusiness docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-qbusiness-2.9.0/setup.py` & `types-aiobotocore-qbusiness-2.9.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-qbusiness",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_qbusiness"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.QBusiness 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.QBusiness 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore qbusiness type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_qbusiness": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness/__init__.py` & `types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,14 @@
     ListPluginsPaginator,
     ListRetrieversPaginator,
     ListWebExperiencesPaginator,
 )
 
 Client = QBusinessClient
 
-
 __all__ = (
     "Client",
     "GetChatControlsConfigurationPaginator",
     "ListApplicationsPaginator",
     "ListConversationsPaginator",
     "ListDataSourceSyncJobsPaginator",
     "ListDataSourcesPaginator",
```

### Comparing `types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness/__init__.pyi` & `types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness/__main__.py` & `types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.QBusiness 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.QBusiness 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness\nOther"
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

### Comparing `types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness/client.py` & `types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("QBusinessClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -149,15 +148,15 @@
 
     async def batch_delete_document(
         self,
         *,
         applicationId: str,
         documents: Sequence[DeleteDocumentTypeDef],
         indexId: str,
-        dataSourceSyncId: str = ...
+        dataSourceSyncId: str = ...,
     ) -> BatchDeleteDocumentResponseTypeDef:
         """
         Asynchronously deletes one or more documents added using the `BatchPutDocument`
         API from an Amazon Q
         index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.batch_delete_document)
@@ -167,15 +166,15 @@
     async def batch_put_document(
         self,
         *,
         applicationId: str,
         documents: Sequence[DocumentTypeDef],
         indexId: str,
         dataSourceSyncId: str = ...,
-        roleArn: str = ...
+        roleArn: str = ...,
     ) -> BatchPutDocumentResponseTypeDef:
         """
         Adds one or more documents to an Amazon Q index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.batch_put_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#batch_put_document)
         """
@@ -196,15 +195,15 @@
         actionExecution: ActionExecutionTypeDef = ...,
         attachments: Sequence[AttachmentInputTypeDef] = ...,
         attributeFilter: "AttributeFilterTypeDef" = ...,
         clientToken: str = ...,
         conversationId: str = ...,
         parentMessageId: str = ...,
         userGroups: Sequence[str] = ...,
-        userMessage: str = ...
+        userMessage: str = ...,
     ) -> ChatSyncOutputTypeDef:
         """
         Starts or continues a non-streaming Amazon Q conversation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.chat_sync)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#chat_sync)
         """
@@ -222,15 +221,15 @@
         *,
         displayName: str,
         roleArn: str,
         attachmentsConfiguration: AttachmentsConfigurationTypeDef = ...,
         clientToken: str = ...,
         description: str = ...,
         encryptionConfiguration: EncryptionConfigurationTypeDef = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates an Amazon Q application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#create_application)
         """
@@ -244,15 +243,15 @@
         indexId: str,
         clientToken: str = ...,
         description: str = ...,
         documentEnrichmentConfiguration: DocumentEnrichmentConfigurationTypeDef = ...,
         roleArn: str = ...,
         syncSchedule: str = ...,
         tags: Sequence[TagTypeDef] = ...,
-        vpcConfiguration: DataSourceVpcConfigurationTypeDef = ...
+        vpcConfiguration: DataSourceVpcConfigurationTypeDef = ...,
     ) -> CreateDataSourceResponseTypeDef:
         """
         Creates a data source connector for an Amazon Q application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#create_data_source)
         """
@@ -261,15 +260,15 @@
         self,
         *,
         applicationId: str,
         displayName: str,
         capacityConfiguration: IndexCapacityConfigurationTypeDef = ...,
         clientToken: str = ...,
         description: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateIndexResponseTypeDef:
         """
         Creates an Amazon Q index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_index)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#create_index)
         """
@@ -279,15 +278,15 @@
         *,
         applicationId: str,
         authConfiguration: PluginAuthConfigurationTypeDef,
         displayName: str,
         serverUrl: str,
         type: PluginTypeType,
         clientToken: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreatePluginResponseTypeDef:
         """
         Creates an Amazon Q plugin.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_plugin)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#create_plugin)
         """
@@ -297,30 +296,30 @@
         *,
         applicationId: str,
         configuration: RetrieverConfigurationTypeDef,
         displayName: str,
         type: RetrieverTypeType,
         clientToken: str = ...,
         roleArn: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRetrieverResponseTypeDef:
         """
         Adds a retriever to your Amazon Q application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_retriever)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#create_retriever)
         """
 
     async def create_user(
         self,
         *,
         applicationId: str,
         userId: str,
         clientToken: str = ...,
-        userAliases: Sequence[UserAliasTypeDef] = ...
+        userAliases: Sequence[UserAliasTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates a universally unique identifier (UUID) mapped to a list of local user
         ids within an
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_user)
@@ -332,15 +331,15 @@
         *,
         applicationId: str,
         clientToken: str = ...,
         samplePromptsControlMode: WebExperienceSamplePromptsControlModeType = ...,
         subtitle: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         title: str = ...,
-        welcomeMessage: str = ...
+        welcomeMessage: str = ...,
     ) -> CreateWebExperienceResponseTypeDef:
         """
         Creates an Amazon Q web experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_web_experience)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#create_web_experience)
         """
@@ -560,15 +559,15 @@
         applicationId: str,
         dataSourceId: str,
         indexId: str,
         endTime: TimestampTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         startTime: TimestampTypeDef = ...,
-        statusFilter: DataSourceSyncJobStatusType = ...
+        statusFilter: DataSourceSyncJobStatusType = ...,
     ) -> ListDataSourceSyncJobsResponseTypeDef:
         """
         Get information about an Amazon Q data source connector synchronization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_data_source_sync_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#list_data_source_sync_jobs)
         """
@@ -586,15 +585,15 @@
     async def list_documents(
         self,
         *,
         applicationId: str,
         indexId: str,
         dataSourceIds: Sequence[str] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListDocumentsResponseTypeDef:
         """
         A list of documents attached to an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_documents)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#list_documents)
         """
@@ -603,15 +602,15 @@
         self,
         *,
         applicationId: str,
         indexId: str,
         updatedEarlierThan: TimestampTypeDef,
         dataSourceId: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListGroupsResponseTypeDef:
         """
         Provides a list of groups that are mapped to users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#list_groups)
         """
@@ -629,15 +628,15 @@
     async def list_messages(
         self,
         *,
         applicationId: str,
         conversationId: str,
         userId: str,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListMessagesResponseTypeDef:
         """
         Gets a list of messages associated with an Amazon Q web experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_messages)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#list_messages)
         """
@@ -686,15 +685,15 @@
         self,
         *,
         applicationId: str,
         conversationId: str,
         messageId: str,
         userId: str,
         messageCopiedAt: TimestampTypeDef = ...,
-        messageUsefulness: MessageUsefulnessFeedbackTypeDef = ...
+        messageUsefulness: MessageUsefulnessFeedbackTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Enables your end user to to provide feedback on their Amazon Q generated chat
         responses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.put_feedback)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#put_feedback)
@@ -704,15 +703,15 @@
         self,
         *,
         applicationId: str,
         groupMembers: GroupMembersTypeDef,
         groupName: str,
         indexId: str,
         type: MembershipTypeType,
-        dataSourceId: str = ...
+        dataSourceId: str = ...,
     ) -> Dict[str, Any]:
         """
         Create, or updates, a mapping of users—who have access to a document—to groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.put_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#put_group)
         """
@@ -757,15 +756,15 @@
     async def update_application(
         self,
         *,
         applicationId: str,
         attachmentsConfiguration: AttachmentsConfigurationTypeDef = ...,
         description: str = ...,
         displayName: str = ...,
-        roleArn: str = ...
+        roleArn: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates an existing Amazon Q application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#update_application)
         """
@@ -774,15 +773,15 @@
         self,
         *,
         applicationId: str,
         blockedPhrasesConfigurationUpdate: BlockedPhrasesConfigurationUpdateTypeDef = ...,
         clientToken: str = ...,
         responseScope: ResponseScopeType = ...,
         topicConfigurationsToCreateOrUpdate: Sequence[TopicConfigurationTypeDef] = ...,
-        topicConfigurationsToDelete: Sequence[TopicConfigurationTypeDef] = ...
+        topicConfigurationsToDelete: Sequence[TopicConfigurationTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Updates an set of chat controls configured for an existing Amazon Q application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_chat_controls_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#update_chat_controls_configuration)
         """
@@ -795,15 +794,15 @@
         indexId: str,
         configuration: Mapping[str, Any] = ...,
         description: str = ...,
         displayName: str = ...,
         documentEnrichmentConfiguration: DocumentEnrichmentConfigurationTypeDef = ...,
         roleArn: str = ...,
         syncSchedule: str = ...,
-        vpcConfiguration: DataSourceVpcConfigurationTypeDef = ...
+        vpcConfiguration: DataSourceVpcConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates an existing Amazon Q data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#update_data_source)
         """
@@ -812,15 +811,15 @@
         self,
         *,
         applicationId: str,
         indexId: str,
         capacityConfiguration: IndexCapacityConfigurationTypeDef = ...,
         description: str = ...,
         displayName: str = ...,
-        documentAttributeConfigurations: Sequence[DocumentAttributeConfigurationTypeDef] = ...
+        documentAttributeConfigurations: Sequence[DocumentAttributeConfigurationTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Updates an Amazon Q index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_index)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#update_index)
         """
@@ -829,15 +828,15 @@
         self,
         *,
         applicationId: str,
         pluginId: str,
         authConfiguration: PluginAuthConfigurationTypeDef = ...,
         displayName: str = ...,
         serverUrl: str = ...,
-        state: PluginStateType = ...
+        state: PluginStateType = ...,
     ) -> Dict[str, Any]:
         """
         Updates an Amazon Q plugin.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_plugin)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#update_plugin)
         """
@@ -845,30 +844,30 @@
     async def update_retriever(
         self,
         *,
         applicationId: str,
         retrieverId: str,
         configuration: RetrieverConfigurationTypeDef = ...,
         displayName: str = ...,
-        roleArn: str = ...
+        roleArn: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the retriever used for your Amazon Q application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_retriever)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#update_retriever)
         """
 
     async def update_user(
         self,
         *,
         applicationId: str,
         userId: str,
         userAliasesToDelete: Sequence[UserAliasTypeDef] = ...,
-        userAliasesToUpdate: Sequence[UserAliasTypeDef] = ...
+        userAliasesToUpdate: Sequence[UserAliasTypeDef] = ...,
     ) -> UpdateUserResponseTypeDef:
         """
         Updates a information associated with a user id.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#update_user)
         """
@@ -878,15 +877,15 @@
         *,
         applicationId: str,
         webExperienceId: str,
         authenticationConfiguration: WebExperienceAuthConfigurationTypeDef = ...,
         samplePromptsControlMode: WebExperienceSamplePromptsControlModeType = ...,
         subtitle: str = ...,
         title: str = ...,
-        welcomeMessage: str = ...
+        welcomeMessage: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates an Amazon Q web experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_web_experience)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#update_web_experience)
         """
```

### Comparing `types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness/client.pyi` & `types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,15 @@
 
     async def batch_delete_document(
         self,
         *,
         applicationId: str,
         documents: Sequence[DeleteDocumentTypeDef],
         indexId: str,
-        dataSourceSyncId: str = ...
+        dataSourceSyncId: str = ...,
     ) -> BatchDeleteDocumentResponseTypeDef:
         """
         Asynchronously deletes one or more documents added using the `BatchPutDocument`
         API from an Amazon Q
         index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.batch_delete_document)
@@ -163,15 +163,15 @@
     async def batch_put_document(
         self,
         *,
         applicationId: str,
         documents: Sequence[DocumentTypeDef],
         indexId: str,
         dataSourceSyncId: str = ...,
-        roleArn: str = ...
+        roleArn: str = ...,
     ) -> BatchPutDocumentResponseTypeDef:
         """
         Adds one or more documents to an Amazon Q index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.batch_put_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#batch_put_document)
         """
@@ -192,15 +192,15 @@
         actionExecution: ActionExecutionTypeDef = ...,
         attachments: Sequence[AttachmentInputTypeDef] = ...,
         attributeFilter: "AttributeFilterTypeDef" = ...,
         clientToken: str = ...,
         conversationId: str = ...,
         parentMessageId: str = ...,
         userGroups: Sequence[str] = ...,
-        userMessage: str = ...
+        userMessage: str = ...,
     ) -> ChatSyncOutputTypeDef:
         """
         Starts or continues a non-streaming Amazon Q conversation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.chat_sync)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#chat_sync)
         """
@@ -218,15 +218,15 @@
         *,
         displayName: str,
         roleArn: str,
         attachmentsConfiguration: AttachmentsConfigurationTypeDef = ...,
         clientToken: str = ...,
         description: str = ...,
         encryptionConfiguration: EncryptionConfigurationTypeDef = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates an Amazon Q application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#create_application)
         """
@@ -240,15 +240,15 @@
         indexId: str,
         clientToken: str = ...,
         description: str = ...,
         documentEnrichmentConfiguration: DocumentEnrichmentConfigurationTypeDef = ...,
         roleArn: str = ...,
         syncSchedule: str = ...,
         tags: Sequence[TagTypeDef] = ...,
-        vpcConfiguration: DataSourceVpcConfigurationTypeDef = ...
+        vpcConfiguration: DataSourceVpcConfigurationTypeDef = ...,
     ) -> CreateDataSourceResponseTypeDef:
         """
         Creates a data source connector for an Amazon Q application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#create_data_source)
         """
@@ -257,15 +257,15 @@
         self,
         *,
         applicationId: str,
         displayName: str,
         capacityConfiguration: IndexCapacityConfigurationTypeDef = ...,
         clientToken: str = ...,
         description: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateIndexResponseTypeDef:
         """
         Creates an Amazon Q index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_index)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#create_index)
         """
@@ -275,15 +275,15 @@
         *,
         applicationId: str,
         authConfiguration: PluginAuthConfigurationTypeDef,
         displayName: str,
         serverUrl: str,
         type: PluginTypeType,
         clientToken: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreatePluginResponseTypeDef:
         """
         Creates an Amazon Q plugin.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_plugin)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#create_plugin)
         """
@@ -293,30 +293,30 @@
         *,
         applicationId: str,
         configuration: RetrieverConfigurationTypeDef,
         displayName: str,
         type: RetrieverTypeType,
         clientToken: str = ...,
         roleArn: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRetrieverResponseTypeDef:
         """
         Adds a retriever to your Amazon Q application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_retriever)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#create_retriever)
         """
 
     async def create_user(
         self,
         *,
         applicationId: str,
         userId: str,
         clientToken: str = ...,
-        userAliases: Sequence[UserAliasTypeDef] = ...
+        userAliases: Sequence[UserAliasTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates a universally unique identifier (UUID) mapped to a list of local user
         ids within an
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_user)
@@ -328,15 +328,15 @@
         *,
         applicationId: str,
         clientToken: str = ...,
         samplePromptsControlMode: WebExperienceSamplePromptsControlModeType = ...,
         subtitle: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         title: str = ...,
-        welcomeMessage: str = ...
+        welcomeMessage: str = ...,
     ) -> CreateWebExperienceResponseTypeDef:
         """
         Creates an Amazon Q web experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_web_experience)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#create_web_experience)
         """
@@ -556,15 +556,15 @@
         applicationId: str,
         dataSourceId: str,
         indexId: str,
         endTime: TimestampTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         startTime: TimestampTypeDef = ...,
-        statusFilter: DataSourceSyncJobStatusType = ...
+        statusFilter: DataSourceSyncJobStatusType = ...,
     ) -> ListDataSourceSyncJobsResponseTypeDef:
         """
         Get information about an Amazon Q data source connector synchronization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_data_source_sync_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#list_data_source_sync_jobs)
         """
@@ -582,15 +582,15 @@
     async def list_documents(
         self,
         *,
         applicationId: str,
         indexId: str,
         dataSourceIds: Sequence[str] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListDocumentsResponseTypeDef:
         """
         A list of documents attached to an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_documents)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#list_documents)
         """
@@ -599,15 +599,15 @@
         self,
         *,
         applicationId: str,
         indexId: str,
         updatedEarlierThan: TimestampTypeDef,
         dataSourceId: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListGroupsResponseTypeDef:
         """
         Provides a list of groups that are mapped to users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#list_groups)
         """
@@ -625,15 +625,15 @@
     async def list_messages(
         self,
         *,
         applicationId: str,
         conversationId: str,
         userId: str,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListMessagesResponseTypeDef:
         """
         Gets a list of messages associated with an Amazon Q web experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_messages)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#list_messages)
         """
@@ -682,15 +682,15 @@
         self,
         *,
         applicationId: str,
         conversationId: str,
         messageId: str,
         userId: str,
         messageCopiedAt: TimestampTypeDef = ...,
-        messageUsefulness: MessageUsefulnessFeedbackTypeDef = ...
+        messageUsefulness: MessageUsefulnessFeedbackTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Enables your end user to to provide feedback on their Amazon Q generated chat
         responses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.put_feedback)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#put_feedback)
@@ -700,15 +700,15 @@
         self,
         *,
         applicationId: str,
         groupMembers: GroupMembersTypeDef,
         groupName: str,
         indexId: str,
         type: MembershipTypeType,
-        dataSourceId: str = ...
+        dataSourceId: str = ...,
     ) -> Dict[str, Any]:
         """
         Create, or updates, a mapping of users—who have access to a document—to groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.put_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#put_group)
         """
@@ -753,15 +753,15 @@
     async def update_application(
         self,
         *,
         applicationId: str,
         attachmentsConfiguration: AttachmentsConfigurationTypeDef = ...,
         description: str = ...,
         displayName: str = ...,
-        roleArn: str = ...
+        roleArn: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates an existing Amazon Q application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#update_application)
         """
@@ -770,15 +770,15 @@
         self,
         *,
         applicationId: str,
         blockedPhrasesConfigurationUpdate: BlockedPhrasesConfigurationUpdateTypeDef = ...,
         clientToken: str = ...,
         responseScope: ResponseScopeType = ...,
         topicConfigurationsToCreateOrUpdate: Sequence[TopicConfigurationTypeDef] = ...,
-        topicConfigurationsToDelete: Sequence[TopicConfigurationTypeDef] = ...
+        topicConfigurationsToDelete: Sequence[TopicConfigurationTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Updates an set of chat controls configured for an existing Amazon Q application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_chat_controls_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#update_chat_controls_configuration)
         """
@@ -791,15 +791,15 @@
         indexId: str,
         configuration: Mapping[str, Any] = ...,
         description: str = ...,
         displayName: str = ...,
         documentEnrichmentConfiguration: DocumentEnrichmentConfigurationTypeDef = ...,
         roleArn: str = ...,
         syncSchedule: str = ...,
-        vpcConfiguration: DataSourceVpcConfigurationTypeDef = ...
+        vpcConfiguration: DataSourceVpcConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates an existing Amazon Q data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#update_data_source)
         """
@@ -808,15 +808,15 @@
         self,
         *,
         applicationId: str,
         indexId: str,
         capacityConfiguration: IndexCapacityConfigurationTypeDef = ...,
         description: str = ...,
         displayName: str = ...,
-        documentAttributeConfigurations: Sequence[DocumentAttributeConfigurationTypeDef] = ...
+        documentAttributeConfigurations: Sequence[DocumentAttributeConfigurationTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Updates an Amazon Q index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_index)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#update_index)
         """
@@ -825,15 +825,15 @@
         self,
         *,
         applicationId: str,
         pluginId: str,
         authConfiguration: PluginAuthConfigurationTypeDef = ...,
         displayName: str = ...,
         serverUrl: str = ...,
-        state: PluginStateType = ...
+        state: PluginStateType = ...,
     ) -> Dict[str, Any]:
         """
         Updates an Amazon Q plugin.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_plugin)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#update_plugin)
         """
@@ -841,30 +841,30 @@
     async def update_retriever(
         self,
         *,
         applicationId: str,
         retrieverId: str,
         configuration: RetrieverConfigurationTypeDef = ...,
         displayName: str = ...,
-        roleArn: str = ...
+        roleArn: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the retriever used for your Amazon Q application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_retriever)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#update_retriever)
         """
 
     async def update_user(
         self,
         *,
         applicationId: str,
         userId: str,
         userAliasesToDelete: Sequence[UserAliasTypeDef] = ...,
-        userAliasesToUpdate: Sequence[UserAliasTypeDef] = ...
+        userAliasesToUpdate: Sequence[UserAliasTypeDef] = ...,
     ) -> UpdateUserResponseTypeDef:
         """
         Updates a information associated with a user id.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#update_user)
         """
@@ -874,15 +874,15 @@
         *,
         applicationId: str,
         webExperienceId: str,
         authenticationConfiguration: WebExperienceAuthConfigurationTypeDef = ...,
         samplePromptsControlMode: WebExperienceSamplePromptsControlModeType = ...,
         subtitle: str = ...,
         title: str = ...,
-        welcomeMessage: str = ...
+        welcomeMessage: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates an Amazon Q web experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_web_experience)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/client/#update_web_experience)
         """
```

### Comparing `types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness/literals.py` & `types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness/literals.py`

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
     "ActionPayloadFieldTypeType",
     "ApplicationStatusType",
     "AttachmentStatusType",
     "AttachmentsControlModeType",
     "AttributeTypeType",
     "AttributeValueOperatorType",
@@ -66,15 +65,14 @@
     "QBusinessServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ActionPayloadFieldTypeType = Literal["ARRAY", "BOOLEAN", "NUMBER", "STRING"]
 ApplicationStatusType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED", "UPDATING"]
 AttachmentStatusType = Literal["FAILED", "SUCCEEDED"]
 AttachmentsControlModeType = Literal["DISABLED", "ENABLED"]
 AttributeTypeType = Literal["DATE", "NUMBER", "STRING", "STRING_LIST"]
 AttributeValueOperatorType = Literal["DELETE"]
 ContentTypeType = Literal[
```

### Comparing `types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness/literals.pyi` & `types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness/paginator.py` & `types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,14 @@
     "ListIndicesPaginator",
     "ListMessagesPaginator",
     "ListPluginsPaginator",
     "ListRetrieversPaginator",
     "ListWebExperiencesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -148,15 +147,15 @@
         *,
         applicationId: str,
         dataSourceId: str,
         indexId: str,
         endTime: TimestampTypeDef = ...,
         startTime: TimestampTypeDef = ...,
         statusFilter: DataSourceSyncJobStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDataSourceSyncJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Paginator.ListDataSourceSyncJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/paginators/#listdatasourcesyncjobspaginator)
         """
 
 
@@ -183,15 +182,15 @@
 
     def paginate(
         self,
         *,
         applicationId: str,
         indexId: str,
         dataSourceIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDocumentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Paginator.ListDocuments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/paginators/#listdocumentspaginator)
         """
 
 
@@ -204,15 +203,15 @@
     def paginate(
         self,
         *,
         applicationId: str,
         indexId: str,
         updatedEarlierThan: TimestampTypeDef,
         dataSourceId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Paginator.ListGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/paginators/#listgroupspaginator)
         """
 
 
@@ -239,15 +238,15 @@
 
     def paginate(
         self,
         *,
         applicationId: str,
         conversationId: str,
         userId: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListMessagesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Paginator.ListMessages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/paginators/#listmessagespaginator)
         """
```

### Comparing `types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness/paginator.pyi` & `types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         *,
         applicationId: str,
         dataSourceId: str,
         indexId: str,
         endTime: TimestampTypeDef = ...,
         startTime: TimestampTypeDef = ...,
         statusFilter: DataSourceSyncJobStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDataSourceSyncJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Paginator.ListDataSourceSyncJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/paginators/#listdatasourcesyncjobspaginator)
         """
 
 class ListDataSourcesPaginator(AioPaginator):
@@ -175,15 +175,15 @@
 
     def paginate(
         self,
         *,
         applicationId: str,
         indexId: str,
         dataSourceIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDocumentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Paginator.ListDocuments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/paginators/#listdocumentspaginator)
         """
 
 class ListGroupsPaginator(AioPaginator):
@@ -195,15 +195,15 @@
     def paginate(
         self,
         *,
         applicationId: str,
         indexId: str,
         updatedEarlierThan: TimestampTypeDef,
         dataSourceId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Paginator.ListGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/paginators/#listgroupspaginator)
         """
 
 class ListIndicesPaginator(AioPaginator):
@@ -228,15 +228,15 @@
 
     def paginate(
         self,
         *,
         applicationId: str,
         conversationId: str,
         userId: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListMessagesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Paginator.ListMessages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/paginators/#listmessagespaginator)
         """
 
 class ListPluginsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness/type_defs.py` & `types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActionExecutionPayloadFieldPaginatorTypeDef",
     "ActionExecutionPayloadFieldTypeDef",
     "ActionReviewPayloadFieldAllowedValueTypeDef",
     "ApplicationTypeDef",
     "AppliedAttachmentsConfigurationTypeDef",
     "BlobTypeDef",
```

### Comparing `types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness/type_defs.pyi` & `types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness.egg-info/PKG-INFO` & `types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-qbusiness
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.QBusiness 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.QBusiness 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/
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
 
 <a id="types-aiobotocore-qbusiness"></a>
 
 # types-aiobotocore-qbusiness
 
 [![PyPI - types-aiobotocore-qbusiness](https://img.shields.io/pypi/v/types-aiobotocore-qbusiness.svg?color=blue)](https://pypi.org/project/types-aiobotocore-qbusiness)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-qbusiness.svg?color=blue)](https://pypi.org/project/types-aiobotocore-qbusiness)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-qbusiness)](https://pepy.tech/project/types-aiobotocore-qbusiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.QBusiness 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness)
+[aiobotocore.QBusiness 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness)
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
 [types-aiobotocore-qbusiness docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qbusiness/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-qbusiness-2.9.0/types_aiobotocore_qbusiness.egg-info/SOURCES.txt` & `types-aiobotocore-qbusiness-2.9.1/types_aiobotocore_qbusiness.egg-info/SOURCES.txt`

 * *Files identical despite different names*

