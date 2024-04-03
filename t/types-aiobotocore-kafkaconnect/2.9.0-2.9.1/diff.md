# Comparing `tmp/types-aiobotocore-kafkaconnect-2.9.0.tar.gz` & `tmp/types-aiobotocore-kafkaconnect-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kafkaconnect-2.9.0.tar", last modified: Wed Dec 13 19:59:37 2023, max compression
+gzip compressed data, was "types-aiobotocore-kafkaconnect-2.9.1.tar", last modified: Thu Jan 18 01:21:00 2024, max compression
```

## Comparing `types-aiobotocore-kafkaconnect-2.9.0.tar` & `types-aiobotocore-kafkaconnect-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:37.765591 types-aiobotocore-kafkaconnect-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:48:23.000000 types-aiobotocore-kafkaconnect-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13580 2023-12-13 19:59:37.765591 types-aiobotocore-kafkaconnect-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11997 2023-12-13 19:48:23.000000 types-aiobotocore-kafkaconnect-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:37.765591 types-aiobotocore-kafkaconnect-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2023-12-13 19:48:23.000000 types-aiobotocore-kafkaconnect-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:37.765591 types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect/
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2023-12-13 19:48:23.000000 types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2023-12-13 19:48:23.000000 types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      952 2023-12-13 19:48:23.000000 types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14155 2023-12-13 19:48:23.000000 types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14151 2023-12-13 19:48:23.000000 types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9472 2023-12-13 19:48:23.000000 types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9470 2023-12-13 19:48:23.000000 types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4432 2023-12-13 19:48:23.000000 types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2023-12-13 19:48:23.000000 types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:48:23.000000 types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    23712 2023-12-13 19:48:24.000000 types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23711 2023-12-13 19:48:23.000000 types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:48:23.000000 types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:37.765591 types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13580 2023-12-13 19:59:37.000000 types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      908 2023-12-13 19:59:37.000000 types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:37.000000 types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:37.000000 types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:37.000000 types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-13 19:59:37.000000 types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:00.821250 types-aiobotocore-kafkaconnect-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:10:11.000000 types-aiobotocore-kafkaconnect-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13600 2024-01-18 01:21:00.821250 types-aiobotocore-kafkaconnect-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11997 2024-01-18 01:10:11.000000 types-aiobotocore-kafkaconnect-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:00.821250 types-aiobotocore-kafkaconnect-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-01-18 01:10:11.000000 types-aiobotocore-kafkaconnect-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:00.821250 types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-01-18 01:10:11.000000 types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-01-18 01:10:11.000000 types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-01-18 01:10:11.000000 types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14156 2024-01-18 01:10:11.000000 types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14153 2024-01-18 01:10:11.000000 types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9470 2024-01-18 01:10:11.000000 types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9470 2024-01-18 01:10:11.000000 types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-01-18 01:10:11.000000 types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-01-18 01:10:11.000000 types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:10:11.000000 types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    23711 2024-01-18 01:10:12.000000 types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23711 2024-01-18 01:10:12.000000 types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:10:11.000000 types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:00.821250 types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13600 2024-01-18 01:21:00.000000 types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-01-18 01:21:00.000000 types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:00.000000 types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:00.000000 types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:00.000000 types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-18 01:21:00.000000 types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kafkaconnect-2.9.0/LICENSE` & `types-aiobotocore-kafkaconnect-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-kafkaconnect-2.9.0/PKG-INFO` & `types-aiobotocore-kafkaconnect-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kafkaconnect
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.KafkaConnect 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.KafkaConnect 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafkaconnect/
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
 
 <a id="types-aiobotocore-kafkaconnect"></a>
 
 # types-aiobotocore-kafkaconnect
 
 [![PyPI - types-aiobotocore-kafkaconnect](https://img.shields.io/pypi/v/types-aiobotocore-kafkaconnect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kafkaconnect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kafkaconnect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kafkaconnect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafkaconnect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kafkaconnect)](https://pepy.tech/project/types-aiobotocore-kafkaconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KafkaConnect 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect)
+[aiobotocore.KafkaConnect 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect)
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
 [types-aiobotocore-kafkaconnect docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafkaconnect/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-kafkaconnect-2.9.0/README.md` & `types-aiobotocore-kafkaconnect-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kafkaconnect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kafkaconnect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafkaconnect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kafkaconnect)](https://pepy.tech/project/types-aiobotocore-kafkaconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KafkaConnect 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect)
+[aiobotocore.KafkaConnect 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect)
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
 [types-aiobotocore-kafkaconnect docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafkaconnect/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-kafkaconnect-2.9.0/setup.py` & `types-aiobotocore-kafkaconnect-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kafkaconnect",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_kafkaconnect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.KafkaConnect 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.KafkaConnect 2.9.1 service generated with"
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
     keywords="aiobotocore kafkaconnect type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_kafkaconnect": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafkaconnect/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect/__init__.py` & `types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     ListConnectorsPaginator,
     ListCustomPluginsPaginator,
     ListWorkerConfigurationsPaginator,
 )
 
 Client = KafkaConnectClient
 
-
 __all__ = (
     "Client",
     "KafkaConnectClient",
     "ListConnectorsPaginator",
     "ListCustomPluginsPaginator",
     "ListWorkerConfigurationsPaginator",
 )
```

### Comparing `types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect/__init__.pyi` & `types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect/__main__.py` & `types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.KafkaConnect 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.KafkaConnect 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafkaconnect//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect\nOther"
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

### Comparing `types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect/client.py` & `types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("KafkaConnectClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -123,30 +122,30 @@
         kafkaClusterClientAuthentication: KafkaClusterClientAuthenticationTypeDef,
         kafkaClusterEncryptionInTransit: KafkaClusterEncryptionInTransitTypeDef,
         kafkaConnectVersion: str,
         plugins: Sequence[PluginTypeDef],
         serviceExecutionRoleArn: str,
         connectorDescription: str = ...,
         logDelivery: LogDeliveryTypeDef = ...,
-        workerConfiguration: WorkerConfigurationTypeDef = ...
+        workerConfiguration: WorkerConfigurationTypeDef = ...,
     ) -> CreateConnectorResponseTypeDef:
         """
         Creates a connector using the specified properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Client.create_connector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafkaconnect/client/#create_connector)
         """
 
     async def create_custom_plugin(
         self,
         *,
         contentType: CustomPluginContentTypeType,
         location: CustomPluginLocationTypeDef,
         name: str,
-        description: str = ...
+        description: str = ...,
     ) -> CreateCustomPluginResponseTypeDef:
         """
         Creates a custom plugin using the specified properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Client.create_custom_plugin)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafkaconnect/client/#create_custom_plugin)
         """
```

### Comparing `types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect/client.pyi` & `types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -119,30 +119,30 @@
         kafkaClusterClientAuthentication: KafkaClusterClientAuthenticationTypeDef,
         kafkaClusterEncryptionInTransit: KafkaClusterEncryptionInTransitTypeDef,
         kafkaConnectVersion: str,
         plugins: Sequence[PluginTypeDef],
         serviceExecutionRoleArn: str,
         connectorDescription: str = ...,
         logDelivery: LogDeliveryTypeDef = ...,
-        workerConfiguration: WorkerConfigurationTypeDef = ...
+        workerConfiguration: WorkerConfigurationTypeDef = ...,
     ) -> CreateConnectorResponseTypeDef:
         """
         Creates a connector using the specified properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Client.create_connector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafkaconnect/client/#create_connector)
         """
 
     async def create_custom_plugin(
         self,
         *,
         contentType: CustomPluginContentTypeType,
         location: CustomPluginLocationTypeDef,
         name: str,
-        description: str = ...
+        description: str = ...,
     ) -> CreateCustomPluginResponseTypeDef:
         """
         Creates a custom plugin using the specified properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Client.create_custom_plugin)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafkaconnect/client/#create_custom_plugin)
         """
```

### Comparing `types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect/literals.py` & `types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect/literals.py`

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
     "ConnectorStateType",
     "CustomPluginContentTypeType",
     "CustomPluginStateType",
     "KafkaClusterClientAuthenticationTypeType",
     "KafkaClusterEncryptionInTransitTypeType",
     "ListConnectorsPaginatorName",
@@ -32,15 +31,14 @@
     "KafkaConnectServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ConnectorStateType = Literal["CREATING", "DELETING", "FAILED", "RUNNING", "UPDATING"]
 CustomPluginContentTypeType = Literal["JAR", "ZIP"]
 CustomPluginStateType = Literal[
     "ACTIVE", "CREATE_FAILED", "CREATING", "DELETING", "UPDATE_FAILED", "UPDATING"
 ]
 KafkaClusterClientAuthenticationTypeType = Literal["IAM", "NONE"]
 KafkaClusterEncryptionInTransitTypeType = Literal["PLAINTEXT", "TLS"]
```

### Comparing `types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect/literals.pyi` & `types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect/paginator.py` & `types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 
 __all__ = (
     "ListConnectorsPaginator",
     "ListCustomPluginsPaginator",
     "ListWorkerConfigurationsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect/paginator.pyi` & `types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect/type_defs.py` & `types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "VpcDescriptionTypeDef",
     "VpcTypeDef",
     "ScaleInPolicyDescriptionTypeDef",
     "ScaleOutPolicyDescriptionTypeDef",
     "ScaleInPolicyTypeDef",
     "ScaleOutPolicyTypeDef",
```

### Comparing `types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect/type_defs.pyi` & `types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect.egg-info/PKG-INFO` & `types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kafkaconnect
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.KafkaConnect 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.KafkaConnect 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafkaconnect/
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
 
 <a id="types-aiobotocore-kafkaconnect"></a>
 
 # types-aiobotocore-kafkaconnect
 
 [![PyPI - types-aiobotocore-kafkaconnect](https://img.shields.io/pypi/v/types-aiobotocore-kafkaconnect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kafkaconnect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kafkaconnect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kafkaconnect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafkaconnect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kafkaconnect)](https://pepy.tech/project/types-aiobotocore-kafkaconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KafkaConnect 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect)
+[aiobotocore.KafkaConnect 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect)
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
 [types-aiobotocore-kafkaconnect docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafkaconnect/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-kafkaconnect-2.9.0/types_aiobotocore_kafkaconnect.egg-info/SOURCES.txt` & `types-aiobotocore-kafkaconnect-2.9.1/types_aiobotocore_kafkaconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

