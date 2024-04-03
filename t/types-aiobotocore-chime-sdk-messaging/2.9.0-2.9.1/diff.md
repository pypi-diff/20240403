# Comparing `tmp/types-aiobotocore-chime-sdk-messaging-2.9.0.tar.gz` & `tmp/types-aiobotocore-chime-sdk-messaging-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-chime-sdk-messaging-2.9.0.tar", last modified: Wed Dec 13 19:58:46 2023, max compression
+gzip compressed data, was "types-aiobotocore-chime-sdk-messaging-2.9.1.tar", last modified: Thu Jan 18 01:20:13 2024, max compression
```

## Comparing `types-aiobotocore-chime-sdk-messaging-2.9.0.tar` & `types-aiobotocore-chime-sdk-messaging-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:46.205999 types-aiobotocore-chime-sdk-messaging-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:42:04.000000 types-aiobotocore-chime-sdk-messaging-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12891 2023-12-13 19:58:46.205999 types-aiobotocore-chime-sdk-messaging-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11282 2023-12-13 19:42:04.000000 types-aiobotocore-chime-sdk-messaging-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:46.205999 types-aiobotocore-chime-sdk-messaging-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2023-12-13 19:42:04.000000 types-aiobotocore-chime-sdk-messaging-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:46.205999 types-aiobotocore-chime-sdk-messaging-2.9.0/types_aiobotocore_chime_sdk_messaging/
--rw-r--r--   0 runner    (1001) docker     (127)      529 2023-12-13 19:42:04.000000 types-aiobotocore-chime-sdk-messaging-2.9.0/types_aiobotocore_chime_sdk_messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2023-12-13 19:42:04.000000 types-aiobotocore-chime-sdk-messaging-2.9.0/types_aiobotocore_chime_sdk_messaging/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      976 2023-12-13 19:42:04.000000 types-aiobotocore-chime-sdk-messaging-2.9.0/types_aiobotocore_chime_sdk_messaging/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40517 2023-12-13 19:42:04.000000 types-aiobotocore-chime-sdk-messaging-2.9.0/types_aiobotocore_chime_sdk_messaging/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    40514 2023-12-13 19:42:04.000000 types-aiobotocore-chime-sdk-messaging-2.9.0/types_aiobotocore_chime_sdk_messaging/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9919 2023-12-13 19:42:04.000000 types-aiobotocore-chime-sdk-messaging-2.9.0/types_aiobotocore_chime_sdk_messaging/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9917 2023-12-13 19:42:04.000000 types-aiobotocore-chime-sdk-messaging-2.9.0/types_aiobotocore_chime_sdk_messaging/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:42:04.000000 types-aiobotocore-chime-sdk-messaging-2.9.0/types_aiobotocore_chime_sdk_messaging/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    39726 2023-12-13 19:42:05.000000 types-aiobotocore-chime-sdk-messaging-2.9.0/types_aiobotocore_chime_sdk_messaging/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    39725 2023-12-13 19:42:04.000000 types-aiobotocore-chime-sdk-messaging-2.9.0/types_aiobotocore_chime_sdk_messaging/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:42:04.000000 types-aiobotocore-chime-sdk-messaging-2.9.0/types_aiobotocore_chime_sdk_messaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:46.205999 types-aiobotocore-chime-sdk-messaging-2.9.0/types_aiobotocore_chime_sdk_messaging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12891 2023-12-13 19:58:46.000000 types-aiobotocore-chime-sdk-messaging-2.9.0/types_aiobotocore_chime_sdk_messaging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      938 2023-12-13 19:58:46.000000 types-aiobotocore-chime-sdk-messaging-2.9.0/types_aiobotocore_chime_sdk_messaging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:46.000000 types-aiobotocore-chime-sdk-messaging-2.9.0/types_aiobotocore_chime_sdk_messaging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:46.000000 types-aiobotocore-chime-sdk-messaging-2.9.0/types_aiobotocore_chime_sdk_messaging.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:46.000000 types-aiobotocore-chime-sdk-messaging-2.9.0/types_aiobotocore_chime_sdk_messaging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:46.000000 types-aiobotocore-chime-sdk-messaging-2.9.0/types_aiobotocore_chime_sdk_messaging.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:13.245476 types-aiobotocore-chime-sdk-messaging-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:04:01.000000 types-aiobotocore-chime-sdk-messaging-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12911 2024-01-18 01:20:13.245476 types-aiobotocore-chime-sdk-messaging-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11282 2024-01-18 01:04:01.000000 types-aiobotocore-chime-sdk-messaging-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:13.245476 types-aiobotocore-chime-sdk-messaging-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-01-18 01:04:01.000000 types-aiobotocore-chime-sdk-messaging-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:13.245476 types-aiobotocore-chime-sdk-messaging-2.9.1/types_aiobotocore_chime_sdk_messaging/
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-01-18 01:04:01.000000 types-aiobotocore-chime-sdk-messaging-2.9.1/types_aiobotocore_chime_sdk_messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-01-18 01:04:01.000000 types-aiobotocore-chime-sdk-messaging-2.9.1/types_aiobotocore_chime_sdk_messaging/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-01-18 01:04:01.000000 types-aiobotocore-chime-sdk-messaging-2.9.1/types_aiobotocore_chime_sdk_messaging/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40534 2024-01-18 01:04:01.000000 types-aiobotocore-chime-sdk-messaging-2.9.1/types_aiobotocore_chime_sdk_messaging/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40531 2024-01-18 01:04:01.000000 types-aiobotocore-chime-sdk-messaging-2.9.1/types_aiobotocore_chime_sdk_messaging/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9917 2024-01-18 01:04:01.000000 types-aiobotocore-chime-sdk-messaging-2.9.1/types_aiobotocore_chime_sdk_messaging/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9917 2024-01-18 01:04:01.000000 types-aiobotocore-chime-sdk-messaging-2.9.1/types_aiobotocore_chime_sdk_messaging/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:04:01.000000 types-aiobotocore-chime-sdk-messaging-2.9.1/types_aiobotocore_chime_sdk_messaging/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    39725 2024-01-18 01:04:02.000000 types-aiobotocore-chime-sdk-messaging-2.9.1/types_aiobotocore_chime_sdk_messaging/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39725 2024-01-18 01:04:02.000000 types-aiobotocore-chime-sdk-messaging-2.9.1/types_aiobotocore_chime_sdk_messaging/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:04:01.000000 types-aiobotocore-chime-sdk-messaging-2.9.1/types_aiobotocore_chime_sdk_messaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:13.245476 types-aiobotocore-chime-sdk-messaging-2.9.1/types_aiobotocore_chime_sdk_messaging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12911 2024-01-18 01:20:13.000000 types-aiobotocore-chime-sdk-messaging-2.9.1/types_aiobotocore_chime_sdk_messaging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-01-18 01:20:13.000000 types-aiobotocore-chime-sdk-messaging-2.9.1/types_aiobotocore_chime_sdk_messaging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:13.000000 types-aiobotocore-chime-sdk-messaging-2.9.1/types_aiobotocore_chime_sdk_messaging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:13.000000 types-aiobotocore-chime-sdk-messaging-2.9.1/types_aiobotocore_chime_sdk_messaging.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:13.000000 types-aiobotocore-chime-sdk-messaging-2.9.1/types_aiobotocore_chime_sdk_messaging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:13.000000 types-aiobotocore-chime-sdk-messaging-2.9.1/types_aiobotocore_chime_sdk_messaging.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-chime-sdk-messaging-2.9.0/LICENSE` & `types-aiobotocore-chime-sdk-messaging-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-chime-sdk-messaging-2.9.0/PKG-INFO` & `types-aiobotocore-chime-sdk-messaging-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-chime-sdk-messaging
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ChimeSDKMessaging 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ChimeSDKMessaging 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/
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
 
 <a id="types-aiobotocore-chime-sdk-messaging"></a>
 
 # types-aiobotocore-chime-sdk-messaging
 
 [![PyPI - types-aiobotocore-chime-sdk-messaging](https://img.shields.io/pypi/v/types-aiobotocore-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-messaging)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-messaging)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime-sdk-messaging)](https://pepy.tech/project/types-aiobotocore-chime-sdk-messaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ChimeSDKMessaging 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
+[aiobotocore.ChimeSDKMessaging 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
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
 [types-aiobotocore-chime-sdk-messaging docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-chime-sdk-messaging-2.9.0/README.md` & `types-aiobotocore-chime-sdk-messaging-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-messaging)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime-sdk-messaging)](https://pepy.tech/project/types-aiobotocore-chime-sdk-messaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ChimeSDKMessaging 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
+[aiobotocore.ChimeSDKMessaging 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
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
 [types-aiobotocore-chime-sdk-messaging docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-chime-sdk-messaging-2.9.0/setup.py` & `types-aiobotocore-chime-sdk-messaging-2.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-chime-sdk-messaging",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_chime_sdk_messaging"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ChimeSDKMessaging 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ChimeSDKMessaging 2.9.1 service generated with"
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
     keywords="aiobotocore chime-sdk-messaging type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_chime_sdk_messaging": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-chime-sdk-messaging-2.9.0/types_aiobotocore_chime_sdk_messaging/__init__.py` & `types-aiobotocore-chime-sdk-messaging-2.9.1/types_aiobotocore_chime_sdk_messaging/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,9 +18,8 @@
     ```
 """
 
 from .client import ChimeSDKMessagingClient
 
 Client = ChimeSDKMessagingClient
 
-
 __all__ = ("ChimeSDKMessagingClient", "Client")
```

### Comparing `types-aiobotocore-chime-sdk-messaging-2.9.0/types_aiobotocore_chime_sdk_messaging/__init__.pyi` & `types-aiobotocore-chime-sdk-messaging-2.9.1/types_aiobotocore_chime_sdk_messaging/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-messaging-2.9.0/types_aiobotocore_chime_sdk_messaging/__main__.py` & `types-aiobotocore-chime-sdk-messaging-2.9.1/types_aiobotocore_chime_sdk_messaging/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ChimeSDKMessaging 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ChimeSDKMessaging 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging\nOther"
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

### Comparing `types-aiobotocore-chime-sdk-messaging-2.9.0/types_aiobotocore_chime_sdk_messaging/client.py` & `types-aiobotocore-chime-sdk-messaging-2.9.1/types_aiobotocore_chime_sdk_messaging/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
     async def batch_create_channel_membership(
         self,
         *,
         ChannelArn: str,
         MemberArns: Sequence[str],
         ChimeBearer: str,
         Type: ChannelMembershipTypeType = ...,
-        SubChannelId: str = ...
+        SubChannelId: str = ...,
     ) -> BatchCreateChannelMembershipResponseTypeDef:
         """
         Adds a specified number of users and bots to a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.batch_create_channel_membership)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#batch_create_channel_membership)
         """
@@ -161,15 +161,15 @@
 
     async def channel_flow_callback(
         self,
         *,
         CallbackId: str,
         ChannelArn: str,
         ChannelMessage: ChannelMessageCallbackTypeDef,
-        DeleteResource: bool = ...
+        DeleteResource: bool = ...,
     ) -> ChannelFlowCallbackResponseTypeDef:
         """
         Calls back Amazon Chime SDK messaging with a processing response message.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.channel_flow_callback)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#channel_flow_callback)
         """
@@ -193,15 +193,15 @@
         Privacy: ChannelPrivacyType = ...,
         Metadata: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ChannelId: str = ...,
         MemberArns: Sequence[str] = ...,
         ModeratorArns: Sequence[str] = ...,
         ElasticChannelConfiguration: ElasticChannelConfigurationTypeDef = ...,
-        ExpirationSettings: ExpirationSettingsTypeDef = ...
+        ExpirationSettings: ExpirationSettingsTypeDef = ...,
     ) -> CreateChannelResponseTypeDef:
         """
         Creates a channel to which you can add users and send messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.create_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#create_channel)
         """
@@ -219,15 +219,15 @@
     async def create_channel_flow(
         self,
         *,
         AppInstanceArn: str,
         Processors: Sequence[ProcessorTypeDef],
         Name: str,
         ClientRequestToken: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateChannelFlowResponseTypeDef:
         """
         Creates a channel flow, a container for processors.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.create_channel_flow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#create_channel_flow)
         """
@@ -235,15 +235,15 @@
     async def create_channel_membership(
         self,
         *,
         ChannelArn: str,
         MemberArn: str,
         Type: ChannelMembershipTypeType,
         ChimeBearer: str,
-        SubChannelId: str = ...
+        SubChannelId: str = ...,
     ) -> CreateChannelMembershipResponseTypeDef:
         """
         Adds a member to a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.create_channel_membership)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#create_channel_membership)
         """
@@ -499,30 +499,30 @@
         self,
         *,
         ChannelArn: str,
         ChimeBearer: str,
         Type: ChannelMembershipTypeType = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        SubChannelId: str = ...
+        SubChannelId: str = ...,
     ) -> ListChannelMembershipsResponseTypeDef:
         """
         Lists all channel memberships in a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channel_memberships)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#list_channel_memberships)
         """
 
     async def list_channel_memberships_for_app_instance_user(
         self,
         *,
         ChimeBearer: str,
         AppInstanceUserArn: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListChannelMembershipsForAppInstanceUserResponseTypeDef:
         """
         Lists all channels that an `AppInstanceUser` or `AppInstanceBot` is a part of.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channel_memberships_for_app_instance_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#list_channel_memberships_for_app_instance_user)
         """
@@ -533,15 +533,15 @@
         ChannelArn: str,
         ChimeBearer: str,
         SortOrder: SortOrderType = ...,
         NotBefore: TimestampTypeDef = ...,
         NotAfter: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        SubChannelId: str = ...
+        SubChannelId: str = ...,
     ) -> ListChannelMessagesResponseTypeDef:
         """
         List all the messages in a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channel_messages)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#list_channel_messages)
         """
@@ -559,15 +559,15 @@
     async def list_channels(
         self,
         *,
         AppInstanceArn: str,
         ChimeBearer: str,
         Privacy: ChannelPrivacyType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListChannelsResponseTypeDef:
         """
         Lists all Channels created under a single Chime App as a paginated list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#list_channels)
         """
@@ -584,15 +584,15 @@
 
     async def list_channels_moderated_by_app_instance_user(
         self,
         *,
         ChimeBearer: str,
         AppInstanceUserArn: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListChannelsModeratedByAppInstanceUserResponseTypeDef:
         """
         A list of the channels moderated by an `AppInstanceUser`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channels_moderated_by_app_instance_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#list_channels_moderated_by_app_instance_user)
         """
@@ -618,45 +618,45 @@
         """
 
     async def put_channel_expiration_settings(
         self,
         *,
         ChannelArn: str,
         ChimeBearer: str = ...,
-        ExpirationSettings: ExpirationSettingsTypeDef = ...
+        ExpirationSettings: ExpirationSettingsTypeDef = ...,
     ) -> PutChannelExpirationSettingsResponseTypeDef:
         """
         Sets the number of days before the channel is automatically deleted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.put_channel_expiration_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#put_channel_expiration_settings)
         """
 
     async def put_channel_membership_preferences(
         self,
         *,
         ChannelArn: str,
         MemberArn: str,
         ChimeBearer: str,
-        Preferences: ChannelMembershipPreferencesTypeDef
+        Preferences: ChannelMembershipPreferencesTypeDef,
     ) -> PutChannelMembershipPreferencesResponseTypeDef:
         """
         Sets the membership preferences of an `AppInstanceUser` or `AppInstanceBot` for
         the specified
         channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.put_channel_membership_preferences)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#put_channel_membership_preferences)
         """
 
     async def put_messaging_streaming_configurations(
         self,
         *,
         AppInstanceArn: str,
-        StreamingConfigurations: Sequence[StreamingConfigurationTypeDef]
+        StreamingConfigurations: Sequence[StreamingConfigurationTypeDef],
     ) -> PutMessagingStreamingConfigurationsResponseTypeDef:
         """
         Sets the data streaming configuration for an `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.put_messaging_streaming_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#put_messaging_streaming_configurations)
         """
@@ -673,15 +673,15 @@
 
     async def search_channels(
         self,
         *,
         Fields: Sequence[SearchFieldTypeDef],
         ChimeBearer: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> SearchChannelsResponseTypeDef:
         """
         Allows the `ChimeBearer` to search channels by channel members.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.search_channels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#search_channels)
         """
@@ -696,15 +696,15 @@
         ClientRequestToken: str,
         ChimeBearer: str,
         Metadata: str = ...,
         PushNotification: PushNotificationConfigurationTypeDef = ...,
         MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
         SubChannelId: str = ...,
         ContentType: str = ...,
-        Target: Sequence[TargetTypeDef] = ...
+        Target: Sequence[TargetTypeDef] = ...,
     ) -> SendChannelMessageResponseTypeDef:
         """
         Sends a message to a particular channel that the member is a part of.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.send_channel_message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#send_channel_message)
         """
@@ -733,15 +733,15 @@
     async def update_channel(
         self,
         *,
         ChannelArn: str,
         ChimeBearer: str,
         Name: str = ...,
         Mode: ChannelModeType = ...,
-        Metadata: str = ...
+        Metadata: str = ...,
     ) -> UpdateChannelResponseTypeDef:
         """
         Update a channel's attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.update_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#update_channel)
         """
@@ -761,15 +761,15 @@
         *,
         ChannelArn: str,
         MessageId: str,
         Content: str,
         ChimeBearer: str,
         Metadata: str = ...,
         SubChannelId: str = ...,
-        ContentType: str = ...
+        ContentType: str = ...,
     ) -> UpdateChannelMessageResponseTypeDef:
         """
         Updates the content of a message.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.update_channel_message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#update_channel_message)
         """
```

### Comparing `types-aiobotocore-chime-sdk-messaging-2.9.0/types_aiobotocore_chime_sdk_messaging/client.pyi` & `types-aiobotocore-chime-sdk-messaging-2.9.1/types_aiobotocore_chime_sdk_messaging/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
     async def batch_create_channel_membership(
         self,
         *,
         ChannelArn: str,
         MemberArns: Sequence[str],
         ChimeBearer: str,
         Type: ChannelMembershipTypeType = ...,
-        SubChannelId: str = ...
+        SubChannelId: str = ...,
     ) -> BatchCreateChannelMembershipResponseTypeDef:
         """
         Adds a specified number of users and bots to a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.batch_create_channel_membership)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#batch_create_channel_membership)
         """
@@ -158,15 +158,15 @@
 
     async def channel_flow_callback(
         self,
         *,
         CallbackId: str,
         ChannelArn: str,
         ChannelMessage: ChannelMessageCallbackTypeDef,
-        DeleteResource: bool = ...
+        DeleteResource: bool = ...,
     ) -> ChannelFlowCallbackResponseTypeDef:
         """
         Calls back Amazon Chime SDK messaging with a processing response message.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.channel_flow_callback)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#channel_flow_callback)
         """
@@ -190,15 +190,15 @@
         Privacy: ChannelPrivacyType = ...,
         Metadata: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ChannelId: str = ...,
         MemberArns: Sequence[str] = ...,
         ModeratorArns: Sequence[str] = ...,
         ElasticChannelConfiguration: ElasticChannelConfigurationTypeDef = ...,
-        ExpirationSettings: ExpirationSettingsTypeDef = ...
+        ExpirationSettings: ExpirationSettingsTypeDef = ...,
     ) -> CreateChannelResponseTypeDef:
         """
         Creates a channel to which you can add users and send messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.create_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#create_channel)
         """
@@ -216,15 +216,15 @@
     async def create_channel_flow(
         self,
         *,
         AppInstanceArn: str,
         Processors: Sequence[ProcessorTypeDef],
         Name: str,
         ClientRequestToken: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateChannelFlowResponseTypeDef:
         """
         Creates a channel flow, a container for processors.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.create_channel_flow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#create_channel_flow)
         """
@@ -232,15 +232,15 @@
     async def create_channel_membership(
         self,
         *,
         ChannelArn: str,
         MemberArn: str,
         Type: ChannelMembershipTypeType,
         ChimeBearer: str,
-        SubChannelId: str = ...
+        SubChannelId: str = ...,
     ) -> CreateChannelMembershipResponseTypeDef:
         """
         Adds a member to a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.create_channel_membership)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#create_channel_membership)
         """
@@ -496,30 +496,30 @@
         self,
         *,
         ChannelArn: str,
         ChimeBearer: str,
         Type: ChannelMembershipTypeType = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        SubChannelId: str = ...
+        SubChannelId: str = ...,
     ) -> ListChannelMembershipsResponseTypeDef:
         """
         Lists all channel memberships in a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channel_memberships)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#list_channel_memberships)
         """
 
     async def list_channel_memberships_for_app_instance_user(
         self,
         *,
         ChimeBearer: str,
         AppInstanceUserArn: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListChannelMembershipsForAppInstanceUserResponseTypeDef:
         """
         Lists all channels that an `AppInstanceUser` or `AppInstanceBot` is a part of.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channel_memberships_for_app_instance_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#list_channel_memberships_for_app_instance_user)
         """
@@ -530,15 +530,15 @@
         ChannelArn: str,
         ChimeBearer: str,
         SortOrder: SortOrderType = ...,
         NotBefore: TimestampTypeDef = ...,
         NotAfter: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        SubChannelId: str = ...
+        SubChannelId: str = ...,
     ) -> ListChannelMessagesResponseTypeDef:
         """
         List all the messages in a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channel_messages)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#list_channel_messages)
         """
@@ -556,15 +556,15 @@
     async def list_channels(
         self,
         *,
         AppInstanceArn: str,
         ChimeBearer: str,
         Privacy: ChannelPrivacyType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListChannelsResponseTypeDef:
         """
         Lists all Channels created under a single Chime App as a paginated list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#list_channels)
         """
@@ -581,15 +581,15 @@
 
     async def list_channels_moderated_by_app_instance_user(
         self,
         *,
         ChimeBearer: str,
         AppInstanceUserArn: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListChannelsModeratedByAppInstanceUserResponseTypeDef:
         """
         A list of the channels moderated by an `AppInstanceUser`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channels_moderated_by_app_instance_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#list_channels_moderated_by_app_instance_user)
         """
@@ -615,45 +615,45 @@
         """
 
     async def put_channel_expiration_settings(
         self,
         *,
         ChannelArn: str,
         ChimeBearer: str = ...,
-        ExpirationSettings: ExpirationSettingsTypeDef = ...
+        ExpirationSettings: ExpirationSettingsTypeDef = ...,
     ) -> PutChannelExpirationSettingsResponseTypeDef:
         """
         Sets the number of days before the channel is automatically deleted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.put_channel_expiration_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#put_channel_expiration_settings)
         """
 
     async def put_channel_membership_preferences(
         self,
         *,
         ChannelArn: str,
         MemberArn: str,
         ChimeBearer: str,
-        Preferences: ChannelMembershipPreferencesTypeDef
+        Preferences: ChannelMembershipPreferencesTypeDef,
     ) -> PutChannelMembershipPreferencesResponseTypeDef:
         """
         Sets the membership preferences of an `AppInstanceUser` or `AppInstanceBot` for
         the specified
         channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.put_channel_membership_preferences)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#put_channel_membership_preferences)
         """
 
     async def put_messaging_streaming_configurations(
         self,
         *,
         AppInstanceArn: str,
-        StreamingConfigurations: Sequence[StreamingConfigurationTypeDef]
+        StreamingConfigurations: Sequence[StreamingConfigurationTypeDef],
     ) -> PutMessagingStreamingConfigurationsResponseTypeDef:
         """
         Sets the data streaming configuration for an `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.put_messaging_streaming_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#put_messaging_streaming_configurations)
         """
@@ -670,15 +670,15 @@
 
     async def search_channels(
         self,
         *,
         Fields: Sequence[SearchFieldTypeDef],
         ChimeBearer: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> SearchChannelsResponseTypeDef:
         """
         Allows the `ChimeBearer` to search channels by channel members.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.search_channels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#search_channels)
         """
@@ -693,15 +693,15 @@
         ClientRequestToken: str,
         ChimeBearer: str,
         Metadata: str = ...,
         PushNotification: PushNotificationConfigurationTypeDef = ...,
         MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
         SubChannelId: str = ...,
         ContentType: str = ...,
-        Target: Sequence[TargetTypeDef] = ...
+        Target: Sequence[TargetTypeDef] = ...,
     ) -> SendChannelMessageResponseTypeDef:
         """
         Sends a message to a particular channel that the member is a part of.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.send_channel_message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#send_channel_message)
         """
@@ -730,15 +730,15 @@
     async def update_channel(
         self,
         *,
         ChannelArn: str,
         ChimeBearer: str,
         Name: str = ...,
         Mode: ChannelModeType = ...,
-        Metadata: str = ...
+        Metadata: str = ...,
     ) -> UpdateChannelResponseTypeDef:
         """
         Update a channel's attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.update_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#update_channel)
         """
@@ -758,15 +758,15 @@
         *,
         ChannelArn: str,
         MessageId: str,
         Content: str,
         ChimeBearer: str,
         Metadata: str = ...,
         SubChannelId: str = ...,
-        ContentType: str = ...
+        ContentType: str = ...,
     ) -> UpdateChannelMessageResponseTypeDef:
         """
         Updates the content of a message.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.update_channel_message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/client/#update_channel_message)
         """
```

### Comparing `types-aiobotocore-chime-sdk-messaging-2.9.0/types_aiobotocore_chime_sdk_messaging/literals.py` & `types-aiobotocore-chime-sdk-messaging-2.9.1/types_aiobotocore_chime_sdk_messaging/literals.py`

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
     "AllowNotificationsType",
     "ChannelMembershipTypeType",
     "ChannelMessagePersistenceTypeType",
     "ChannelMessageStatusType",
     "ChannelMessageTypeType",
     "ChannelModeType",
@@ -39,15 +38,14 @@
     "SortOrderType",
     "ChimeSDKMessagingServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AllowNotificationsType = Literal["ALL", "FILTERED", "NONE"]
 ChannelMembershipTypeType = Literal["DEFAULT", "HIDDEN"]
 ChannelMessagePersistenceTypeType = Literal["NON_PERSISTENT", "PERSISTENT"]
 ChannelMessageStatusType = Literal["DENIED", "FAILED", "PENDING", "SENT"]
 ChannelMessageTypeType = Literal["CONTROL", "STANDARD"]
 ChannelModeType = Literal["RESTRICTED", "UNRESTRICTED"]
 ChannelPrivacyType = Literal["PRIVATE", "PUBLIC"]
```

### Comparing `types-aiobotocore-chime-sdk-messaging-2.9.0/types_aiobotocore_chime_sdk_messaging/literals.pyi` & `types-aiobotocore-chime-sdk-messaging-2.9.1/types_aiobotocore_chime_sdk_messaging/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-messaging-2.9.0/types_aiobotocore_chime_sdk_messaging/type_defs.py` & `types-aiobotocore-chime-sdk-messaging-2.9.1/types_aiobotocore_chime_sdk_messaging/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AppInstanceUserMembershipSummaryTypeDef",
     "AssociateChannelFlowRequestRequestTypeDef",
     "IdentityTypeDef",
     "BatchCreateChannelMembershipErrorTypeDef",
     "BatchCreateChannelMembershipRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
```

### Comparing `types-aiobotocore-chime-sdk-messaging-2.9.0/types_aiobotocore_chime_sdk_messaging/type_defs.pyi` & `types-aiobotocore-chime-sdk-messaging-2.9.1/types_aiobotocore_chime_sdk_messaging/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-messaging-2.9.0/types_aiobotocore_chime_sdk_messaging.egg-info/PKG-INFO` & `types-aiobotocore-chime-sdk-messaging-2.9.1/types_aiobotocore_chime_sdk_messaging.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-chime-sdk-messaging
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ChimeSDKMessaging 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ChimeSDKMessaging 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/
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
 
 <a id="types-aiobotocore-chime-sdk-messaging"></a>
 
 # types-aiobotocore-chime-sdk-messaging
 
 [![PyPI - types-aiobotocore-chime-sdk-messaging](https://img.shields.io/pypi/v/types-aiobotocore-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-messaging)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-messaging)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime-sdk-messaging)](https://pepy.tech/project/types-aiobotocore-chime-sdk-messaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ChimeSDKMessaging 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
+[aiobotocore.ChimeSDKMessaging 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
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
 [types-aiobotocore-chime-sdk-messaging docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-chime-sdk-messaging-2.9.0/types_aiobotocore_chime_sdk_messaging.egg-info/SOURCES.txt` & `types-aiobotocore-chime-sdk-messaging-2.9.1/types_aiobotocore_chime_sdk_messaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

