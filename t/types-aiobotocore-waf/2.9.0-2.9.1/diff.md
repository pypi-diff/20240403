# Comparing `tmp/types-aiobotocore-waf-2.9.0.tar.gz` & `tmp/types-aiobotocore-waf-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-waf-2.9.0.tar", last modified: Wed Dec 13 20:00:44 2023, max compression
+gzip compressed data, was "types-aiobotocore-waf-2.9.1.tar", last modified: Thu Jan 18 01:22:01 2024, max compression
```

## Comparing `types-aiobotocore-waf-2.9.0.tar` & `types-aiobotocore-waf-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:44.489018 types-aiobotocore-waf-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:57:36.000000 types-aiobotocore-waf-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15139 2023-12-13 20:00:44.485018 types-aiobotocore-waf-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13592 2023-12-13 19:57:36.000000 types-aiobotocore-waf-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:44.489018 types-aiobotocore-waf-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-12-13 19:57:36.000000 types-aiobotocore-waf-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:44.485018 types-aiobotocore-waf-2.9.0/types_aiobotocore_waf/
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2023-12-13 19:57:36.000000 types-aiobotocore-waf-2.9.0/types_aiobotocore_waf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2023-12-13 19:57:36.000000 types-aiobotocore-waf-2.9.0/types_aiobotocore_waf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-13 19:57:36.000000 types-aiobotocore-waf-2.9.0/types_aiobotocore_waf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52666 2023-12-13 19:57:39.000000 types-aiobotocore-waf-2.9.0/types_aiobotocore_waf/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    52662 2023-12-13 19:57:36.000000 types-aiobotocore-waf-2.9.0/types_aiobotocore_waf/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14247 2023-12-13 19:57:40.000000 types-aiobotocore-waf-2.9.0/types_aiobotocore_waf/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14245 2023-12-13 19:57:40.000000 types-aiobotocore-waf-2.9.0/types_aiobotocore_waf/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18480 2023-12-13 19:57:39.000000 types-aiobotocore-waf-2.9.0/types_aiobotocore_waf/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    18462 2023-12-13 19:57:39.000000 types-aiobotocore-waf-2.9.0/types_aiobotocore_waf/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:57:36.000000 types-aiobotocore-waf-2.9.0/types_aiobotocore_waf/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    53453 2023-12-13 19:57:41.000000 types-aiobotocore-waf-2.9.0/types_aiobotocore_waf/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    53452 2023-12-13 19:57:40.000000 types-aiobotocore-waf-2.9.0/types_aiobotocore_waf/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:57:36.000000 types-aiobotocore-waf-2.9.0/types_aiobotocore_waf/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:44.485018 types-aiobotocore-waf-2.9.0/types_aiobotocore_waf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15139 2023-12-13 20:00:44.000000 types-aiobotocore-waf-2.9.0/types_aiobotocore_waf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      737 2023-12-13 20:00:44.000000 types-aiobotocore-waf-2.9.0/types_aiobotocore_waf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:44.000000 types-aiobotocore-waf-2.9.0/types_aiobotocore_waf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:44.000000 types-aiobotocore-waf-2.9.0/types_aiobotocore_waf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:44.000000 types-aiobotocore-waf-2.9.0/types_aiobotocore_waf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 20:00:44.000000 types-aiobotocore-waf-2.9.0/types_aiobotocore_waf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:01.580976 types-aiobotocore-waf-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:19:05.000000 types-aiobotocore-waf-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15159 2024-01-18 01:22:01.580976 types-aiobotocore-waf-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13592 2024-01-18 01:19:05.000000 types-aiobotocore-waf-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:22:01.580976 types-aiobotocore-waf-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-01-18 01:19:05.000000 types-aiobotocore-waf-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:01.580976 types-aiobotocore-waf-2.9.1/types_aiobotocore_waf/
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-01-18 01:19:05.000000 types-aiobotocore-waf-2.9.1/types_aiobotocore_waf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-01-18 01:19:05.000000 types-aiobotocore-waf-2.9.1/types_aiobotocore_waf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-18 01:19:05.000000 types-aiobotocore-waf-2.9.1/types_aiobotocore_waf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52672 2024-01-18 01:19:06.000000 types-aiobotocore-waf-2.9.1/types_aiobotocore_waf/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52669 2024-01-18 01:19:06.000000 types-aiobotocore-waf-2.9.1/types_aiobotocore_waf/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14245 2024-01-18 01:19:06.000000 types-aiobotocore-waf-2.9.1/types_aiobotocore_waf/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14245 2024-01-18 01:19:06.000000 types-aiobotocore-waf-2.9.1/types_aiobotocore_waf/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18479 2024-01-18 01:19:06.000000 types-aiobotocore-waf-2.9.1/types_aiobotocore_waf/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18462 2024-01-18 01:19:06.000000 types-aiobotocore-waf-2.9.1/types_aiobotocore_waf/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:05.000000 types-aiobotocore-waf-2.9.1/types_aiobotocore_waf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    53452 2024-01-18 01:19:07.000000 types-aiobotocore-waf-2.9.1/types_aiobotocore_waf/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53452 2024-01-18 01:19:07.000000 types-aiobotocore-waf-2.9.1/types_aiobotocore_waf/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:19:05.000000 types-aiobotocore-waf-2.9.1/types_aiobotocore_waf/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:01.580976 types-aiobotocore-waf-2.9.1/types_aiobotocore_waf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15159 2024-01-18 01:22:01.000000 types-aiobotocore-waf-2.9.1/types_aiobotocore_waf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-01-18 01:22:01.000000 types-aiobotocore-waf-2.9.1/types_aiobotocore_waf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:22:01.000000 types-aiobotocore-waf-2.9.1/types_aiobotocore_waf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:22:01.000000 types-aiobotocore-waf-2.9.1/types_aiobotocore_waf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:22:01.000000 types-aiobotocore-waf-2.9.1/types_aiobotocore_waf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:22:01.000000 types-aiobotocore-waf-2.9.1/types_aiobotocore_waf.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-waf-2.9.0/LICENSE` & `types-aiobotocore-waf-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-waf-2.9.0/PKG-INFO` & `types-aiobotocore-waf-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-waf
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.WAF 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.WAF 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/
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
 
 <a id="types-aiobotocore-waf"></a>
 
 # types-aiobotocore-waf
 
 [![PyPI - types-aiobotocore-waf](https://img.shields.io/pypi/v/types-aiobotocore-waf.svg?color=blue)](https://pypi.org/project/types-aiobotocore-waf)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-waf.svg?color=blue)](https://pypi.org/project/types-aiobotocore-waf)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-waf)](https://pepy.tech/project/types-aiobotocore-waf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WAF 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
+[aiobotocore.WAF 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
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
 [types-aiobotocore-waf docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-waf-2.9.0/README.md` & `types-aiobotocore-waf-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-waf.svg?color=blue)](https://pypi.org/project/types-aiobotocore-waf)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-waf)](https://pepy.tech/project/types-aiobotocore-waf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WAF 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
+[aiobotocore.WAF 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
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
 [types-aiobotocore-waf docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-waf-2.9.0/setup.py` & `types-aiobotocore-waf-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-waf",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_waf"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.WAF 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.WAF 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore waf type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_waf": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-waf-2.9.0/types_aiobotocore_waf/__init__.py` & `types-aiobotocore-waf-2.9.1/types_aiobotocore_waf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,14 @@
     ListSubscribedRuleGroupsPaginator,
     ListWebACLsPaginator,
     ListXssMatchSetsPaginator,
 )
 
 Client = WAFClient
 
-
 __all__ = (
     "Client",
     "GetRateBasedRuleManagedKeysPaginator",
     "ListActivatedRulesInRuleGroupPaginator",
     "ListByteMatchSetsPaginator",
     "ListGeoMatchSetsPaginator",
     "ListIPSetsPaginator",
```

### Comparing `types-aiobotocore-waf-2.9.0/types_aiobotocore_waf/__init__.pyi` & `types-aiobotocore-waf-2.9.1/types_aiobotocore_waf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-2.9.0/types_aiobotocore_waf/__main__.py` & `types-aiobotocore-waf-2.9.1/types_aiobotocore_waf/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.WAF 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.WAF 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF\nOther"
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

### Comparing `types-aiobotocore-waf-2.9.0/types_aiobotocore_waf/client.py` & `types-aiobotocore-waf-2.9.1/types_aiobotocore_waf/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("WAFClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -234,15 +233,15 @@
         self,
         *,
         Name: str,
         MetricName: str,
         RateKey: Literal["IP"],
         RateLimit: int,
         ChangeToken: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRateBasedRuleResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.create_rate_based_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/client/#create_rate_based_rule)
         """
@@ -310,15 +309,15 @@
     async def create_web_acl(
         self,
         *,
         Name: str,
         MetricName: str,
         DefaultAction: WafActionTypeDef,
         ChangeToken: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateWebACLResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.create_web_acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/client/#create_web_acl)
         """
@@ -886,29 +885,29 @@
         """
 
     async def update_regex_match_set(
         self,
         *,
         RegexMatchSetId: str,
         Updates: Sequence[RegexMatchSetUpdateTypeDef],
-        ChangeToken: str
+        ChangeToken: str,
     ) -> UpdateRegexMatchSetResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.update_regex_match_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/client/#update_regex_match_set)
         """
 
     async def update_regex_pattern_set(
         self,
         *,
         RegexPatternSetId: str,
         Updates: Sequence[RegexPatternSetUpdateTypeDef],
-        ChangeToken: str
+        ChangeToken: str,
     ) -> UpdateRegexPatternSetResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.update_regex_pattern_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/client/#update_regex_pattern_set)
         """
@@ -934,44 +933,44 @@
         """
 
     async def update_size_constraint_set(
         self,
         *,
         SizeConstraintSetId: str,
         ChangeToken: str,
-        Updates: Sequence[SizeConstraintSetUpdateTypeDef]
+        Updates: Sequence[SizeConstraintSetUpdateTypeDef],
     ) -> UpdateSizeConstraintSetResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.update_size_constraint_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/client/#update_size_constraint_set)
         """
 
     async def update_sql_injection_match_set(
         self,
         *,
         SqlInjectionMatchSetId: str,
         ChangeToken: str,
-        Updates: Sequence[SqlInjectionMatchSetUpdateTypeDef]
+        Updates: Sequence[SqlInjectionMatchSetUpdateTypeDef],
     ) -> UpdateSqlInjectionMatchSetResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.update_sql_injection_match_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/client/#update_sql_injection_match_set)
         """
 
     async def update_web_acl(
         self,
         *,
         WebACLId: str,
         ChangeToken: str,
         Updates: Sequence[WebACLUpdateTypeDef] = ...,
-        DefaultAction: WafActionTypeDef = ...
+        DefaultAction: WafActionTypeDef = ...,
     ) -> UpdateWebACLResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.update_web_acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/client/#update_web_acl)
         """
```

### Comparing `types-aiobotocore-waf-2.9.0/types_aiobotocore_waf/client.pyi` & `types-aiobotocore-waf-2.9.1/types_aiobotocore_waf/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -230,15 +230,15 @@
         self,
         *,
         Name: str,
         MetricName: str,
         RateKey: Literal["IP"],
         RateLimit: int,
         ChangeToken: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRateBasedRuleResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.create_rate_based_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/client/#create_rate_based_rule)
         """
@@ -306,15 +306,15 @@
     async def create_web_acl(
         self,
         *,
         Name: str,
         MetricName: str,
         DefaultAction: WafActionTypeDef,
         ChangeToken: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateWebACLResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.create_web_acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/client/#create_web_acl)
         """
@@ -882,29 +882,29 @@
         """
 
     async def update_regex_match_set(
         self,
         *,
         RegexMatchSetId: str,
         Updates: Sequence[RegexMatchSetUpdateTypeDef],
-        ChangeToken: str
+        ChangeToken: str,
     ) -> UpdateRegexMatchSetResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.update_regex_match_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/client/#update_regex_match_set)
         """
 
     async def update_regex_pattern_set(
         self,
         *,
         RegexPatternSetId: str,
         Updates: Sequence[RegexPatternSetUpdateTypeDef],
-        ChangeToken: str
+        ChangeToken: str,
     ) -> UpdateRegexPatternSetResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.update_regex_pattern_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/client/#update_regex_pattern_set)
         """
@@ -930,44 +930,44 @@
         """
 
     async def update_size_constraint_set(
         self,
         *,
         SizeConstraintSetId: str,
         ChangeToken: str,
-        Updates: Sequence[SizeConstraintSetUpdateTypeDef]
+        Updates: Sequence[SizeConstraintSetUpdateTypeDef],
     ) -> UpdateSizeConstraintSetResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.update_size_constraint_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/client/#update_size_constraint_set)
         """
 
     async def update_sql_injection_match_set(
         self,
         *,
         SqlInjectionMatchSetId: str,
         ChangeToken: str,
-        Updates: Sequence[SqlInjectionMatchSetUpdateTypeDef]
+        Updates: Sequence[SqlInjectionMatchSetUpdateTypeDef],
     ) -> UpdateSqlInjectionMatchSetResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.update_sql_injection_match_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/client/#update_sql_injection_match_set)
         """
 
     async def update_web_acl(
         self,
         *,
         WebACLId: str,
         ChangeToken: str,
         Updates: Sequence[WebACLUpdateTypeDef] = ...,
-        DefaultAction: WafActionTypeDef = ...
+        DefaultAction: WafActionTypeDef = ...,
     ) -> UpdateWebACLResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.update_web_acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/client/#update_web_acl)
         """
```

### Comparing `types-aiobotocore-waf-2.9.0/types_aiobotocore_waf/literals.py` & `types-aiobotocore-waf-2.9.1/types_aiobotocore_waf/literals.py`

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
     "ChangeActionType",
     "ChangeTokenStatusType",
     "ComparisonOperatorType",
     "GeoMatchConstraintTypeType",
     "GeoMatchConstraintValueType",
     "GetRateBasedRuleManagedKeysPaginatorName",
@@ -53,15 +52,14 @@
     "WafRuleTypeType",
     "WAFServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 ChangeActionType = Literal["DELETE", "INSERT"]
 ChangeTokenStatusType = Literal["INSYNC", "PENDING", "PROVISIONED"]
 ComparisonOperatorType = Literal["EQ", "GE", "GT", "LE", "LT", "NE"]
 GeoMatchConstraintTypeType = Literal["Country"]
 GeoMatchConstraintValueType = Literal[
     "AD",
     "AE",
```

### Comparing `types-aiobotocore-waf-2.9.0/types_aiobotocore_waf/literals.pyi` & `types-aiobotocore-waf-2.9.1/types_aiobotocore_waf/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-2.9.0/types_aiobotocore_waf/paginator.py` & `types-aiobotocore-waf-2.9.1/types_aiobotocore_waf/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,14 @@
     "ListSizeConstraintSetsPaginator",
     "ListSqlInjectionMatchSetsPaginator",
     "ListSubscribedRuleGroupsPaginator",
     "ListWebACLsPaginator",
     "ListXssMatchSetsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-waf-2.9.0/types_aiobotocore_waf/paginator.pyi` & `types-aiobotocore-waf-2.9.1/types_aiobotocore_waf/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-2.9.0/types_aiobotocore_waf/type_defs.py` & `types-aiobotocore-waf-2.9.1/types_aiobotocore_waf/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ExcludedRuleTypeDef",
     "WafActionTypeDef",
     "WafOverrideActionTypeDef",
     "ByteMatchSetSummaryTypeDef",
     "FieldToMatchTypeDef",
     "CreateByteMatchSetRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-waf-2.9.0/types_aiobotocore_waf/type_defs.pyi` & `types-aiobotocore-waf-2.9.1/types_aiobotocore_waf/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-2.9.0/types_aiobotocore_waf.egg-info/PKG-INFO` & `types-aiobotocore-waf-2.9.1/types_aiobotocore_waf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-waf
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.WAF 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.WAF 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/
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
 
 <a id="types-aiobotocore-waf"></a>
 
 # types-aiobotocore-waf
 
 [![PyPI - types-aiobotocore-waf](https://img.shields.io/pypi/v/types-aiobotocore-waf.svg?color=blue)](https://pypi.org/project/types-aiobotocore-waf)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-waf.svg?color=blue)](https://pypi.org/project/types-aiobotocore-waf)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-waf)](https://pepy.tech/project/types-aiobotocore-waf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WAF 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
+[aiobotocore.WAF 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
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
 [types-aiobotocore-waf docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-waf-2.9.0/types_aiobotocore_waf.egg-info/SOURCES.txt` & `types-aiobotocore-waf-2.9.1/types_aiobotocore_waf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

