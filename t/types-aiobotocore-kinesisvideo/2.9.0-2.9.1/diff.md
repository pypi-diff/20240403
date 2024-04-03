# Comparing `tmp/types-aiobotocore-kinesisvideo-2.9.0.tar.gz` & `tmp/types-aiobotocore-kinesisvideo-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kinesisvideo-2.9.0.tar", last modified: Wed Dec 13 19:59:41 2023, max compression
+gzip compressed data, was "types-aiobotocore-kinesisvideo-2.9.1.tar", last modified: Thu Jan 18 01:21:04 2024, max compression
```

## Comparing `types-aiobotocore-kinesisvideo-2.9.0.tar` & `types-aiobotocore-kinesisvideo-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:41.837557 types-aiobotocore-kinesisvideo-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:48:39.000000 types-aiobotocore-kinesisvideo-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13838 2023-12-13 19:59:41.837557 types-aiobotocore-kinesisvideo-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12255 2023-12-13 19:48:39.000000 types-aiobotocore-kinesisvideo-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:41.837557 types-aiobotocore-kinesisvideo-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2023-12-13 19:48:39.000000 types-aiobotocore-kinesisvideo-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:41.833557 types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo/
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2023-12-13 19:48:39.000000 types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2023-12-13 19:48:39.000000 types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      952 2023-12-13 19:48:39.000000 types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26800 2023-12-13 19:48:39.000000 types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    26796 2023-12-13 19:48:39.000000 types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10877 2023-12-13 19:48:40.000000 types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10875 2023-12-13 19:48:39.000000 types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6099 2023-12-13 19:48:39.000000 types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6093 2023-12-13 19:48:39.000000 types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:48:39.000000 types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    23680 2023-12-13 19:48:40.000000 types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23679 2023-12-13 19:48:40.000000 types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:48:39.000000 types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:41.837557 types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13838 2023-12-13 19:59:41.000000 types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      908 2023-12-13 19:59:41.000000 types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:41.000000 types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:41.000000 types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:41.000000 types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-13 19:59:41.000000 types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:04.553234 types-aiobotocore-kinesisvideo-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:10:26.000000 types-aiobotocore-kinesisvideo-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13858 2024-01-18 01:21:04.553234 types-aiobotocore-kinesisvideo-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12255 2024-01-18 01:10:26.000000 types-aiobotocore-kinesisvideo-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:04.553234 types-aiobotocore-kinesisvideo-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-01-18 01:10:26.000000 types-aiobotocore-kinesisvideo-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:04.549234 types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-01-18 01:10:26.000000 types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-01-18 01:10:26.000000 types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-01-18 01:10:26.000000 types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26810 2024-01-18 01:10:28.000000 types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26807 2024-01-18 01:10:28.000000 types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10875 2024-01-18 01:10:28.000000 types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10875 2024-01-18 01:10:28.000000 types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-01-18 01:10:28.000000 types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6096 2024-01-18 01:10:28.000000 types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:10:26.000000 types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    23679 2024-01-18 01:10:28.000000 types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23679 2024-01-18 01:10:28.000000 types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:10:26.000000 types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:04.553234 types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13858 2024-01-18 01:21:04.000000 types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-01-18 01:21:04.000000 types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:04.000000 types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:04.000000 types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:04.000000 types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-18 01:21:04.000000 types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kinesisvideo-2.9.0/LICENSE` & `types-aiobotocore-kinesisvideo-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-kinesisvideo-2.9.0/PKG-INFO` & `types-aiobotocore-kinesisvideo-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesisvideo
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.KinesisVideo 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.KinesisVideo 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/
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
 
 <a id="types-aiobotocore-kinesisvideo"></a>
 
 # types-aiobotocore-kinesisvideo
 
 [![PyPI - types-aiobotocore-kinesisvideo](https://img.shields.io/pypi/v/types-aiobotocore-kinesisvideo.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisvideo)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesisvideo.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisvideo)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesisvideo)](https://pepy.tech/project/types-aiobotocore-kinesisvideo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KinesisVideo 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
+[aiobotocore.KinesisVideo 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
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
 [types-aiobotocore-kinesisvideo docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-kinesisvideo-2.9.0/README.md` & `types-aiobotocore-kinesisvideo-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesisvideo.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisvideo)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesisvideo)](https://pepy.tech/project/types-aiobotocore-kinesisvideo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KinesisVideo 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
+[aiobotocore.KinesisVideo 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
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
 [types-aiobotocore-kinesisvideo docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-kinesisvideo-2.9.0/setup.py` & `types-aiobotocore-kinesisvideo-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kinesisvideo",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_kinesisvideo"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.KinesisVideo 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.KinesisVideo 2.9.1 service generated with"
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
     keywords="aiobotocore kinesisvideo type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_kinesisvideo": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo/__init__.py` & `types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     ListEdgeAgentConfigurationsPaginator,
     ListSignalingChannelsPaginator,
     ListStreamsPaginator,
 )
 
 Client = KinesisVideoClient
 
-
 __all__ = (
     "Client",
     "DescribeMappedResourceConfigurationPaginator",
     "KinesisVideoClient",
     "ListEdgeAgentConfigurationsPaginator",
     "ListSignalingChannelsPaginator",
     "ListStreamsPaginator",
```

### Comparing `types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo/__init__.pyi` & `types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo/__main__.py` & `types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.KinesisVideo 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.KinesisVideo 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo\nOther"
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

### Comparing `types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo/client.py` & `types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -58,26 +58,23 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("KinesisVideoClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     AccountChannelLimitExceededException: Type[BotocoreClientError]
     AccountStreamLimitExceededException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ClientLimitExceededException: Type[BotocoreClientError]
     DeviceStreamLimitExceededException: Type[BotocoreClientError]
@@ -88,15 +85,14 @@
     NotAuthorizedException: Type[BotocoreClientError]
     ResourceInUseException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     StreamEdgeConfigurationNotFoundException: Type[BotocoreClientError]
     TagsPerResourceExceededLimitException: Type[BotocoreClientError]
     VersionMismatchException: Type[BotocoreClientError]
 
-
 class KinesisVideoClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/)
     """
 
     meta: ClientMeta
@@ -128,15 +124,15 @@
 
     async def create_signaling_channel(
         self,
         *,
         ChannelName: str,
         ChannelType: ChannelTypeType = ...,
         SingleMasterConfiguration: SingleMasterConfigurationTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateSignalingChannelOutputTypeDef:
         """
         Creates a signaling channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.create_signaling_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#create_signaling_channel)
         """
@@ -145,15 +141,15 @@
         self,
         *,
         StreamName: str,
         DeviceName: str = ...,
         MediaType: str = ...,
         KmsKeyId: str = ...,
         DataRetentionInHours: int = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateStreamOutputTypeDef:
         """
         Creates a new Kinesis video stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.create_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#create_stream)
         """
@@ -213,15 +209,15 @@
 
     async def describe_mapped_resource_configuration(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeMappedResourceConfigurationOutputTypeDef:
         """
         Returns the most current information about the stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.describe_mapped_resource_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#describe_mapped_resource_configuration)
         """
@@ -290,15 +286,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#get_data_endpoint)
         """
 
     async def get_signaling_channel_endpoint(
         self,
         *,
         ChannelARN: str,
-        SingleMasterChannelEndpointConfiguration: SingleMasterChannelEndpointConfigurationTypeDef = ...
+        SingleMasterChannelEndpointConfiguration: SingleMasterChannelEndpointConfigurationTypeDef = ...,
     ) -> GetSignalingChannelEndpointOutputTypeDef:
         """
         Provides an endpoint for the specified signaling channel to send and receive
         messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.get_signaling_channel_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#get_signaling_channel_endpoint)
@@ -316,29 +312,29 @@
         """
 
     async def list_signaling_channels(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
-        ChannelNameCondition: ChannelNameConditionTypeDef = ...
+        ChannelNameCondition: ChannelNameConditionTypeDef = ...,
     ) -> ListSignalingChannelsOutputTypeDef:
         """
         Returns an array of `ChannelInfo` objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.list_signaling_channels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#list_signaling_channels)
         """
 
     async def list_streams(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
-        StreamNameCondition: StreamNameConditionTypeDef = ...
+        StreamNameCondition: StreamNameConditionTypeDef = ...,
     ) -> ListStreamsOutputTypeDef:
         """
         Returns an array of `StreamInfo` objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.list_streams)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#list_streams)
         """
@@ -414,30 +410,30 @@
     async def update_data_retention(
         self,
         *,
         CurrentVersion: str,
         Operation: UpdateDataRetentionOperationType,
         DataRetentionChangeInHours: int,
         StreamName: str = ...,
-        StreamARN: str = ...
+        StreamARN: str = ...,
     ) -> Dict[str, Any]:
         """
         Increases or decreases the stream's data retention period by the value that you
         specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_data_retention)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#update_data_retention)
         """
 
     async def update_image_generation_configuration(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
-        ImageGenerationConfiguration: ImageGenerationConfigurationTypeDef = ...
+        ImageGenerationConfiguration: ImageGenerationConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the `StreamInfo` and `ImageProcessingConfiguration` fields.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_image_generation_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#update_image_generation_configuration)
         """
@@ -453,29 +449,29 @@
         """
 
     async def update_notification_configuration(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
-        NotificationConfiguration: NotificationConfigurationTypeDef = ...
+        NotificationConfiguration: NotificationConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the notification information for a stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_notification_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#update_notification_configuration)
         """
 
     async def update_signaling_channel(
         self,
         *,
         ChannelARN: str,
         CurrentVersion: str,
-        SingleMasterConfiguration: SingleMasterConfigurationTypeDef = ...
+        SingleMasterConfiguration: SingleMasterConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the existing signaling channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_signaling_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#update_signaling_channel)
         """
@@ -483,15 +479,15 @@
     async def update_stream(
         self,
         *,
         CurrentVersion: str,
         StreamName: str = ...,
         StreamARN: str = ...,
         DeviceName: str = ...,
-        MediaType: str = ...
+        MediaType: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates stream metadata, such as the device name and media type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#update_stream)
         """
```

### Comparing `types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo/client.pyi` & `types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,21 +60,23 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("KinesisVideoClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     AccountChannelLimitExceededException: Type[BotocoreClientError]
     AccountStreamLimitExceededException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ClientLimitExceededException: Type[BotocoreClientError]
     DeviceStreamLimitExceededException: Type[BotocoreClientError]
@@ -85,14 +87,15 @@
     NotAuthorizedException: Type[BotocoreClientError]
     ResourceInUseException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     StreamEdgeConfigurationNotFoundException: Type[BotocoreClientError]
     TagsPerResourceExceededLimitException: Type[BotocoreClientError]
     VersionMismatchException: Type[BotocoreClientError]
 
+
 class KinesisVideoClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/)
     """
 
     meta: ClientMeta
@@ -124,15 +127,15 @@
 
     async def create_signaling_channel(
         self,
         *,
         ChannelName: str,
         ChannelType: ChannelTypeType = ...,
         SingleMasterConfiguration: SingleMasterConfigurationTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateSignalingChannelOutputTypeDef:
         """
         Creates a signaling channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.create_signaling_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#create_signaling_channel)
         """
@@ -141,15 +144,15 @@
         self,
         *,
         StreamName: str,
         DeviceName: str = ...,
         MediaType: str = ...,
         KmsKeyId: str = ...,
         DataRetentionInHours: int = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateStreamOutputTypeDef:
         """
         Creates a new Kinesis video stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.create_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#create_stream)
         """
@@ -209,15 +212,15 @@
 
     async def describe_mapped_resource_configuration(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeMappedResourceConfigurationOutputTypeDef:
         """
         Returns the most current information about the stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.describe_mapped_resource_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#describe_mapped_resource_configuration)
         """
@@ -286,15 +289,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#get_data_endpoint)
         """
 
     async def get_signaling_channel_endpoint(
         self,
         *,
         ChannelARN: str,
-        SingleMasterChannelEndpointConfiguration: SingleMasterChannelEndpointConfigurationTypeDef = ...
+        SingleMasterChannelEndpointConfiguration: SingleMasterChannelEndpointConfigurationTypeDef = ...,
     ) -> GetSignalingChannelEndpointOutputTypeDef:
         """
         Provides an endpoint for the specified signaling channel to send and receive
         messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.get_signaling_channel_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#get_signaling_channel_endpoint)
@@ -312,29 +315,29 @@
         """
 
     async def list_signaling_channels(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
-        ChannelNameCondition: ChannelNameConditionTypeDef = ...
+        ChannelNameCondition: ChannelNameConditionTypeDef = ...,
     ) -> ListSignalingChannelsOutputTypeDef:
         """
         Returns an array of `ChannelInfo` objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.list_signaling_channels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#list_signaling_channels)
         """
 
     async def list_streams(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
-        StreamNameCondition: StreamNameConditionTypeDef = ...
+        StreamNameCondition: StreamNameConditionTypeDef = ...,
     ) -> ListStreamsOutputTypeDef:
         """
         Returns an array of `StreamInfo` objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.list_streams)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#list_streams)
         """
@@ -410,30 +413,30 @@
     async def update_data_retention(
         self,
         *,
         CurrentVersion: str,
         Operation: UpdateDataRetentionOperationType,
         DataRetentionChangeInHours: int,
         StreamName: str = ...,
-        StreamARN: str = ...
+        StreamARN: str = ...,
     ) -> Dict[str, Any]:
         """
         Increases or decreases the stream's data retention period by the value that you
         specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_data_retention)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#update_data_retention)
         """
 
     async def update_image_generation_configuration(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
-        ImageGenerationConfiguration: ImageGenerationConfigurationTypeDef = ...
+        ImageGenerationConfiguration: ImageGenerationConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the `StreamInfo` and `ImageProcessingConfiguration` fields.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_image_generation_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#update_image_generation_configuration)
         """
@@ -449,29 +452,29 @@
         """
 
     async def update_notification_configuration(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
-        NotificationConfiguration: NotificationConfigurationTypeDef = ...
+        NotificationConfiguration: NotificationConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the notification information for a stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_notification_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#update_notification_configuration)
         """
 
     async def update_signaling_channel(
         self,
         *,
         ChannelARN: str,
         CurrentVersion: str,
-        SingleMasterConfiguration: SingleMasterConfigurationTypeDef = ...
+        SingleMasterConfiguration: SingleMasterConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the existing signaling channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_signaling_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#update_signaling_channel)
         """
@@ -479,15 +482,15 @@
     async def update_stream(
         self,
         *,
         CurrentVersion: str,
         StreamName: str = ...,
         StreamARN: str = ...,
         DeviceName: str = ...,
-        MediaType: str = ...
+        MediaType: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates stream metadata, such as the device name and media type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#update_stream)
         """
```

### Comparing `types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo/literals.py` & `types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo/literals.py`

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
     "APINameType",
     "ChannelProtocolType",
     "ChannelRoleType",
     "ChannelTypeType",
     "ComparisonOperatorType",
     "ConfigurationStatusType",
@@ -45,15 +44,14 @@
     "KinesisVideoServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 APINameType = Literal[
     "GET_CLIP",
     "GET_DASH_STREAMING_SESSION_URL",
     "GET_HLS_STREAMING_SESSION_URL",
     "GET_IMAGES",
     "GET_MEDIA",
     "GET_MEDIA_FOR_FRAGMENT_LIST",
```

### Comparing `types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo/literals.pyi` & `types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo/paginator.py` & `types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 __all__ = (
     "DescribeMappedResourceConfigurationPaginator",
     "ListEdgeAgentConfigurationsPaginator",
     "ListSignalingChannelsPaginator",
     "ListStreamsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -67,15 +66,15 @@
     """
 
     def paginate(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeMappedResourceConfigurationOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.DescribeMappedResourceConfiguration.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/paginators/#describemappedresourceconfigurationpaginator)
         """
 
 
@@ -100,15 +99,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/paginators/#listsignalingchannelspaginator)
     """
 
     def paginate(
         self,
         *,
         ChannelNameCondition: ChannelNameConditionTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSignalingChannelsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListSignalingChannels.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/paginators/#listsignalingchannelspaginator)
         """
 
 
@@ -118,13 +117,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/paginators/#liststreamspaginator)
     """
 
     def paginate(
         self,
         *,
         StreamNameCondition: StreamNameConditionTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListStreamsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListStreams.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/paginators/#liststreamspaginator)
         """
```

### Comparing `types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo/paginator.pyi` & `types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     """
 
     def paginate(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeMappedResourceConfigurationOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.DescribeMappedResourceConfiguration.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/paginators/#describemappedresourceconfigurationpaginator)
         """
 
 class ListEdgeAgentConfigurationsPaginator(AioPaginator):
@@ -95,15 +95,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/paginators/#listsignalingchannelspaginator)
     """
 
     def paginate(
         self,
         *,
         ChannelNameCondition: ChannelNameConditionTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSignalingChannelsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListSignalingChannels.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/paginators/#listsignalingchannelspaginator)
         """
 
 class ListStreamsPaginator(AioPaginator):
@@ -112,13 +112,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/paginators/#liststreamspaginator)
     """
 
     def paginate(
         self,
         *,
         StreamNameCondition: StreamNameConditionTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListStreamsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListStreams.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/paginators/#liststreamspaginator)
         """
```

### Comparing `types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo/type_defs.py` & `types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "SingleMasterConfigurationTypeDef",
     "ChannelNameConditionTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "CreateStreamInputRequestTypeDef",
     "DeleteEdgeConfigurationInputRequestTypeDef",
```

### Comparing `types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo/type_defs.pyi` & `types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo.egg-info/PKG-INFO` & `types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesisvideo
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.KinesisVideo 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.KinesisVideo 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/
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
 
 <a id="types-aiobotocore-kinesisvideo"></a>
 
 # types-aiobotocore-kinesisvideo
 
 [![PyPI - types-aiobotocore-kinesisvideo](https://img.shields.io/pypi/v/types-aiobotocore-kinesisvideo.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisvideo)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesisvideo.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisvideo)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesisvideo)](https://pepy.tech/project/types-aiobotocore-kinesisvideo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KinesisVideo 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
+[aiobotocore.KinesisVideo 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
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
 [types-aiobotocore-kinesisvideo docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-kinesisvideo-2.9.0/types_aiobotocore_kinesisvideo.egg-info/SOURCES.txt` & `types-aiobotocore-kinesisvideo-2.9.1/types_aiobotocore_kinesisvideo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

