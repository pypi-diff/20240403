# Comparing `tmp/types-aiobotocore-ivschat-2.9.0.tar.gz` & `tmp/types-aiobotocore-ivschat-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ivschat-2.9.0.tar", last modified: Wed Dec 13 19:59:37 2023, max compression
+gzip compressed data, was "types-aiobotocore-ivschat-2.9.1.tar", last modified: Thu Jan 18 01:21:00 2024, max compression
```

## Comparing `types-aiobotocore-ivschat-2.9.0.tar` & `types-aiobotocore-ivschat-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:37.009597 types-aiobotocore-ivschat-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:48:18.000000 types-aiobotocore-ivschat-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12287 2023-12-13 19:59:37.009597 types-aiobotocore-ivschat-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10724 2023-12-13 19:48:18.000000 types-aiobotocore-ivschat-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:37.009597 types-aiobotocore-ivschat-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2023-12-13 19:48:18.000000 types-aiobotocore-ivschat-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:37.009597 types-aiobotocore-ivschat-2.9.0/types_aiobotocore_ivschat/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2023-12-13 19:48:18.000000 types-aiobotocore-ivschat-2.9.0/types_aiobotocore_ivschat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2023-12-13 19:48:18.000000 types-aiobotocore-ivschat-2.9.0/types_aiobotocore_ivschat/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      932 2023-12-13 19:48:18.000000 types-aiobotocore-ivschat-2.9.0/types_aiobotocore_ivschat/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14884 2023-12-13 19:48:18.000000 types-aiobotocore-ivschat-2.9.0/types_aiobotocore_ivschat/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14881 2023-12-13 19:48:18.000000 types-aiobotocore-ivschat-2.9.0/types_aiobotocore_ivschat/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8848 2023-12-13 19:48:18.000000 types-aiobotocore-ivschat-2.9.0/types_aiobotocore_ivschat/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8846 2023-12-13 19:48:18.000000 types-aiobotocore-ivschat-2.9.0/types_aiobotocore_ivschat/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:48:18.000000 types-aiobotocore-ivschat-2.9.0/types_aiobotocore_ivschat/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12666 2023-12-13 19:48:19.000000 types-aiobotocore-ivschat-2.9.0/types_aiobotocore_ivschat/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12665 2023-12-13 19:48:19.000000 types-aiobotocore-ivschat-2.9.0/types_aiobotocore_ivschat/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:48:18.000000 types-aiobotocore-ivschat-2.9.0/types_aiobotocore_ivschat/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:37.009597 types-aiobotocore-ivschat-2.9.0/types_aiobotocore_ivschat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12287 2023-12-13 19:59:36.000000 types-aiobotocore-ivschat-2.9.0/types_aiobotocore_ivschat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      734 2023-12-13 19:59:36.000000 types-aiobotocore-ivschat-2.9.0/types_aiobotocore_ivschat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:36.000000 types-aiobotocore-ivschat-2.9.0/types_aiobotocore_ivschat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:36.000000 types-aiobotocore-ivschat-2.9.0/types_aiobotocore_ivschat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:36.000000 types-aiobotocore-ivschat-2.9.0/types_aiobotocore_ivschat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-13 19:59:36.000000 types-aiobotocore-ivschat-2.9.0/types_aiobotocore_ivschat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:00.141253 types-aiobotocore-ivschat-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:10:06.000000 types-aiobotocore-ivschat-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-01-18 01:21:00.141253 types-aiobotocore-ivschat-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10724 2024-01-18 01:10:06.000000 types-aiobotocore-ivschat-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:00.141253 types-aiobotocore-ivschat-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-01-18 01:10:06.000000 types-aiobotocore-ivschat-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:00.141253 types-aiobotocore-ivschat-2.9.1/types_aiobotocore_ivschat/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-01-18 01:10:06.000000 types-aiobotocore-ivschat-2.9.1/types_aiobotocore_ivschat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-01-18 01:10:06.000000 types-aiobotocore-ivschat-2.9.1/types_aiobotocore_ivschat/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-01-18 01:10:06.000000 types-aiobotocore-ivschat-2.9.1/types_aiobotocore_ivschat/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14890 2024-01-18 01:10:07.000000 types-aiobotocore-ivschat-2.9.1/types_aiobotocore_ivschat/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14887 2024-01-18 01:10:06.000000 types-aiobotocore-ivschat-2.9.1/types_aiobotocore_ivschat/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-01-18 01:10:07.000000 types-aiobotocore-ivschat-2.9.1/types_aiobotocore_ivschat/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-01-18 01:10:07.000000 types-aiobotocore-ivschat-2.9.1/types_aiobotocore_ivschat/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:10:06.000000 types-aiobotocore-ivschat-2.9.1/types_aiobotocore_ivschat/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12665 2024-01-18 01:10:09.000000 types-aiobotocore-ivschat-2.9.1/types_aiobotocore_ivschat/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12665 2024-01-18 01:10:09.000000 types-aiobotocore-ivschat-2.9.1/types_aiobotocore_ivschat/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:10:06.000000 types-aiobotocore-ivschat-2.9.1/types_aiobotocore_ivschat/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:00.141253 types-aiobotocore-ivschat-2.9.1/types_aiobotocore_ivschat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-01-18 01:21:00.000000 types-aiobotocore-ivschat-2.9.1/types_aiobotocore_ivschat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-01-18 01:21:00.000000 types-aiobotocore-ivschat-2.9.1/types_aiobotocore_ivschat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:00.000000 types-aiobotocore-ivschat-2.9.1/types_aiobotocore_ivschat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:00.000000 types-aiobotocore-ivschat-2.9.1/types_aiobotocore_ivschat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:00.000000 types-aiobotocore-ivschat-2.9.1/types_aiobotocore_ivschat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-18 01:21:00.000000 types-aiobotocore-ivschat-2.9.1/types_aiobotocore_ivschat.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ivschat-2.9.0/LICENSE` & `types-aiobotocore-ivschat-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-ivschat-2.9.0/PKG-INFO` & `types-aiobotocore-ivschat-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ivschat
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ivschat 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ivschat 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivschat/
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
 
 <a id="types-aiobotocore-ivschat"></a>
 
 # types-aiobotocore-ivschat
 
 [![PyPI - types-aiobotocore-ivschat](https://img.shields.io/pypi/v/types-aiobotocore-ivschat.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ivschat)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ivschat.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ivschat)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivschat/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ivschat)](https://pepy.tech/project/types-aiobotocore-ivschat)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ivschat 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
+[aiobotocore.ivschat 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
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
 [types-aiobotocore-ivschat docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivschat/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ivschat-2.9.0/README.md` & `types-aiobotocore-ivschat-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ivschat.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ivschat)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivschat/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ivschat)](https://pepy.tech/project/types-aiobotocore-ivschat)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ivschat 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
+[aiobotocore.ivschat 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
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
 [types-aiobotocore-ivschat docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivschat/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ivschat-2.9.0/setup.py` & `types-aiobotocore-ivschat-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ivschat",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_ivschat"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ivschat 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.ivschat 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore ivschat type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_ivschat": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivschat/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-ivschat-2.9.0/types_aiobotocore_ivschat/__main__.py` & `types-aiobotocore-ivschat-2.9.1/types_aiobotocore_ivschat/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ivschat 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ivschat 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivschat//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat\nOther"
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

### Comparing `types-aiobotocore-ivschat-2.9.0/types_aiobotocore_ivschat/client.py` & `types-aiobotocore-ivschat-2.9.1/types_aiobotocore_ivschat/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     async def create_chat_token(
         self,
         *,
         roomIdentifier: str,
         userId: str,
         attributes: Mapping[str, str] = ...,
         capabilities: Sequence[ChatTokenCapabilityType] = ...,
-        sessionDurationInMinutes: int = ...
+        sessionDurationInMinutes: int = ...,
     ) -> CreateChatTokenResponseTypeDef:
         """
         Creates an encrypted token that is used by a chat participant to establish an
         individual WebSocket chat connection to a
         room.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat.Client.create_chat_token)
@@ -114,15 +114,15 @@
         """
 
     async def create_logging_configuration(
         self,
         *,
         destinationConfiguration: DestinationConfigurationTypeDef,
         name: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateLoggingConfigurationResponseTypeDef:
         """
         Creates a logging configuration that allows clients to store and record sent
         messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat.Client.create_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivschat/client/#create_logging_configuration)
@@ -132,15 +132,15 @@
         self,
         *,
         loggingConfigurationIdentifiers: Sequence[str] = ...,
         maximumMessageLength: int = ...,
         maximumMessageRatePerSecond: int = ...,
         messageReviewHandler: MessageReviewHandlerTypeDef = ...,
         name: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateRoomResponseTypeDef:
         """
         Creates a room that allows clients to connect and pass messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat.Client.create_room)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivschat/client/#create_room)
         """
@@ -232,15 +232,15 @@
     async def list_rooms(
         self,
         *,
         loggingConfigurationIdentifier: str = ...,
         maxResults: int = ...,
         messageReviewHandlerUri: str = ...,
         name: str = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListRoomsResponseTypeDef:
         """
         Gets summary information about all your rooms in the AWS region where the API
         request is
         processed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat.Client.list_rooms)
@@ -284,15 +284,15 @@
         """
 
     async def update_logging_configuration(
         self,
         *,
         identifier: str,
         destinationConfiguration: DestinationConfigurationTypeDef = ...,
-        name: str = ...
+        name: str = ...,
     ) -> UpdateLoggingConfigurationResponseTypeDef:
         """
         Updates a specified logging configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat.Client.update_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivschat/client/#update_logging_configuration)
         """
@@ -301,15 +301,15 @@
         self,
         *,
         identifier: str,
         loggingConfigurationIdentifiers: Sequence[str] = ...,
         maximumMessageLength: int = ...,
         maximumMessageRatePerSecond: int = ...,
         messageReviewHandler: MessageReviewHandlerTypeDef = ...,
-        name: str = ...
+        name: str = ...,
     ) -> UpdateRoomResponseTypeDef:
         """
         Updates a room’s configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat.Client.update_room)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivschat/client/#update_room)
         """
```

### Comparing `types-aiobotocore-ivschat-2.9.0/types_aiobotocore_ivschat/client.pyi` & `types-aiobotocore-ivschat-2.9.1/types_aiobotocore_ivschat/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     async def create_chat_token(
         self,
         *,
         roomIdentifier: str,
         userId: str,
         attributes: Mapping[str, str] = ...,
         capabilities: Sequence[ChatTokenCapabilityType] = ...,
-        sessionDurationInMinutes: int = ...
+        sessionDurationInMinutes: int = ...,
     ) -> CreateChatTokenResponseTypeDef:
         """
         Creates an encrypted token that is used by a chat participant to establish an
         individual WebSocket chat connection to a
         room.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat.Client.create_chat_token)
@@ -111,15 +111,15 @@
         """
 
     async def create_logging_configuration(
         self,
         *,
         destinationConfiguration: DestinationConfigurationTypeDef,
         name: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateLoggingConfigurationResponseTypeDef:
         """
         Creates a logging configuration that allows clients to store and record sent
         messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat.Client.create_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivschat/client/#create_logging_configuration)
@@ -129,15 +129,15 @@
         self,
         *,
         loggingConfigurationIdentifiers: Sequence[str] = ...,
         maximumMessageLength: int = ...,
         maximumMessageRatePerSecond: int = ...,
         messageReviewHandler: MessageReviewHandlerTypeDef = ...,
         name: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateRoomResponseTypeDef:
         """
         Creates a room that allows clients to connect and pass messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat.Client.create_room)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivschat/client/#create_room)
         """
@@ -229,15 +229,15 @@
     async def list_rooms(
         self,
         *,
         loggingConfigurationIdentifier: str = ...,
         maxResults: int = ...,
         messageReviewHandlerUri: str = ...,
         name: str = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListRoomsResponseTypeDef:
         """
         Gets summary information about all your rooms in the AWS region where the API
         request is
         processed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat.Client.list_rooms)
@@ -281,15 +281,15 @@
         """
 
     async def update_logging_configuration(
         self,
         *,
         identifier: str,
         destinationConfiguration: DestinationConfigurationTypeDef = ...,
-        name: str = ...
+        name: str = ...,
     ) -> UpdateLoggingConfigurationResponseTypeDef:
         """
         Updates a specified logging configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat.Client.update_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivschat/client/#update_logging_configuration)
         """
@@ -298,15 +298,15 @@
         self,
         *,
         identifier: str,
         loggingConfigurationIdentifiers: Sequence[str] = ...,
         maximumMessageLength: int = ...,
         maximumMessageRatePerSecond: int = ...,
         messageReviewHandler: MessageReviewHandlerTypeDef = ...,
-        name: str = ...
+        name: str = ...,
     ) -> UpdateRoomResponseTypeDef:
         """
         Updates a room’s configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat.Client.update_room)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivschat/client/#update_room)
         """
```

### Comparing `types-aiobotocore-ivschat-2.9.0/types_aiobotocore_ivschat/literals.py` & `types-aiobotocore-ivschat-2.9.1/types_aiobotocore_ivschat/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,28 +15,26 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ChatTokenCapabilityType",
     "CreateLoggingConfigurationStateType",
     "FallbackResultType",
     "LoggingConfigurationStateType",
     "UpdateLoggingConfigurationStateType",
     "ivschatServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 ChatTokenCapabilityType = Literal["DELETE_MESSAGE", "DISCONNECT_USER", "SEND_MESSAGE"]
 CreateLoggingConfigurationStateType = Literal["ACTIVE"]
 FallbackResultType = Literal["ALLOW", "DENY"]
 LoggingConfigurationStateType = Literal[
     "ACTIVE", "CREATE_FAILED", "CREATING", "DELETE_FAILED", "DELETING", "UPDATE_FAILED", "UPDATING"
 ]
 UpdateLoggingConfigurationStateType = Literal["ACTIVE"]
```

### Comparing `types-aiobotocore-ivschat-2.9.0/types_aiobotocore_ivschat/literals.pyi` & `types-aiobotocore-ivschat-2.9.1/types_aiobotocore_ivschat/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ivschat-2.9.0/types_aiobotocore_ivschat/type_defs.py` & `types-aiobotocore-ivschat-2.9.1/types_aiobotocore_ivschat/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CloudWatchLogsDestinationConfigurationTypeDef",
     "CreateChatTokenRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "MessageReviewHandlerTypeDef",
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     "DeleteMessageRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-ivschat-2.9.0/types_aiobotocore_ivschat/type_defs.pyi` & `types-aiobotocore-ivschat-2.9.1/types_aiobotocore_ivschat/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ivschat-2.9.0/types_aiobotocore_ivschat.egg-info/PKG-INFO` & `types-aiobotocore-ivschat-2.9.1/types_aiobotocore_ivschat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ivschat
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ivschat 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ivschat 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivschat/
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
 
 <a id="types-aiobotocore-ivschat"></a>
 
 # types-aiobotocore-ivschat
 
 [![PyPI - types-aiobotocore-ivschat](https://img.shields.io/pypi/v/types-aiobotocore-ivschat.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ivschat)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ivschat.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ivschat)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivschat/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ivschat)](https://pepy.tech/project/types-aiobotocore-ivschat)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ivschat 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
+[aiobotocore.ivschat 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
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
 [types-aiobotocore-ivschat docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivschat/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ivschat-2.9.0/types_aiobotocore_ivschat.egg-info/SOURCES.txt` & `types-aiobotocore-ivschat-2.9.1/types_aiobotocore_ivschat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

