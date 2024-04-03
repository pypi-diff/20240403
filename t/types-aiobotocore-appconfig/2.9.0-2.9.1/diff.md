# Comparing `tmp/types-aiobotocore-appconfig-2.9.0.tar.gz` & `tmp/types-aiobotocore-appconfig-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-appconfig-2.9.0.tar", last modified: Wed Dec 13 19:58:33 2023, max compression
+gzip compressed data, was "types-aiobotocore-appconfig-2.9.1.tar", last modified: Thu Jan 18 01:20:01 2024, max compression
```

## Comparing `types-aiobotocore-appconfig-2.9.0.tar` & `types-aiobotocore-appconfig-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:33.130108 types-aiobotocore-appconfig-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:40:57.000000 types-aiobotocore-appconfig-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14263 2023-12-13 19:58:33.130108 types-aiobotocore-appconfig-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12692 2023-12-13 19:40:57.000000 types-aiobotocore-appconfig-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:33.130108 types-aiobotocore-appconfig-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2023-12-13 19:40:57.000000 types-aiobotocore-appconfig-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:33.130108 types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig/
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2023-12-13 19:40:57.000000 types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2023-12-13 19:40:57.000000 types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-12-13 19:40:57.000000 types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35224 2023-12-13 19:40:57.000000 types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    35220 2023-12-13 19:40:57.000000 types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10971 2023-12-13 19:40:58.000000 types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10969 2023-12-13 19:40:57.000000 types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10379 2023-12-13 19:40:57.000000 types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10369 2023-12-13 19:40:57.000000 types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:40:57.000000 types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    28650 2023-12-13 19:40:58.000000 types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    28649 2023-12-13 19:40:58.000000 types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:40:57.000000 types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:33.130108 types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14263 2023-12-13 19:58:33.000000 types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-12-13 19:58:33.000000 types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:33.000000 types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:33.000000 types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:33.000000 types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-13 19:58:33.000000 types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:01.353522 types-aiobotocore-appconfig-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:02:56.000000 types-aiobotocore-appconfig-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14283 2024-01-18 01:20:01.353522 types-aiobotocore-appconfig-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12692 2024-01-18 01:02:56.000000 types-aiobotocore-appconfig-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:01.353522 types-aiobotocore-appconfig-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-01-18 01:02:56.000000 types-aiobotocore-appconfig-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:01.349522 types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig/
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-01-18 01:02:56.000000 types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-01-18 01:02:56.000000 types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-01-18 01:02:56.000000 types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35237 2024-01-18 01:02:57.000000 types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35234 2024-01-18 01:02:57.000000 types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10969 2024-01-18 01:02:57.000000 types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10969 2024-01-18 01:02:57.000000 types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-01-18 01:02:57.000000 types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-01-18 01:02:57.000000 types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:02:56.000000 types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    28649 2024-01-18 01:02:58.000000 types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28649 2024-01-18 01:02:57.000000 types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:02:56.000000 types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:01.349522 types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14283 2024-01-18 01:20:01.000000 types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-01-18 01:20:01.000000 types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:01.000000 types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:01.000000 types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:01.000000 types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-18 01:20:01.000000 types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-appconfig-2.9.0/LICENSE` & `types-aiobotocore-appconfig-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-appconfig-2.9.0/PKG-INFO` & `types-aiobotocore-appconfig-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appconfig
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AppConfig 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AppConfig 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/
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
 
 <a id="types-aiobotocore-appconfig"></a>
 
 # types-aiobotocore-appconfig
 
 [![PyPI - types-aiobotocore-appconfig](https://img.shields.io/pypi/v/types-aiobotocore-appconfig.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appconfig)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appconfig.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appconfig)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appconfig)](https://pepy.tech/project/types-aiobotocore-appconfig)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppConfig 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
+[aiobotocore.AppConfig 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
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
 [types-aiobotocore-appconfig docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-appconfig-2.9.0/README.md` & `types-aiobotocore-appconfig-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appconfig.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appconfig)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appconfig)](https://pepy.tech/project/types-aiobotocore-appconfig)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppConfig 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
+[aiobotocore.AppConfig 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
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
 [types-aiobotocore-appconfig docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-appconfig-2.9.0/setup.py` & `types-aiobotocore-appconfig-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-appconfig",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_appconfig"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.AppConfig 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.AppConfig 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore appconfig type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_appconfig": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig/__init__.py` & `types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     ListExtensionAssociationsPaginator,
     ListExtensionsPaginator,
     ListHostedConfigurationVersionsPaginator,
 )
 
 Client = AppConfigClient
 
-
 __all__ = (
     "AppConfigClient",
     "Client",
     "ListApplicationsPaginator",
     "ListConfigurationProfilesPaginator",
     "ListDeploymentStrategiesPaginator",
     "ListDeploymentsPaginator",
```

### Comparing `types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig/__init__.pyi` & `types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig/__main__.py` & `types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AppConfig 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.AppConfig 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig\nOther"
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

### Comparing `types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig/client.py` & `types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("AppConfigClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -136,15 +135,15 @@
         Name: str,
         LocationUri: str,
         Description: str = ...,
         RetrievalRoleArn: str = ...,
         Validators: Sequence[ValidatorTypeDef] = ...,
         Tags: Mapping[str, str] = ...,
         Type: str = ...,
-        KmsKeyIdentifier: str = ...
+        KmsKeyIdentifier: str = ...,
     ) -> ConfigurationProfileTypeDef:
         """
         Creates a configuration profile, which is information that enables AppConfig to
         access the configuration
         source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.create_configuration_profile)
@@ -157,15 +156,15 @@
         Name: str,
         DeploymentDurationInMinutes: int,
         GrowthFactor: float,
         Description: str = ...,
         FinalBakeTimeInMinutes: int = ...,
         GrowthType: GrowthTypeType = ...,
         ReplicateTo: ReplicateToType = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> DeploymentStrategyResponseTypeDef:
         """
         Creates a deployment strategy that defines important criteria for rolling out
         your configuration to the designated
         targets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.create_deployment_strategy)
@@ -175,15 +174,15 @@
     async def create_environment(
         self,
         *,
         ApplicationId: str,
         Name: str,
         Description: str = ...,
         Monitors: Sequence[MonitorTypeDef] = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> EnvironmentResponseTypeDef:
         """
         Creates an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.create_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#create_environment)
         """
@@ -192,15 +191,15 @@
         self,
         *,
         Name: str,
         Actions: Mapping[ActionPointType, Sequence[ActionTypeDef]],
         Description: str = ...,
         Parameters: Mapping[str, ParameterTypeDef] = ...,
         Tags: Mapping[str, str] = ...,
-        LatestVersionNumber: int = ...
+        LatestVersionNumber: int = ...,
     ) -> ExtensionTypeDef:
         """
         Creates an AppConfig extension.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.create_extension)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#create_extension)
         """
@@ -208,15 +207,15 @@
     async def create_extension_association(
         self,
         *,
         ExtensionIdentifier: str,
         ResourceIdentifier: str,
         ExtensionVersionNumber: int = ...,
         Parameters: Mapping[str, str] = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> ExtensionAssociationTypeDef:
         """
         When you create an extension or configure an Amazon Web Services authored
         extension, you associate the extension with an AppConfig application,
         environment, or configuration
         profile.
 
@@ -229,15 +228,15 @@
         *,
         ApplicationId: str,
         ConfigurationProfileId: str,
         Content: BlobTypeDef,
         ContentType: str,
         Description: str = ...,
         LatestVersionNumber: int = ...,
-        VersionLabel: str = ...
+        VersionLabel: str = ...,
     ) -> HostedConfigurationVersionTypeDef:
         """
         Creates a new configuration in the AppConfig hosted configuration store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.create_hosted_configuration_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#create_hosted_configuration_version)
         """
@@ -336,15 +335,15 @@
     async def get_configuration(
         self,
         *,
         Application: str,
         Environment: str,
         Configuration: str,
         ClientId: str,
-        ClientConfigurationVersion: str = ...
+        ClientConfigurationVersion: str = ...,
     ) -> ConfigurationTypeDef:
         """
         (Deprecated) Retrieves the latest deployed configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.get_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#get_configuration)
         """
@@ -472,15 +471,15 @@
     async def list_extension_associations(
         self,
         *,
         ResourceIdentifier: str = ...,
         ExtensionIdentifier: str = ...,
         ExtensionVersionNumber: int = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ExtensionAssociationsTypeDef:
         """
         Lists all AppConfig extension associations in the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.list_extension_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#list_extension_associations)
         """
@@ -499,15 +498,15 @@
     async def list_hosted_configuration_versions(
         self,
         *,
         ApplicationId: str,
         ConfigurationProfileId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        VersionLabel: str = ...
+        VersionLabel: str = ...,
     ) -> HostedConfigurationVersionsTypeDef:
         """
         Lists configurations stored in the AppConfig hosted configuration store by
         version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.list_hosted_configuration_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#list_hosted_configuration_versions)
@@ -527,15 +526,15 @@
         ApplicationId: str,
         EnvironmentId: str,
         DeploymentStrategyId: str,
         ConfigurationProfileId: str,
         ConfigurationVersion: str,
         Description: str = ...,
         Tags: Mapping[str, str] = ...,
-        KmsKeyIdentifier: str = ...
+        KmsKeyIdentifier: str = ...,
     ) -> DeploymentTypeDef:
         """
         Starts a deployment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.start_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#start_deployment)
         """
@@ -585,15 +584,15 @@
         *,
         ApplicationId: str,
         ConfigurationProfileId: str,
         Name: str = ...,
         Description: str = ...,
         RetrievalRoleArn: str = ...,
         Validators: Sequence[ValidatorTypeDef] = ...,
-        KmsKeyIdentifier: str = ...
+        KmsKeyIdentifier: str = ...,
     ) -> ConfigurationProfileTypeDef:
         """
         Updates a configuration profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.update_configuration_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#update_configuration_profile)
         """
@@ -602,15 +601,15 @@
         self,
         *,
         DeploymentStrategyId: str,
         Description: str = ...,
         DeploymentDurationInMinutes: int = ...,
         FinalBakeTimeInMinutes: int = ...,
         GrowthFactor: float = ...,
-        GrowthType: GrowthTypeType = ...
+        GrowthType: GrowthTypeType = ...,
     ) -> DeploymentStrategyResponseTypeDef:
         """
         Updates a deployment strategy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.update_deployment_strategy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#update_deployment_strategy)
         """
@@ -618,15 +617,15 @@
     async def update_environment(
         self,
         *,
         ApplicationId: str,
         EnvironmentId: str,
         Name: str = ...,
         Description: str = ...,
-        Monitors: Sequence[MonitorTypeDef] = ...
+        Monitors: Sequence[MonitorTypeDef] = ...,
     ) -> EnvironmentResponseTypeDef:
         """
         Updates an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.update_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#update_environment)
         """
@@ -634,15 +633,15 @@
     async def update_extension(
         self,
         *,
         ExtensionIdentifier: str,
         Description: str = ...,
         Actions: Mapping[ActionPointType, Sequence[ActionTypeDef]] = ...,
         Parameters: Mapping[str, ParameterTypeDef] = ...,
-        VersionNumber: int = ...
+        VersionNumber: int = ...,
     ) -> ExtensionTypeDef:
         """
         Updates an AppConfig extension.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.update_extension)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#update_extension)
         """
```

### Comparing `types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig/client.pyi` & `types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         Name: str,
         LocationUri: str,
         Description: str = ...,
         RetrievalRoleArn: str = ...,
         Validators: Sequence[ValidatorTypeDef] = ...,
         Tags: Mapping[str, str] = ...,
         Type: str = ...,
-        KmsKeyIdentifier: str = ...
+        KmsKeyIdentifier: str = ...,
     ) -> ConfigurationProfileTypeDef:
         """
         Creates a configuration profile, which is information that enables AppConfig to
         access the configuration
         source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.create_configuration_profile)
@@ -153,15 +153,15 @@
         Name: str,
         DeploymentDurationInMinutes: int,
         GrowthFactor: float,
         Description: str = ...,
         FinalBakeTimeInMinutes: int = ...,
         GrowthType: GrowthTypeType = ...,
         ReplicateTo: ReplicateToType = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> DeploymentStrategyResponseTypeDef:
         """
         Creates a deployment strategy that defines important criteria for rolling out
         your configuration to the designated
         targets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.create_deployment_strategy)
@@ -171,15 +171,15 @@
     async def create_environment(
         self,
         *,
         ApplicationId: str,
         Name: str,
         Description: str = ...,
         Monitors: Sequence[MonitorTypeDef] = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> EnvironmentResponseTypeDef:
         """
         Creates an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.create_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#create_environment)
         """
@@ -188,15 +188,15 @@
         self,
         *,
         Name: str,
         Actions: Mapping[ActionPointType, Sequence[ActionTypeDef]],
         Description: str = ...,
         Parameters: Mapping[str, ParameterTypeDef] = ...,
         Tags: Mapping[str, str] = ...,
-        LatestVersionNumber: int = ...
+        LatestVersionNumber: int = ...,
     ) -> ExtensionTypeDef:
         """
         Creates an AppConfig extension.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.create_extension)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#create_extension)
         """
@@ -204,15 +204,15 @@
     async def create_extension_association(
         self,
         *,
         ExtensionIdentifier: str,
         ResourceIdentifier: str,
         ExtensionVersionNumber: int = ...,
         Parameters: Mapping[str, str] = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> ExtensionAssociationTypeDef:
         """
         When you create an extension or configure an Amazon Web Services authored
         extension, you associate the extension with an AppConfig application,
         environment, or configuration
         profile.
 
@@ -225,15 +225,15 @@
         *,
         ApplicationId: str,
         ConfigurationProfileId: str,
         Content: BlobTypeDef,
         ContentType: str,
         Description: str = ...,
         LatestVersionNumber: int = ...,
-        VersionLabel: str = ...
+        VersionLabel: str = ...,
     ) -> HostedConfigurationVersionTypeDef:
         """
         Creates a new configuration in the AppConfig hosted configuration store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.create_hosted_configuration_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#create_hosted_configuration_version)
         """
@@ -332,15 +332,15 @@
     async def get_configuration(
         self,
         *,
         Application: str,
         Environment: str,
         Configuration: str,
         ClientId: str,
-        ClientConfigurationVersion: str = ...
+        ClientConfigurationVersion: str = ...,
     ) -> ConfigurationTypeDef:
         """
         (Deprecated) Retrieves the latest deployed configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.get_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#get_configuration)
         """
@@ -468,15 +468,15 @@
     async def list_extension_associations(
         self,
         *,
         ResourceIdentifier: str = ...,
         ExtensionIdentifier: str = ...,
         ExtensionVersionNumber: int = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ExtensionAssociationsTypeDef:
         """
         Lists all AppConfig extension associations in the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.list_extension_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#list_extension_associations)
         """
@@ -495,15 +495,15 @@
     async def list_hosted_configuration_versions(
         self,
         *,
         ApplicationId: str,
         ConfigurationProfileId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        VersionLabel: str = ...
+        VersionLabel: str = ...,
     ) -> HostedConfigurationVersionsTypeDef:
         """
         Lists configurations stored in the AppConfig hosted configuration store by
         version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.list_hosted_configuration_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#list_hosted_configuration_versions)
@@ -523,15 +523,15 @@
         ApplicationId: str,
         EnvironmentId: str,
         DeploymentStrategyId: str,
         ConfigurationProfileId: str,
         ConfigurationVersion: str,
         Description: str = ...,
         Tags: Mapping[str, str] = ...,
-        KmsKeyIdentifier: str = ...
+        KmsKeyIdentifier: str = ...,
     ) -> DeploymentTypeDef:
         """
         Starts a deployment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.start_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#start_deployment)
         """
@@ -581,15 +581,15 @@
         *,
         ApplicationId: str,
         ConfigurationProfileId: str,
         Name: str = ...,
         Description: str = ...,
         RetrievalRoleArn: str = ...,
         Validators: Sequence[ValidatorTypeDef] = ...,
-        KmsKeyIdentifier: str = ...
+        KmsKeyIdentifier: str = ...,
     ) -> ConfigurationProfileTypeDef:
         """
         Updates a configuration profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.update_configuration_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#update_configuration_profile)
         """
@@ -598,15 +598,15 @@
         self,
         *,
         DeploymentStrategyId: str,
         Description: str = ...,
         DeploymentDurationInMinutes: int = ...,
         FinalBakeTimeInMinutes: int = ...,
         GrowthFactor: float = ...,
-        GrowthType: GrowthTypeType = ...
+        GrowthType: GrowthTypeType = ...,
     ) -> DeploymentStrategyResponseTypeDef:
         """
         Updates a deployment strategy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.update_deployment_strategy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#update_deployment_strategy)
         """
@@ -614,15 +614,15 @@
     async def update_environment(
         self,
         *,
         ApplicationId: str,
         EnvironmentId: str,
         Name: str = ...,
         Description: str = ...,
-        Monitors: Sequence[MonitorTypeDef] = ...
+        Monitors: Sequence[MonitorTypeDef] = ...,
     ) -> EnvironmentResponseTypeDef:
         """
         Updates an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.update_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#update_environment)
         """
@@ -630,15 +630,15 @@
     async def update_extension(
         self,
         *,
         ExtensionIdentifier: str,
         Description: str = ...,
         Actions: Mapping[ActionPointType, Sequence[ActionTypeDef]] = ...,
         Parameters: Mapping[str, ParameterTypeDef] = ...,
-        VersionNumber: int = ...
+        VersionNumber: int = ...,
     ) -> ExtensionTypeDef:
         """
         Updates an AppConfig extension.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.update_extension)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/client/#update_extension)
         """
```

### Comparing `types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig/literals.py` & `types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig/literals.py`

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
     "ActionPointType",
     "DeploymentEventTypeType",
     "DeploymentStateType",
     "EnvironmentStateType",
     "GrowthTypeType",
     "ListApplicationsPaginatorName",
@@ -40,15 +39,14 @@
     "AppConfigServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ActionPointType = Literal[
     "ON_DEPLOYMENT_BAKING",
     "ON_DEPLOYMENT_COMPLETE",
     "ON_DEPLOYMENT_ROLLED_BACK",
     "ON_DEPLOYMENT_START",
     "ON_DEPLOYMENT_STEP",
     "PRE_CREATE_HOSTED_CONFIGURATION_VERSION",
```

### Comparing `types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig/literals.pyi` & `types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig/paginator.py` & `types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,14 @@
     "ListDeploymentsPaginator",
     "ListEnvironmentsPaginator",
     "ListExtensionAssociationsPaginator",
     "ListExtensionsPaginator",
     "ListHostedConfigurationVersionsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -126,15 +125,15 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationId: str,
         EnvironmentId: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DeploymentsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Paginator.ListDeployments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/paginators/#listdeploymentspaginator)
         """
 
 
@@ -161,15 +160,15 @@
 
     def paginate(
         self,
         *,
         ResourceIdentifier: str = ...,
         ExtensionIdentifier: str = ...,
         ExtensionVersionNumber: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ExtensionAssociationsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Paginator.ListExtensionAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/paginators/#listextensionassociationspaginator)
         """
 
 
@@ -196,13 +195,13 @@
 
     def paginate(
         self,
         *,
         ApplicationId: str,
         ConfigurationProfileId: str,
         VersionLabel: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[HostedConfigurationVersionsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Paginator.ListHostedConfigurationVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/paginators/#listhostedconfigurationversionspaginator)
         """
```

### Comparing `types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig/paginator.pyi` & `types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationId: str,
         EnvironmentId: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DeploymentsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Paginator.ListDeployments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/paginators/#listdeploymentspaginator)
         """
 
 class ListEnvironmentsPaginator(AioPaginator):
@@ -153,15 +153,15 @@
 
     def paginate(
         self,
         *,
         ResourceIdentifier: str = ...,
         ExtensionIdentifier: str = ...,
         ExtensionVersionNumber: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ExtensionAssociationsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Paginator.ListExtensionAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/paginators/#listextensionassociationspaginator)
         """
 
 class ListExtensionsPaginator(AioPaginator):
@@ -186,13 +186,13 @@
 
     def paginate(
         self,
         *,
         ApplicationId: str,
         ConfigurationProfileId: str,
         VersionLabel: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[HostedConfigurationVersionsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Paginator.ListHostedConfigurationVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/paginators/#listhostedconfigurationversionspaginator)
         """
```

### Comparing `types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig/type_defs.py` & `types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActionInvocationTypeDef",
     "ActionTypeDef",
     "ResponseMetadataTypeDef",
     "ApplicationTypeDef",
     "AppliedExtensionTypeDef",
     "BlobTypeDef",
```

### Comparing `types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig/type_defs.pyi` & `types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig.egg-info/PKG-INFO` & `types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appconfig
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AppConfig 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AppConfig 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/
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
 
 <a id="types-aiobotocore-appconfig"></a>
 
 # types-aiobotocore-appconfig
 
 [![PyPI - types-aiobotocore-appconfig](https://img.shields.io/pypi/v/types-aiobotocore-appconfig.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appconfig)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appconfig.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appconfig)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appconfig)](https://pepy.tech/project/types-aiobotocore-appconfig)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppConfig 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
+[aiobotocore.AppConfig 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
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
 [types-aiobotocore-appconfig docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-appconfig-2.9.0/types_aiobotocore_appconfig.egg-info/SOURCES.txt` & `types-aiobotocore-appconfig-2.9.1/types_aiobotocore_appconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

