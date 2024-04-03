# Comparing `tmp/types-aiobotocore-evidently-2.9.0.tar.gz` & `tmp/types-aiobotocore-evidently-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-evidently-2.9.0.tar", last modified: Wed Dec 13 19:59:18 2023, max compression
+gzip compressed data, was "types-aiobotocore-evidently-2.9.1.tar", last modified: Thu Jan 18 01:20:42 2024, max compression
```

## Comparing `types-aiobotocore-evidently-2.9.0.tar` & `types-aiobotocore-evidently-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:18.293747 types-aiobotocore-evidently-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:46:07.000000 types-aiobotocore-evidently-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13839 2023-12-13 19:59:18.293747 types-aiobotocore-evidently-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12258 2023-12-13 19:46:07.000000 types-aiobotocore-evidently-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:18.293747 types-aiobotocore-evidently-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2023-12-13 19:46:07.000000 types-aiobotocore-evidently-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:18.293747 types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently/
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2023-12-13 19:46:07.000000 types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2023-12-13 19:46:07.000000 types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      960 2023-12-13 19:46:07.000000 types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32484 2023-12-13 19:46:08.000000 types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    32480 2023-12-13 19:46:07.000000 types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10847 2023-12-13 19:46:08.000000 types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10845 2023-12-13 19:46:08.000000 types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7890 2023-12-13 19:46:08.000000 types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7882 2023-12-13 19:46:08.000000 types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:46:07.000000 types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    37596 2023-12-13 19:46:08.000000 types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    37595 2023-12-13 19:46:08.000000 types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:46:07.000000 types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:18.293747 types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13839 2023-12-13 19:59:18.000000 types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-12-13 19:59:18.000000 types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:18.000000 types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:18.000000 types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:18.000000 types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-13 19:59:18.000000 types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:42.845333 types-aiobotocore-evidently-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:08:01.000000 types-aiobotocore-evidently-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13859 2024-01-18 01:20:42.845333 types-aiobotocore-evidently-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12258 2024-01-18 01:08:01.000000 types-aiobotocore-evidently-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:42.845333 types-aiobotocore-evidently-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-01-18 01:08:01.000000 types-aiobotocore-evidently-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:42.845333 types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently/
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-01-18 01:08:01.000000 types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-01-18 01:08:01.000000 types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-01-18 01:08:01.000000 types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32498 2024-01-18 01:08:02.000000 types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32495 2024-01-18 01:08:01.000000 types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10845 2024-01-18 01:08:02.000000 types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10845 2024-01-18 01:08:02.000000 types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-01-18 01:08:02.000000 types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7885 2024-01-18 01:08:02.000000 types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:08:01.000000 types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    37595 2024-01-18 01:08:04.000000 types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37595 2024-01-18 01:08:04.000000 types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:08:01.000000 types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:42.845333 types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13859 2024-01-18 01:20:42.000000 types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-01-18 01:20:42.000000 types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:42.000000 types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:42.000000 types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:42.000000 types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-18 01:20:42.000000 types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-evidently-2.9.0/LICENSE` & `types-aiobotocore-evidently-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-evidently-2.9.0/PKG-INFO` & `types-aiobotocore-evidently-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-evidently
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CloudWatchEvidently 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CloudWatchEvidently 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/
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
 
 <a id="types-aiobotocore-evidently"></a>
 
 # types-aiobotocore-evidently
 
 [![PyPI - types-aiobotocore-evidently](https://img.shields.io/pypi/v/types-aiobotocore-evidently.svg?color=blue)](https://pypi.org/project/types-aiobotocore-evidently)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-evidently.svg?color=blue)](https://pypi.org/project/types-aiobotocore-evidently)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-evidently)](https://pepy.tech/project/types-aiobotocore-evidently)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatchEvidently 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
+[aiobotocore.CloudWatchEvidently 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
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
 [types-aiobotocore-evidently docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-evidently-2.9.0/README.md` & `types-aiobotocore-evidently-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-evidently.svg?color=blue)](https://pypi.org/project/types-aiobotocore-evidently)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-evidently)](https://pepy.tech/project/types-aiobotocore-evidently)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatchEvidently 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
+[aiobotocore.CloudWatchEvidently 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
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
 [types-aiobotocore-evidently docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-evidently-2.9.0/setup.py` & `types-aiobotocore-evidently-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-evidently",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_evidently"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CloudWatchEvidently 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.CloudWatchEvidently 2.9.1 service generated with"
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
     keywords="aiobotocore evidently type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_evidently": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently/__init__.py` & `types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     ListProjectsPaginator,
     ListSegmentReferencesPaginator,
     ListSegmentsPaginator,
 )
 
 Client = CloudWatchEvidentlyClient
 
-
 __all__ = (
     "Client",
     "CloudWatchEvidentlyClient",
     "ListExperimentsPaginator",
     "ListFeaturesPaginator",
     "ListLaunchesPaginator",
     "ListProjectsPaginator",
```

### Comparing `types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently/__init__.pyi` & `types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently/__main__.py` & `types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudWatchEvidently 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CloudWatchEvidently 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently\nOther"
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

### Comparing `types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently/client.py` & `types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CloudWatchEvidentlyClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -166,15 +165,15 @@
         project: str,
         treatments: Sequence[TreatmentConfigTypeDef],
         description: str = ...,
         onlineAbConfig: OnlineAbConfigTypeDef = ...,
         randomizationSalt: str = ...,
         samplingRate: int = ...,
         segment: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateExperimentResponseTypeDef:
         """
         Creates an Evidently *experiment*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.create_experiment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#create_experiment)
         """
@@ -185,15 +184,15 @@
         name: str,
         project: str,
         variations: Sequence[VariationConfigTypeDef],
         defaultVariation: str = ...,
         description: str = ...,
         entityOverrides: Mapping[str, str] = ...,
         evaluationStrategy: FeatureEvaluationStrategyType = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateFeatureResponseTypeDef:
         """
         Creates an Evidently *feature* that you want to launch or test.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.create_feature)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#create_feature)
         """
@@ -204,15 +203,15 @@
         groups: Sequence[LaunchGroupConfigTypeDef],
         name: str,
         project: str,
         description: str = ...,
         metricMonitors: Sequence[MetricMonitorConfigTypeDef] = ...,
         randomizationSalt: str = ...,
         scheduledSplitsConfig: ScheduledSplitsLaunchConfigTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateLaunchResponseTypeDef:
         """
         Creates a *launch* of a given feature.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.create_launch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#create_launch)
         """
@@ -220,15 +219,15 @@
     async def create_project(
         self,
         *,
         name: str,
         appConfigResource: ProjectAppConfigResourceConfigTypeDef = ...,
         dataDelivery: ProjectDataDeliveryConfigTypeDef = ...,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateProjectResponseTypeDef:
         """
         Creates a project, which is the logical object in Evidently that can contain
         features, launches, and
         experiments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.create_project)
@@ -327,15 +326,15 @@
         project: str,
         treatmentNames: Sequence[str],
         baseStat: Literal["Mean"] = ...,
         endTime: TimestampTypeDef = ...,
         period: int = ...,
         reportNames: Sequence[Literal["BayesianInference"]] = ...,
         resultStats: Sequence[ExperimentResultRequestTypeType] = ...,
-        startTime: TimestampTypeDef = ...
+        startTime: TimestampTypeDef = ...,
     ) -> GetExperimentResultsResponseTypeDef:
         """
         Retrieves the results of a running or completed experiment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.get_experiment_results)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#get_experiment_results)
         """
@@ -374,15 +373,15 @@
 
     async def list_experiments(
         self,
         *,
         project: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        status: ExperimentStatusType = ...
+        status: ExperimentStatusType = ...,
     ) -> ListExperimentsResponseTypeDef:
         """
         Returns configuration details about all the experiments in the specified
         project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.list_experiments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#list_experiments)
@@ -400,15 +399,15 @@
 
     async def list_launches(
         self,
         *,
         project: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        status: LaunchStatusType = ...
+        status: LaunchStatusType = ...,
     ) -> ListLaunchesResponseTypeDef:
         """
         Returns configuration details about all the launches in the specified project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.list_launches)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#list_launches)
         """
@@ -427,15 +426,15 @@
 
     async def list_segment_references(
         self,
         *,
         segment: str,
         type: SegmentReferenceResourceTypeType,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListSegmentReferencesResponseTypeDef:
         """
         Use this operation to find which experiments or launches are using a specified
         segment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.list_segment_references)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#list_segment_references)
@@ -493,30 +492,30 @@
 
     async def stop_experiment(
         self,
         *,
         experiment: str,
         project: str,
         desiredState: ExperimentStopDesiredStateType = ...,
-        reason: str = ...
+        reason: str = ...,
     ) -> StopExperimentResponseTypeDef:
         """
         Stops an experiment that is currently running.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.stop_experiment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#stop_experiment)
         """
 
     async def stop_launch(
         self,
         *,
         launch: str,
         project: str,
         desiredState: LaunchStopDesiredStateType = ...,
-        reason: str = ...
+        reason: str = ...,
     ) -> StopLaunchResponseTypeDef:
         """
         Stops a launch that is currently running.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.stop_launch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#stop_launch)
         """
@@ -559,15 +558,15 @@
         description: str = ...,
         metricGoals: Sequence[MetricGoalConfigTypeDef] = ...,
         onlineAbConfig: OnlineAbConfigTypeDef = ...,
         randomizationSalt: str = ...,
         removeSegment: bool = ...,
         samplingRate: int = ...,
         segment: str = ...,
-        treatments: Sequence[TreatmentConfigTypeDef] = ...
+        treatments: Sequence[TreatmentConfigTypeDef] = ...,
     ) -> UpdateExperimentResponseTypeDef:
         """
         Updates an Evidently experiment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.update_experiment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#update_experiment)
         """
@@ -578,15 +577,15 @@
         feature: str,
         project: str,
         addOrUpdateVariations: Sequence[VariationConfigTypeDef] = ...,
         defaultVariation: str = ...,
         description: str = ...,
         entityOverrides: Mapping[str, str] = ...,
         evaluationStrategy: FeatureEvaluationStrategyType = ...,
-        removeVariations: Sequence[str] = ...
+        removeVariations: Sequence[str] = ...,
     ) -> UpdateFeatureResponseTypeDef:
         """
         Updates an existing feature.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.update_feature)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#update_feature)
         """
@@ -596,43 +595,43 @@
         *,
         launch: str,
         project: str,
         description: str = ...,
         groups: Sequence[LaunchGroupConfigTypeDef] = ...,
         metricMonitors: Sequence[MetricMonitorConfigTypeDef] = ...,
         randomizationSalt: str = ...,
-        scheduledSplitsConfig: ScheduledSplitsLaunchConfigTypeDef = ...
+        scheduledSplitsConfig: ScheduledSplitsLaunchConfigTypeDef = ...,
     ) -> UpdateLaunchResponseTypeDef:
         """
         Updates a launch of a given feature.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.update_launch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#update_launch)
         """
 
     async def update_project(
         self,
         *,
         project: str,
         appConfigResource: ProjectAppConfigResourceConfigTypeDef = ...,
-        description: str = ...
+        description: str = ...,
     ) -> UpdateProjectResponseTypeDef:
         """
         Updates the description of an existing project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.update_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#update_project)
         """
 
     async def update_project_data_delivery(
         self,
         *,
         project: str,
         cloudWatchLogs: CloudWatchLogsDestinationConfigTypeDef = ...,
-        s3Destination: S3DestinationConfigTypeDef = ...
+        s3Destination: S3DestinationConfigTypeDef = ...,
     ) -> UpdateProjectDataDeliveryResponseTypeDef:
         """
         Updates the data storage options for this project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.update_project_data_delivery)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#update_project_data_delivery)
         """
```

### Comparing `types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently/client.pyi` & `types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
         project: str,
         treatments: Sequence[TreatmentConfigTypeDef],
         description: str = ...,
         onlineAbConfig: OnlineAbConfigTypeDef = ...,
         randomizationSalt: str = ...,
         samplingRate: int = ...,
         segment: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateExperimentResponseTypeDef:
         """
         Creates an Evidently *experiment*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.create_experiment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#create_experiment)
         """
@@ -181,15 +181,15 @@
         name: str,
         project: str,
         variations: Sequence[VariationConfigTypeDef],
         defaultVariation: str = ...,
         description: str = ...,
         entityOverrides: Mapping[str, str] = ...,
         evaluationStrategy: FeatureEvaluationStrategyType = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateFeatureResponseTypeDef:
         """
         Creates an Evidently *feature* that you want to launch or test.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.create_feature)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#create_feature)
         """
@@ -200,15 +200,15 @@
         groups: Sequence[LaunchGroupConfigTypeDef],
         name: str,
         project: str,
         description: str = ...,
         metricMonitors: Sequence[MetricMonitorConfigTypeDef] = ...,
         randomizationSalt: str = ...,
         scheduledSplitsConfig: ScheduledSplitsLaunchConfigTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateLaunchResponseTypeDef:
         """
         Creates a *launch* of a given feature.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.create_launch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#create_launch)
         """
@@ -216,15 +216,15 @@
     async def create_project(
         self,
         *,
         name: str,
         appConfigResource: ProjectAppConfigResourceConfigTypeDef = ...,
         dataDelivery: ProjectDataDeliveryConfigTypeDef = ...,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateProjectResponseTypeDef:
         """
         Creates a project, which is the logical object in Evidently that can contain
         features, launches, and
         experiments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.create_project)
@@ -323,15 +323,15 @@
         project: str,
         treatmentNames: Sequence[str],
         baseStat: Literal["Mean"] = ...,
         endTime: TimestampTypeDef = ...,
         period: int = ...,
         reportNames: Sequence[Literal["BayesianInference"]] = ...,
         resultStats: Sequence[ExperimentResultRequestTypeType] = ...,
-        startTime: TimestampTypeDef = ...
+        startTime: TimestampTypeDef = ...,
     ) -> GetExperimentResultsResponseTypeDef:
         """
         Retrieves the results of a running or completed experiment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.get_experiment_results)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#get_experiment_results)
         """
@@ -370,15 +370,15 @@
 
     async def list_experiments(
         self,
         *,
         project: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        status: ExperimentStatusType = ...
+        status: ExperimentStatusType = ...,
     ) -> ListExperimentsResponseTypeDef:
         """
         Returns configuration details about all the experiments in the specified
         project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.list_experiments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#list_experiments)
@@ -396,15 +396,15 @@
 
     async def list_launches(
         self,
         *,
         project: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        status: LaunchStatusType = ...
+        status: LaunchStatusType = ...,
     ) -> ListLaunchesResponseTypeDef:
         """
         Returns configuration details about all the launches in the specified project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.list_launches)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#list_launches)
         """
@@ -423,15 +423,15 @@
 
     async def list_segment_references(
         self,
         *,
         segment: str,
         type: SegmentReferenceResourceTypeType,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListSegmentReferencesResponseTypeDef:
         """
         Use this operation to find which experiments or launches are using a specified
         segment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.list_segment_references)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#list_segment_references)
@@ -489,30 +489,30 @@
 
     async def stop_experiment(
         self,
         *,
         experiment: str,
         project: str,
         desiredState: ExperimentStopDesiredStateType = ...,
-        reason: str = ...
+        reason: str = ...,
     ) -> StopExperimentResponseTypeDef:
         """
         Stops an experiment that is currently running.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.stop_experiment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#stop_experiment)
         """
 
     async def stop_launch(
         self,
         *,
         launch: str,
         project: str,
         desiredState: LaunchStopDesiredStateType = ...,
-        reason: str = ...
+        reason: str = ...,
     ) -> StopLaunchResponseTypeDef:
         """
         Stops a launch that is currently running.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.stop_launch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#stop_launch)
         """
@@ -555,15 +555,15 @@
         description: str = ...,
         metricGoals: Sequence[MetricGoalConfigTypeDef] = ...,
         onlineAbConfig: OnlineAbConfigTypeDef = ...,
         randomizationSalt: str = ...,
         removeSegment: bool = ...,
         samplingRate: int = ...,
         segment: str = ...,
-        treatments: Sequence[TreatmentConfigTypeDef] = ...
+        treatments: Sequence[TreatmentConfigTypeDef] = ...,
     ) -> UpdateExperimentResponseTypeDef:
         """
         Updates an Evidently experiment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.update_experiment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#update_experiment)
         """
@@ -574,15 +574,15 @@
         feature: str,
         project: str,
         addOrUpdateVariations: Sequence[VariationConfigTypeDef] = ...,
         defaultVariation: str = ...,
         description: str = ...,
         entityOverrides: Mapping[str, str] = ...,
         evaluationStrategy: FeatureEvaluationStrategyType = ...,
-        removeVariations: Sequence[str] = ...
+        removeVariations: Sequence[str] = ...,
     ) -> UpdateFeatureResponseTypeDef:
         """
         Updates an existing feature.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.update_feature)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#update_feature)
         """
@@ -592,43 +592,43 @@
         *,
         launch: str,
         project: str,
         description: str = ...,
         groups: Sequence[LaunchGroupConfigTypeDef] = ...,
         metricMonitors: Sequence[MetricMonitorConfigTypeDef] = ...,
         randomizationSalt: str = ...,
-        scheduledSplitsConfig: ScheduledSplitsLaunchConfigTypeDef = ...
+        scheduledSplitsConfig: ScheduledSplitsLaunchConfigTypeDef = ...,
     ) -> UpdateLaunchResponseTypeDef:
         """
         Updates a launch of a given feature.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.update_launch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#update_launch)
         """
 
     async def update_project(
         self,
         *,
         project: str,
         appConfigResource: ProjectAppConfigResourceConfigTypeDef = ...,
-        description: str = ...
+        description: str = ...,
     ) -> UpdateProjectResponseTypeDef:
         """
         Updates the description of an existing project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.update_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#update_project)
         """
 
     async def update_project_data_delivery(
         self,
         *,
         project: str,
         cloudWatchLogs: CloudWatchLogsDestinationConfigTypeDef = ...,
-        s3Destination: S3DestinationConfigTypeDef = ...
+        s3Destination: S3DestinationConfigTypeDef = ...,
     ) -> UpdateProjectDataDeliveryResponseTypeDef:
         """
         Updates the data storage options for this project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.update_project_data_delivery)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#update_project_data_delivery)
         """
```

### Comparing `types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently/literals.py` & `types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently/literals.py`

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
     "ChangeDirectionEnumType",
     "EventTypeType",
     "ExperimentBaseStatType",
     "ExperimentReportNameType",
     "ExperimentResultRequestTypeType",
     "ExperimentResultResponseTypeType",
@@ -47,15 +46,14 @@
     "CloudWatchEvidentlyServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ChangeDirectionEnumType = Literal["DECREASE", "INCREASE"]
 EventTypeType = Literal["aws.evidently.custom", "aws.evidently.evaluation"]
 ExperimentBaseStatType = Literal["Mean"]
 ExperimentReportNameType = Literal["BayesianInference"]
 ExperimentResultRequestTypeType = Literal[
     "BaseStat", "ConfidenceInterval", "PValue", "TreatmentEffect"
 ]
```

### Comparing `types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently/literals.pyi` & `types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently/paginator.py` & `types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,14 @@
     "ListFeaturesPaginator",
     "ListLaunchesPaginator",
     "ListProjectsPaginator",
     "ListSegmentReferencesPaginator",
     "ListSegmentsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -74,15 +73,15 @@
     """
 
     def paginate(
         self,
         *,
         project: str,
         status: ExperimentStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListExperimentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListExperiments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/paginators/#listexperimentspaginator)
         """
 
 
@@ -108,15 +107,15 @@
     """
 
     def paginate(
         self,
         *,
         project: str,
         status: LaunchStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListLaunchesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListLaunches.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/paginators/#listlaunchespaginator)
         """
 
 
@@ -142,15 +141,15 @@
     """
 
     def paginate(
         self,
         *,
         segment: str,
         type: SegmentReferenceResourceTypeType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSegmentReferencesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListSegmentReferences.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/paginators/#listsegmentreferencespaginator)
         """
```

### Comparing `types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently/paginator.pyi` & `types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     """
 
     def paginate(
         self,
         *,
         project: str,
         status: ExperimentStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListExperimentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListExperiments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/paginators/#listexperimentspaginator)
         """
 
 class ListFeaturesPaginator(AioPaginator):
@@ -103,15 +103,15 @@
     """
 
     def paginate(
         self,
         *,
         project: str,
         status: LaunchStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListLaunchesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListLaunches.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/paginators/#listlaunchespaginator)
         """
 
 class ListProjectsPaginator(AioPaginator):
@@ -135,15 +135,15 @@
     """
 
     def paginate(
         self,
         *,
         segment: str,
         type: SegmentReferenceResourceTypeType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSegmentReferencesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListSegmentReferences.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/paginators/#listsegmentreferencespaginator)
         """
 
 class ListSegmentsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently/type_defs.py` & `types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "EvaluationRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CloudWatchLogsDestinationConfigTypeDef",
     "CloudWatchLogsDestinationTypeDef",
     "OnlineAbConfigTypeDef",
     "TreatmentConfigTypeDef",
```

### Comparing `types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently/type_defs.pyi` & `types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently.egg-info/PKG-INFO` & `types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-evidently
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CloudWatchEvidently 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CloudWatchEvidently 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/
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
 
 <a id="types-aiobotocore-evidently"></a>
 
 # types-aiobotocore-evidently
 
 [![PyPI - types-aiobotocore-evidently](https://img.shields.io/pypi/v/types-aiobotocore-evidently.svg?color=blue)](https://pypi.org/project/types-aiobotocore-evidently)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-evidently.svg?color=blue)](https://pypi.org/project/types-aiobotocore-evidently)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-evidently)](https://pepy.tech/project/types-aiobotocore-evidently)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatchEvidently 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
+[aiobotocore.CloudWatchEvidently 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
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
 [types-aiobotocore-evidently docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-evidently-2.9.0/types_aiobotocore_evidently.egg-info/SOURCES.txt` & `types-aiobotocore-evidently-2.9.1/types_aiobotocore_evidently.egg-info/SOURCES.txt`

 * *Files identical despite different names*

