# Comparing `tmp/mypy-boto3-cleanroomsml-1.34.0.tar.gz` & `tmp/mypy-boto3-cleanroomsml-1.34.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cleanroomsml-1.34.0.tar", last modified: Wed Dec 13 21:22:08 2023, max compression
+gzip compressed data, was "mypy-boto3-cleanroomsml-1.34.77.tar", last modified: Wed Apr  3 19:32:38 2024, max compression
```

## Comparing `mypy-boto3-cleanroomsml-1.34.0.tar` & `mypy-boto3-cleanroomsml-1.34.77.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:08.167149 mypy-boto3-cleanroomsml-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:06:41.000000 mypy-boto3-cleanroomsml-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13680 2023-12-13 21:22:08.167149 mypy-boto3-cleanroomsml-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12127 2023-12-13 21:06:41.000000 mypy-boto3-cleanroomsml-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:08.167149 mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml/
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2023-12-13 21:06:41.000000 mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2023-12-13 21:06:41.000000 mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      925 2023-12-13 21:06:41.000000 mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22396 2023-12-13 21:06:41.000000 mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    22392 2023-12-13 21:06:41.000000 mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10453 2023-12-13 21:06:41.000000 mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10451 2023-12-13 21:06:41.000000 mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6751 2023-12-13 21:06:41.000000 mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6744 2023-12-13 21:06:41.000000 mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:06:41.000000 mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    22502 2023-12-13 21:06:41.000000 mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22501 2023-12-13 21:06:41.000000 mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:06:41.000000 mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:08.167149 mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13680 2023-12-13 21:22:08.000000 mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      775 2023-12-13 21:22:08.000000 mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:08.000000 mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:08.000000 mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:22:08.000000 mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-13 21:22:08.000000 mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:22:08.167149 mypy-boto3-cleanroomsml-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2023-12-13 21:06:41.000000 mypy-boto3-cleanroomsml-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:38.176163 mypy-boto3-cleanroomsml-1.34.77/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-03 19:31:57.000000 mypy-boto3-cleanroomsml-1.34.77/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13703 2024-04-03 19:32:38.176163 mypy-boto3-cleanroomsml-1.34.77/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12128 2024-04-03 19:31:57.000000 mypy-boto3-cleanroomsml-1.34.77/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:38.176163 mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml/
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-03 19:31:57.000000 mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-03 19:31:57.000000 mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-03 19:31:57.000000 mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22377 2024-04-03 19:31:58.000000 mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22374 2024-04-03 19:31:57.000000 mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-04-03 19:31:58.000000 mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-04-03 19:31:58.000000 mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-04-03 19:31:58.000000 mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-04-03 19:31:58.000000 mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:31:57.000000 mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    22241 2024-04-03 19:31:58.000000 mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22241 2024-04-03 19:31:58.000000 mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-03 19:31:57.000000 mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:38.176163 mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13703 2024-04-03 19:32:38.000000 mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-03 19:32:38.000000 mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:32:38.000000 mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:32:38.000000 mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 19:32:38.000000 mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 19:32:38.000000 mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:32:38.176163 mypy-boto3-cleanroomsml-1.34.77/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-03 19:31:57.000000 mypy-boto3-cleanroomsml-1.34.77/setup.py
```

### Comparing `mypy-boto3-cleanroomsml-1.34.0/LICENSE` & `mypy-boto3-cleanroomsml-1.34.77/LICENSE`

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

### Comparing `mypy-boto3-cleanroomsml-1.34.0/PKG-INFO` & `mypy-boto3-cleanroomsml-1.34.77/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cleanroomsml
-Version: 1.34.0
-Summary: Type annotations for boto3.CleanRoomsML 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.77
+Summary: Type annotations for boto3.CleanRoomsML 1.34.77 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanroomsml/
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
 
 <a id="mypy-boto3-cleanroomsml"></a>
 
 # mypy-boto3-cleanroomsml
 
 [![PyPI - mypy-boto3-cleanroomsml](https://img.shields.io/pypi/v/mypy-boto3-cleanroomsml.svg?color=blue)](https://pypi.org/project/mypy-boto3-cleanroomsml)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cleanroomsml.svg?color=blue)](https://pypi.org/project/mypy-boto3-cleanroomsml)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanroomsml/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cleanroomsml)](https://pepy.tech/project/mypy-boto3-cleanroomsml)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CleanRoomsML 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML)
+[boto3.CleanRoomsML 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cleanroomsml docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanroomsml/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cleanroomsml-1.34.0/README.md` & `mypy-boto3-cleanroomsml-1.34.77/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cleanroomsml.svg?color=blue)](https://pypi.org/project/mypy-boto3-cleanroomsml)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanroomsml/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cleanroomsml)](https://pepy.tech/project/mypy-boto3-cleanroomsml)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CleanRoomsML 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML)
+[boto3.CleanRoomsML 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cleanroomsml docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanroomsml/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml/__init__.py` & `mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     ListAudienceModelsPaginator,
     ListConfiguredAudienceModelsPaginator,
     ListTrainingDatasetsPaginator,
 )
 
 Client = CleanRoomsMLClient
 
-
 __all__ = (
     "CleanRoomsMLClient",
     "Client",
     "ListAudienceExportJobsPaginator",
     "ListAudienceGenerationJobsPaginator",
     "ListAudienceModelsPaginator",
     "ListConfiguredAudienceModelsPaginator",
```

### Comparing `mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml/__init__.pyi` & `mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml/__main__.py` & `mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CleanRoomsML 1.34.0\nVersion:         1.34.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanroomsml//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.CleanRoomsML 1.34.77\n"
+        "Version:         1.34.77\n"
+        "Builder version: 7.23.2\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanroomsml//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.0")
+    print("1.34.77")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml/client.py` & `mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CleanRoomsMLClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -118,15 +117,15 @@
         *,
         name: str,
         trainingDatasetArn: str,
         description: str = ...,
         kmsKeyArn: str = ...,
         tags: Mapping[str, str] = ...,
         trainingDataEndTime: TimestampTypeDef = ...,
-        trainingDataStartTime: TimestampTypeDef = ...
+        trainingDataStartTime: TimestampTypeDef = ...,
     ) -> CreateAudienceModelResponseTypeDef:
         """
         Defines the information necessary to create an audience model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.create_audience_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanroomsml/client/#create_audience_model)
         """
@@ -138,15 +137,15 @@
         name: str,
         outputConfig: ConfiguredAudienceModelOutputConfigTypeDef,
         sharedAudienceMetrics: Sequence[SharedAudienceMetricsType],
         audienceSizeConfig: AudienceSizeConfigTypeDef = ...,
         childResourceTagOnCreatePolicy: TagOnCreatePolicyType = ...,
         description: str = ...,
         minMatchingSeedSize: int = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateConfiguredAudienceModelResponseTypeDef:
         """
         Defines the information necessary to create a configured audience model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.create_configured_audience_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanroomsml/client/#create_configured_audience_model)
         """
@@ -154,19 +153,18 @@
     def create_training_dataset(
         self,
         *,
         name: str,
         roleArn: str,
         trainingData: Sequence[DatasetTypeDef],
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateTrainingDatasetResponseTypeDef:
         """
-        Defines the information necessary to create a training dataset, or seed
-        audience.
+        Defines the information necessary to create a training dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.create_training_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanroomsml/client/#create_training_dataset)
         """
 
     def delete_audience_generation_job(
         self, *, audienceGenerationJobArn: str
@@ -289,15 +287,15 @@
 
     def list_audience_generation_jobs(
         self,
         *,
         collaborationId: str = ...,
         configuredAudienceModelArn: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListAudienceGenerationJobsResponseTypeDef:
         """
         Returns a list of audience generation jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.list_audience_generation_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanroomsml/client/#list_audience_generation_jobs)
         """
@@ -342,30 +340,30 @@
 
     def put_configured_audience_model_policy(
         self,
         *,
         configuredAudienceModelArn: str,
         configuredAudienceModelPolicy: str,
         policyExistenceCondition: PolicyExistenceConditionType = ...,
-        previousPolicyHash: str = ...
+        previousPolicyHash: str = ...,
     ) -> PutConfiguredAudienceModelPolicyResponseTypeDef:
         """
         Create or update the resource policy for a configured audience model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.put_configured_audience_model_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanroomsml/client/#put_configured_audience_model_policy)
         """
 
     def start_audience_export_job(
         self,
         *,
         audienceGenerationJobArn: str,
         audienceSize: AudienceSizeTypeDef,
         name: str,
-        description: str = ...
+        description: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Export an audience of a specified size after you have generated an audience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.start_audience_export_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanroomsml/client/#start_audience_export_job)
         """
@@ -375,15 +373,15 @@
         *,
         configuredAudienceModelArn: str,
         name: str,
         seedAudience: AudienceGenerationJobDataSourceTypeDef,
         collaborationId: str = ...,
         description: str = ...,
         includeSeedInOutput: bool = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> StartAudienceGenerationJobResponseTypeDef:
         """
         Information necessary to start the audience generation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.start_audience_generation_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanroomsml/client/#start_audience_generation_job)
         """
@@ -409,15 +407,15 @@
         *,
         configuredAudienceModelArn: str,
         audienceModelArn: str = ...,
         audienceSizeConfig: AudienceSizeConfigTypeDef = ...,
         description: str = ...,
         minMatchingSeedSize: int = ...,
         outputConfig: ConfiguredAudienceModelOutputConfigTypeDef = ...,
-        sharedAudienceMetrics: Sequence[SharedAudienceMetricsType] = ...
+        sharedAudienceMetrics: Sequence[SharedAudienceMetricsType] = ...,
     ) -> UpdateConfiguredAudienceModelResponseTypeDef:
         """
         Provides the information necessary to update a configured audience model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.update_configured_audience_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanroomsml/client/#update_configured_audience_model)
         """
```

### Comparing `mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml/client.pyi` & `mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         *,
         name: str,
         trainingDatasetArn: str,
         description: str = ...,
         kmsKeyArn: str = ...,
         tags: Mapping[str, str] = ...,
         trainingDataEndTime: TimestampTypeDef = ...,
-        trainingDataStartTime: TimestampTypeDef = ...
+        trainingDataStartTime: TimestampTypeDef = ...,
     ) -> CreateAudienceModelResponseTypeDef:
         """
         Defines the information necessary to create an audience model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.create_audience_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanroomsml/client/#create_audience_model)
         """
@@ -134,15 +134,15 @@
         name: str,
         outputConfig: ConfiguredAudienceModelOutputConfigTypeDef,
         sharedAudienceMetrics: Sequence[SharedAudienceMetricsType],
         audienceSizeConfig: AudienceSizeConfigTypeDef = ...,
         childResourceTagOnCreatePolicy: TagOnCreatePolicyType = ...,
         description: str = ...,
         minMatchingSeedSize: int = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateConfiguredAudienceModelResponseTypeDef:
         """
         Defines the information necessary to create a configured audience model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.create_configured_audience_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanroomsml/client/#create_configured_audience_model)
         """
@@ -150,19 +150,18 @@
     def create_training_dataset(
         self,
         *,
         name: str,
         roleArn: str,
         trainingData: Sequence[DatasetTypeDef],
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateTrainingDatasetResponseTypeDef:
         """
-        Defines the information necessary to create a training dataset, or seed
-        audience.
+        Defines the information necessary to create a training dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.create_training_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanroomsml/client/#create_training_dataset)
         """
 
     def delete_audience_generation_job(
         self, *, audienceGenerationJobArn: str
@@ -285,15 +284,15 @@
 
     def list_audience_generation_jobs(
         self,
         *,
         collaborationId: str = ...,
         configuredAudienceModelArn: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListAudienceGenerationJobsResponseTypeDef:
         """
         Returns a list of audience generation jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.list_audience_generation_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanroomsml/client/#list_audience_generation_jobs)
         """
@@ -338,30 +337,30 @@
 
     def put_configured_audience_model_policy(
         self,
         *,
         configuredAudienceModelArn: str,
         configuredAudienceModelPolicy: str,
         policyExistenceCondition: PolicyExistenceConditionType = ...,
-        previousPolicyHash: str = ...
+        previousPolicyHash: str = ...,
     ) -> PutConfiguredAudienceModelPolicyResponseTypeDef:
         """
         Create or update the resource policy for a configured audience model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.put_configured_audience_model_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanroomsml/client/#put_configured_audience_model_policy)
         """
 
     def start_audience_export_job(
         self,
         *,
         audienceGenerationJobArn: str,
         audienceSize: AudienceSizeTypeDef,
         name: str,
-        description: str = ...
+        description: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Export an audience of a specified size after you have generated an audience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.start_audience_export_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanroomsml/client/#start_audience_export_job)
         """
@@ -371,15 +370,15 @@
         *,
         configuredAudienceModelArn: str,
         name: str,
         seedAudience: AudienceGenerationJobDataSourceTypeDef,
         collaborationId: str = ...,
         description: str = ...,
         includeSeedInOutput: bool = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> StartAudienceGenerationJobResponseTypeDef:
         """
         Information necessary to start the audience generation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.start_audience_generation_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanroomsml/client/#start_audience_generation_job)
         """
@@ -405,15 +404,15 @@
         *,
         configuredAudienceModelArn: str,
         audienceModelArn: str = ...,
         audienceSizeConfig: AudienceSizeConfigTypeDef = ...,
         description: str = ...,
         minMatchingSeedSize: int = ...,
         outputConfig: ConfiguredAudienceModelOutputConfigTypeDef = ...,
-        sharedAudienceMetrics: Sequence[SharedAudienceMetricsType] = ...
+        sharedAudienceMetrics: Sequence[SharedAudienceMetricsType] = ...,
     ) -> UpdateConfiguredAudienceModelResponseTypeDef:
         """
         Provides the information necessary to update a configured audience model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.update_configured_audience_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanroomsml/client/#update_configured_audience_model)
         """
```

### Comparing `mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml/literals.py` & `mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,19 +15,17 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AudienceExportJobStatusType",
     "AudienceGenerationJobStatusType",
-    "AudienceModelMetricTypeType",
     "AudienceModelStatusType",
     "AudienceSizeTypeType",
     "ColumnTypeType",
     "ConfiguredAudienceModelStatusType",
     "DatasetTypeType",
     "ListAudienceExportJobsPaginatorName",
     "ListAudienceGenerationJobsPaginatorName",
@@ -40,30 +38,26 @@
     "TrainingDatasetStatusType",
     "CleanRoomsMLServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 AudienceExportJobStatusType = Literal[
     "ACTIVE", "CREATE_FAILED", "CREATE_IN_PROGRESS", "CREATE_PENDING"
 ]
 AudienceGenerationJobStatusType = Literal[
     "ACTIVE",
     "CREATE_FAILED",
     "CREATE_IN_PROGRESS",
     "CREATE_PENDING",
     "DELETE_FAILED",
     "DELETE_IN_PROGRESS",
     "DELETE_PENDING",
 ]
-AudienceModelMetricTypeType = Literal[
-    "MEAN_RECIPROCAL_RANK", "NORMALIZED_DISCOUNTED_CUMULATIVE_GAIN", "PRECISION", "RECALL"
-]
 AudienceModelStatusType = Literal[
     "ACTIVE",
     "CREATE_FAILED",
     "CREATE_IN_PROGRESS",
     "CREATE_PENDING",
     "DELETE_FAILED",
     "DELETE_IN_PROGRESS",
@@ -107,14 +101,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -125,14 +120,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -150,14 +146,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -180,14 +177,15 @@
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -248,15 +246,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -328,17 +325,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -428,19 +427,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml/literals.pyi` & `mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml/literals.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AudienceExportJobStatusType",
     "AudienceGenerationJobStatusType",
-    "AudienceModelMetricTypeType",
     "AudienceModelStatusType",
     "AudienceSizeTypeType",
     "ColumnTypeType",
     "ConfiguredAudienceModelStatusType",
     "DatasetTypeType",
     "ListAudienceExportJobsPaginatorName",
     "ListAudienceGenerationJobsPaginatorName",
@@ -51,17 +50,14 @@
     "CREATE_FAILED",
     "CREATE_IN_PROGRESS",
     "CREATE_PENDING",
     "DELETE_FAILED",
     "DELETE_IN_PROGRESS",
     "DELETE_PENDING",
 ]
-AudienceModelMetricTypeType = Literal[
-    "MEAN_RECIPROCAL_RANK", "NORMALIZED_DISCOUNTED_CUMULATIVE_GAIN", "PRECISION", "RECALL"
-]
 AudienceModelStatusType = Literal[
     "ACTIVE",
     "CREATE_FAILED",
     "CREATE_IN_PROGRESS",
     "CREATE_PENDING",
     "DELETE_FAILED",
     "DELETE_IN_PROGRESS",
@@ -105,14 +101,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -123,14 +120,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -148,14 +146,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -178,14 +177,15 @@
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -246,15 +246,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -326,17 +325,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -426,19 +427,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml/paginator.py` & `mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     "ListAudienceExportJobsPaginator",
     "ListAudienceGenerationJobsPaginator",
     "ListAudienceModelsPaginator",
     "ListConfiguredAudienceModelsPaginator",
     "ListTrainingDatasetsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -82,15 +81,15 @@
     """
 
     def paginate(
         self,
         *,
         collaborationId: str = ...,
         configuredAudienceModelArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListAudienceGenerationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Paginator.ListAudienceGenerationJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanroomsml/paginators/#listaudiencegenerationjobspaginator)
         """
```

### Comparing `mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml/paginator.pyi` & `mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     """
 
     def paginate(
         self,
         *,
         collaborationId: str = ...,
         configuredAudienceModelArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListAudienceGenerationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Paginator.ListAudienceGenerationJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanroomsml/paginators/#listaudiencegenerationjobspaginator)
         """
 
 class ListAudienceModelsPaginator(Paginator):
```

### Comparing `mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml/type_defs.py` & `mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AudienceExportJobStatusType,
     AudienceGenerationJobStatusType,
-    AudienceModelMetricTypeType,
     AudienceModelStatusType,
     AudienceSizeTypeType,
     ColumnTypeType,
     PolicyExistenceConditionType,
     SharedAudienceMetricsType,
     TagOnCreatePolicyType,
 )
@@ -37,21 +36,19 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "S3ConfigMapTypeDef",
     "AudienceSizeTypeDef",
     "StatusDetailsTypeDef",
     "AudienceGenerationJobSummaryTypeDef",
-    "AudienceModelMetricTypeDef",
     "AudienceModelSummaryTypeDef",
     "AudienceSizeConfigTypeDef",
     "ColumnSchemaTypeDef",
     "TimestampTypeDef",
     "ResponseMetadataTypeDef",
     "GlueDataSourceTypeDef",
     "DeleteAudienceGenerationJobRequestRequestTypeDef",
@@ -146,22 +143,14 @@
         "status": AudienceGenerationJobStatusType,
         "updateTime": datetime,
         "collaborationId": NotRequired[str],
         "description": NotRequired[str],
         "startedBy": NotRequired[str],
     },
 )
-AudienceModelMetricTypeDef = TypedDict(
-    "AudienceModelMetricTypeDef",
-    {
-        "forTopKItemPredictions": int,
-        "type": AudienceModelMetricTypeType,
-        "value": float,
-    },
-)
 AudienceModelSummaryTypeDef = TypedDict(
     "AudienceModelSummaryTypeDef",
     {
         "audienceModelArn": str,
         "createTime": datetime,
         "name": str,
         "status": AudienceModelStatusType,
@@ -185,18 +174,18 @@
     },
 )
 TimestampTypeDef = Union[datetime, str]
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 GlueDataSourceTypeDef = TypedDict(
     "GlueDataSourceTypeDef",
     {
         "databaseName": str,
         "tableName": str,
@@ -434,15 +423,14 @@
 GetAudienceModelResponseTypeDef = TypedDict(
     "GetAudienceModelResponseTypeDef",
     {
         "audienceModelArn": str,
         "createTime": datetime,
         "description": str,
         "kmsKeyArn": str,
-        "metrics": List[AudienceModelMetricTypeDef],
         "name": str,
         "status": AudienceModelStatusType,
         "statusDetails": StatusDetailsTypeDef,
         "tags": Dict[str, str],
         "trainingDataEndTime": datetime,
         "trainingDataStartTime": datetime,
         "trainingDatasetArn": str,
@@ -570,14 +558,15 @@
         "tags": NotRequired[Mapping[str, str]],
     },
 )
 AudienceQualityMetricsTypeDef = TypedDict(
     "AudienceQualityMetricsTypeDef",
     {
         "relevanceMetrics": List[RelevanceMetricTypeDef],
+        "recallMetric": NotRequired[float],
     },
 )
 ListAudienceExportJobsResponseTypeDef = TypedDict(
     "ListAudienceExportJobsResponseTypeDef",
     {
         "audienceExportJobs": List[AudienceExportJobSummaryTypeDef],
         "nextToken": str,
```

### Comparing `mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml/type_defs.pyi` & `mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AudienceExportJobStatusType,
     AudienceGenerationJobStatusType,
-    AudienceModelMetricTypeType,
     AudienceModelStatusType,
     AudienceSizeTypeType,
     ColumnTypeType,
     PolicyExistenceConditionType,
     SharedAudienceMetricsType,
     TagOnCreatePolicyType,
 )
@@ -42,15 +41,14 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "S3ConfigMapTypeDef",
     "AudienceSizeTypeDef",
     "StatusDetailsTypeDef",
     "AudienceGenerationJobSummaryTypeDef",
-    "AudienceModelMetricTypeDef",
     "AudienceModelSummaryTypeDef",
     "AudienceSizeConfigTypeDef",
     "ColumnSchemaTypeDef",
     "TimestampTypeDef",
     "ResponseMetadataTypeDef",
     "GlueDataSourceTypeDef",
     "DeleteAudienceGenerationJobRequestRequestTypeDef",
@@ -145,22 +143,14 @@
         "status": AudienceGenerationJobStatusType,
         "updateTime": datetime,
         "collaborationId": NotRequired[str],
         "description": NotRequired[str],
         "startedBy": NotRequired[str],
     },
 )
-AudienceModelMetricTypeDef = TypedDict(
-    "AudienceModelMetricTypeDef",
-    {
-        "forTopKItemPredictions": int,
-        "type": AudienceModelMetricTypeType,
-        "value": float,
-    },
-)
 AudienceModelSummaryTypeDef = TypedDict(
     "AudienceModelSummaryTypeDef",
     {
         "audienceModelArn": str,
         "createTime": datetime,
         "name": str,
         "status": AudienceModelStatusType,
@@ -184,18 +174,18 @@
     },
 )
 TimestampTypeDef = Union[datetime, str]
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 GlueDataSourceTypeDef = TypedDict(
     "GlueDataSourceTypeDef",
     {
         "databaseName": str,
         "tableName": str,
@@ -433,15 +423,14 @@
 GetAudienceModelResponseTypeDef = TypedDict(
     "GetAudienceModelResponseTypeDef",
     {
         "audienceModelArn": str,
         "createTime": datetime,
         "description": str,
         "kmsKeyArn": str,
-        "metrics": List[AudienceModelMetricTypeDef],
         "name": str,
         "status": AudienceModelStatusType,
         "statusDetails": StatusDetailsTypeDef,
         "tags": Dict[str, str],
         "trainingDataEndTime": datetime,
         "trainingDataStartTime": datetime,
         "trainingDatasetArn": str,
@@ -569,14 +558,15 @@
         "tags": NotRequired[Mapping[str, str]],
     },
 )
 AudienceQualityMetricsTypeDef = TypedDict(
     "AudienceQualityMetricsTypeDef",
     {
         "relevanceMetrics": List[RelevanceMetricTypeDef],
+        "recallMetric": NotRequired[float],
     },
 )
 ListAudienceExportJobsResponseTypeDef = TypedDict(
     "ListAudienceExportJobsResponseTypeDef",
     {
         "audienceExportJobs": List[AudienceExportJobSummaryTypeDef],
         "nextToken": str,
```

### Comparing `mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml.egg-info/PKG-INFO` & `mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cleanroomsml
-Version: 1.34.0
-Summary: Type annotations for boto3.CleanRoomsML 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.77
+Summary: Type annotations for boto3.CleanRoomsML 1.34.77 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanroomsml/
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
 
 <a id="mypy-boto3-cleanroomsml"></a>
 
 # mypy-boto3-cleanroomsml
 
 [![PyPI - mypy-boto3-cleanroomsml](https://img.shields.io/pypi/v/mypy-boto3-cleanroomsml.svg?color=blue)](https://pypi.org/project/mypy-boto3-cleanroomsml)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cleanroomsml.svg?color=blue)](https://pypi.org/project/mypy-boto3-cleanroomsml)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanroomsml/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cleanroomsml)](https://pepy.tech/project/mypy-boto3-cleanroomsml)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CleanRoomsML 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML)
+[boto3.CleanRoomsML 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cleanroomsml docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanroomsml/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cleanroomsml-1.34.0/mypy_boto3_cleanroomsml.egg-info/SOURCES.txt` & `mypy-boto3-cleanroomsml-1.34.77/mypy_boto3_cleanroomsml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanroomsml-1.34.0/setup.py` & `mypy-boto3-cleanroomsml-1.34.77/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,48 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cleanroomsml",
-    version="1.34.0",
+    version="1.34.77",
     packages=["mypy_boto3_cleanroomsml"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.CleanRoomsML 1.34.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
-    ),
+    description="Type annotations for boto3.CleanRoomsML 1.34.77 service generated with mypy-boto3-builder 7.23.2",
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
     keywords="boto3 cleanroomsml type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_cleanroomsml": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanroomsml/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

