# Comparing `tmp/types-aiobotocore-route53resolver-2.9.0.tar.gz` & `tmp/types-aiobotocore-route53resolver-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-route53resolver-2.9.0.tar", last modified: Wed Dec 13 20:00:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-route53resolver-2.9.1.tar", last modified: Thu Jan 18 01:21:41 2024, max compression
```

## Comparing `types-aiobotocore-route53resolver-2.9.0.tar` & `types-aiobotocore-route53resolver-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:21.869211 types-aiobotocore-route53resolver-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:54:58.000000 types-aiobotocore-route53resolver-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16185 2023-12-13 20:00:21.869211 types-aiobotocore-route53resolver-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14590 2023-12-13 19:54:58.000000 types-aiobotocore-route53resolver-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:21.869211 types-aiobotocore-route53resolver-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2023-12-13 19:54:58.000000 types-aiobotocore-route53resolver-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:21.869211 types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver/
--rw-r--r--   0 runner    (1001) docker     (127)     4570 2023-12-13 19:54:58.000000 types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2023-12-13 19:54:58.000000 types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      964 2023-12-13 19:54:58.000000 types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    62391 2023-12-13 19:54:58.000000 types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    62387 2023-12-13 19:54:58.000000 types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14889 2023-12-13 19:54:58.000000 types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14887 2023-12-13 19:54:58.000000 types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    21615 2023-12-13 19:54:58.000000 types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    21597 2023-12-13 19:54:58.000000 types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:54:58.000000 types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    55696 2023-12-13 19:54:59.000000 types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    55695 2023-12-13 19:54:59.000000 types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:54:58.000000 types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:21.869211 types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16185 2023-12-13 20:00:21.000000 types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      965 2023-12-13 20:00:21.000000 types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:21.000000 types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:21.000000 types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:21.000000 types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-13 20:00:21.000000 types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:41.049070 types-aiobotocore-route53resolver-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:16:31.000000 types-aiobotocore-route53resolver-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16205 2024-01-18 01:21:41.049070 types-aiobotocore-route53resolver-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14590 2024-01-18 01:16:31.000000 types-aiobotocore-route53resolver-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:41.049070 types-aiobotocore-route53resolver-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-01-18 01:16:31.000000 types-aiobotocore-route53resolver-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:41.049070 types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver/
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-01-18 01:16:31.000000 types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-01-18 01:16:31.000000 types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-01-18 01:16:31.000000 types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62405 2024-01-18 01:16:32.000000 types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62402 2024-01-18 01:16:32.000000 types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14887 2024-01-18 01:16:32.000000 types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14887 2024-01-18 01:16:32.000000 types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    21622 2024-01-18 01:16:32.000000 types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21605 2024-01-18 01:16:32.000000 types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:16:31.000000 types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    55695 2024-01-18 01:16:33.000000 types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55695 2024-01-18 01:16:33.000000 types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:16:31.000000 types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:41.049070 types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16205 2024-01-18 01:21:41.000000 types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-01-18 01:21:41.000000 types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:41.000000 types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:41.000000 types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:41.000000 types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-01-18 01:21:41.000000 types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-route53resolver-2.9.0/LICENSE` & `types-aiobotocore-route53resolver-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-route53resolver-2.9.0/PKG-INFO` & `types-aiobotocore-route53resolver-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-route53resolver
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Route53Resolver 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Route53Resolver 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/
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
 
 <a id="types-aiobotocore-route53resolver"></a>
 
 # types-aiobotocore-route53resolver
 
 [![PyPI - types-aiobotocore-route53resolver](https://img.shields.io/pypi/v/types-aiobotocore-route53resolver.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53resolver)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53resolver.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53resolver)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53resolver)](https://pepy.tech/project/types-aiobotocore-route53resolver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Route53Resolver 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
+[aiobotocore.Route53Resolver 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
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
 [types-aiobotocore-route53resolver docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-route53resolver-2.9.0/README.md` & `types-aiobotocore-route53resolver-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53resolver.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53resolver)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53resolver)](https://pepy.tech/project/types-aiobotocore-route53resolver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Route53Resolver 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
+[aiobotocore.Route53Resolver 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
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
 [types-aiobotocore-route53resolver docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-route53resolver-2.9.0/setup.py` & `types-aiobotocore-route53resolver-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-route53resolver",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_route53resolver"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Route53Resolver 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.Route53Resolver 2.9.1 service generated with"
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
     keywords="aiobotocore route53resolver type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_route53resolver": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver/__init__.py` & `types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,14 @@
     ListResolverRuleAssociationsPaginator,
     ListResolverRulesPaginator,
     ListTagsForResourcePaginator,
 )
 
 Client = Route53ResolverClient
 
-
 __all__ = (
     "Client",
     "ListFirewallConfigsPaginator",
     "ListFirewallDomainListsPaginator",
     "ListFirewallDomainsPaginator",
     "ListFirewallRuleGroupAssociationsPaginator",
     "ListFirewallRuleGroupsPaginator",
```

### Comparing `types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver/__init__.pyi` & `types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver/__main__.py` & `types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Route53Resolver 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Route53Resolver 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver\nOther"
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

### Comparing `types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver/client.py` & `types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("Route53ResolverClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -189,15 +188,15 @@
         *,
         CreatorRequestId: str,
         FirewallRuleGroupId: str,
         VpcId: str,
         Priority: int,
         Name: str,
         MutationProtection: MutationProtectionStatusType = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> AssociateFirewallRuleGroupResponseTypeDef:
         """
         Associates a  FirewallRuleGroup with a VPC, to provide DNS filtering for the
         VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.associate_firewall_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#associate_firewall_rule_group)
@@ -267,15 +266,15 @@
         FirewallDomainListId: str,
         Priority: int,
         Action: ActionType,
         Name: str,
         BlockResponse: BlockResponseType = ...,
         BlockOverrideDomain: str = ...,
         BlockOverrideDnsType: Literal["CNAME"] = ...,
-        BlockOverrideTtl: int = ...
+        BlockOverrideTtl: int = ...,
     ) -> CreateFirewallRuleResponseTypeDef:
         """
         Creates a single DNS Firewall rule in the specified rule group, using the
         specified domain
         list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_firewall_rule)
@@ -297,15 +296,15 @@
         self,
         *,
         CreatorRequestId: str,
         Name: str,
         PreferredInstanceType: str,
         OutpostArn: str,
         InstanceCount: int = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateOutpostResolverResponseTypeDef:
         """
         Creates an Route 53 Resolver on an Outpost.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_outpost_resolver)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#create_outpost_resolver)
         """
@@ -317,30 +316,30 @@
         SecurityGroupIds: Sequence[str],
         Direction: ResolverEndpointDirectionType,
         IpAddresses: Sequence[IpAddressRequestTypeDef],
         Name: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ResolverEndpointType: ResolverEndpointTypeType = ...,
         OutpostArn: str = ...,
-        PreferredInstanceType: str = ...
+        PreferredInstanceType: str = ...,
     ) -> CreateResolverEndpointResponseTypeDef:
         """
         Creates a Resolver endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_resolver_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#create_resolver_endpoint)
         """
 
     async def create_resolver_query_log_config(
         self,
         *,
         Name: str,
         DestinationArn: str,
         CreatorRequestId: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateResolverQueryLogConfigResponseTypeDef:
         """
         Creates a Resolver query logging configuration, which defines where you want
         Resolver to save DNS query logs that originate in your
         VPCs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_resolver_query_log_config)
@@ -352,15 +351,15 @@
         *,
         CreatorRequestId: str,
         RuleType: RuleTypeOptionType,
         DomainName: str,
         Name: str = ...,
         TargetIps: Sequence[TargetAddressTypeDef] = ...,
         ResolverEndpointId: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateResolverRuleResponseTypeDef:
         """
         For DNS queries that originate in your VPCs, specifies which Resolver endpoint
         the queries pass through, one domain name that you want to forward to your
         network, and the IP addresses of the DNS resolvers in your
         network.
 
@@ -699,15 +698,15 @@
         self,
         *,
         FirewallRuleGroupId: str = ...,
         VpcId: str = ...,
         Priority: int = ...,
         Status: FirewallRuleGroupAssociationStatusType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListFirewallRuleGroupAssociationsResponseTypeDef:
         """
         Retrieves the firewall rule group associations that you have defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_firewall_rule_group_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#list_firewall_rule_group_associations)
         """
@@ -726,15 +725,15 @@
     async def list_firewall_rules(
         self,
         *,
         FirewallRuleGroupId: str,
         Priority: int = ...,
         Action: ActionType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListFirewallRulesResponseTypeDef:
         """
         Retrieves the firewall rules that you have defined for the specified firewall
         rule
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_firewall_rules)
@@ -800,15 +799,15 @@
     async def list_resolver_query_log_config_associations(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         SortBy: str = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListResolverQueryLogConfigAssociationsResponseTypeDef:
         """
         Lists information about associations between Amazon VPCs and query logging
         configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_resolver_query_log_config_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#list_resolver_query_log_config_associations)
@@ -817,15 +816,15 @@
     async def list_resolver_query_log_configs(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         SortBy: str = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListResolverQueryLogConfigsResponseTypeDef:
         """
         Lists information about the specified query logging configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_resolver_query_log_configs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#list_resolver_query_log_configs)
         """
@@ -931,15 +930,15 @@
         """
 
     async def update_firewall_domains(
         self,
         *,
         FirewallDomainListId: str,
         Operation: FirewallDomainUpdateOperationType,
-        Domains: Sequence[str]
+        Domains: Sequence[str],
     ) -> UpdateFirewallDomainsResponseTypeDef:
         """
         Updates the firewall domain list from an array of domain specifications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_firewall_domains)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#update_firewall_domains)
         """
@@ -951,45 +950,45 @@
         FirewallDomainListId: str,
         Priority: int = ...,
         Action: ActionType = ...,
         BlockResponse: BlockResponseType = ...,
         BlockOverrideDomain: str = ...,
         BlockOverrideDnsType: Literal["CNAME"] = ...,
         BlockOverrideTtl: int = ...,
-        Name: str = ...
+        Name: str = ...,
     ) -> UpdateFirewallRuleResponseTypeDef:
         """
         Updates the specified firewall rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_firewall_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#update_firewall_rule)
         """
 
     async def update_firewall_rule_group_association(
         self,
         *,
         FirewallRuleGroupAssociationId: str,
         Priority: int = ...,
         MutationProtection: MutationProtectionStatusType = ...,
-        Name: str = ...
+        Name: str = ...,
     ) -> UpdateFirewallRuleGroupAssociationResponseTypeDef:
         """
         Changes the association of a  FirewallRuleGroup with a VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_firewall_rule_group_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#update_firewall_rule_group_association)
         """
 
     async def update_outpost_resolver(
         self,
         *,
         Id: str,
         Name: str = ...,
         InstanceCount: int = ...,
-        PreferredInstanceType: str = ...
+        PreferredInstanceType: str = ...,
     ) -> UpdateOutpostResolverResponseTypeDef:
         """
         You can use `UpdateOutpostResolver` to update the instance count, type, or name
         of a Resolver on an
         Outpost.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_outpost_resolver)
@@ -1020,15 +1019,15 @@
 
     async def update_resolver_endpoint(
         self,
         *,
         ResolverEndpointId: str,
         Name: str = ...,
         ResolverEndpointType: ResolverEndpointTypeType = ...,
-        UpdateIpAddresses: Sequence[UpdateIpAddressTypeDef] = ...
+        UpdateIpAddresses: Sequence[UpdateIpAddressTypeDef] = ...,
     ) -> UpdateResolverEndpointResponseTypeDef:
         """
         Updates the name, or enpoint type for an inbound or an outbound Resolver
         endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_resolver_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#update_resolver_endpoint)
```

### Comparing `types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver/client.pyi` & `types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,15 @@
         *,
         CreatorRequestId: str,
         FirewallRuleGroupId: str,
         VpcId: str,
         Priority: int,
         Name: str,
         MutationProtection: MutationProtectionStatusType = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> AssociateFirewallRuleGroupResponseTypeDef:
         """
         Associates a  FirewallRuleGroup with a VPC, to provide DNS filtering for the
         VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.associate_firewall_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#associate_firewall_rule_group)
@@ -263,15 +263,15 @@
         FirewallDomainListId: str,
         Priority: int,
         Action: ActionType,
         Name: str,
         BlockResponse: BlockResponseType = ...,
         BlockOverrideDomain: str = ...,
         BlockOverrideDnsType: Literal["CNAME"] = ...,
-        BlockOverrideTtl: int = ...
+        BlockOverrideTtl: int = ...,
     ) -> CreateFirewallRuleResponseTypeDef:
         """
         Creates a single DNS Firewall rule in the specified rule group, using the
         specified domain
         list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_firewall_rule)
@@ -293,15 +293,15 @@
         self,
         *,
         CreatorRequestId: str,
         Name: str,
         PreferredInstanceType: str,
         OutpostArn: str,
         InstanceCount: int = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateOutpostResolverResponseTypeDef:
         """
         Creates an Route 53 Resolver on an Outpost.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_outpost_resolver)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#create_outpost_resolver)
         """
@@ -313,30 +313,30 @@
         SecurityGroupIds: Sequence[str],
         Direction: ResolverEndpointDirectionType,
         IpAddresses: Sequence[IpAddressRequestTypeDef],
         Name: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ResolverEndpointType: ResolverEndpointTypeType = ...,
         OutpostArn: str = ...,
-        PreferredInstanceType: str = ...
+        PreferredInstanceType: str = ...,
     ) -> CreateResolverEndpointResponseTypeDef:
         """
         Creates a Resolver endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_resolver_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#create_resolver_endpoint)
         """
 
     async def create_resolver_query_log_config(
         self,
         *,
         Name: str,
         DestinationArn: str,
         CreatorRequestId: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateResolverQueryLogConfigResponseTypeDef:
         """
         Creates a Resolver query logging configuration, which defines where you want
         Resolver to save DNS query logs that originate in your
         VPCs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_resolver_query_log_config)
@@ -348,15 +348,15 @@
         *,
         CreatorRequestId: str,
         RuleType: RuleTypeOptionType,
         DomainName: str,
         Name: str = ...,
         TargetIps: Sequence[TargetAddressTypeDef] = ...,
         ResolverEndpointId: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateResolverRuleResponseTypeDef:
         """
         For DNS queries that originate in your VPCs, specifies which Resolver endpoint
         the queries pass through, one domain name that you want to forward to your
         network, and the IP addresses of the DNS resolvers in your
         network.
 
@@ -695,15 +695,15 @@
         self,
         *,
         FirewallRuleGroupId: str = ...,
         VpcId: str = ...,
         Priority: int = ...,
         Status: FirewallRuleGroupAssociationStatusType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListFirewallRuleGroupAssociationsResponseTypeDef:
         """
         Retrieves the firewall rule group associations that you have defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_firewall_rule_group_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#list_firewall_rule_group_associations)
         """
@@ -722,15 +722,15 @@
     async def list_firewall_rules(
         self,
         *,
         FirewallRuleGroupId: str,
         Priority: int = ...,
         Action: ActionType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListFirewallRulesResponseTypeDef:
         """
         Retrieves the firewall rules that you have defined for the specified firewall
         rule
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_firewall_rules)
@@ -796,15 +796,15 @@
     async def list_resolver_query_log_config_associations(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         SortBy: str = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListResolverQueryLogConfigAssociationsResponseTypeDef:
         """
         Lists information about associations between Amazon VPCs and query logging
         configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_resolver_query_log_config_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#list_resolver_query_log_config_associations)
@@ -813,15 +813,15 @@
     async def list_resolver_query_log_configs(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         SortBy: str = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListResolverQueryLogConfigsResponseTypeDef:
         """
         Lists information about the specified query logging configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_resolver_query_log_configs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#list_resolver_query_log_configs)
         """
@@ -927,15 +927,15 @@
         """
 
     async def update_firewall_domains(
         self,
         *,
         FirewallDomainListId: str,
         Operation: FirewallDomainUpdateOperationType,
-        Domains: Sequence[str]
+        Domains: Sequence[str],
     ) -> UpdateFirewallDomainsResponseTypeDef:
         """
         Updates the firewall domain list from an array of domain specifications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_firewall_domains)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#update_firewall_domains)
         """
@@ -947,45 +947,45 @@
         FirewallDomainListId: str,
         Priority: int = ...,
         Action: ActionType = ...,
         BlockResponse: BlockResponseType = ...,
         BlockOverrideDomain: str = ...,
         BlockOverrideDnsType: Literal["CNAME"] = ...,
         BlockOverrideTtl: int = ...,
-        Name: str = ...
+        Name: str = ...,
     ) -> UpdateFirewallRuleResponseTypeDef:
         """
         Updates the specified firewall rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_firewall_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#update_firewall_rule)
         """
 
     async def update_firewall_rule_group_association(
         self,
         *,
         FirewallRuleGroupAssociationId: str,
         Priority: int = ...,
         MutationProtection: MutationProtectionStatusType = ...,
-        Name: str = ...
+        Name: str = ...,
     ) -> UpdateFirewallRuleGroupAssociationResponseTypeDef:
         """
         Changes the association of a  FirewallRuleGroup with a VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_firewall_rule_group_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#update_firewall_rule_group_association)
         """
 
     async def update_outpost_resolver(
         self,
         *,
         Id: str,
         Name: str = ...,
         InstanceCount: int = ...,
-        PreferredInstanceType: str = ...
+        PreferredInstanceType: str = ...,
     ) -> UpdateOutpostResolverResponseTypeDef:
         """
         You can use `UpdateOutpostResolver` to update the instance count, type, or name
         of a Resolver on an
         Outpost.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_outpost_resolver)
@@ -1016,15 +1016,15 @@
 
     async def update_resolver_endpoint(
         self,
         *,
         ResolverEndpointId: str,
         Name: str = ...,
         ResolverEndpointType: ResolverEndpointTypeType = ...,
-        UpdateIpAddresses: Sequence[UpdateIpAddressTypeDef] = ...
+        UpdateIpAddresses: Sequence[UpdateIpAddressTypeDef] = ...,
     ) -> UpdateResolverEndpointResponseTypeDef:
         """
         Updates the name, or enpoint type for an inbound or an outbound Resolver
         endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_resolver_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#update_resolver_endpoint)
```

### Comparing `types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver/literals.py` & `types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver/literals.py`

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
     "ActionType",
     "AutodefinedReverseFlagType",
     "BlockOverrideDnsTypeType",
     "BlockResponseType",
     "FirewallDomainImportOperationType",
     "FirewallDomainListStatusType",
@@ -67,15 +66,14 @@
     "Route53ResolverServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ActionType = Literal["ALERT", "ALLOW", "BLOCK"]
 AutodefinedReverseFlagType = Literal["DISABLE", "ENABLE", "USE_LOCAL_RESOURCE_SETTING"]
 BlockOverrideDnsTypeType = Literal["CNAME"]
 BlockResponseType = Literal["NODATA", "NXDOMAIN", "OVERRIDE"]
 FirewallDomainImportOperationType = Literal["REPLACE"]
 FirewallDomainListStatusType = Literal[
     "COMPLETE", "COMPLETE_IMPORT_FAILED", "DELETING", "IMPORTING", "UPDATING"
```

### Comparing `types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver/literals.pyi` & `types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver/paginator.py` & `types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,14 @@
     "ListResolverQueryLogConfigAssociationsPaginator",
     "ListResolverQueryLogConfigsPaginator",
     "ListResolverRuleAssociationsPaginator",
     "ListResolverRulesPaginator",
     "ListTagsForResourcePaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -162,15 +161,15 @@
     def paginate(
         self,
         *,
         FirewallRuleGroupId: str = ...,
         VpcId: str = ...,
         Priority: int = ...,
         Status: FirewallRuleGroupAssociationStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFirewallRuleGroupAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallRuleGroupAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/paginators/#listfirewallrulegroupassociationspaginator)
         """
 
 
@@ -197,15 +196,15 @@
 
     def paginate(
         self,
         *,
         FirewallRuleGroupId: str,
         Priority: int = ...,
         Action: ActionType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFirewallRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/paginators/#listfirewallrulespaginator)
         """
 
 
@@ -245,15 +244,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/paginators/#listresolverdnssecconfigspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResolverDnssecConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverDnssecConfigs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/paginators/#listresolverdnssecconfigspaginator)
         """
 
 
@@ -278,15 +277,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/paginators/#listresolverendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResolverEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverEndpoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/paginators/#listresolverendpointspaginator)
         """
 
 
@@ -298,15 +297,15 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResolverQueryLogConfigAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverQueryLogConfigAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/paginators/#listresolverquerylogconfigassociationspaginator)
         """
 
 
@@ -318,15 +317,15 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResolverQueryLogConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverQueryLogConfigs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/paginators/#listresolverquerylogconfigspaginator)
         """
 
 
@@ -336,15 +335,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/paginators/#listresolverruleassociationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResolverRuleAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverRuleAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/paginators/#listresolverruleassociationspaginator)
         """
 
 
@@ -354,15 +353,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/paginators/#listresolverrulespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResolverRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/paginators/#listresolverrulespaginator)
         """
```

### Comparing `types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver/paginator.pyi` & `types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
     def paginate(
         self,
         *,
         FirewallRuleGroupId: str = ...,
         VpcId: str = ...,
         Priority: int = ...,
         Status: FirewallRuleGroupAssociationStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFirewallRuleGroupAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallRuleGroupAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/paginators/#listfirewallrulegroupassociationspaginator)
         """
 
 class ListFirewallRuleGroupsPaginator(AioPaginator):
@@ -189,15 +189,15 @@
 
     def paginate(
         self,
         *,
         FirewallRuleGroupId: str,
         Priority: int = ...,
         Action: ActionType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFirewallRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/paginators/#listfirewallrulespaginator)
         """
 
 class ListOutpostResolversPaginator(AioPaginator):
@@ -234,15 +234,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/paginators/#listresolverdnssecconfigspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResolverDnssecConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverDnssecConfigs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/paginators/#listresolverdnssecconfigspaginator)
         """
 
 class ListResolverEndpointIpAddressesPaginator(AioPaginator):
@@ -265,15 +265,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/paginators/#listresolverendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResolverEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverEndpoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/paginators/#listresolverendpointspaginator)
         """
 
 class ListResolverQueryLogConfigAssociationsPaginator(AioPaginator):
@@ -284,15 +284,15 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResolverQueryLogConfigAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverQueryLogConfigAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/paginators/#listresolverquerylogconfigassociationspaginator)
         """
 
 class ListResolverQueryLogConfigsPaginator(AioPaginator):
@@ -303,15 +303,15 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResolverQueryLogConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverQueryLogConfigs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/paginators/#listresolverquerylogconfigspaginator)
         """
 
 class ListResolverRuleAssociationsPaginator(AioPaginator):
@@ -320,15 +320,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/paginators/#listresolverruleassociationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResolverRuleAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverRuleAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/paginators/#listresolverruleassociationspaginator)
         """
 
 class ListResolverRulesPaginator(AioPaginator):
@@ -337,15 +337,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/paginators/#listresolverrulespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResolverRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/paginators/#listresolverrulespaginator)
         """
 
 class ListTagsForResourcePaginator(AioPaginator):
```

### Comparing `types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver/type_defs.py` & `types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TagTypeDef",
     "FirewallRuleGroupAssociationTypeDef",
     "ResponseMetadataTypeDef",
     "IpAddressUpdateTypeDef",
     "ResolverEndpointTypeDef",
     "AssociateResolverQueryLogConfigRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver/type_defs.pyi` & `types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver.egg-info/PKG-INFO` & `types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-route53resolver
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Route53Resolver 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Route53Resolver 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/
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
 
 <a id="types-aiobotocore-route53resolver"></a>
 
 # types-aiobotocore-route53resolver
 
 [![PyPI - types-aiobotocore-route53resolver](https://img.shields.io/pypi/v/types-aiobotocore-route53resolver.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53resolver)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53resolver.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53resolver)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53resolver)](https://pepy.tech/project/types-aiobotocore-route53resolver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Route53Resolver 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
+[aiobotocore.Route53Resolver 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
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
 [types-aiobotocore-route53resolver docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-route53resolver-2.9.0/types_aiobotocore_route53resolver.egg-info/SOURCES.txt` & `types-aiobotocore-route53resolver-2.9.1/types_aiobotocore_route53resolver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

