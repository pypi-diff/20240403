# Comparing `tmp/types-aiobotocore-wafv2-2.9.0.tar.gz` & `tmp/types-aiobotocore-wafv2-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-wafv2-2.9.0.tar", last modified: Wed Dec 13 20:00:45 2023, max compression
+gzip compressed data, was "types-aiobotocore-wafv2-2.9.1.tar", last modified: Thu Jan 18 01:22:02 2024, max compression
```

## Comparing `types-aiobotocore-wafv2-2.9.0.tar` & `types-aiobotocore-wafv2-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:45.245011 types-aiobotocore-wafv2-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:57:48.000000 types-aiobotocore-wafv2-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12113 2023-12-13 20:00:45.245011 types-aiobotocore-wafv2-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10558 2023-12-13 19:57:48.000000 types-aiobotocore-wafv2-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:45.245011 types-aiobotocore-wafv2-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2023-12-13 19:57:48.000000 types-aiobotocore-wafv2-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:45.245011 types-aiobotocore-wafv2-2.9.0/types_aiobotocore_wafv2/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2023-12-13 19:57:48.000000 types-aiobotocore-wafv2-2.9.0/types_aiobotocore_wafv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2023-12-13 19:57:48.000000 types-aiobotocore-wafv2-2.9.0/types_aiobotocore_wafv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      913 2023-12-13 19:57:48.000000 types-aiobotocore-wafv2-2.9.0/types_aiobotocore_wafv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39261 2023-12-13 19:57:49.000000 types-aiobotocore-wafv2-2.9.0/types_aiobotocore_wafv2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    39258 2023-12-13 19:57:49.000000 types-aiobotocore-wafv2-2.9.0/types_aiobotocore_wafv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14044 2023-12-13 19:57:49.000000 types-aiobotocore-wafv2-2.9.0/types_aiobotocore_wafv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14042 2023-12-13 19:57:49.000000 types-aiobotocore-wafv2-2.9.0/types_aiobotocore_wafv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:57:48.000000 types-aiobotocore-wafv2-2.9.0/types_aiobotocore_wafv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    59634 2023-12-13 19:57:50.000000 types-aiobotocore-wafv2-2.9.0/types_aiobotocore_wafv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    59633 2023-12-13 19:57:49.000000 types-aiobotocore-wafv2-2.9.0/types_aiobotocore_wafv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:57:48.000000 types-aiobotocore-wafv2-2.9.0/types_aiobotocore_wafv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:45.245011 types-aiobotocore-wafv2-2.9.0/types_aiobotocore_wafv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12113 2023-12-13 20:00:45.000000 types-aiobotocore-wafv2-2.9.0/types_aiobotocore_wafv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      700 2023-12-13 20:00:45.000000 types-aiobotocore-wafv2-2.9.0/types_aiobotocore_wafv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:45.000000 types-aiobotocore-wafv2-2.9.0/types_aiobotocore_wafv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:45.000000 types-aiobotocore-wafv2-2.9.0/types_aiobotocore_wafv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:45.000000 types-aiobotocore-wafv2-2.9.0/types_aiobotocore_wafv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-13 20:00:45.000000 types-aiobotocore-wafv2-2.9.0/types_aiobotocore_wafv2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:02.268973 types-aiobotocore-wafv2-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:19:16.000000 types-aiobotocore-wafv2-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12133 2024-01-18 01:22:02.268973 types-aiobotocore-wafv2-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10558 2024-01-18 01:19:16.000000 types-aiobotocore-wafv2-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:22:02.268973 types-aiobotocore-wafv2-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-01-18 01:19:16.000000 types-aiobotocore-wafv2-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:02.268973 types-aiobotocore-wafv2-2.9.1/types_aiobotocore_wafv2/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-01-18 01:19:16.000000 types-aiobotocore-wafv2-2.9.1/types_aiobotocore_wafv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-01-18 01:19:16.000000 types-aiobotocore-wafv2-2.9.1/types_aiobotocore_wafv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-01-18 01:19:16.000000 types-aiobotocore-wafv2-2.9.1/types_aiobotocore_wafv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39274 2024-01-18 01:19:16.000000 types-aiobotocore-wafv2-2.9.1/types_aiobotocore_wafv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39271 2024-01-18 01:19:16.000000 types-aiobotocore-wafv2-2.9.1/types_aiobotocore_wafv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14042 2024-01-18 01:19:16.000000 types-aiobotocore-wafv2-2.9.1/types_aiobotocore_wafv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14042 2024-01-18 01:19:16.000000 types-aiobotocore-wafv2-2.9.1/types_aiobotocore_wafv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:16.000000 types-aiobotocore-wafv2-2.9.1/types_aiobotocore_wafv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    59633 2024-01-18 01:19:18.000000 types-aiobotocore-wafv2-2.9.1/types_aiobotocore_wafv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59633 2024-01-18 01:19:17.000000 types-aiobotocore-wafv2-2.9.1/types_aiobotocore_wafv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:19:16.000000 types-aiobotocore-wafv2-2.9.1/types_aiobotocore_wafv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:02.268973 types-aiobotocore-wafv2-2.9.1/types_aiobotocore_wafv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12133 2024-01-18 01:22:02.000000 types-aiobotocore-wafv2-2.9.1/types_aiobotocore_wafv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-01-18 01:22:02.000000 types-aiobotocore-wafv2-2.9.1/types_aiobotocore_wafv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:22:02.000000 types-aiobotocore-wafv2-2.9.1/types_aiobotocore_wafv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:22:02.000000 types-aiobotocore-wafv2-2.9.1/types_aiobotocore_wafv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:22:02.000000 types-aiobotocore-wafv2-2.9.1/types_aiobotocore_wafv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-18 01:22:02.000000 types-aiobotocore-wafv2-2.9.1/types_aiobotocore_wafv2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-wafv2-2.9.0/LICENSE` & `types-aiobotocore-wafv2-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-wafv2-2.9.0/PKG-INFO` & `types-aiobotocore-wafv2-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-wafv2
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.WAFV2 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.WAFV2 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/
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
 
 <a id="types-aiobotocore-wafv2"></a>
 
 # types-aiobotocore-wafv2
 
 [![PyPI - types-aiobotocore-wafv2](https://img.shields.io/pypi/v/types-aiobotocore-wafv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wafv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-wafv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wafv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-wafv2)](https://pepy.tech/project/types-aiobotocore-wafv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WAFV2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
+[aiobotocore.WAFV2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
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
 [types-aiobotocore-wafv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-wafv2-2.9.0/README.md` & `types-aiobotocore-wafv2-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-wafv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wafv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-wafv2)](https://pepy.tech/project/types-aiobotocore-wafv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WAFV2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
+[aiobotocore.WAFV2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
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
 [types-aiobotocore-wafv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-wafv2-2.9.0/setup.py` & `types-aiobotocore-wafv2-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-wafv2",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_wafv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.WAFV2 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.WAFV2 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore wafv2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_wafv2": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-wafv2-2.9.0/types_aiobotocore_wafv2/__main__.py` & `types-aiobotocore-wafv2-2.9.1/types_aiobotocore_wafv2/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.WAFV2 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.WAFV2 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2\nOther"
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

### Comparing `types-aiobotocore-wafv2-2.9.0/types_aiobotocore_wafv2/client.py` & `types-aiobotocore-wafv2-2.9.1/types_aiobotocore_wafv2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,15 @@
         self,
         *,
         Name: str,
         Scope: ScopeType,
         IPAddressVersion: IPAddressVersionType,
         Addresses: Sequence[str],
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateIPSetResponseTypeDef:
         """
         Creates an  IPSet, which you use to identify web requests that originate from
         specific IP addresses or ranges of IP
         addresses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.create_ip_set)
@@ -199,15 +199,15 @@
     async def create_regex_pattern_set(
         self,
         *,
         Name: str,
         Scope: ScopeType,
         RegularExpressionList: Sequence[RegexTypeDef],
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRegexPatternSetResponseTypeDef:
         """
         Creates a  RegexPatternSet, which you reference in a
         RegexPatternSetReferenceStatement, to have WAF inspect a web request component
         for the specified
         patterns.
 
@@ -221,15 +221,15 @@
         Name: str,
         Scope: ScopeType,
         Capacity: int,
         VisibilityConfig: VisibilityConfigTypeDef,
         Description: str = ...,
         Rules: Sequence[RuleTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...
+        CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,
     ) -> CreateRuleGroupResponseTypeDef:
         """
         Creates a  RuleGroup per the specifications provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.create_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#create_rule_group)
         """
@@ -244,15 +244,15 @@
         Description: str = ...,
         Rules: Sequence[RuleTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,
         CaptchaConfig: CaptchaConfigTypeDef = ...,
         ChallengeConfig: ChallengeConfigTypeDef = ...,
         TokenDomains: Sequence[str] = ...,
-        AssociationConfig: AssociationConfigTypeDef = ...
+        AssociationConfig: AssociationConfigTypeDef = ...,
     ) -> CreateWebACLResponseTypeDef:
         """
         Creates a  WebACL per the specifications provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.create_web_acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#create_web_acl)
         """
@@ -457,15 +457,15 @@
     async def get_rate_based_statement_managed_keys(
         self,
         *,
         Scope: ScopeType,
         WebACLName: str,
         WebACLId: str,
         RuleName: str,
-        RuleGroupRuleName: str = ...
+        RuleGroupRuleName: str = ...,
     ) -> GetRateBasedStatementManagedKeysResponseTypeDef:
         """
         Retrieves the IP addresses that are currently blocked by a rate-based rule
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.get_rate_based_statement_managed_keys)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#get_rate_based_statement_managed_keys)
@@ -494,15 +494,15 @@
     async def get_sampled_requests(
         self,
         *,
         WebAclArn: str,
         RuleMetricName: str,
         Scope: ScopeType,
         TimeWindow: TimeWindowTypeDef,
-        MaxItems: int
+        MaxItems: int,
     ) -> GetSampledRequestsResponseTypeDef:
         """
         Gets detailed information about a specified number of requests--a sample--that
         WAF randomly selects from among the first 5,000 requests that your Amazon Web
         Services resource received during a time range that you
         choose.
 
@@ -543,15 +543,15 @@
     async def list_available_managed_rule_group_versions(
         self,
         *,
         VendorName: str,
         Name: str,
         Scope: ScopeType,
         NextMarker: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> ListAvailableManagedRuleGroupVersionsResponseTypeDef:
         """
         Returns a list of the available versions for the specified managed rule group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.list_available_managed_rule_group_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#list_available_managed_rule_group_versions)
         """
@@ -679,15 +679,15 @@
         self,
         *,
         Name: str,
         Scope: ScopeType,
         Id: str,
         LockToken: str,
         RecommendedVersion: str = ...,
-        VersionsToPublish: Mapping[str, VersionToPublishTypeDef] = ...
+        VersionsToPublish: Mapping[str, VersionToPublishTypeDef] = ...,
     ) -> PutManagedRuleSetVersionsResponseTypeDef:
         """
         Defines the versions of your managed rule set that you are offering to the
         customers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.put_managed_rule_set_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#put_managed_rule_set_versions)
@@ -721,15 +721,15 @@
         self,
         *,
         Name: str,
         Scope: ScopeType,
         Id: str,
         Addresses: Sequence[str],
         LockToken: str,
-        Description: str = ...
+        Description: str = ...,
     ) -> UpdateIPSetResponseTypeDef:
         """
         Updates the specified  IPSet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.update_ip_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#update_ip_set)
         """
@@ -738,15 +738,15 @@
         self,
         *,
         Name: str,
         Scope: ScopeType,
         Id: str,
         LockToken: str,
         VersionToExpire: str,
-        ExpiryTimestamp: TimestampTypeDef
+        ExpiryTimestamp: TimestampTypeDef,
     ) -> UpdateManagedRuleSetVersionExpiryDateResponseTypeDef:
         """
         Updates the expiration information for your managed rule set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.update_managed_rule_set_version_expiry_date)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#update_managed_rule_set_version_expiry_date)
         """
@@ -755,15 +755,15 @@
         self,
         *,
         Name: str,
         Scope: ScopeType,
         Id: str,
         RegularExpressionList: Sequence[RegexTypeDef],
         LockToken: str,
-        Description: str = ...
+        Description: str = ...,
     ) -> UpdateRegexPatternSetResponseTypeDef:
         """
         Updates the specified  RegexPatternSet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.update_regex_pattern_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#update_regex_pattern_set)
         """
@@ -774,15 +774,15 @@
         Name: str,
         Scope: ScopeType,
         Id: str,
         VisibilityConfig: VisibilityConfigTypeDef,
         LockToken: str,
         Description: str = ...,
         Rules: Sequence[RuleTypeDef] = ...,
-        CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...
+        CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,
     ) -> UpdateRuleGroupResponseTypeDef:
         """
         Updates the specified  RuleGroup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.update_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#update_rule_group)
         """
@@ -798,15 +798,15 @@
         LockToken: str,
         Description: str = ...,
         Rules: Sequence[RuleTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,
         CaptchaConfig: CaptchaConfigTypeDef = ...,
         ChallengeConfig: ChallengeConfigTypeDef = ...,
         TokenDomains: Sequence[str] = ...,
-        AssociationConfig: AssociationConfigTypeDef = ...
+        AssociationConfig: AssociationConfigTypeDef = ...,
     ) -> UpdateWebACLResponseTypeDef:
         """
         Updates the specified  WebACL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.update_web_acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#update_web_acl)
         """
```

### Comparing `types-aiobotocore-wafv2-2.9.0/types_aiobotocore_wafv2/client.pyi` & `types-aiobotocore-wafv2-2.9.1/types_aiobotocore_wafv2/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,15 @@
         self,
         *,
         Name: str,
         Scope: ScopeType,
         IPAddressVersion: IPAddressVersionType,
         Addresses: Sequence[str],
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateIPSetResponseTypeDef:
         """
         Creates an  IPSet, which you use to identify web requests that originate from
         specific IP addresses or ranges of IP
         addresses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.create_ip_set)
@@ -196,15 +196,15 @@
     async def create_regex_pattern_set(
         self,
         *,
         Name: str,
         Scope: ScopeType,
         RegularExpressionList: Sequence[RegexTypeDef],
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRegexPatternSetResponseTypeDef:
         """
         Creates a  RegexPatternSet, which you reference in a
         RegexPatternSetReferenceStatement, to have WAF inspect a web request component
         for the specified
         patterns.
 
@@ -218,15 +218,15 @@
         Name: str,
         Scope: ScopeType,
         Capacity: int,
         VisibilityConfig: VisibilityConfigTypeDef,
         Description: str = ...,
         Rules: Sequence[RuleTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...
+        CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,
     ) -> CreateRuleGroupResponseTypeDef:
         """
         Creates a  RuleGroup per the specifications provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.create_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#create_rule_group)
         """
@@ -241,15 +241,15 @@
         Description: str = ...,
         Rules: Sequence[RuleTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,
         CaptchaConfig: CaptchaConfigTypeDef = ...,
         ChallengeConfig: ChallengeConfigTypeDef = ...,
         TokenDomains: Sequence[str] = ...,
-        AssociationConfig: AssociationConfigTypeDef = ...
+        AssociationConfig: AssociationConfigTypeDef = ...,
     ) -> CreateWebACLResponseTypeDef:
         """
         Creates a  WebACL per the specifications provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.create_web_acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#create_web_acl)
         """
@@ -454,15 +454,15 @@
     async def get_rate_based_statement_managed_keys(
         self,
         *,
         Scope: ScopeType,
         WebACLName: str,
         WebACLId: str,
         RuleName: str,
-        RuleGroupRuleName: str = ...
+        RuleGroupRuleName: str = ...,
     ) -> GetRateBasedStatementManagedKeysResponseTypeDef:
         """
         Retrieves the IP addresses that are currently blocked by a rate-based rule
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.get_rate_based_statement_managed_keys)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#get_rate_based_statement_managed_keys)
@@ -491,15 +491,15 @@
     async def get_sampled_requests(
         self,
         *,
         WebAclArn: str,
         RuleMetricName: str,
         Scope: ScopeType,
         TimeWindow: TimeWindowTypeDef,
-        MaxItems: int
+        MaxItems: int,
     ) -> GetSampledRequestsResponseTypeDef:
         """
         Gets detailed information about a specified number of requests--a sample--that
         WAF randomly selects from among the first 5,000 requests that your Amazon Web
         Services resource received during a time range that you
         choose.
 
@@ -540,15 +540,15 @@
     async def list_available_managed_rule_group_versions(
         self,
         *,
         VendorName: str,
         Name: str,
         Scope: ScopeType,
         NextMarker: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> ListAvailableManagedRuleGroupVersionsResponseTypeDef:
         """
         Returns a list of the available versions for the specified managed rule group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.list_available_managed_rule_group_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#list_available_managed_rule_group_versions)
         """
@@ -676,15 +676,15 @@
         self,
         *,
         Name: str,
         Scope: ScopeType,
         Id: str,
         LockToken: str,
         RecommendedVersion: str = ...,
-        VersionsToPublish: Mapping[str, VersionToPublishTypeDef] = ...
+        VersionsToPublish: Mapping[str, VersionToPublishTypeDef] = ...,
     ) -> PutManagedRuleSetVersionsResponseTypeDef:
         """
         Defines the versions of your managed rule set that you are offering to the
         customers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.put_managed_rule_set_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#put_managed_rule_set_versions)
@@ -718,15 +718,15 @@
         self,
         *,
         Name: str,
         Scope: ScopeType,
         Id: str,
         Addresses: Sequence[str],
         LockToken: str,
-        Description: str = ...
+        Description: str = ...,
     ) -> UpdateIPSetResponseTypeDef:
         """
         Updates the specified  IPSet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.update_ip_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#update_ip_set)
         """
@@ -735,15 +735,15 @@
         self,
         *,
         Name: str,
         Scope: ScopeType,
         Id: str,
         LockToken: str,
         VersionToExpire: str,
-        ExpiryTimestamp: TimestampTypeDef
+        ExpiryTimestamp: TimestampTypeDef,
     ) -> UpdateManagedRuleSetVersionExpiryDateResponseTypeDef:
         """
         Updates the expiration information for your managed rule set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.update_managed_rule_set_version_expiry_date)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#update_managed_rule_set_version_expiry_date)
         """
@@ -752,15 +752,15 @@
         self,
         *,
         Name: str,
         Scope: ScopeType,
         Id: str,
         RegularExpressionList: Sequence[RegexTypeDef],
         LockToken: str,
-        Description: str = ...
+        Description: str = ...,
     ) -> UpdateRegexPatternSetResponseTypeDef:
         """
         Updates the specified  RegexPatternSet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.update_regex_pattern_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#update_regex_pattern_set)
         """
@@ -771,15 +771,15 @@
         Name: str,
         Scope: ScopeType,
         Id: str,
         VisibilityConfig: VisibilityConfigTypeDef,
         LockToken: str,
         Description: str = ...,
         Rules: Sequence[RuleTypeDef] = ...,
-        CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...
+        CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,
     ) -> UpdateRuleGroupResponseTypeDef:
         """
         Updates the specified  RuleGroup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.update_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#update_rule_group)
         """
@@ -795,15 +795,15 @@
         LockToken: str,
         Description: str = ...,
         Rules: Sequence[RuleTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,
         CaptchaConfig: CaptchaConfigTypeDef = ...,
         ChallengeConfig: ChallengeConfigTypeDef = ...,
         TokenDomains: Sequence[str] = ...,
-        AssociationConfig: AssociationConfigTypeDef = ...
+        AssociationConfig: AssociationConfigTypeDef = ...,
     ) -> UpdateWebACLResponseTypeDef:
         """
         Updates the specified  WebACL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.update_web_acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#update_web_acl)
         """
```

### Comparing `types-aiobotocore-wafv2-2.9.0/types_aiobotocore_wafv2/literals.py` & `types-aiobotocore-wafv2-2.9.1/types_aiobotocore_wafv2/literals.py`

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
     "ActionValueType",
     "AssociatedResourceTypeType",
     "BodyParsingFallbackBehaviorType",
     "ComparisonOperatorType",
     "CountryCodeType",
     "FailureReasonType",
@@ -49,15 +48,14 @@
     "TextTransformationTypeType",
     "WAFV2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 ActionValueType = Literal["ALLOW", "BLOCK", "CAPTCHA", "CHALLENGE", "COUNT", "EXCLUDED_AS_COUNT"]
 AssociatedResourceTypeType = Literal["CLOUDFRONT"]
 BodyParsingFallbackBehaviorType = Literal["EVALUATE_AS_STRING", "MATCH", "NO_MATCH"]
 ComparisonOperatorType = Literal["EQ", "GE", "GT", "LE", "LT", "NE"]
 CountryCodeType = Literal[
     "AD",
     "AE",
```

### Comparing `types-aiobotocore-wafv2-2.9.0/types_aiobotocore_wafv2/literals.pyi` & `types-aiobotocore-wafv2-2.9.1/types_aiobotocore_wafv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wafv2-2.9.0/types_aiobotocore_wafv2/type_defs.py` & `types-aiobotocore-wafv2-2.9.1/types_aiobotocore_wafv2/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "APIKeySummaryTypeDef",
     "AWSManagedRulesBotControlRuleSetTypeDef",
     "ActionConditionTypeDef",
     "AddressFieldTypeDef",
     "AndStatementTypeDef",
     "AssociateWebACLRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-wafv2-2.9.0/types_aiobotocore_wafv2/type_defs.pyi` & `types-aiobotocore-wafv2-2.9.1/types_aiobotocore_wafv2/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wafv2-2.9.0/types_aiobotocore_wafv2.egg-info/PKG-INFO` & `types-aiobotocore-wafv2-2.9.1/types_aiobotocore_wafv2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-wafv2
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.WAFV2 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.WAFV2 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/
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
 
 <a id="types-aiobotocore-wafv2"></a>
 
 # types-aiobotocore-wafv2
 
 [![PyPI - types-aiobotocore-wafv2](https://img.shields.io/pypi/v/types-aiobotocore-wafv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wafv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-wafv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wafv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-wafv2)](https://pepy.tech/project/types-aiobotocore-wafv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WAFV2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
+[aiobotocore.WAFV2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
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
 [types-aiobotocore-wafv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-wafv2-2.9.0/types_aiobotocore_wafv2.egg-info/SOURCES.txt` & `types-aiobotocore-wafv2-2.9.1/types_aiobotocore_wafv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

