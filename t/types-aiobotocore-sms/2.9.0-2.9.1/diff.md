# Comparing `tmp/types-aiobotocore-sms-2.9.0.tar.gz` & `tmp/types-aiobotocore-sms-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sms-2.9.0.tar", last modified: Wed Dec 13 20:00:32 2023, max compression
+gzip compressed data, was "types-aiobotocore-sms-2.9.1.tar", last modified: Thu Jan 18 01:21:51 2024, max compression
```

## Comparing `types-aiobotocore-sms-2.9.0.tar` & `types-aiobotocore-sms-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:32.865117 types-aiobotocore-sms-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:56:35.000000 types-aiobotocore-sms-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13261 2023-12-13 20:00:32.865117 types-aiobotocore-sms-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11714 2023-12-13 19:56:35.000000 types-aiobotocore-sms-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:32.865117 types-aiobotocore-sms-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-12-13 19:56:35.000000 types-aiobotocore-sms-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:32.865117 types-aiobotocore-sms-2.9.0/types_aiobotocore_sms/
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2023-12-13 19:56:35.000000 types-aiobotocore-sms-2.9.0/types_aiobotocore_sms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2023-12-13 19:56:35.000000 types-aiobotocore-sms-2.9.0/types_aiobotocore_sms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-13 19:56:35.000000 types-aiobotocore-sms-2.9.0/types_aiobotocore_sms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27781 2023-12-13 19:56:35.000000 types-aiobotocore-sms-2.9.0/types_aiobotocore_sms/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    27777 2023-12-13 19:56:35.000000 types-aiobotocore-sms-2.9.0/types_aiobotocore_sms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11549 2023-12-13 19:56:35.000000 types-aiobotocore-sms-2.9.0/types_aiobotocore_sms/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11547 2023-12-13 19:56:35.000000 types-aiobotocore-sms-2.9.0/types_aiobotocore_sms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6255 2023-12-13 19:56:35.000000 types-aiobotocore-sms-2.9.0/types_aiobotocore_sms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6248 2023-12-13 19:56:35.000000 types-aiobotocore-sms-2.9.0/types_aiobotocore_sms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:56:35.000000 types-aiobotocore-sms-2.9.0/types_aiobotocore_sms/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    27570 2023-12-13 19:56:36.000000 types-aiobotocore-sms-2.9.0/types_aiobotocore_sms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    27569 2023-12-13 19:56:35.000000 types-aiobotocore-sms-2.9.0/types_aiobotocore_sms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:56:35.000000 types-aiobotocore-sms-2.9.0/types_aiobotocore_sms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:32.865117 types-aiobotocore-sms-2.9.0/types_aiobotocore_sms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13261 2023-12-13 20:00:32.000000 types-aiobotocore-sms-2.9.0/types_aiobotocore_sms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      737 2023-12-13 20:00:32.000000 types-aiobotocore-sms-2.9.0/types_aiobotocore_sms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:32.000000 types-aiobotocore-sms-2.9.0/types_aiobotocore_sms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:32.000000 types-aiobotocore-sms-2.9.0/types_aiobotocore_sms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:32.000000 types-aiobotocore-sms-2.9.0/types_aiobotocore_sms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 20:00:32.000000 types-aiobotocore-sms-2.9.0/types_aiobotocore_sms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:51.049024 types-aiobotocore-sms-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:18:07.000000 types-aiobotocore-sms-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13281 2024-01-18 01:21:51.049024 types-aiobotocore-sms-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11714 2024-01-18 01:18:07.000000 types-aiobotocore-sms-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:51.049024 types-aiobotocore-sms-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-01-18 01:18:06.000000 types-aiobotocore-sms-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:51.049024 types-aiobotocore-sms-2.9.1/types_aiobotocore_sms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-01-18 01:18:07.000000 types-aiobotocore-sms-2.9.1/types_aiobotocore_sms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-01-18 01:18:07.000000 types-aiobotocore-sms-2.9.1/types_aiobotocore_sms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-18 01:18:07.000000 types-aiobotocore-sms-2.9.1/types_aiobotocore_sms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27789 2024-01-18 01:18:07.000000 types-aiobotocore-sms-2.9.1/types_aiobotocore_sms/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27786 2024-01-18 01:18:07.000000 types-aiobotocore-sms-2.9.1/types_aiobotocore_sms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11547 2024-01-18 01:18:07.000000 types-aiobotocore-sms-2.9.1/types_aiobotocore_sms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11547 2024-01-18 01:18:07.000000 types-aiobotocore-sms-2.9.1/types_aiobotocore_sms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-01-18 01:18:07.000000 types-aiobotocore-sms-2.9.1/types_aiobotocore_sms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6249 2024-01-18 01:18:07.000000 types-aiobotocore-sms-2.9.1/types_aiobotocore_sms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:18:07.000000 types-aiobotocore-sms-2.9.1/types_aiobotocore_sms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    27569 2024-01-18 01:18:07.000000 types-aiobotocore-sms-2.9.1/types_aiobotocore_sms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27569 2024-01-18 01:18:07.000000 types-aiobotocore-sms-2.9.1/types_aiobotocore_sms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:18:07.000000 types-aiobotocore-sms-2.9.1/types_aiobotocore_sms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:51.049024 types-aiobotocore-sms-2.9.1/types_aiobotocore_sms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13281 2024-01-18 01:21:51.000000 types-aiobotocore-sms-2.9.1/types_aiobotocore_sms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-01-18 01:21:51.000000 types-aiobotocore-sms-2.9.1/types_aiobotocore_sms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:51.000000 types-aiobotocore-sms-2.9.1/types_aiobotocore_sms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:51.000000 types-aiobotocore-sms-2.9.1/types_aiobotocore_sms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:51.000000 types-aiobotocore-sms-2.9.1/types_aiobotocore_sms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:21:51.000000 types-aiobotocore-sms-2.9.1/types_aiobotocore_sms.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sms-2.9.0/LICENSE` & `types-aiobotocore-sms-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-sms-2.9.0/PKG-INFO` & `types-aiobotocore-sms-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sms
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SMS 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SMS 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/
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
 
 <a id="types-aiobotocore-sms"></a>
 
 # types-aiobotocore-sms
 
 [![PyPI - types-aiobotocore-sms](https://img.shields.io/pypi/v/types-aiobotocore-sms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sms)](https://pepy.tech/project/types-aiobotocore-sms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SMS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
+[aiobotocore.SMS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
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
 [types-aiobotocore-sms docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-sms-2.9.0/README.md` & `types-aiobotocore-sms-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sms)](https://pepy.tech/project/types-aiobotocore-sms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SMS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
+[aiobotocore.SMS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
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
 [types-aiobotocore-sms docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-sms-2.9.0/setup.py` & `types-aiobotocore-sms-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sms",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_sms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SMS 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.SMS 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore sms type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_sms": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-sms-2.9.0/types_aiobotocore_sms/__init__.py` & `types-aiobotocore-sms-2.9.1/types_aiobotocore_sms/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     GetReplicationRunsPaginator,
     GetServersPaginator,
     ListAppsPaginator,
 )
 
 Client = SMSClient
 
-
 __all__ = (
     "Client",
     "GetConnectorsPaginator",
     "GetReplicationJobsPaginator",
     "GetReplicationRunsPaginator",
     "GetServersPaginator",
     "ListAppsPaginator",
```

### Comparing `types-aiobotocore-sms-2.9.0/types_aiobotocore_sms/__init__.pyi` & `types-aiobotocore-sms-2.9.1/types_aiobotocore_sms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sms-2.9.0/types_aiobotocore_sms/__main__.py` & `types-aiobotocore-sms-2.9.1/types_aiobotocore_sms/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SMS 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.SMS 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS\nOther"
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

### Comparing `types-aiobotocore-sms-2.9.0/types_aiobotocore_sms/client.py` & `types-aiobotocore-sms-2.9.1/types_aiobotocore_sms/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SMSClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -127,15 +126,15 @@
         self,
         *,
         name: str = ...,
         description: str = ...,
         roleName: str = ...,
         clientToken: str = ...,
         serverGroups: Sequence[ServerGroupTypeDef] = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAppResponseTypeDef:
         """
         Creates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.create_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#create_app)
         """
@@ -148,29 +147,29 @@
         frequency: int = ...,
         runOnce: bool = ...,
         licenseType: LicenseTypeType = ...,
         roleName: str = ...,
         description: str = ...,
         numberOfRecentAmisToKeep: int = ...,
         encrypted: bool = ...,
-        kmsKeyId: str = ...
+        kmsKeyId: str = ...,
     ) -> CreateReplicationJobResponseTypeDef:
         """
         Creates a replication job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.create_replication_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#create_replication_job)
         """
 
     async def delete_app(
         self,
         *,
         appId: str = ...,
         forceStopAppReplication: bool = ...,
-        forceTerminateApp: bool = ...
+        forceTerminateApp: bool = ...,
     ) -> Dict[str, Any]:
         """
         Deletes the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.delete_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#delete_app)
         """
@@ -343,15 +342,15 @@
         """
 
     async def get_servers(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
-        vmServerAddressList: Sequence[VmServerAddressTypeDef] = ...
+        vmServerAddressList: Sequence[VmServerAddressTypeDef] = ...,
     ) -> GetServersResponseTypeDef:
         """
         Describes the servers in your server catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.get_servers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#get_servers)
         """
@@ -404,30 +403,30 @@
 
     async def put_app_launch_configuration(
         self,
         *,
         appId: str = ...,
         roleName: str = ...,
         autoLaunch: bool = ...,
-        serverGroupLaunchConfigurations: Sequence[ServerGroupLaunchConfigurationTypeDef] = ...
+        serverGroupLaunchConfigurations: Sequence[ServerGroupLaunchConfigurationTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates or updates the launch configuration for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.put_app_launch_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#put_app_launch_configuration)
         """
 
     async def put_app_replication_configuration(
         self,
         *,
         appId: str = ...,
         serverGroupReplicationConfigurations: Sequence[
             ServerGroupReplicationConfigurationTypeDef
-        ] = ...
+        ] = ...,
     ) -> Dict[str, Any]:
         """
         Creates or updates the replication configuration for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.put_app_replication_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#put_app_replication_configuration)
         """
@@ -435,15 +434,15 @@
     async def put_app_validation_configuration(
         self,
         *,
         appId: str,
         appValidationConfigurations: Sequence[AppValidationConfigurationTypeDef] = ...,
         serverGroupValidationConfigurations: Sequence[
             ServerGroupValidationConfigurationTypeDef
-        ] = ...
+        ] = ...,
     ) -> Dict[str, Any]:
         """
         Creates or updates a validation configuration for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.put_app_validation_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#put_app_validation_configuration)
         """
@@ -500,15 +499,15 @@
         self,
         *,
         appId: str = ...,
         name: str = ...,
         description: str = ...,
         roleName: str = ...,
         serverGroups: Sequence[ServerGroupTypeDef] = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> UpdateAppResponseTypeDef:
         """
         Updates the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.update_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#update_app)
         """
@@ -520,15 +519,15 @@
         frequency: int = ...,
         nextReplicationRunStartTime: TimestampTypeDef = ...,
         licenseType: LicenseTypeType = ...,
         roleName: str = ...,
         description: str = ...,
         numberOfRecentAmisToKeep: int = ...,
         encrypted: bool = ...,
-        kmsKeyId: str = ...
+        kmsKeyId: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the specified settings for the specified replication job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.update_replication_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#update_replication_job)
         """
```

### Comparing `types-aiobotocore-sms-2.9.0/types_aiobotocore_sms/client.pyi` & `types-aiobotocore-sms-2.9.1/types_aiobotocore_sms/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         self,
         *,
         name: str = ...,
         description: str = ...,
         roleName: str = ...,
         clientToken: str = ...,
         serverGroups: Sequence[ServerGroupTypeDef] = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAppResponseTypeDef:
         """
         Creates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.create_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#create_app)
         """
@@ -144,29 +144,29 @@
         frequency: int = ...,
         runOnce: bool = ...,
         licenseType: LicenseTypeType = ...,
         roleName: str = ...,
         description: str = ...,
         numberOfRecentAmisToKeep: int = ...,
         encrypted: bool = ...,
-        kmsKeyId: str = ...
+        kmsKeyId: str = ...,
     ) -> CreateReplicationJobResponseTypeDef:
         """
         Creates a replication job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.create_replication_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#create_replication_job)
         """
 
     async def delete_app(
         self,
         *,
         appId: str = ...,
         forceStopAppReplication: bool = ...,
-        forceTerminateApp: bool = ...
+        forceTerminateApp: bool = ...,
     ) -> Dict[str, Any]:
         """
         Deletes the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.delete_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#delete_app)
         """
@@ -339,15 +339,15 @@
         """
 
     async def get_servers(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
-        vmServerAddressList: Sequence[VmServerAddressTypeDef] = ...
+        vmServerAddressList: Sequence[VmServerAddressTypeDef] = ...,
     ) -> GetServersResponseTypeDef:
         """
         Describes the servers in your server catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.get_servers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#get_servers)
         """
@@ -400,30 +400,30 @@
 
     async def put_app_launch_configuration(
         self,
         *,
         appId: str = ...,
         roleName: str = ...,
         autoLaunch: bool = ...,
-        serverGroupLaunchConfigurations: Sequence[ServerGroupLaunchConfigurationTypeDef] = ...
+        serverGroupLaunchConfigurations: Sequence[ServerGroupLaunchConfigurationTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates or updates the launch configuration for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.put_app_launch_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#put_app_launch_configuration)
         """
 
     async def put_app_replication_configuration(
         self,
         *,
         appId: str = ...,
         serverGroupReplicationConfigurations: Sequence[
             ServerGroupReplicationConfigurationTypeDef
-        ] = ...
+        ] = ...,
     ) -> Dict[str, Any]:
         """
         Creates or updates the replication configuration for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.put_app_replication_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#put_app_replication_configuration)
         """
@@ -431,15 +431,15 @@
     async def put_app_validation_configuration(
         self,
         *,
         appId: str,
         appValidationConfigurations: Sequence[AppValidationConfigurationTypeDef] = ...,
         serverGroupValidationConfigurations: Sequence[
             ServerGroupValidationConfigurationTypeDef
-        ] = ...
+        ] = ...,
     ) -> Dict[str, Any]:
         """
         Creates or updates a validation configuration for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.put_app_validation_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#put_app_validation_configuration)
         """
@@ -496,15 +496,15 @@
         self,
         *,
         appId: str = ...,
         name: str = ...,
         description: str = ...,
         roleName: str = ...,
         serverGroups: Sequence[ServerGroupTypeDef] = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> UpdateAppResponseTypeDef:
         """
         Updates the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.update_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#update_app)
         """
@@ -516,15 +516,15 @@
         frequency: int = ...,
         nextReplicationRunStartTime: TimestampTypeDef = ...,
         licenseType: LicenseTypeType = ...,
         roleName: str = ...,
         description: str = ...,
         numberOfRecentAmisToKeep: int = ...,
         encrypted: bool = ...,
-        kmsKeyId: str = ...
+        kmsKeyId: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the specified settings for the specified replication job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.update_replication_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#update_replication_job)
         """
```

### Comparing `types-aiobotocore-sms-2.9.0/types_aiobotocore_sms/literals.py` & `types-aiobotocore-sms-2.9.1/types_aiobotocore_sms/literals.py`

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
     "AppLaunchConfigurationStatusType",
     "AppLaunchStatusType",
     "AppReplicationConfigurationStatusType",
     "AppReplicationStatusType",
     "AppStatusType",
     "AppValidationStrategyType",
@@ -48,15 +47,14 @@
     "SMSServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AppLaunchConfigurationStatusType = Literal["CONFIGURED", "NOT_CONFIGURED"]
 AppLaunchStatusType = Literal[
     "CONFIGURATION_INVALID",
     "CONFIGURATION_IN_PROGRESS",
     "DELTA_LAUNCH_FAILED",
     "DELTA_LAUNCH_IN_PROGRESS",
     "LAUNCHED",
```

### Comparing `types-aiobotocore-sms-2.9.0/types_aiobotocore_sms/literals.pyi` & `types-aiobotocore-sms-2.9.1/types_aiobotocore_sms/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sms-2.9.0/types_aiobotocore_sms/paginator.py` & `types-aiobotocore-sms-2.9.1/types_aiobotocore_sms/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,14 @@
     "GetConnectorsPaginator",
     "GetReplicationJobsPaginator",
     "GetReplicationRunsPaginator",
     "GetServersPaginator",
     "ListAppsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -114,15 +113,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/paginators/#getserverspaginator)
     """
 
     def paginate(
         self,
         *,
         vmServerAddressList: Sequence[VmServerAddressTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetServers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/paginators/#getserverspaginator)
         """
```

### Comparing `types-aiobotocore-sms-2.9.0/types_aiobotocore_sms/paginator.pyi` & `types-aiobotocore-sms-2.9.1/types_aiobotocore_sms/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/paginators/#getserverspaginator)
     """
 
     def paginate(
         self,
         *,
         vmServerAddressList: Sequence[VmServerAddressTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetServers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/paginators/#getserverspaginator)
         """
 
 class ListAppsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-sms-2.9.0/types_aiobotocore_sms/type_defs.py` & `types-aiobotocore-sms-2.9.1/types_aiobotocore_sms/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "LaunchDetailsTypeDef",
     "ConnectorTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "TimestampTypeDef",
     "DeleteAppLaunchConfigurationRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-sms-2.9.0/types_aiobotocore_sms/type_defs.pyi` & `types-aiobotocore-sms-2.9.1/types_aiobotocore_sms/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sms-2.9.0/types_aiobotocore_sms.egg-info/PKG-INFO` & `types-aiobotocore-sms-2.9.1/types_aiobotocore_sms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sms
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SMS 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SMS 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/
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
 
 <a id="types-aiobotocore-sms"></a>
 
 # types-aiobotocore-sms
 
 [![PyPI - types-aiobotocore-sms](https://img.shields.io/pypi/v/types-aiobotocore-sms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sms)](https://pepy.tech/project/types-aiobotocore-sms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SMS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
+[aiobotocore.SMS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
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
 [types-aiobotocore-sms docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-sms-2.9.0/types_aiobotocore_sms.egg-info/SOURCES.txt` & `types-aiobotocore-sms-2.9.1/types_aiobotocore_sms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

