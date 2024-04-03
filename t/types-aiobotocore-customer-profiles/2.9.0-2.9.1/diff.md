# Comparing `tmp/types-aiobotocore-customer-profiles-2.9.0.tar.gz` & `tmp/types-aiobotocore-customer-profiles-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-customer-profiles-2.9.0.tar", last modified: Wed Dec 13 19:59:02 2023, max compression
+gzip compressed data, was "types-aiobotocore-customer-profiles-2.9.1.tar", last modified: Thu Jan 18 01:20:28 2024, max compression
```

## Comparing `types-aiobotocore-customer-profiles-2.9.0.tar` & `types-aiobotocore-customer-profiles-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:02.713866 types-aiobotocore-customer-profiles-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:43:40.000000 types-aiobotocore-customer-profiles-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13585 2023-12-13 19:59:02.713866 types-aiobotocore-customer-profiles-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11983 2023-12-13 19:43:40.000000 types-aiobotocore-customer-profiles-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:02.713866 types-aiobotocore-customer-profiles-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2023-12-13 19:43:40.000000 types-aiobotocore-customer-profiles-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:02.713866 types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles/
--rw-r--r--   0 runner    (1001) docker     (127)      737 2023-12-13 19:43:40.000000 types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2023-12-13 19:43:40.000000 types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      970 2023-12-13 19:43:40.000000 types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43411 2023-12-13 19:43:40.000000 types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    43407 2023-12-13 19:43:40.000000 types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13551 2023-12-13 19:43:40.000000 types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13549 2023-12-13 19:43:40.000000 types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2023-12-13 19:43:40.000000 types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2023-12-13 19:43:40.000000 types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:43:40.000000 types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    56803 2023-12-13 19:43:41.000000 types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    56802 2023-12-13 19:43:41.000000 types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:43:40.000000 types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:02.713866 types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13585 2023-12-13 19:59:02.000000 types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2023-12-13 19:59:02.000000 types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:02.000000 types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:02.000000 types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:02.000000 types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-13 19:59:02.000000 types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:28.393406 types-aiobotocore-customer-profiles-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:05:35.000000 types-aiobotocore-customer-profiles-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13605 2024-01-18 01:20:28.393406 types-aiobotocore-customer-profiles-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11983 2024-01-18 01:05:35.000000 types-aiobotocore-customer-profiles-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:28.393406 types-aiobotocore-customer-profiles-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-01-18 01:05:35.000000 types-aiobotocore-customer-profiles-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:28.393406 types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-01-18 01:05:35.000000 types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-01-18 01:05:35.000000 types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-01-18 01:05:35.000000 types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43426 2024-01-18 01:05:35.000000 types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43423 2024-01-18 01:05:35.000000 types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13549 2024-01-18 01:05:35.000000 types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13549 2024-01-18 01:05:35.000000 types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-01-18 01:05:35.000000 types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-01-18 01:05:35.000000 types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:05:35.000000 types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    56802 2024-01-18 01:05:37.000000 types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56802 2024-01-18 01:05:36.000000 types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:05:35.000000 types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:28.393406 types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13605 2024-01-18 01:20:28.000000 types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-01-18 01:20:28.000000 types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:28.000000 types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:28.000000 types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:28.000000 types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-18 01:20:28.000000 types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-customer-profiles-2.9.0/LICENSE` & `types-aiobotocore-customer-profiles-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-customer-profiles-2.9.0/PKG-INFO` & `types-aiobotocore-customer-profiles-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-customer-profiles
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CustomerProfiles 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CustomerProfiles 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/
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
 
 <a id="types-aiobotocore-customer-profiles"></a>
 
 # types-aiobotocore-customer-profiles
 
 [![PyPI - types-aiobotocore-customer-profiles](https://img.shields.io/pypi/v/types-aiobotocore-customer-profiles.svg?color=blue)](https://pypi.org/project/types-aiobotocore-customer-profiles)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-customer-profiles.svg?color=blue)](https://pypi.org/project/types-aiobotocore-customer-profiles)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-customer-profiles)](https://pepy.tech/project/types-aiobotocore-customer-profiles)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CustomerProfiles 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
+[aiobotocore.CustomerProfiles 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
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
 [types-aiobotocore-customer-profiles docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-customer-profiles-2.9.0/README.md` & `types-aiobotocore-customer-profiles-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-customer-profiles.svg?color=blue)](https://pypi.org/project/types-aiobotocore-customer-profiles)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-customer-profiles)](https://pepy.tech/project/types-aiobotocore-customer-profiles)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CustomerProfiles 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
+[aiobotocore.CustomerProfiles 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
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
 [types-aiobotocore-customer-profiles docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-customer-profiles-2.9.0/setup.py` & `types-aiobotocore-customer-profiles-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-customer-profiles",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_customer_profiles"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CustomerProfiles 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.CustomerProfiles 2.9.1 service generated with"
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
     keywords="aiobotocore customer-profiles type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_customer_profiles": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles/__init__.py` & `types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,9 +22,8 @@
 """
 
 from .client import CustomerProfilesClient
 from .paginator import ListEventStreamsPaginator
 
 Client = CustomerProfilesClient
 
-
 __all__ = ("Client", "CustomerProfilesClient", "ListEventStreamsPaginator")
```

### Comparing `types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles/__init__.pyi` & `types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles/__main__.py` & `types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CustomerProfiles 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CustomerProfiles 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles\nOther"
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

### Comparing `types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles/client.py` & `types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CustomerProfilesClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -172,15 +171,15 @@
         DomainName: str,
         CalculatedAttributeName: str,
         AttributeDetails: AttributeDetailsTypeDef,
         Statistic: StatisticType,
         DisplayName: str = ...,
         Description: str = ...,
         Conditions: ConditionsTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateCalculatedAttributeDefinitionResponseTypeDef:
         """
         Creates a new calculated attribute definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_calculated_attribute_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/client/#create_calculated_attribute_definition)
         """
@@ -190,15 +189,15 @@
         *,
         DomainName: str,
         DefaultExpirationDays: int,
         DefaultEncryptionKey: str = ...,
         DeadLetterQueueUrl: str = ...,
         Matching: MatchingRequestTypeDef = ...,
         RuleBasedMatching: RuleBasedMatchingRequestTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateDomainResponseTypeDef:
         """
         Creates a domain, which is a container for all customer data, such as customer
         profile attributes, object types, profile keys, and encryption
         keys.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_domain)
@@ -221,15 +220,15 @@
         self,
         *,
         DomainName: str,
         WorkflowType: Literal["APPFLOW_INTEGRATION"],
         IntegrationConfig: IntegrationConfigTypeDef,
         ObjectTypeName: str,
         RoleArn: str,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateIntegrationWorkflowResponseTypeDef:
         """
         Creates an integration workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_integration_workflow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/client/#create_integration_workflow)
         """
@@ -256,15 +255,15 @@
         BusinessEmailAddress: str = ...,
         Address: AddressTypeDef = ...,
         ShippingAddress: AddressTypeDef = ...,
         MailingAddress: AddressTypeDef = ...,
         BillingAddress: AddressTypeDef = ...,
         Attributes: Mapping[str, str] = ...,
         PartyTypeString: str = ...,
-        GenderString: str = ...
+        GenderString: str = ...,
     ) -> CreateProfileResponseTypeDef:
         """
         Creates a standard profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/client/#create_profile)
         """
@@ -383,15 +382,15 @@
 
     async def get_auto_merging_preview(
         self,
         *,
         DomainName: str,
         Consolidation: ConsolidationTypeDef,
         ConflictResolution: ConflictResolutionTypeDef,
-        MinAllowedConfidenceScoreForMerging: float = ...
+        MinAllowedConfidenceScoreForMerging: float = ...,
     ) -> GetAutoMergingPreviewResponseTypeDef:
         """
         Tests the auto-merging settings of your Identity Resolution Job without merging
         your
         data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_auto_merging_preview)
@@ -494,15 +493,15 @@
         self,
         *,
         DomainName: str,
         MatchType: MatchTypeType,
         SearchKey: str,
         SearchValue: str,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetSimilarProfilesResponseTypeDef:
         """
         Returns a set of profiles that belong to the same matching group using the
         `matchId` or
         `profileId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_similar_profiles)
@@ -590,15 +589,15 @@
 
     async def list_integrations(
         self,
         *,
         DomainName: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        IncludeHidden: bool = ...
+        IncludeHidden: bool = ...,
     ) -> ListIntegrationsResponseTypeDef:
         """
         Lists all of the integrations in your domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_integrations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/client/#list_integrations)
         """
@@ -627,15 +626,15 @@
         self,
         *,
         DomainName: str,
         ObjectTypeName: str,
         ProfileId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        ObjectFilter: ObjectFilterTypeDef = ...
+        ObjectFilter: ObjectFilterTypeDef = ...,
     ) -> ListProfileObjectsResponseTypeDef:
         """
         Returns a list of objects associated with a profile of a given
         ProfileObjectType.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_profile_objects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/client/#list_profile_objects)
@@ -666,30 +665,30 @@
         *,
         DomainName: str,
         WorkflowType: Literal["APPFLOW_INTEGRATION"] = ...,
         Status: StatusType = ...,
         QueryStartDate: TimestampTypeDef = ...,
         QueryEndDate: TimestampTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListWorkflowsResponseTypeDef:
         """
         Query to list all workflows.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_workflows)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/client/#list_workflows)
         """
 
     async def merge_profiles(
         self,
         *,
         DomainName: str,
         MainProfileId: str,
         ProfileIdsToBeMerged: Sequence[str],
-        FieldSourceProfileIds: FieldSourceProfileIdsTypeDef = ...
+        FieldSourceProfileIds: FieldSourceProfileIdsTypeDef = ...,
     ) -> MergeProfilesResponseTypeDef:
         """
         Runs an AWS Lambda job that does the following: * All the profileKeys in the
         `ProfileToBeMerged` will be moved to the main
         profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.merge_profiles)
@@ -700,15 +699,15 @@
         self,
         *,
         DomainName: str,
         Uri: str = ...,
         ObjectTypeName: str = ...,
         Tags: Mapping[str, str] = ...,
         FlowDefinition: FlowDefinitionTypeDef = ...,
-        ObjectTypeNames: Mapping[str, str] = ...
+        ObjectTypeNames: Mapping[str, str] = ...,
     ) -> PutIntegrationResponseTypeDef:
         """
         Adds an integration between the service and a third-party service, which
         includes Amazon AppFlow and Amazon
         Connect.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.put_integration)
@@ -734,15 +733,15 @@
         TemplateId: str = ...,
         ExpirationDays: int = ...,
         EncryptionKey: str = ...,
         AllowProfileCreation: bool = ...,
         SourceLastUpdatedTimestampFormat: str = ...,
         Fields: Mapping[str, ObjectTypeFieldTypeDef] = ...,
         Keys: Mapping[str, Sequence[ObjectTypeKeyTypeDef]] = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> PutProfileObjectTypeResponseTypeDef:
         """
         Defines a ProfileObjectType.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.put_profile_object_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/client/#put_profile_object_type)
         """
@@ -752,15 +751,15 @@
         *,
         DomainName: str,
         KeyName: str,
         Values: Sequence[str],
         NextToken: str = ...,
         MaxResults: int = ...,
         AdditionalSearchKeys: Sequence[AdditionalSearchKeyTypeDef] = ...,
-        LogicalOperator: logicalOperatorType = ...
+        LogicalOperator: logicalOperatorType = ...,
     ) -> SearchProfilesResponseTypeDef:
         """
         Searches for profiles within a specific domain using one or more predefined
         search keys (e.g., _fullName, _phone, _email, _account, etc.) and/or
         custom-defined search
         keys.
 
@@ -790,15 +789,15 @@
     async def update_calculated_attribute_definition(
         self,
         *,
         DomainName: str,
         CalculatedAttributeName: str,
         DisplayName: str = ...,
         Description: str = ...,
-        Conditions: ConditionsTypeDef = ...
+        Conditions: ConditionsTypeDef = ...,
     ) -> UpdateCalculatedAttributeDefinitionResponseTypeDef:
         """
         Updates an existing calculated attribute definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.update_calculated_attribute_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/client/#update_calculated_attribute_definition)
         """
@@ -808,15 +807,15 @@
         *,
         DomainName: str,
         DefaultExpirationDays: int = ...,
         DefaultEncryptionKey: str = ...,
         DeadLetterQueueUrl: str = ...,
         Matching: MatchingRequestTypeDef = ...,
         RuleBasedMatching: RuleBasedMatchingRequestTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> UpdateDomainResponseTypeDef:
         """
         Updates the properties of a domain, including creating or selecting a dead
         letter queue or an encryption
         key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.update_domain)
@@ -846,15 +845,15 @@
         BusinessEmailAddress: str = ...,
         Address: UpdateAddressTypeDef = ...,
         ShippingAddress: UpdateAddressTypeDef = ...,
         MailingAddress: UpdateAddressTypeDef = ...,
         BillingAddress: UpdateAddressTypeDef = ...,
         Attributes: Mapping[str, str] = ...,
         PartyTypeString: str = ...,
-        GenderString: str = ...
+        GenderString: str = ...,
     ) -> UpdateProfileResponseTypeDef:
         """
         Updates the properties of a profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.update_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/client/#update_profile)
         """
```

### Comparing `types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles/client.pyi` & `types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,15 @@
         DomainName: str,
         CalculatedAttributeName: str,
         AttributeDetails: AttributeDetailsTypeDef,
         Statistic: StatisticType,
         DisplayName: str = ...,
         Description: str = ...,
         Conditions: ConditionsTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateCalculatedAttributeDefinitionResponseTypeDef:
         """
         Creates a new calculated attribute definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_calculated_attribute_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/client/#create_calculated_attribute_definition)
         """
@@ -186,15 +186,15 @@
         *,
         DomainName: str,
         DefaultExpirationDays: int,
         DefaultEncryptionKey: str = ...,
         DeadLetterQueueUrl: str = ...,
         Matching: MatchingRequestTypeDef = ...,
         RuleBasedMatching: RuleBasedMatchingRequestTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateDomainResponseTypeDef:
         """
         Creates a domain, which is a container for all customer data, such as customer
         profile attributes, object types, profile keys, and encryption
         keys.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_domain)
@@ -217,15 +217,15 @@
         self,
         *,
         DomainName: str,
         WorkflowType: Literal["APPFLOW_INTEGRATION"],
         IntegrationConfig: IntegrationConfigTypeDef,
         ObjectTypeName: str,
         RoleArn: str,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateIntegrationWorkflowResponseTypeDef:
         """
         Creates an integration workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_integration_workflow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/client/#create_integration_workflow)
         """
@@ -252,15 +252,15 @@
         BusinessEmailAddress: str = ...,
         Address: AddressTypeDef = ...,
         ShippingAddress: AddressTypeDef = ...,
         MailingAddress: AddressTypeDef = ...,
         BillingAddress: AddressTypeDef = ...,
         Attributes: Mapping[str, str] = ...,
         PartyTypeString: str = ...,
-        GenderString: str = ...
+        GenderString: str = ...,
     ) -> CreateProfileResponseTypeDef:
         """
         Creates a standard profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/client/#create_profile)
         """
@@ -379,15 +379,15 @@
 
     async def get_auto_merging_preview(
         self,
         *,
         DomainName: str,
         Consolidation: ConsolidationTypeDef,
         ConflictResolution: ConflictResolutionTypeDef,
-        MinAllowedConfidenceScoreForMerging: float = ...
+        MinAllowedConfidenceScoreForMerging: float = ...,
     ) -> GetAutoMergingPreviewResponseTypeDef:
         """
         Tests the auto-merging settings of your Identity Resolution Job without merging
         your
         data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_auto_merging_preview)
@@ -490,15 +490,15 @@
         self,
         *,
         DomainName: str,
         MatchType: MatchTypeType,
         SearchKey: str,
         SearchValue: str,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetSimilarProfilesResponseTypeDef:
         """
         Returns a set of profiles that belong to the same matching group using the
         `matchId` or
         `profileId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_similar_profiles)
@@ -586,15 +586,15 @@
 
     async def list_integrations(
         self,
         *,
         DomainName: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        IncludeHidden: bool = ...
+        IncludeHidden: bool = ...,
     ) -> ListIntegrationsResponseTypeDef:
         """
         Lists all of the integrations in your domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_integrations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/client/#list_integrations)
         """
@@ -623,15 +623,15 @@
         self,
         *,
         DomainName: str,
         ObjectTypeName: str,
         ProfileId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        ObjectFilter: ObjectFilterTypeDef = ...
+        ObjectFilter: ObjectFilterTypeDef = ...,
     ) -> ListProfileObjectsResponseTypeDef:
         """
         Returns a list of objects associated with a profile of a given
         ProfileObjectType.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_profile_objects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/client/#list_profile_objects)
@@ -662,30 +662,30 @@
         *,
         DomainName: str,
         WorkflowType: Literal["APPFLOW_INTEGRATION"] = ...,
         Status: StatusType = ...,
         QueryStartDate: TimestampTypeDef = ...,
         QueryEndDate: TimestampTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListWorkflowsResponseTypeDef:
         """
         Query to list all workflows.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_workflows)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/client/#list_workflows)
         """
 
     async def merge_profiles(
         self,
         *,
         DomainName: str,
         MainProfileId: str,
         ProfileIdsToBeMerged: Sequence[str],
-        FieldSourceProfileIds: FieldSourceProfileIdsTypeDef = ...
+        FieldSourceProfileIds: FieldSourceProfileIdsTypeDef = ...,
     ) -> MergeProfilesResponseTypeDef:
         """
         Runs an AWS Lambda job that does the following: * All the profileKeys in the
         `ProfileToBeMerged` will be moved to the main
         profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.merge_profiles)
@@ -696,15 +696,15 @@
         self,
         *,
         DomainName: str,
         Uri: str = ...,
         ObjectTypeName: str = ...,
         Tags: Mapping[str, str] = ...,
         FlowDefinition: FlowDefinitionTypeDef = ...,
-        ObjectTypeNames: Mapping[str, str] = ...
+        ObjectTypeNames: Mapping[str, str] = ...,
     ) -> PutIntegrationResponseTypeDef:
         """
         Adds an integration between the service and a third-party service, which
         includes Amazon AppFlow and Amazon
         Connect.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.put_integration)
@@ -730,15 +730,15 @@
         TemplateId: str = ...,
         ExpirationDays: int = ...,
         EncryptionKey: str = ...,
         AllowProfileCreation: bool = ...,
         SourceLastUpdatedTimestampFormat: str = ...,
         Fields: Mapping[str, ObjectTypeFieldTypeDef] = ...,
         Keys: Mapping[str, Sequence[ObjectTypeKeyTypeDef]] = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> PutProfileObjectTypeResponseTypeDef:
         """
         Defines a ProfileObjectType.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.put_profile_object_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/client/#put_profile_object_type)
         """
@@ -748,15 +748,15 @@
         *,
         DomainName: str,
         KeyName: str,
         Values: Sequence[str],
         NextToken: str = ...,
         MaxResults: int = ...,
         AdditionalSearchKeys: Sequence[AdditionalSearchKeyTypeDef] = ...,
-        LogicalOperator: logicalOperatorType = ...
+        LogicalOperator: logicalOperatorType = ...,
     ) -> SearchProfilesResponseTypeDef:
         """
         Searches for profiles within a specific domain using one or more predefined
         search keys (e.g., _fullName, _phone, _email, _account, etc.) and/or
         custom-defined search
         keys.
 
@@ -786,15 +786,15 @@
     async def update_calculated_attribute_definition(
         self,
         *,
         DomainName: str,
         CalculatedAttributeName: str,
         DisplayName: str = ...,
         Description: str = ...,
-        Conditions: ConditionsTypeDef = ...
+        Conditions: ConditionsTypeDef = ...,
     ) -> UpdateCalculatedAttributeDefinitionResponseTypeDef:
         """
         Updates an existing calculated attribute definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.update_calculated_attribute_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/client/#update_calculated_attribute_definition)
         """
@@ -804,15 +804,15 @@
         *,
         DomainName: str,
         DefaultExpirationDays: int = ...,
         DefaultEncryptionKey: str = ...,
         DeadLetterQueueUrl: str = ...,
         Matching: MatchingRequestTypeDef = ...,
         RuleBasedMatching: RuleBasedMatchingRequestTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> UpdateDomainResponseTypeDef:
         """
         Updates the properties of a domain, including creating or selecting a dead
         letter queue or an encryption
         key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.update_domain)
@@ -842,15 +842,15 @@
         BusinessEmailAddress: str = ...,
         Address: UpdateAddressTypeDef = ...,
         ShippingAddress: UpdateAddressTypeDef = ...,
         MailingAddress: UpdateAddressTypeDef = ...,
         BillingAddress: UpdateAddressTypeDef = ...,
         Attributes: Mapping[str, str] = ...,
         PartyTypeString: str = ...,
-        GenderString: str = ...
+        GenderString: str = ...,
     ) -> UpdateProfileResponseTypeDef:
         """
         Updates the properties of a profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.update_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/client/#update_profile)
         """
```

### Comparing `types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles/literals.py` & `types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles/literals.py`

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
     "AttributeMatchingModelType",
     "ConflictResolvingModelType",
     "DataPullModeType",
     "EventStreamDestinationStatusType",
     "EventStreamStateType",
     "FieldContentTypeType",
@@ -53,15 +52,14 @@
     "CustomerProfilesServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AttributeMatchingModelType = Literal["MANY_TO_MANY", "ONE_TO_ONE"]
 ConflictResolvingModelType = Literal["RECENCY", "SOURCE"]
 DataPullModeType = Literal["Complete", "Incremental"]
 EventStreamDestinationStatusType = Literal["HEALTHY", "UNHEALTHY"]
 EventStreamStateType = Literal["RUNNING", "STOPPED"]
 FieldContentTypeType = Literal["EMAIL_ADDRESS", "NAME", "NUMBER", "PHONE_NUMBER", "STRING"]
 GenderType = Literal["FEMALE", "MALE", "UNSPECIFIED"]
```

### Comparing `types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles/literals.pyi` & `types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles/paginator.py` & `types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import ListEventStreamsResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListEventStreamsPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles/paginator.pyi` & `types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles/type_defs.py` & `types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AddProfileKeyRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AdditionalSearchKeyTypeDef",
     "AddressTypeDef",
     "AppflowIntegrationWorkflowAttributesTypeDef",
     "AppflowIntegrationWorkflowMetricsTypeDef",
```

### Comparing `types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles/type_defs.pyi` & `types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles.egg-info/PKG-INFO` & `types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-customer-profiles
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CustomerProfiles 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CustomerProfiles 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/
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
 
 <a id="types-aiobotocore-customer-profiles"></a>
 
 # types-aiobotocore-customer-profiles
 
 [![PyPI - types-aiobotocore-customer-profiles](https://img.shields.io/pypi/v/types-aiobotocore-customer-profiles.svg?color=blue)](https://pypi.org/project/types-aiobotocore-customer-profiles)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-customer-profiles.svg?color=blue)](https://pypi.org/project/types-aiobotocore-customer-profiles)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-customer-profiles)](https://pepy.tech/project/types-aiobotocore-customer-profiles)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CustomerProfiles 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
+[aiobotocore.CustomerProfiles 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
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
 [types-aiobotocore-customer-profiles docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-customer-profiles-2.9.0/types_aiobotocore_customer_profiles.egg-info/SOURCES.txt` & `types-aiobotocore-customer-profiles-2.9.1/types_aiobotocore_customer_profiles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

