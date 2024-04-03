# Comparing `tmp/types-aiobotocore-mediaconvert-2.9.0.tar.gz` & `tmp/types-aiobotocore-mediaconvert-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mediaconvert-2.9.0.tar", last modified: Wed Dec 13 19:59:52 2023, max compression
+gzip compressed data, was "types-aiobotocore-mediaconvert-2.9.1.tar", last modified: Thu Jan 18 01:21:14 2024, max compression
```

## Comparing `types-aiobotocore-mediaconvert-2.9.0.tar` & `types-aiobotocore-mediaconvert-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:52.681467 types-aiobotocore-mediaconvert-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:49:57.000000 types-aiobotocore-mediaconvert-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13778 2023-12-13 19:59:52.681467 types-aiobotocore-mediaconvert-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12195 2023-12-13 19:49:57.000000 types-aiobotocore-mediaconvert-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:52.681467 types-aiobotocore-mediaconvert-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2023-12-13 19:49:57.000000 types-aiobotocore-mediaconvert-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:52.681467 types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert/
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2023-12-13 19:49:57.000000 types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2023-12-13 19:49:57.000000 types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      952 2023-12-13 19:49:57.000000 types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24280 2023-12-13 19:49:57.000000 types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    24276 2023-12-13 19:49:57.000000 types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    57003 2023-12-13 19:50:00.000000 types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    57001 2023-12-13 19:49:58.000000 types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7037 2023-12-13 19:49:57.000000 types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7030 2023-12-13 19:49:57.000000 types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:49:57.000000 types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   148548 2023-12-13 19:50:02.000000 types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   148547 2023-12-13 19:50:01.000000 types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:49:57.000000 types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:52.681467 types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13778 2023-12-13 19:59:52.000000 types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      908 2023-12-13 19:59:52.000000 types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:52.000000 types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:52.000000 types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:52.000000 types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-13 19:59:52.000000 types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:14.633188 types-aiobotocore-mediaconvert-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:11:41.000000 types-aiobotocore-mediaconvert-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13798 2024-01-18 01:21:14.633188 types-aiobotocore-mediaconvert-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-01-18 01:11:41.000000 types-aiobotocore-mediaconvert-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:14.633188 types-aiobotocore-mediaconvert-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-01-18 01:11:41.000000 types-aiobotocore-mediaconvert-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:14.633188 types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert/
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-01-18 01:11:41.000000 types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-01-18 01:11:41.000000 types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-01-18 01:11:41.000000 types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24290 2024-01-18 01:11:41.000000 types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24287 2024-01-18 01:11:41.000000 types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    57001 2024-01-18 01:11:44.000000 types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57001 2024-01-18 01:11:44.000000 types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-01-18 01:11:41.000000 types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7035 2024-01-18 01:11:41.000000 types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:11:41.000000 types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   148547 2024-01-18 01:11:47.000000 types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   148547 2024-01-18 01:11:46.000000 types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:11:41.000000 types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:14.633188 types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13798 2024-01-18 01:21:14.000000 types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-01-18 01:21:14.000000 types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:14.000000 types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:14.000000 types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:14.000000 types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-18 01:21:14.000000 types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mediaconvert-2.9.0/LICENSE` & `types-aiobotocore-mediaconvert-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-mediaconvert-2.9.0/PKG-INFO` & `types-aiobotocore-mediaconvert-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mediaconvert
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MediaConvert 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MediaConvert 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/
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
 
 <a id="types-aiobotocore-mediaconvert"></a>
 
 # types-aiobotocore-mediaconvert
 
 [![PyPI - types-aiobotocore-mediaconvert](https://img.shields.io/pypi/v/types-aiobotocore-mediaconvert.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediaconvert)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediaconvert.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediaconvert)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediaconvert)](https://pepy.tech/project/types-aiobotocore-mediaconvert)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaConvert 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
+[aiobotocore.MediaConvert 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
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
 [types-aiobotocore-mediaconvert docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mediaconvert-2.9.0/README.md` & `types-aiobotocore-mediaconvert-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediaconvert.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediaconvert)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediaconvert)](https://pepy.tech/project/types-aiobotocore-mediaconvert)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaConvert 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
+[aiobotocore.MediaConvert 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
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
 [types-aiobotocore-mediaconvert docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mediaconvert-2.9.0/setup.py` & `types-aiobotocore-mediaconvert-2.9.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mediaconvert",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_mediaconvert"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MediaConvert 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.MediaConvert 2.9.1 service generated with"
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
     keywords="aiobotocore mediaconvert type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_mediaconvert": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert/__init__.py` & `types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     ListJobTemplatesPaginator,
     ListPresetsPaginator,
     ListQueuesPaginator,
 )
 
 Client = MediaConvertClient
 
-
 __all__ = (
     "Client",
     "DescribeEndpointsPaginator",
     "ListJobTemplatesPaginator",
     "ListJobsPaginator",
     "ListPresetsPaginator",
     "ListQueuesPaginator",
```

### Comparing `types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert/__init__.pyi` & `types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert/__main__.py` & `types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MediaConvert 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.MediaConvert 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert\nOther"
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

### Comparing `types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert/client.py` & `types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("MediaConvertClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -159,15 +158,15 @@
         HopDestinations: Sequence[HopDestinationTypeDef] = ...,
         JobTemplate: str = ...,
         Priority: int = ...,
         Queue: str = ...,
         SimulateReservedQueue: SimulateReservedQueueType = ...,
         StatusUpdateInterval: StatusUpdateIntervalType = ...,
         Tags: Mapping[str, str] = ...,
-        UserMetadata: Mapping[str, str] = ...
+        UserMetadata: Mapping[str, str] = ...,
     ) -> CreateJobResponseTypeDef:
         """
         Create a new transcoding job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.create_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#create_job)
         """
@@ -180,15 +179,15 @@
         AccelerationSettings: AccelerationSettingsTypeDef = ...,
         Category: str = ...,
         Description: str = ...,
         HopDestinations: Sequence[HopDestinationTypeDef] = ...,
         Priority: int = ...,
         Queue: str = ...,
         StatusUpdateInterval: StatusUpdateIntervalType = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateJobTemplateResponseTypeDef:
         """
         Create a new job template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.create_job_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#create_job_template)
         """
@@ -196,15 +195,15 @@
     async def create_preset(
         self,
         *,
         Name: str,
         Settings: PresetSettingsTypeDef,
         Category: str = ...,
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreatePresetResponseTypeDef:
         """
         Create a new preset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.create_preset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#create_preset)
         """
@@ -213,15 +212,15 @@
         self,
         *,
         Name: str,
         Description: str = ...,
         PricingPlan: PricingPlanType = ...,
         ReservationPlanSettings: ReservationPlanSettingsTypeDef = ...,
         Status: QueueStatusType = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateQueueResponseTypeDef:
         """
         Create a new transcoding queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.create_queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#create_queue)
         """
@@ -337,15 +336,15 @@
     async def list_job_templates(
         self,
         *,
         Category: str = ...,
         ListBy: JobTemplateListByType = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Order: OrderType = ...
+        Order: OrderType = ...,
     ) -> ListJobTemplatesResponseTypeDef:
         """
         Retrieve a JSON array of up to twenty of your job templates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.list_job_templates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#list_job_templates)
         """
@@ -353,15 +352,15 @@
     async def list_jobs(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         Order: OrderType = ...,
         Queue: str = ...,
-        Status: JobStatusType = ...
+        Status: JobStatusType = ...,
     ) -> ListJobsResponseTypeDef:
         """
         Retrieve a JSON array of up to twenty of your most recently created jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.list_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#list_jobs)
         """
@@ -369,30 +368,30 @@
     async def list_presets(
         self,
         *,
         Category: str = ...,
         ListBy: PresetListByType = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Order: OrderType = ...
+        Order: OrderType = ...,
     ) -> ListPresetsResponseTypeDef:
         """
         Retrieve a JSON array of up to twenty of your presets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.list_presets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#list_presets)
         """
 
     async def list_queues(
         self,
         *,
         ListBy: QueueListByType = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Order: OrderType = ...
+        Order: OrderType = ...,
     ) -> ListQueuesResponseTypeDef:
         """
         Retrieve a JSON array of up to twenty of your queues.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.list_queues)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#list_queues)
         """
@@ -436,45 +435,45 @@
         AccelerationSettings: AccelerationSettingsTypeDef = ...,
         Category: str = ...,
         Description: str = ...,
         HopDestinations: Sequence[HopDestinationTypeDef] = ...,
         Priority: int = ...,
         Queue: str = ...,
         Settings: JobTemplateSettingsTypeDef = ...,
-        StatusUpdateInterval: StatusUpdateIntervalType = ...
+        StatusUpdateInterval: StatusUpdateIntervalType = ...,
     ) -> UpdateJobTemplateResponseTypeDef:
         """
         Modify one of your existing job templates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.update_job_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#update_job_template)
         """
 
     async def update_preset(
         self,
         *,
         Name: str,
         Category: str = ...,
         Description: str = ...,
-        Settings: PresetSettingsTypeDef = ...
+        Settings: PresetSettingsTypeDef = ...,
     ) -> UpdatePresetResponseTypeDef:
         """
         Modify one of your existing presets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.update_preset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#update_preset)
         """
 
     async def update_queue(
         self,
         *,
         Name: str,
         Description: str = ...,
         ReservationPlanSettings: ReservationPlanSettingsTypeDef = ...,
-        Status: QueueStatusType = ...
+        Status: QueueStatusType = ...,
     ) -> UpdateQueueResponseTypeDef:
         """
         Modify one of your existing queues.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.update_queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#update_queue)
         """
```

### Comparing `types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert/client.pyi` & `types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         HopDestinations: Sequence[HopDestinationTypeDef] = ...,
         JobTemplate: str = ...,
         Priority: int = ...,
         Queue: str = ...,
         SimulateReservedQueue: SimulateReservedQueueType = ...,
         StatusUpdateInterval: StatusUpdateIntervalType = ...,
         Tags: Mapping[str, str] = ...,
-        UserMetadata: Mapping[str, str] = ...
+        UserMetadata: Mapping[str, str] = ...,
     ) -> CreateJobResponseTypeDef:
         """
         Create a new transcoding job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.create_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#create_job)
         """
@@ -176,15 +176,15 @@
         AccelerationSettings: AccelerationSettingsTypeDef = ...,
         Category: str = ...,
         Description: str = ...,
         HopDestinations: Sequence[HopDestinationTypeDef] = ...,
         Priority: int = ...,
         Queue: str = ...,
         StatusUpdateInterval: StatusUpdateIntervalType = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateJobTemplateResponseTypeDef:
         """
         Create a new job template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.create_job_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#create_job_template)
         """
@@ -192,15 +192,15 @@
     async def create_preset(
         self,
         *,
         Name: str,
         Settings: PresetSettingsTypeDef,
         Category: str = ...,
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreatePresetResponseTypeDef:
         """
         Create a new preset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.create_preset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#create_preset)
         """
@@ -209,15 +209,15 @@
         self,
         *,
         Name: str,
         Description: str = ...,
         PricingPlan: PricingPlanType = ...,
         ReservationPlanSettings: ReservationPlanSettingsTypeDef = ...,
         Status: QueueStatusType = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateQueueResponseTypeDef:
         """
         Create a new transcoding queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.create_queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#create_queue)
         """
@@ -333,15 +333,15 @@
     async def list_job_templates(
         self,
         *,
         Category: str = ...,
         ListBy: JobTemplateListByType = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Order: OrderType = ...
+        Order: OrderType = ...,
     ) -> ListJobTemplatesResponseTypeDef:
         """
         Retrieve a JSON array of up to twenty of your job templates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.list_job_templates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#list_job_templates)
         """
@@ -349,15 +349,15 @@
     async def list_jobs(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         Order: OrderType = ...,
         Queue: str = ...,
-        Status: JobStatusType = ...
+        Status: JobStatusType = ...,
     ) -> ListJobsResponseTypeDef:
         """
         Retrieve a JSON array of up to twenty of your most recently created jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.list_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#list_jobs)
         """
@@ -365,30 +365,30 @@
     async def list_presets(
         self,
         *,
         Category: str = ...,
         ListBy: PresetListByType = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Order: OrderType = ...
+        Order: OrderType = ...,
     ) -> ListPresetsResponseTypeDef:
         """
         Retrieve a JSON array of up to twenty of your presets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.list_presets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#list_presets)
         """
 
     async def list_queues(
         self,
         *,
         ListBy: QueueListByType = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Order: OrderType = ...
+        Order: OrderType = ...,
     ) -> ListQueuesResponseTypeDef:
         """
         Retrieve a JSON array of up to twenty of your queues.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.list_queues)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#list_queues)
         """
@@ -432,45 +432,45 @@
         AccelerationSettings: AccelerationSettingsTypeDef = ...,
         Category: str = ...,
         Description: str = ...,
         HopDestinations: Sequence[HopDestinationTypeDef] = ...,
         Priority: int = ...,
         Queue: str = ...,
         Settings: JobTemplateSettingsTypeDef = ...,
-        StatusUpdateInterval: StatusUpdateIntervalType = ...
+        StatusUpdateInterval: StatusUpdateIntervalType = ...,
     ) -> UpdateJobTemplateResponseTypeDef:
         """
         Modify one of your existing job templates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.update_job_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#update_job_template)
         """
 
     async def update_preset(
         self,
         *,
         Name: str,
         Category: str = ...,
         Description: str = ...,
-        Settings: PresetSettingsTypeDef = ...
+        Settings: PresetSettingsTypeDef = ...,
     ) -> UpdatePresetResponseTypeDef:
         """
         Modify one of your existing presets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.update_preset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#update_preset)
         """
 
     async def update_queue(
         self,
         *,
         Name: str,
         Description: str = ...,
         ReservationPlanSettings: ReservationPlanSettingsTypeDef = ...,
-        Status: QueueStatusType = ...
+        Status: QueueStatusType = ...,
     ) -> UpdateQueueResponseTypeDef:
         """
         Modify one of your existing queues.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.update_queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#update_queue)
         """
```

### Comparing `types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert/literals.py` & `types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert/literals.py`

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
     "AacAudioDescriptionBroadcasterMixType",
     "AacCodecProfileType",
     "AacCodingModeType",
     "AacRateControlModeType",
     "AacRawFormatType",
     "AacSpecificationType",
@@ -442,15 +441,14 @@
     "MediaConvertServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AacAudioDescriptionBroadcasterMixType = Literal["BROADCASTER_MIXED_AD", "NORMAL"]
 AacCodecProfileType = Literal["HEV1", "HEV2", "LC"]
 AacCodingModeType = Literal[
     "AD_RECEIVER_MIX", "CODING_MODE_1_0", "CODING_MODE_1_1", "CODING_MODE_2_0", "CODING_MODE_5_1"
 ]
 AacRateControlModeType = Literal["CBR", "VBR"]
 AacRawFormatType = Literal["LATM_LOAS", "NONE"]
```

### Comparing `types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert/literals.pyi` & `types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert/paginator.py` & `types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,14 @@
     "DescribeEndpointsPaginator",
     "ListJobTemplatesPaginator",
     "ListJobsPaginator",
     "ListPresetsPaginator",
     "ListQueuesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -76,15 +75,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/paginators/#describeendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         Mode: DescribeEndpointsModeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.DescribeEndpoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/paginators/#describeendpointspaginator)
         """
 
 
@@ -96,15 +95,15 @@
 
     def paginate(
         self,
         *,
         Category: str = ...,
         ListBy: JobTemplateListByType = ...,
         Order: OrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListJobTemplatesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListJobTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/paginators/#listjobtemplatespaginator)
         """
 
 
@@ -116,15 +115,15 @@
 
     def paginate(
         self,
         *,
         Order: OrderType = ...,
         Queue: str = ...,
         Status: JobStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListJobsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/paginators/#listjobspaginator)
         """
 
 
@@ -136,15 +135,15 @@
 
     def paginate(
         self,
         *,
         Category: str = ...,
         ListBy: PresetListByType = ...,
         Order: OrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPresetsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListPresets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/paginators/#listpresetspaginator)
         """
 
 
@@ -155,13 +154,13 @@
     """
 
     def paginate(
         self,
         *,
         ListBy: QueueListByType = ...,
         Order: OrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListQueuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListQueues.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/paginators/#listqueuespaginator)
         """
```

### Comparing `types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert/paginator.pyi` & `types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/paginators/#describeendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         Mode: DescribeEndpointsModeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.DescribeEndpoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/paginators/#describeendpointspaginator)
         """
 
 class ListJobTemplatesPaginator(AioPaginator):
@@ -92,15 +92,15 @@
 
     def paginate(
         self,
         *,
         Category: str = ...,
         ListBy: JobTemplateListByType = ...,
         Order: OrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListJobTemplatesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListJobTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/paginators/#listjobtemplatespaginator)
         """
 
 class ListJobsPaginator(AioPaginator):
@@ -111,15 +111,15 @@
 
     def paginate(
         self,
         *,
         Order: OrderType = ...,
         Queue: str = ...,
         Status: JobStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListJobsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/paginators/#listjobspaginator)
         """
 
 class ListPresetsPaginator(AioPaginator):
@@ -130,15 +130,15 @@
 
     def paginate(
         self,
         *,
         Category: str = ...,
         ListBy: PresetListByType = ...,
         Order: OrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPresetsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListPresets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/paginators/#listpresetspaginator)
         """
 
 class ListQueuesPaginator(AioPaginator):
@@ -148,13 +148,13 @@
     """
 
     def paginate(
         self,
         *,
         ListBy: QueueListByType = ...,
         Order: OrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListQueuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListQueues.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/paginators/#listqueuespaginator)
         """
```

### Comparing `types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert/type_defs.py` & `types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -436,15 +436,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AacSettingsTypeDef",
     "Ac3SettingsTypeDef",
     "AccelerationSettingsTypeDef",
     "AdvancedInputFilterSettingsTypeDef",
     "AiffSettingsTypeDef",
     "AllowedRenditionSizeTypeDef",
```

### Comparing `types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert/type_defs.pyi` & `types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert.egg-info/PKG-INFO` & `types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mediaconvert
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MediaConvert 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MediaConvert 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/
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
 
 <a id="types-aiobotocore-mediaconvert"></a>
 
 # types-aiobotocore-mediaconvert
 
 [![PyPI - types-aiobotocore-mediaconvert](https://img.shields.io/pypi/v/types-aiobotocore-mediaconvert.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediaconvert)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediaconvert.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediaconvert)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediaconvert)](https://pepy.tech/project/types-aiobotocore-mediaconvert)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaConvert 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
+[aiobotocore.MediaConvert 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
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
 [types-aiobotocore-mediaconvert docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mediaconvert-2.9.0/types_aiobotocore_mediaconvert.egg-info/SOURCES.txt` & `types-aiobotocore-mediaconvert-2.9.1/types_aiobotocore_mediaconvert.egg-info/SOURCES.txt`

 * *Files identical despite different names*

