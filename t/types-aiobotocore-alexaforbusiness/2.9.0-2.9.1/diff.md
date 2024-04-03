# Comparing `tmp/types-aiobotocore-alexaforbusiness-2.9.0.tar.gz` & `tmp/types-aiobotocore-alexaforbusiness-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-alexaforbusiness-2.9.0.tar", last modified: Wed Dec 13 19:58:30 2023, max compression
+gzip compressed data, was "types-aiobotocore-alexaforbusiness-2.9.1.tar", last modified: Thu Jan 18 01:19:58 2024, max compression
```

## Comparing `types-aiobotocore-alexaforbusiness-2.9.0.tar` & `types-aiobotocore-alexaforbusiness-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:30.122133 types-aiobotocore-alexaforbusiness-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:40:38.000000 types-aiobotocore-alexaforbusiness-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15334 2023-12-13 19:58:30.122133 types-aiobotocore-alexaforbusiness-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13735 2023-12-13 19:40:38.000000 types-aiobotocore-alexaforbusiness-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:30.122133 types-aiobotocore-alexaforbusiness-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2023-12-13 19:40:38.000000 types-aiobotocore-alexaforbusiness-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:30.122133 types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness/
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2023-12-13 19:40:38.000000 types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2023-12-13 19:40:38.000000 types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      968 2023-12-13 19:40:38.000000 types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    71120 2023-12-13 19:40:38.000000 types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    71116 2023-12-13 19:40:38.000000 types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13173 2023-12-13 19:40:39.000000 types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13171 2023-12-13 19:40:39.000000 types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    17039 2023-12-13 19:40:39.000000 types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    17024 2023-12-13 19:40:38.000000 types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:40:38.000000 types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    62518 2023-12-13 19:40:40.000000 types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    62517 2023-12-13 19:40:39.000000 types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:40:38.000000 types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:30.122133 types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15334 2023-12-13 19:58:30.000000 types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      984 2023-12-13 19:58:30.000000 types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:30.000000 types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:30.000000 types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:30.000000 types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-13 19:58:30.000000 types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:58.613535 types-aiobotocore-alexaforbusiness-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:02:37.000000 types-aiobotocore-alexaforbusiness-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-01-18 01:19:58.613535 types-aiobotocore-alexaforbusiness-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13735 2024-01-18 01:02:37.000000 types-aiobotocore-alexaforbusiness-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:19:58.613535 types-aiobotocore-alexaforbusiness-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-01-18 01:02:37.000000 types-aiobotocore-alexaforbusiness-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:58.609535 types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness/
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-01-18 01:02:37.000000 types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-01-18 01:02:37.000000 types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-01-18 01:02:37.000000 types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71149 2024-01-18 01:02:38.000000 types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71146 2024-01-18 01:02:38.000000 types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13171 2024-01-18 01:02:38.000000 types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13171 2024-01-18 01:02:38.000000 types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    17045 2024-01-18 01:02:38.000000 types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17031 2024-01-18 01:02:38.000000 types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:02:37.000000 types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    62517 2024-01-18 01:02:40.000000 types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62517 2024-01-18 01:02:39.000000 types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:02:37.000000 types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:58.609535 types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-01-18 01:19:58.000000 types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-18 01:19:58.000000 types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:19:58.000000 types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:19:58.000000 types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:19:58.000000 types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-18 01:19:58.000000 types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-alexaforbusiness-2.9.0/LICENSE` & `types-aiobotocore-alexaforbusiness-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-alexaforbusiness-2.9.0/PKG-INFO` & `types-aiobotocore-alexaforbusiness-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-alexaforbusiness
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AlexaForBusiness 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AlexaForBusiness 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/
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
 
 <a id="types-aiobotocore-alexaforbusiness"></a>
 
 # types-aiobotocore-alexaforbusiness
 
 [![PyPI - types-aiobotocore-alexaforbusiness](https://img.shields.io/pypi/v/types-aiobotocore-alexaforbusiness.svg?color=blue)](https://pypi.org/project/types-aiobotocore-alexaforbusiness)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-alexaforbusiness.svg?color=blue)](https://pypi.org/project/types-aiobotocore-alexaforbusiness)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-alexaforbusiness)](https://pepy.tech/project/types-aiobotocore-alexaforbusiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AlexaForBusiness 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
+[aiobotocore.AlexaForBusiness 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
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
 [types-aiobotocore-alexaforbusiness docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-alexaforbusiness-2.9.0/README.md` & `types-aiobotocore-alexaforbusiness-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-alexaforbusiness.svg?color=blue)](https://pypi.org/project/types-aiobotocore-alexaforbusiness)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-alexaforbusiness)](https://pepy.tech/project/types-aiobotocore-alexaforbusiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AlexaForBusiness 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
+[aiobotocore.AlexaForBusiness 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
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
 [types-aiobotocore-alexaforbusiness docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-alexaforbusiness-2.9.0/setup.py` & `types-aiobotocore-alexaforbusiness-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-alexaforbusiness",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_alexaforbusiness"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.AlexaForBusiness 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.AlexaForBusiness 2.9.1 service generated with"
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
     keywords="aiobotocore alexaforbusiness type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_alexaforbusiness": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness/__init__.py` & `types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,14 @@
     SearchRoomsPaginator,
     SearchSkillGroupsPaginator,
     SearchUsersPaginator,
 )
 
 Client = AlexaForBusinessClient
 
-
 __all__ = (
     "AlexaForBusinessClient",
     "Client",
     "ListBusinessReportSchedulesPaginator",
     "ListConferenceProvidersPaginator",
     "ListDeviceEventsPaginator",
     "ListSkillsPaginator",
```

### Comparing `types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness/__init__.pyi` & `types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness/__main__.py` & `types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AlexaForBusiness 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.AlexaForBusiness 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness\nOther"
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

### Comparing `types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness/client.py` & `types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("AlexaForBusinessClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -247,15 +246,15 @@
 
     async def create_address_book(
         self,
         *,
         Name: str,
         Description: str = ...,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAddressBookResponseTypeDef:
         """
         Creates an address book with the specified details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.create_address_book)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#create_address_book)
         """
@@ -266,15 +265,15 @@
         Format: BusinessReportFormatType,
         ContentRange: BusinessReportContentRangeTypeDef,
         ScheduleName: str = ...,
         S3BucketName: str = ...,
         S3KeyPrefix: str = ...,
         Recurrence: BusinessReportRecurrenceTypeDef = ...,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateBusinessReportScheduleResponseTypeDef:
         """
         Creates a recurring schedule for usage reports to deliver to the specified S3
         location with a specified daily or weekly
         interval.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.create_business_report_schedule)
@@ -286,15 +285,15 @@
         *,
         ConferenceProviderName: str,
         ConferenceProviderType: ConferenceProviderTypeType,
         MeetingSetting: MeetingSettingTypeDef,
         IPDialIn: IPDialInTypeDef = ...,
         PSTNDialIn: PSTNDialInTypeDef = ...,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateConferenceProviderResponseTypeDef:
         """
         Adds a new conference provider under the user's AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.create_conference_provider)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#create_conference_provider)
         """
@@ -305,30 +304,30 @@
         FirstName: str,
         DisplayName: str = ...,
         LastName: str = ...,
         PhoneNumber: str = ...,
         PhoneNumbers: Sequence[PhoneNumberTypeDef] = ...,
         SipAddresses: Sequence[SipAddressTypeDef] = ...,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateContactResponseTypeDef:
         """
         Creates a contact with the specified details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.create_contact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#create_contact)
         """
 
     async def create_gateway_group(
         self,
         *,
         Name: str,
         ClientRequestToken: str,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateGatewayGroupResponseTypeDef:
         """
         Creates a gateway group with the specified details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.create_gateway_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#create_gateway_group)
         """
@@ -342,15 +341,15 @@
         ClientRequestToken: str,
         Description: str = ...,
         EapMethod: Literal["EAP_TLS"] = ...,
         CurrentPassword: str = ...,
         NextPassword: str = ...,
         CertificateAuthorityArn: str = ...,
         TrustAnchors: Sequence[str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateNetworkProfileResponseTypeDef:
         """
         Creates a network profile with the specified details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.create_network_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#create_network_profile)
         """
@@ -367,15 +366,15 @@
         Locale: str = ...,
         ClientRequestToken: str = ...,
         SetupModeDisabled: bool = ...,
         MaxVolumeLimit: int = ...,
         PSTNEnabled: bool = ...,
         DataRetentionOptIn: bool = ...,
         MeetingRoomConfiguration: CreateMeetingRoomConfigurationTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateProfileResponseTypeDef:
         """
         Creates a new room profile with the specified details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.create_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#create_profile)
         """
@@ -384,30 +383,30 @@
         self,
         *,
         RoomName: str,
         Description: str = ...,
         ProfileArn: str = ...,
         ProviderCalendarId: str = ...,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRoomResponseTypeDef:
         """
         Creates a room with the specified details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.create_room)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#create_room)
         """
 
     async def create_skill_group(
         self,
         *,
         SkillGroupName: str,
         Description: str = ...,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateSkillGroupResponseTypeDef:
         """
         Creates a skill group with a specified name and description.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.create_skill_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#create_skill_group)
         """
@@ -416,15 +415,15 @@
         self,
         *,
         UserId: str,
         FirstName: str = ...,
         LastName: str = ...,
         Email: str = ...,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateUserResponseTypeDef:
         """
         Creates a user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.create_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#create_user)
         """
@@ -753,15 +752,15 @@
 
     async def list_device_events(
         self,
         *,
         DeviceArn: str,
         EventType: DeviceEventTypeType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListDeviceEventsResponseTypeDef:
         """
         Lists the device event history, including device connection status, for up to
         30
         days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.list_device_events)
@@ -791,15 +790,15 @@
     async def list_skills(
         self,
         *,
         SkillGroupArn: str = ...,
         EnablementType: EnablementTypeFilterType = ...,
         SkillType: SkillTypeFilterType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListSkillsResponseTypeDef:
         """
         Lists all enabled skills in a specific skill group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.list_skills)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#list_skills)
         """
@@ -857,15 +856,15 @@
         """
 
     async def put_invitation_configuration(
         self,
         *,
         OrganizationName: str,
         ContactEmail: str = ...,
-        PrivateSkillIds: Sequence[str] = ...
+        PrivateSkillIds: Sequence[str] = ...,
     ) -> Dict[str, Any]:
         """
         Configures the email template for the user enrollment invitation with the
         specified
         attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.put_invitation_configuration)
@@ -897,15 +896,15 @@
         *,
         ClientId: str,
         UserCode: str,
         ProductId: str,
         AmazonId: str,
         DeviceSerialNumber: str = ...,
         RoomArn: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> RegisterAVSDeviceResponseTypeDef:
         """
         Registers an Alexa-enabled device built by an Original Equipment Manufacturer
         (OEM) using Alexa Voice Service
         (AVS).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.register_avs_device)
@@ -940,15 +939,15 @@
 
     async def search_address_books(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         SortCriteria: Sequence[SortTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> SearchAddressBooksResponseTypeDef:
         """
         Searches address books and lists the ones that meet a set of filter and sort
         criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.search_address_books)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#search_address_books)
@@ -956,15 +955,15 @@
 
     async def search_contacts(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         SortCriteria: Sequence[SortTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> SearchContactsResponseTypeDef:
         """
         Searches contacts and lists the ones that meet a set of filter and sort
         criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.search_contacts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#search_contacts)
@@ -972,30 +971,30 @@
 
     async def search_devices(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        SortCriteria: Sequence[SortTypeDef] = ...
+        SortCriteria: Sequence[SortTypeDef] = ...,
     ) -> SearchDevicesResponseTypeDef:
         """
         Searches devices and lists the ones that meet a set of filter criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.search_devices)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#search_devices)
         """
 
     async def search_network_profiles(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        SortCriteria: Sequence[SortTypeDef] = ...
+        SortCriteria: Sequence[SortTypeDef] = ...,
     ) -> SearchNetworkProfilesResponseTypeDef:
         """
         Searches network profiles and lists the ones that meet a set of filter and sort
         criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.search_network_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#search_network_profiles)
@@ -1003,45 +1002,45 @@
 
     async def search_profiles(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        SortCriteria: Sequence[SortTypeDef] = ...
+        SortCriteria: Sequence[SortTypeDef] = ...,
     ) -> SearchProfilesResponseTypeDef:
         """
         Searches room profiles and lists the ones that meet a set of filter criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.search_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#search_profiles)
         """
 
     async def search_rooms(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        SortCriteria: Sequence[SortTypeDef] = ...
+        SortCriteria: Sequence[SortTypeDef] = ...,
     ) -> SearchRoomsResponseTypeDef:
         """
         Searches rooms and lists the ones that meet a set of filter and sort criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.search_rooms)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#search_rooms)
         """
 
     async def search_skill_groups(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        SortCriteria: Sequence[SortTypeDef] = ...
+        SortCriteria: Sequence[SortTypeDef] = ...,
     ) -> SearchSkillGroupsResponseTypeDef:
         """
         Searches skill groups and lists the ones that meet a set of filter and sort
         criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.search_skill_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#search_skill_groups)
@@ -1049,30 +1048,30 @@
 
     async def search_users(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        SortCriteria: Sequence[SortTypeDef] = ...
+        SortCriteria: Sequence[SortTypeDef] = ...,
     ) -> SearchUsersResponseTypeDef:
         """
         Searches users and lists the ones that meet a set of filter and sort criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.search_users)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#search_users)
         """
 
     async def send_announcement(
         self,
         *,
         RoomFilters: Sequence[FilterTypeDef],
         Content: ContentTypeDef,
         ClientRequestToken: str,
-        TimeToLiveInSeconds: int = ...
+        TimeToLiveInSeconds: int = ...,
     ) -> SendAnnouncementResponseTypeDef:
         """
         Triggers an asynchronous flow to send text, SSML, or audio announcements to
         rooms that are identified by a search or
         filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.send_announcement)
@@ -1135,15 +1134,15 @@
         self,
         *,
         ScheduleArn: str,
         S3BucketName: str = ...,
         S3KeyPrefix: str = ...,
         Format: BusinessReportFormatType = ...,
         ScheduleName: str = ...,
-        Recurrence: BusinessReportRecurrenceTypeDef = ...
+        Recurrence: BusinessReportRecurrenceTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the configuration of the report delivery schedule with the specified
         schedule
         ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.update_business_report_schedule)
@@ -1153,15 +1152,15 @@
     async def update_conference_provider(
         self,
         *,
         ConferenceProviderArn: str,
         ConferenceProviderType: ConferenceProviderTypeType,
         MeetingSetting: MeetingSettingTypeDef,
         IPDialIn: IPDialInTypeDef = ...,
-        PSTNDialIn: PSTNDialInTypeDef = ...
+        PSTNDialIn: PSTNDialInTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates an existing conference provider's settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.update_conference_provider)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#update_conference_provider)
         """
@@ -1171,15 +1170,15 @@
         *,
         ContactArn: str,
         DisplayName: str = ...,
         FirstName: str = ...,
         LastName: str = ...,
         PhoneNumber: str = ...,
         PhoneNumbers: Sequence[PhoneNumberTypeDef] = ...,
-        SipAddresses: Sequence[SipAddressTypeDef] = ...
+        SipAddresses: Sequence[SipAddressTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Updates the contact details by the contact ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.update_contact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#update_contact)
         """
@@ -1194,15 +1193,15 @@
 
     async def update_gateway(
         self,
         *,
         GatewayArn: str,
         Name: str = ...,
         Description: str = ...,
-        SoftwareVersion: str = ...
+        SoftwareVersion: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the details of a gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.update_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#update_gateway)
         """
@@ -1222,15 +1221,15 @@
         *,
         NetworkProfileArn: str,
         NetworkProfileName: str = ...,
         Description: str = ...,
         CurrentPassword: str = ...,
         NextPassword: str = ...,
         CertificateAuthorityArn: str = ...,
-        TrustAnchors: Sequence[str] = ...
+        TrustAnchors: Sequence[str] = ...,
     ) -> Dict[str, Any]:
         """
         Updates a network profile by the network profile ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.update_network_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#update_network_profile)
         """
@@ -1247,15 +1246,15 @@
         TemperatureUnit: TemperatureUnitType = ...,
         WakeWord: WakeWordType = ...,
         Locale: str = ...,
         SetupModeDisabled: bool = ...,
         MaxVolumeLimit: int = ...,
         PSTNEnabled: bool = ...,
         DataRetentionOptIn: bool = ...,
-        MeetingRoomConfiguration: UpdateMeetingRoomConfigurationTypeDef = ...
+        MeetingRoomConfiguration: UpdateMeetingRoomConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates an existing room profile by room profile ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.update_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#update_profile)
         """
@@ -1263,15 +1262,15 @@
     async def update_room(
         self,
         *,
         RoomArn: str = ...,
         RoomName: str = ...,
         Description: str = ...,
         ProviderCalendarId: str = ...,
-        ProfileArn: str = ...
+        ProfileArn: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates room details by room ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.update_room)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#update_room)
         """
```

### Comparing `types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness/client.pyi` & `types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -243,15 +243,15 @@
 
     async def create_address_book(
         self,
         *,
         Name: str,
         Description: str = ...,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAddressBookResponseTypeDef:
         """
         Creates an address book with the specified details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.create_address_book)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#create_address_book)
         """
@@ -262,15 +262,15 @@
         Format: BusinessReportFormatType,
         ContentRange: BusinessReportContentRangeTypeDef,
         ScheduleName: str = ...,
         S3BucketName: str = ...,
         S3KeyPrefix: str = ...,
         Recurrence: BusinessReportRecurrenceTypeDef = ...,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateBusinessReportScheduleResponseTypeDef:
         """
         Creates a recurring schedule for usage reports to deliver to the specified S3
         location with a specified daily or weekly
         interval.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.create_business_report_schedule)
@@ -282,15 +282,15 @@
         *,
         ConferenceProviderName: str,
         ConferenceProviderType: ConferenceProviderTypeType,
         MeetingSetting: MeetingSettingTypeDef,
         IPDialIn: IPDialInTypeDef = ...,
         PSTNDialIn: PSTNDialInTypeDef = ...,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateConferenceProviderResponseTypeDef:
         """
         Adds a new conference provider under the user's AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.create_conference_provider)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#create_conference_provider)
         """
@@ -301,30 +301,30 @@
         FirstName: str,
         DisplayName: str = ...,
         LastName: str = ...,
         PhoneNumber: str = ...,
         PhoneNumbers: Sequence[PhoneNumberTypeDef] = ...,
         SipAddresses: Sequence[SipAddressTypeDef] = ...,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateContactResponseTypeDef:
         """
         Creates a contact with the specified details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.create_contact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#create_contact)
         """
 
     async def create_gateway_group(
         self,
         *,
         Name: str,
         ClientRequestToken: str,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateGatewayGroupResponseTypeDef:
         """
         Creates a gateway group with the specified details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.create_gateway_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#create_gateway_group)
         """
@@ -338,15 +338,15 @@
         ClientRequestToken: str,
         Description: str = ...,
         EapMethod: Literal["EAP_TLS"] = ...,
         CurrentPassword: str = ...,
         NextPassword: str = ...,
         CertificateAuthorityArn: str = ...,
         TrustAnchors: Sequence[str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateNetworkProfileResponseTypeDef:
         """
         Creates a network profile with the specified details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.create_network_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#create_network_profile)
         """
@@ -363,15 +363,15 @@
         Locale: str = ...,
         ClientRequestToken: str = ...,
         SetupModeDisabled: bool = ...,
         MaxVolumeLimit: int = ...,
         PSTNEnabled: bool = ...,
         DataRetentionOptIn: bool = ...,
         MeetingRoomConfiguration: CreateMeetingRoomConfigurationTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateProfileResponseTypeDef:
         """
         Creates a new room profile with the specified details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.create_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#create_profile)
         """
@@ -380,30 +380,30 @@
         self,
         *,
         RoomName: str,
         Description: str = ...,
         ProfileArn: str = ...,
         ProviderCalendarId: str = ...,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRoomResponseTypeDef:
         """
         Creates a room with the specified details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.create_room)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#create_room)
         """
 
     async def create_skill_group(
         self,
         *,
         SkillGroupName: str,
         Description: str = ...,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateSkillGroupResponseTypeDef:
         """
         Creates a skill group with a specified name and description.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.create_skill_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#create_skill_group)
         """
@@ -412,15 +412,15 @@
         self,
         *,
         UserId: str,
         FirstName: str = ...,
         LastName: str = ...,
         Email: str = ...,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateUserResponseTypeDef:
         """
         Creates a user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.create_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#create_user)
         """
@@ -749,15 +749,15 @@
 
     async def list_device_events(
         self,
         *,
         DeviceArn: str,
         EventType: DeviceEventTypeType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListDeviceEventsResponseTypeDef:
         """
         Lists the device event history, including device connection status, for up to
         30
         days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.list_device_events)
@@ -787,15 +787,15 @@
     async def list_skills(
         self,
         *,
         SkillGroupArn: str = ...,
         EnablementType: EnablementTypeFilterType = ...,
         SkillType: SkillTypeFilterType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListSkillsResponseTypeDef:
         """
         Lists all enabled skills in a specific skill group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.list_skills)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#list_skills)
         """
@@ -853,15 +853,15 @@
         """
 
     async def put_invitation_configuration(
         self,
         *,
         OrganizationName: str,
         ContactEmail: str = ...,
-        PrivateSkillIds: Sequence[str] = ...
+        PrivateSkillIds: Sequence[str] = ...,
     ) -> Dict[str, Any]:
         """
         Configures the email template for the user enrollment invitation with the
         specified
         attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.put_invitation_configuration)
@@ -893,15 +893,15 @@
         *,
         ClientId: str,
         UserCode: str,
         ProductId: str,
         AmazonId: str,
         DeviceSerialNumber: str = ...,
         RoomArn: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> RegisterAVSDeviceResponseTypeDef:
         """
         Registers an Alexa-enabled device built by an Original Equipment Manufacturer
         (OEM) using Alexa Voice Service
         (AVS).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.register_avs_device)
@@ -936,15 +936,15 @@
 
     async def search_address_books(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         SortCriteria: Sequence[SortTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> SearchAddressBooksResponseTypeDef:
         """
         Searches address books and lists the ones that meet a set of filter and sort
         criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.search_address_books)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#search_address_books)
@@ -952,15 +952,15 @@
 
     async def search_contacts(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         SortCriteria: Sequence[SortTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> SearchContactsResponseTypeDef:
         """
         Searches contacts and lists the ones that meet a set of filter and sort
         criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.search_contacts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#search_contacts)
@@ -968,30 +968,30 @@
 
     async def search_devices(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        SortCriteria: Sequence[SortTypeDef] = ...
+        SortCriteria: Sequence[SortTypeDef] = ...,
     ) -> SearchDevicesResponseTypeDef:
         """
         Searches devices and lists the ones that meet a set of filter criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.search_devices)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#search_devices)
         """
 
     async def search_network_profiles(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        SortCriteria: Sequence[SortTypeDef] = ...
+        SortCriteria: Sequence[SortTypeDef] = ...,
     ) -> SearchNetworkProfilesResponseTypeDef:
         """
         Searches network profiles and lists the ones that meet a set of filter and sort
         criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.search_network_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#search_network_profiles)
@@ -999,45 +999,45 @@
 
     async def search_profiles(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        SortCriteria: Sequence[SortTypeDef] = ...
+        SortCriteria: Sequence[SortTypeDef] = ...,
     ) -> SearchProfilesResponseTypeDef:
         """
         Searches room profiles and lists the ones that meet a set of filter criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.search_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#search_profiles)
         """
 
     async def search_rooms(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        SortCriteria: Sequence[SortTypeDef] = ...
+        SortCriteria: Sequence[SortTypeDef] = ...,
     ) -> SearchRoomsResponseTypeDef:
         """
         Searches rooms and lists the ones that meet a set of filter and sort criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.search_rooms)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#search_rooms)
         """
 
     async def search_skill_groups(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        SortCriteria: Sequence[SortTypeDef] = ...
+        SortCriteria: Sequence[SortTypeDef] = ...,
     ) -> SearchSkillGroupsResponseTypeDef:
         """
         Searches skill groups and lists the ones that meet a set of filter and sort
         criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.search_skill_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#search_skill_groups)
@@ -1045,30 +1045,30 @@
 
     async def search_users(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        SortCriteria: Sequence[SortTypeDef] = ...
+        SortCriteria: Sequence[SortTypeDef] = ...,
     ) -> SearchUsersResponseTypeDef:
         """
         Searches users and lists the ones that meet a set of filter and sort criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.search_users)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#search_users)
         """
 
     async def send_announcement(
         self,
         *,
         RoomFilters: Sequence[FilterTypeDef],
         Content: ContentTypeDef,
         ClientRequestToken: str,
-        TimeToLiveInSeconds: int = ...
+        TimeToLiveInSeconds: int = ...,
     ) -> SendAnnouncementResponseTypeDef:
         """
         Triggers an asynchronous flow to send text, SSML, or audio announcements to
         rooms that are identified by a search or
         filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.send_announcement)
@@ -1131,15 +1131,15 @@
         self,
         *,
         ScheduleArn: str,
         S3BucketName: str = ...,
         S3KeyPrefix: str = ...,
         Format: BusinessReportFormatType = ...,
         ScheduleName: str = ...,
-        Recurrence: BusinessReportRecurrenceTypeDef = ...
+        Recurrence: BusinessReportRecurrenceTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the configuration of the report delivery schedule with the specified
         schedule
         ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.update_business_report_schedule)
@@ -1149,15 +1149,15 @@
     async def update_conference_provider(
         self,
         *,
         ConferenceProviderArn: str,
         ConferenceProviderType: ConferenceProviderTypeType,
         MeetingSetting: MeetingSettingTypeDef,
         IPDialIn: IPDialInTypeDef = ...,
-        PSTNDialIn: PSTNDialInTypeDef = ...
+        PSTNDialIn: PSTNDialInTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates an existing conference provider's settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.update_conference_provider)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#update_conference_provider)
         """
@@ -1167,15 +1167,15 @@
         *,
         ContactArn: str,
         DisplayName: str = ...,
         FirstName: str = ...,
         LastName: str = ...,
         PhoneNumber: str = ...,
         PhoneNumbers: Sequence[PhoneNumberTypeDef] = ...,
-        SipAddresses: Sequence[SipAddressTypeDef] = ...
+        SipAddresses: Sequence[SipAddressTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Updates the contact details by the contact ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.update_contact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#update_contact)
         """
@@ -1190,15 +1190,15 @@
 
     async def update_gateway(
         self,
         *,
         GatewayArn: str,
         Name: str = ...,
         Description: str = ...,
-        SoftwareVersion: str = ...
+        SoftwareVersion: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the details of a gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.update_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#update_gateway)
         """
@@ -1218,15 +1218,15 @@
         *,
         NetworkProfileArn: str,
         NetworkProfileName: str = ...,
         Description: str = ...,
         CurrentPassword: str = ...,
         NextPassword: str = ...,
         CertificateAuthorityArn: str = ...,
-        TrustAnchors: Sequence[str] = ...
+        TrustAnchors: Sequence[str] = ...,
     ) -> Dict[str, Any]:
         """
         Updates a network profile by the network profile ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.update_network_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#update_network_profile)
         """
@@ -1243,15 +1243,15 @@
         TemperatureUnit: TemperatureUnitType = ...,
         WakeWord: WakeWordType = ...,
         Locale: str = ...,
         SetupModeDisabled: bool = ...,
         MaxVolumeLimit: int = ...,
         PSTNEnabled: bool = ...,
         DataRetentionOptIn: bool = ...,
-        MeetingRoomConfiguration: UpdateMeetingRoomConfigurationTypeDef = ...
+        MeetingRoomConfiguration: UpdateMeetingRoomConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates an existing room profile by room profile ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.update_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#update_profile)
         """
@@ -1259,15 +1259,15 @@
     async def update_room(
         self,
         *,
         RoomArn: str = ...,
         RoomName: str = ...,
         Description: str = ...,
         ProviderCalendarId: str = ...,
-        ProfileArn: str = ...
+        ProfileArn: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates room details by room ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.update_room)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/client/#update_room)
         """
```

### Comparing `types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness/literals.py` & `types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness/literals.py`

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
     "BusinessReportFailureCodeType",
     "BusinessReportFormatType",
     "BusinessReportIntervalType",
     "BusinessReportStatusType",
     "CommsProtocolType",
     "ConferenceProviderTypeType",
@@ -65,15 +64,14 @@
     "AlexaForBusinessServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 BusinessReportFailureCodeType = Literal["ACCESS_DENIED", "INTERNAL_FAILURE", "NO_SUCH_BUCKET"]
 BusinessReportFormatType = Literal["CSV", "CSV_ZIP"]
 BusinessReportIntervalType = Literal["ONE_DAY", "ONE_WEEK", "THIRTY_DAYS"]
 BusinessReportStatusType = Literal["FAILED", "RUNNING", "SUCCEEDED"]
 CommsProtocolType = Literal["H323", "SIP", "SIPS"]
 ConferenceProviderTypeType = Literal[
     "BLUEJEANS",
```

### Comparing `types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness/literals.pyi` & `types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness/paginator.py` & `types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,14 @@
     "SearchDevicesPaginator",
     "SearchProfilesPaginator",
     "SearchRoomsPaginator",
     "SearchSkillGroupsPaginator",
     "SearchUsersPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -134,15 +133,15 @@
     """
 
     def paginate(
         self,
         *,
         DeviceArn: str,
         EventType: DeviceEventTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDeviceEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Paginator.ListDeviceEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/paginators/#listdeviceeventspaginator)
         """
 
 
@@ -154,15 +153,15 @@
 
     def paginate(
         self,
         *,
         SkillGroupArn: str = ...,
         EnablementType: EnablementTypeFilterType = ...,
         SkillType: SkillTypeFilterType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSkillsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Paginator.ListSkills.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/paginators/#listskillspaginator)
         """
 
 
@@ -233,15 +232,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         SortCriteria: Sequence[SortTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Paginator.SearchDevices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/paginators/#searchdevicespaginator)
         """
 
 
@@ -252,15 +251,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         SortCriteria: Sequence[SortTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Paginator.SearchProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/paginators/#searchprofilespaginator)
         """
 
 
@@ -271,15 +270,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         SortCriteria: Sequence[SortTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchRoomsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Paginator.SearchRooms.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/paginators/#searchroomspaginator)
         """
 
 
@@ -290,15 +289,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         SortCriteria: Sequence[SortTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchSkillGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Paginator.SearchSkillGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/paginators/#searchskillgroupspaginator)
         """
 
 
@@ -309,13 +308,13 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         SortCriteria: Sequence[SortTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Paginator.SearchUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/paginators/#searchuserspaginator)
         """
```

### Comparing `types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness/paginator.pyi` & `types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
     """
 
     def paginate(
         self,
         *,
         DeviceArn: str,
         EventType: DeviceEventTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDeviceEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Paginator.ListDeviceEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/paginators/#listdeviceeventspaginator)
         """
 
 class ListSkillsPaginator(AioPaginator):
@@ -148,15 +148,15 @@
 
     def paginate(
         self,
         *,
         SkillGroupArn: str = ...,
         EnablementType: EnablementTypeFilterType = ...,
         SkillType: SkillTypeFilterType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSkillsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Paginator.ListSkills.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/paginators/#listskillspaginator)
         """
 
 class ListSkillsStoreCategoriesPaginator(AioPaginator):
@@ -222,15 +222,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         SortCriteria: Sequence[SortTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Paginator.SearchDevices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/paginators/#searchdevicespaginator)
         """
 
 class SearchProfilesPaginator(AioPaginator):
@@ -240,15 +240,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         SortCriteria: Sequence[SortTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Paginator.SearchProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/paginators/#searchprofilespaginator)
         """
 
 class SearchRoomsPaginator(AioPaginator):
@@ -258,15 +258,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         SortCriteria: Sequence[SortTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchRoomsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Paginator.SearchRooms.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/paginators/#searchroomspaginator)
         """
 
 class SearchSkillGroupsPaginator(AioPaginator):
@@ -276,15 +276,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         SortCriteria: Sequence[SortTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchSkillGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Paginator.SearchSkillGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/paginators/#searchskillgroupspaginator)
         """
 
 class SearchUsersPaginator(AioPaginator):
@@ -294,13 +294,13 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         SortCriteria: Sequence[SortTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Paginator.SearchUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/paginators/#searchuserspaginator)
         """
```

### Comparing `types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness/type_defs.py` & `types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AddressBookDataTypeDef",
     "AddressBookTypeDef",
     "ApproveSkillRequestRequestTypeDef",
     "AssociateContactWithAddressBookRequestRequestTypeDef",
     "AssociateDeviceWithNetworkProfileRequestRequestTypeDef",
     "AssociateDeviceWithRoomRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness/type_defs.pyi` & `types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness.egg-info/PKG-INFO` & `types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-alexaforbusiness
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AlexaForBusiness 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AlexaForBusiness 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/
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
 
 <a id="types-aiobotocore-alexaforbusiness"></a>
 
 # types-aiobotocore-alexaforbusiness
 
 [![PyPI - types-aiobotocore-alexaforbusiness](https://img.shields.io/pypi/v/types-aiobotocore-alexaforbusiness.svg?color=blue)](https://pypi.org/project/types-aiobotocore-alexaforbusiness)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-alexaforbusiness.svg?color=blue)](https://pypi.org/project/types-aiobotocore-alexaforbusiness)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-alexaforbusiness)](https://pepy.tech/project/types-aiobotocore-alexaforbusiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AlexaForBusiness 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
+[aiobotocore.AlexaForBusiness 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
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
 [types-aiobotocore-alexaforbusiness docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-alexaforbusiness-2.9.0/types_aiobotocore_alexaforbusiness.egg-info/SOURCES.txt` & `types-aiobotocore-alexaforbusiness-2.9.1/types_aiobotocore_alexaforbusiness.egg-info/SOURCES.txt`

 * *Files identical despite different names*

