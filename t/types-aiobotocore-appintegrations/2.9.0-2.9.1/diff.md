# Comparing `tmp/types-aiobotocore-appintegrations-2.9.0.tar.gz` & `tmp/types-aiobotocore-appintegrations-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-appintegrations-2.9.0.tar", last modified: Wed Dec 13 19:58:34 2023, max compression
+gzip compressed data, was "types-aiobotocore-appintegrations-2.9.1.tar", last modified: Thu Jan 18 01:20:02 2024, max compression
```

## Comparing `types-aiobotocore-appintegrations-2.9.0.tar` & `types-aiobotocore-appintegrations-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:34.606095 types-aiobotocore-appintegrations-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:41:03.000000 types-aiobotocore-appintegrations-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14316 2023-12-13 19:58:34.606095 types-aiobotocore-appintegrations-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12714 2023-12-13 19:41:03.000000 types-aiobotocore-appintegrations-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:34.606095 types-aiobotocore-appintegrations-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2023-12-13 19:41:03.000000 types-aiobotocore-appintegrations-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:34.606095 types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2023-12-13 19:41:03.000000 types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2023-12-13 19:41:03.000000 types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      978 2023-12-13 19:41:03.000000 types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19869 2023-12-13 19:41:03.000000 types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    19865 2023-12-13 19:41:03.000000 types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9256 2023-12-13 19:41:04.000000 types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9254 2023-12-13 19:41:04.000000 types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7282 2023-12-13 19:41:03.000000 types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7275 2023-12-13 19:41:03.000000 types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:41:03.000000 types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    15756 2023-12-13 19:41:05.000000 types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15755 2023-12-13 19:41:04.000000 types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:41:03.000000 types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:34.606095 types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14316 2023-12-13 19:58:34.000000 types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      965 2023-12-13 19:58:34.000000 types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:34.000000 types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:34.000000 types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:34.000000 types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-13 19:58:34.000000 types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:02.709516 types-aiobotocore-appintegrations-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:03:02.000000 types-aiobotocore-appintegrations-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14336 2024-01-18 01:20:02.709516 types-aiobotocore-appintegrations-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12714 2024-01-18 01:03:02.000000 types-aiobotocore-appintegrations-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:02.709516 types-aiobotocore-appintegrations-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-01-18 01:03:02.000000 types-aiobotocore-appintegrations-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:02.709516 types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-01-18 01:03:02.000000 types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-01-18 01:03:02.000000 types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-01-18 01:03:02.000000 types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19872 2024-01-18 01:03:03.000000 types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19869 2024-01-18 01:03:03.000000 types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9254 2024-01-18 01:03:03.000000 types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9254 2024-01-18 01:03:03.000000 types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7281 2024-01-18 01:03:03.000000 types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-01-18 01:03:03.000000 types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:03:02.000000 types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    15755 2024-01-18 01:03:03.000000 types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15755 2024-01-18 01:03:03.000000 types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:03:02.000000 types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:02.709516 types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14336 2024-01-18 01:20:02.000000 types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-01-18 01:20:02.000000 types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:02.000000 types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:02.000000 types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:02.000000 types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-01-18 01:20:02.000000 types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-appintegrations-2.9.0/LICENSE` & `types-aiobotocore-appintegrations-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-appintegrations-2.9.0/PKG-INFO` & `types-aiobotocore-appintegrations-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appintegrations
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AppIntegrationsService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AppIntegrationsService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/
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
 
 <a id="types-aiobotocore-appintegrations"></a>
 
 # types-aiobotocore-appintegrations
 
 [![PyPI - types-aiobotocore-appintegrations](https://img.shields.io/pypi/v/types-aiobotocore-appintegrations.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appintegrations)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appintegrations.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appintegrations)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appintegrations)](https://pepy.tech/project/types-aiobotocore-appintegrations)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppIntegrationsService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
+[aiobotocore.AppIntegrationsService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
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
 [types-aiobotocore-appintegrations docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-appintegrations-2.9.0/README.md` & `types-aiobotocore-appintegrations-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appintegrations.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appintegrations)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appintegrations)](https://pepy.tech/project/types-aiobotocore-appintegrations)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppIntegrationsService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
+[aiobotocore.AppIntegrationsService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
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
 [types-aiobotocore-appintegrations docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-appintegrations-2.9.0/setup.py` & `types-aiobotocore-appintegrations-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-appintegrations",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_appintegrations"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.AppIntegrationsService 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.AppIntegrationsService 2.9.1 service generated with"
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
     keywords="aiobotocore appintegrations type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_appintegrations": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations/__init__.py` & `types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     ListDataIntegrationsPaginator,
     ListEventIntegrationAssociationsPaginator,
     ListEventIntegrationsPaginator,
 )
 
 Client = AppIntegrationsServiceClient
 
-
 __all__ = (
     "AppIntegrationsServiceClient",
     "Client",
     "ListApplicationsPaginator",
     "ListDataIntegrationAssociationsPaginator",
     "ListDataIntegrationsPaginator",
     "ListEventIntegrationAssociationsPaginator",
```

### Comparing `types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations/__init__.pyi` & `types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations/__main__.py` & `types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AppIntegrationsService 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.AppIntegrationsService 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService\nOther"
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

### Comparing `types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations/client.py` & `types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("AppIntegrationsServiceClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -116,15 +115,15 @@
         Name: str,
         Namespace: str,
         ApplicationSourceConfig: ApplicationSourceConfigTypeDef,
         Description: str = ...,
         Subscriptions: Sequence[SubscriptionTypeDef] = ...,
         Publications: Sequence[PublicationTypeDef] = ...,
         ClientToken: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateApplicationResponseTypeDef:
         """
         This API is in preview release and subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/client/#create_application)
         """
@@ -136,15 +135,15 @@
         KmsKey: str,
         SourceURI: str,
         Description: str = ...,
         ScheduleConfig: ScheduleConfigurationTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         ClientToken: str = ...,
         FileConfiguration: FileConfigurationTypeDef = ...,
-        ObjectConfiguration: Mapping[str, Mapping[str, Sequence[str]]] = ...
+        ObjectConfiguration: Mapping[str, Mapping[str, Sequence[str]]] = ...,
     ) -> CreateDataIntegrationResponseTypeDef:
         """
         Creates and persists a DataIntegration resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService.Client.create_data_integration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/client/#create_data_integration)
         """
@@ -153,15 +152,15 @@
         self,
         *,
         Name: str,
         EventFilter: EventFilterTypeDef,
         EventBridgeBus: str,
         Description: str = ...,
         ClientToken: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateEventIntegrationResponseTypeDef:
         """
         Creates an EventIntegration, given a specified name, description, and a
         reference to an Amazon EventBridge bus in your account and a partner event
         source that pushes events to that
         bus.
 
@@ -303,15 +302,15 @@
         self,
         *,
         Arn: str,
         Name: str = ...,
         Description: str = ...,
         ApplicationSourceConfig: ApplicationSourceConfigTypeDef = ...,
         Subscriptions: Sequence[SubscriptionTypeDef] = ...,
-        Publications: Sequence[PublicationTypeDef] = ...
+        Publications: Sequence[PublicationTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         This API is in preview release and subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService.Client.update_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/client/#update_application)
         """
```

### Comparing `types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations/client.pyi` & `types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         Name: str,
         Namespace: str,
         ApplicationSourceConfig: ApplicationSourceConfigTypeDef,
         Description: str = ...,
         Subscriptions: Sequence[SubscriptionTypeDef] = ...,
         Publications: Sequence[PublicationTypeDef] = ...,
         ClientToken: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateApplicationResponseTypeDef:
         """
         This API is in preview release and subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/client/#create_application)
         """
@@ -132,15 +132,15 @@
         KmsKey: str,
         SourceURI: str,
         Description: str = ...,
         ScheduleConfig: ScheduleConfigurationTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         ClientToken: str = ...,
         FileConfiguration: FileConfigurationTypeDef = ...,
-        ObjectConfiguration: Mapping[str, Mapping[str, Sequence[str]]] = ...
+        ObjectConfiguration: Mapping[str, Mapping[str, Sequence[str]]] = ...,
     ) -> CreateDataIntegrationResponseTypeDef:
         """
         Creates and persists a DataIntegration resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService.Client.create_data_integration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/client/#create_data_integration)
         """
@@ -149,15 +149,15 @@
         self,
         *,
         Name: str,
         EventFilter: EventFilterTypeDef,
         EventBridgeBus: str,
         Description: str = ...,
         ClientToken: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateEventIntegrationResponseTypeDef:
         """
         Creates an EventIntegration, given a specified name, description, and a
         reference to an Amazon EventBridge bus in your account and a partner event
         source that pushes events to that
         bus.
 
@@ -299,15 +299,15 @@
         self,
         *,
         Arn: str,
         Name: str = ...,
         Description: str = ...,
         ApplicationSourceConfig: ApplicationSourceConfigTypeDef = ...,
         Subscriptions: Sequence[SubscriptionTypeDef] = ...,
-        Publications: Sequence[PublicationTypeDef] = ...
+        Publications: Sequence[PublicationTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         This API is in preview release and subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService.Client.update_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/client/#update_application)
         """
```

### Comparing `types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations/literals.py` & `types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,29 +15,27 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListApplicationsPaginatorName",
     "ListDataIntegrationAssociationsPaginatorName",
     "ListDataIntegrationsPaginatorName",
     "ListEventIntegrationAssociationsPaginatorName",
     "ListEventIntegrationsPaginatorName",
     "AppIntegrationsServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ListApplicationsPaginatorName = Literal["list_applications"]
 ListDataIntegrationAssociationsPaginatorName = Literal["list_data_integration_associations"]
 ListDataIntegrationsPaginatorName = Literal["list_data_integrations"]
 ListEventIntegrationAssociationsPaginatorName = Literal["list_event_integration_associations"]
 ListEventIntegrationsPaginatorName = Literal["list_event_integrations"]
 AppIntegrationsServiceServiceName = Literal["appintegrations"]
 ServiceName = Literal[
```

### Comparing `types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations/literals.pyi` & `types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations/paginator.py` & `types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     "ListApplicationsPaginator",
     "ListDataIntegrationAssociationsPaginator",
     "ListDataIntegrationsPaginator",
     "ListEventIntegrationAssociationsPaginator",
     "ListEventIntegrationsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations/paginator.pyi` & `types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations/type_defs.py` & `types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ExternalUrlConfigTypeDef",
     "ApplicationSummaryTypeDef",
     "PublicationTypeDef",
     "SubscriptionTypeDef",
     "ResponseMetadataTypeDef",
     "FileConfigurationTypeDef",
```

### Comparing `types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations/type_defs.pyi` & `types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations.egg-info/PKG-INFO` & `types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appintegrations
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AppIntegrationsService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AppIntegrationsService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/
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
 
 <a id="types-aiobotocore-appintegrations"></a>
 
 # types-aiobotocore-appintegrations
 
 [![PyPI - types-aiobotocore-appintegrations](https://img.shields.io/pypi/v/types-aiobotocore-appintegrations.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appintegrations)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appintegrations.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appintegrations)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appintegrations)](https://pepy.tech/project/types-aiobotocore-appintegrations)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppIntegrationsService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
+[aiobotocore.AppIntegrationsService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
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
 [types-aiobotocore-appintegrations docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-appintegrations-2.9.0/types_aiobotocore_appintegrations.egg-info/SOURCES.txt` & `types-aiobotocore-appintegrations-2.9.1/types_aiobotocore_appintegrations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

