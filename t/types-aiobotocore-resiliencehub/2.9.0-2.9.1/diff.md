# Comparing `tmp/types-aiobotocore-resiliencehub-2.9.0.tar.gz` & `tmp/types-aiobotocore-resiliencehub-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-resiliencehub-2.9.0.tar", last modified: Wed Dec 13 20:00:17 2023, max compression
+gzip compressed data, was "types-aiobotocore-resiliencehub-2.9.1.tar", last modified: Thu Jan 18 01:21:37 2024, max compression
```

## Comparing `types-aiobotocore-resiliencehub-2.9.0.tar` & `types-aiobotocore-resiliencehub-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:17.749247 types-aiobotocore-resiliencehub-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:54:38.000000 types-aiobotocore-resiliencehub-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12541 2023-12-13 20:00:17.749247 types-aiobotocore-resiliencehub-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10954 2023-12-13 19:54:38.000000 types-aiobotocore-resiliencehub-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:17.753248 types-aiobotocore-resiliencehub-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2023-12-13 19:54:38.000000 types-aiobotocore-resiliencehub-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:17.749247 types-aiobotocore-resiliencehub-2.9.0/types_aiobotocore_resiliencehub/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2023-12-13 19:54:38.000000 types-aiobotocore-resiliencehub-2.9.0/types_aiobotocore_resiliencehub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2023-12-13 19:54:38.000000 types-aiobotocore-resiliencehub-2.9.0/types_aiobotocore_resiliencehub/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      956 2023-12-13 19:54:38.000000 types-aiobotocore-resiliencehub-2.9.0/types_aiobotocore_resiliencehub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44100 2023-12-13 19:54:38.000000 types-aiobotocore-resiliencehub-2.9.0/types_aiobotocore_resiliencehub/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    44097 2023-12-13 19:54:38.000000 types-aiobotocore-resiliencehub-2.9.0/types_aiobotocore_resiliencehub/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12392 2023-12-13 19:54:38.000000 types-aiobotocore-resiliencehub-2.9.0/types_aiobotocore_resiliencehub/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    12390 2023-12-13 19:54:38.000000 types-aiobotocore-resiliencehub-2.9.0/types_aiobotocore_resiliencehub/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:54:38.000000 types-aiobotocore-resiliencehub-2.9.0/types_aiobotocore_resiliencehub/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    53362 2023-12-13 19:54:39.000000 types-aiobotocore-resiliencehub-2.9.0/types_aiobotocore_resiliencehub/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    53361 2023-12-13 19:54:39.000000 types-aiobotocore-resiliencehub-2.9.0/types_aiobotocore_resiliencehub/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:54:38.000000 types-aiobotocore-resiliencehub-2.9.0/types_aiobotocore_resiliencehub/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:17.749247 types-aiobotocore-resiliencehub-2.9.0/types_aiobotocore_resiliencehub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12541 2023-12-13 20:00:17.000000 types-aiobotocore-resiliencehub-2.9.0/types_aiobotocore_resiliencehub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      836 2023-12-13 20:00:17.000000 types-aiobotocore-resiliencehub-2.9.0/types_aiobotocore_resiliencehub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:17.000000 types-aiobotocore-resiliencehub-2.9.0/types_aiobotocore_resiliencehub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:17.000000 types-aiobotocore-resiliencehub-2.9.0/types_aiobotocore_resiliencehub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:17.000000 types-aiobotocore-resiliencehub-2.9.0/types_aiobotocore_resiliencehub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-13 20:00:17.000000 types-aiobotocore-resiliencehub-2.9.0/types_aiobotocore_resiliencehub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:37.341086 types-aiobotocore-resiliencehub-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:16:10.000000 types-aiobotocore-resiliencehub-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12561 2024-01-18 01:21:37.341086 types-aiobotocore-resiliencehub-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10954 2024-01-18 01:16:10.000000 types-aiobotocore-resiliencehub-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:37.341086 types-aiobotocore-resiliencehub-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-01-18 01:16:10.000000 types-aiobotocore-resiliencehub-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:37.337086 types-aiobotocore-resiliencehub-2.9.1/types_aiobotocore_resiliencehub/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-01-18 01:16:10.000000 types-aiobotocore-resiliencehub-2.9.1/types_aiobotocore_resiliencehub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-01-18 01:16:10.000000 types-aiobotocore-resiliencehub-2.9.1/types_aiobotocore_resiliencehub/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-01-18 01:16:10.000000 types-aiobotocore-resiliencehub-2.9.1/types_aiobotocore_resiliencehub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44122 2024-01-18 01:16:11.000000 types-aiobotocore-resiliencehub-2.9.1/types_aiobotocore_resiliencehub/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44119 2024-01-18 01:16:11.000000 types-aiobotocore-resiliencehub-2.9.1/types_aiobotocore_resiliencehub/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12390 2024-01-18 01:16:11.000000 types-aiobotocore-resiliencehub-2.9.1/types_aiobotocore_resiliencehub/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12390 2024-01-18 01:16:11.000000 types-aiobotocore-resiliencehub-2.9.1/types_aiobotocore_resiliencehub/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:16:10.000000 types-aiobotocore-resiliencehub-2.9.1/types_aiobotocore_resiliencehub/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    53361 2024-01-18 01:16:15.000000 types-aiobotocore-resiliencehub-2.9.1/types_aiobotocore_resiliencehub/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53361 2024-01-18 01:16:15.000000 types-aiobotocore-resiliencehub-2.9.1/types_aiobotocore_resiliencehub/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:16:10.000000 types-aiobotocore-resiliencehub-2.9.1/types_aiobotocore_resiliencehub/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:37.341086 types-aiobotocore-resiliencehub-2.9.1/types_aiobotocore_resiliencehub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12561 2024-01-18 01:21:37.000000 types-aiobotocore-resiliencehub-2.9.1/types_aiobotocore_resiliencehub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-01-18 01:21:37.000000 types-aiobotocore-resiliencehub-2.9.1/types_aiobotocore_resiliencehub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:37.000000 types-aiobotocore-resiliencehub-2.9.1/types_aiobotocore_resiliencehub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:37.000000 types-aiobotocore-resiliencehub-2.9.1/types_aiobotocore_resiliencehub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:37.000000 types-aiobotocore-resiliencehub-2.9.1/types_aiobotocore_resiliencehub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-18 01:21:37.000000 types-aiobotocore-resiliencehub-2.9.1/types_aiobotocore_resiliencehub.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-resiliencehub-2.9.0/LICENSE` & `types-aiobotocore-resiliencehub-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-resiliencehub-2.9.0/PKG-INFO` & `types-aiobotocore-resiliencehub-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-resiliencehub
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ResilienceHub 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ResilienceHub 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/
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
 
 <a id="types-aiobotocore-resiliencehub"></a>
 
 # types-aiobotocore-resiliencehub
 
 [![PyPI - types-aiobotocore-resiliencehub](https://img.shields.io/pypi/v/types-aiobotocore-resiliencehub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resiliencehub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resiliencehub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resiliencehub)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-resiliencehub)](https://pepy.tech/project/types-aiobotocore-resiliencehub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ResilienceHub 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
+[aiobotocore.ResilienceHub 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
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
 [types-aiobotocore-resiliencehub docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-resiliencehub-2.9.0/README.md` & `types-aiobotocore-resiliencehub-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resiliencehub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resiliencehub)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-resiliencehub)](https://pepy.tech/project/types-aiobotocore-resiliencehub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ResilienceHub 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
+[aiobotocore.ResilienceHub 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
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
 [types-aiobotocore-resiliencehub docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-resiliencehub-2.9.0/setup.py` & `types-aiobotocore-resiliencehub-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-resiliencehub",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_resiliencehub"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ResilienceHub 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ResilienceHub 2.9.1 service generated with"
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
     keywords="aiobotocore resiliencehub type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_resiliencehub": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-resiliencehub-2.9.0/types_aiobotocore_resiliencehub/__main__.py` & `types-aiobotocore-resiliencehub-2.9.1/types_aiobotocore_resiliencehub/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ResilienceHub 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ResilienceHub 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub\nOther"
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

### Comparing `types-aiobotocore-resiliencehub-2.9.0/types_aiobotocore_resiliencehub/client.py` & `types-aiobotocore-resiliencehub-2.9.1/types_aiobotocore_resiliencehub/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#add_draft_app_version_resource_mappings)
         """
 
     async def batch_update_recommendation_status(
         self,
         *,
         appArn: str,
-        requestEntries: Sequence[UpdateRecommendationStatusRequestEntryTypeDef]
+        requestEntries: Sequence[UpdateRecommendationStatusRequestEntryTypeDef],
     ) -> BatchUpdateRecommendationStatusResponseTypeDef:
         """
         Enables you to include or exclude one or more operational recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.batch_update_recommendation_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#batch_update_recommendation_status)
         """
@@ -182,15 +182,15 @@
         name: str,
         assessmentSchedule: AppAssessmentScheduleTypeType = ...,
         clientToken: str = ...,
         description: str = ...,
         eventSubscriptions: Sequence[EventSubscriptionTypeDef] = ...,
         permissionModel: PermissionModelTypeDef = ...,
         policyArn: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateAppResponseTypeDef:
         """
         Creates an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#create_app)
         """
@@ -199,15 +199,15 @@
         self,
         *,
         appArn: str,
         name: str,
         type: str,
         additionalInfo: Mapping[str, Sequence[str]] = ...,
         clientToken: str = ...,
-        id: str = ...
+        id: str = ...,
     ) -> CreateAppVersionAppComponentResponseTypeDef:
         """
         Creates a new Application Component in the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_app_version_app_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#create_app_version_app_component)
         """
@@ -220,15 +220,15 @@
         logicalResourceId: LogicalResourceIdTypeDef,
         physicalResourceId: str,
         resourceType: str,
         additionalInfo: Mapping[str, Sequence[str]] = ...,
         awsAccountId: str = ...,
         awsRegion: str = ...,
         clientToken: str = ...,
-        resourceName: str = ...
+        resourceName: str = ...,
     ) -> CreateAppVersionResourceResponseTypeDef:
         """
         Adds a resource to the Resilience Hub application and assigns it to the
         specified Application
         Components.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_app_version_resource)
@@ -241,15 +241,15 @@
         assessmentArn: str,
         name: str,
         bucketName: str = ...,
         clientToken: str = ...,
         format: TemplateFormatType = ...,
         recommendationIds: Sequence[str] = ...,
         recommendationTypes: Sequence[RenderRecommendationTypeType] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateRecommendationTemplateResponseTypeDef:
         """
         Creates a new recommendation template for the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_recommendation_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#create_recommendation_template)
         """
@@ -259,15 +259,15 @@
         *,
         policy: Mapping[DisruptionTypeType, FailurePolicyTypeDef],
         policyName: str,
         tier: ResiliencyPolicyTierType,
         clientToken: str = ...,
         dataLocationConstraint: DataLocationConstraintType = ...,
         policyDescription: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateResiliencyPolicyResponseTypeDef:
         """
         Creates a resiliency policy for an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_resiliency_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#create_resiliency_policy)
         """
@@ -295,15 +295,15 @@
     async def delete_app_input_source(
         self,
         *,
         appArn: str,
         clientToken: str = ...,
         eksSourceClusterNamespace: EksSourceClusterNamespaceTypeDef = ...,
         sourceArn: str = ...,
-        terraformSource: TerraformSourceTypeDef = ...
+        terraformSource: TerraformSourceTypeDef = ...,
     ) -> DeleteAppInputSourceResponseTypeDef:
         """
         Deletes the input source and all of its imported resources from the Resilience
         Hub
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.delete_app_input_source)
@@ -325,15 +325,15 @@
         *,
         appArn: str,
         awsAccountId: str = ...,
         awsRegion: str = ...,
         clientToken: str = ...,
         logicalResourceId: LogicalResourceIdTypeDef = ...,
         physicalResourceId: str = ...,
-        resourceName: str = ...
+        resourceName: str = ...,
     ) -> DeleteAppVersionResourceResponseTypeDef:
         """
         Deletes a resource from the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.delete_app_version_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#delete_app_version_resource)
         """
@@ -401,15 +401,15 @@
         *,
         appArn: str,
         appVersion: str,
         awsAccountId: str = ...,
         awsRegion: str = ...,
         logicalResourceId: LogicalResourceIdTypeDef = ...,
         physicalResourceId: str = ...,
-        resourceName: str = ...
+        resourceName: str = ...,
     ) -> DescribeAppVersionResourceResponseTypeDef:
         """
         Describes a resource of the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.describe_app_version_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#describe_app_version_resource)
         """
@@ -473,15 +473,15 @@
     async def import_resources_to_draft_app_version(
         self,
         *,
         appArn: str,
         eksSources: Sequence[EksSourceTypeDef] = ...,
         importStrategy: ResourceImportStrategyTypeType = ...,
         sourceArns: Sequence[str] = ...,
-        terraformSources: Sequence[TerraformSourceTypeDef] = ...
+        terraformSources: Sequence[TerraformSourceTypeDef] = ...,
     ) -> ImportResourcesToDraftAppVersionResponseTypeDef:
         """
         Imports resources to Resilience Hub application draft version from different
         input
         sources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.import_resources_to_draft_app_version)
@@ -514,15 +514,15 @@
         appArn: str = ...,
         assessmentName: str = ...,
         assessmentStatus: Sequence[AssessmentStatusType] = ...,
         complianceStatus: ComplianceStatusType = ...,
         invoker: AssessmentInvokerType = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        reverseOrder: bool = ...
+        reverseOrder: bool = ...,
     ) -> ListAppAssessmentsResponseTypeDef:
         """
         Lists the assessments for an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_assessments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#list_app_assessments)
         """
@@ -580,15 +580,15 @@
     async def list_app_version_resources(
         self,
         *,
         appArn: str,
         appVersion: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        resolutionId: str = ...
+        resolutionId: str = ...,
     ) -> ListAppVersionResourcesResponseTypeDef:
         """
         Lists all the resources in an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_version_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#list_app_version_resources)
         """
@@ -596,15 +596,15 @@
     async def list_app_versions(
         self,
         *,
         appArn: str,
         endTime: TimestampTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        startTime: TimestampTypeDef = ...
+        startTime: TimestampTypeDef = ...,
     ) -> ListAppVersionsResponseTypeDef:
         """
         Lists the different versions for the Resilience Hub applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#list_app_versions)
         """
@@ -614,15 +614,15 @@
         *,
         appArn: str = ...,
         fromLastAssessmentTime: TimestampTypeDef = ...,
         maxResults: int = ...,
         name: str = ...,
         nextToken: str = ...,
         reverseOrder: bool = ...,
-        toLastAssessmentTime: TimestampTypeDef = ...
+        toLastAssessmentTime: TimestampTypeDef = ...,
     ) -> ListAppsResponseTypeDef:
         """
         Lists your Resilience Hub applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_apps)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#list_apps)
         """
@@ -632,15 +632,15 @@
         *,
         assessmentArn: str,
         maxResults: int = ...,
         name: str = ...,
         nextToken: str = ...,
         recommendationTemplateArn: str = ...,
         reverseOrder: bool = ...,
-        status: Sequence[RecommendationTemplateStatusType] = ...
+        status: Sequence[RecommendationTemplateStatusType] = ...,
     ) -> ListRecommendationTemplatesResponseTypeDef:
         """
         Lists the recommendation templates for the Resilience Hub applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_recommendation_templates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#list_recommendation_templates)
         """
@@ -700,15 +700,15 @@
     async def list_unsupported_app_version_resources(
         self,
         *,
         appArn: str,
         appVersion: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        resolutionId: str = ...
+        resolutionId: str = ...,
     ) -> ListUnsupportedAppVersionResourcesResponseTypeDef:
         """
         Lists the resources that are not currently supported in Resilience Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_unsupported_app_version_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#list_unsupported_app_version_resources)
         """
@@ -739,15 +739,15 @@
         *,
         appArn: str,
         appRegistryAppNames: Sequence[str] = ...,
         eksSourceNames: Sequence[str] = ...,
         logicalStackNames: Sequence[str] = ...,
         resourceGroupNames: Sequence[str] = ...,
         resourceNames: Sequence[str] = ...,
-        terraformSourceNames: Sequence[str] = ...
+        terraformSourceNames: Sequence[str] = ...,
     ) -> RemoveDraftAppVersionResourceMappingsResponseTypeDef:
         """
         Removes resource mappings from a draft application version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.remove_draft_app_version_resource_mappings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#remove_draft_app_version_resource_mappings)
         """
@@ -765,15 +765,15 @@
     async def start_app_assessment(
         self,
         *,
         appArn: str,
         appVersion: str,
         assessmentName: str,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> StartAppAssessmentResponseTypeDef:
         """
         Creates a new application assessment for an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.start_app_assessment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#start_app_assessment)
         """
@@ -799,15 +799,15 @@
         *,
         appArn: str,
         assessmentSchedule: AppAssessmentScheduleTypeType = ...,
         clearResiliencyPolicyArn: bool = ...,
         description: str = ...,
         eventSubscriptions: Sequence[EventSubscriptionTypeDef] = ...,
         permissionModel: PermissionModelTypeDef = ...,
-        policyArn: str = ...
+        policyArn: str = ...,
     ) -> UpdateAppResponseTypeDef:
         """
         Updates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#update_app)
         """
@@ -825,15 +825,15 @@
     async def update_app_version_app_component(
         self,
         *,
         appArn: str,
         id: str,
         additionalInfo: Mapping[str, Sequence[str]] = ...,
         name: str = ...,
-        type: str = ...
+        type: str = ...,
     ) -> UpdateAppVersionAppComponentResponseTypeDef:
         """
         Updates an existing Application Component in the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_app_version_app_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#update_app_version_app_component)
         """
@@ -846,15 +846,15 @@
         appComponents: Sequence[str] = ...,
         awsAccountId: str = ...,
         awsRegion: str = ...,
         excluded: bool = ...,
         logicalResourceId: LogicalResourceIdTypeDef = ...,
         physicalResourceId: str = ...,
         resourceName: str = ...,
-        resourceType: str = ...
+        resourceType: str = ...,
     ) -> UpdateAppVersionResourceResponseTypeDef:
         """
         Updates the resource details in the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_app_version_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#update_app_version_resource)
         """
@@ -863,15 +863,15 @@
         self,
         *,
         policyArn: str,
         dataLocationConstraint: DataLocationConstraintType = ...,
         policy: Mapping[DisruptionTypeType, FailurePolicyTypeDef] = ...,
         policyDescription: str = ...,
         policyName: str = ...,
-        tier: ResiliencyPolicyTierType = ...
+        tier: ResiliencyPolicyTierType = ...,
     ) -> UpdateResiliencyPolicyResponseTypeDef:
         """
         Updates a resiliency policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_resiliency_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#update_resiliency_policy)
         """
```

### Comparing `types-aiobotocore-resiliencehub-2.9.0/types_aiobotocore_resiliencehub/client.pyi` & `types-aiobotocore-resiliencehub-2.9.1/types_aiobotocore_resiliencehub/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#add_draft_app_version_resource_mappings)
         """
 
     async def batch_update_recommendation_status(
         self,
         *,
         appArn: str,
-        requestEntries: Sequence[UpdateRecommendationStatusRequestEntryTypeDef]
+        requestEntries: Sequence[UpdateRecommendationStatusRequestEntryTypeDef],
     ) -> BatchUpdateRecommendationStatusResponseTypeDef:
         """
         Enables you to include or exclude one or more operational recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.batch_update_recommendation_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#batch_update_recommendation_status)
         """
@@ -179,15 +179,15 @@
         name: str,
         assessmentSchedule: AppAssessmentScheduleTypeType = ...,
         clientToken: str = ...,
         description: str = ...,
         eventSubscriptions: Sequence[EventSubscriptionTypeDef] = ...,
         permissionModel: PermissionModelTypeDef = ...,
         policyArn: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateAppResponseTypeDef:
         """
         Creates an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#create_app)
         """
@@ -196,15 +196,15 @@
         self,
         *,
         appArn: str,
         name: str,
         type: str,
         additionalInfo: Mapping[str, Sequence[str]] = ...,
         clientToken: str = ...,
-        id: str = ...
+        id: str = ...,
     ) -> CreateAppVersionAppComponentResponseTypeDef:
         """
         Creates a new Application Component in the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_app_version_app_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#create_app_version_app_component)
         """
@@ -217,15 +217,15 @@
         logicalResourceId: LogicalResourceIdTypeDef,
         physicalResourceId: str,
         resourceType: str,
         additionalInfo: Mapping[str, Sequence[str]] = ...,
         awsAccountId: str = ...,
         awsRegion: str = ...,
         clientToken: str = ...,
-        resourceName: str = ...
+        resourceName: str = ...,
     ) -> CreateAppVersionResourceResponseTypeDef:
         """
         Adds a resource to the Resilience Hub application and assigns it to the
         specified Application
         Components.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_app_version_resource)
@@ -238,15 +238,15 @@
         assessmentArn: str,
         name: str,
         bucketName: str = ...,
         clientToken: str = ...,
         format: TemplateFormatType = ...,
         recommendationIds: Sequence[str] = ...,
         recommendationTypes: Sequence[RenderRecommendationTypeType] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateRecommendationTemplateResponseTypeDef:
         """
         Creates a new recommendation template for the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_recommendation_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#create_recommendation_template)
         """
@@ -256,15 +256,15 @@
         *,
         policy: Mapping[DisruptionTypeType, FailurePolicyTypeDef],
         policyName: str,
         tier: ResiliencyPolicyTierType,
         clientToken: str = ...,
         dataLocationConstraint: DataLocationConstraintType = ...,
         policyDescription: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateResiliencyPolicyResponseTypeDef:
         """
         Creates a resiliency policy for an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_resiliency_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#create_resiliency_policy)
         """
@@ -292,15 +292,15 @@
     async def delete_app_input_source(
         self,
         *,
         appArn: str,
         clientToken: str = ...,
         eksSourceClusterNamespace: EksSourceClusterNamespaceTypeDef = ...,
         sourceArn: str = ...,
-        terraformSource: TerraformSourceTypeDef = ...
+        terraformSource: TerraformSourceTypeDef = ...,
     ) -> DeleteAppInputSourceResponseTypeDef:
         """
         Deletes the input source and all of its imported resources from the Resilience
         Hub
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.delete_app_input_source)
@@ -322,15 +322,15 @@
         *,
         appArn: str,
         awsAccountId: str = ...,
         awsRegion: str = ...,
         clientToken: str = ...,
         logicalResourceId: LogicalResourceIdTypeDef = ...,
         physicalResourceId: str = ...,
-        resourceName: str = ...
+        resourceName: str = ...,
     ) -> DeleteAppVersionResourceResponseTypeDef:
         """
         Deletes a resource from the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.delete_app_version_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#delete_app_version_resource)
         """
@@ -398,15 +398,15 @@
         *,
         appArn: str,
         appVersion: str,
         awsAccountId: str = ...,
         awsRegion: str = ...,
         logicalResourceId: LogicalResourceIdTypeDef = ...,
         physicalResourceId: str = ...,
-        resourceName: str = ...
+        resourceName: str = ...,
     ) -> DescribeAppVersionResourceResponseTypeDef:
         """
         Describes a resource of the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.describe_app_version_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#describe_app_version_resource)
         """
@@ -470,15 +470,15 @@
     async def import_resources_to_draft_app_version(
         self,
         *,
         appArn: str,
         eksSources: Sequence[EksSourceTypeDef] = ...,
         importStrategy: ResourceImportStrategyTypeType = ...,
         sourceArns: Sequence[str] = ...,
-        terraformSources: Sequence[TerraformSourceTypeDef] = ...
+        terraformSources: Sequence[TerraformSourceTypeDef] = ...,
     ) -> ImportResourcesToDraftAppVersionResponseTypeDef:
         """
         Imports resources to Resilience Hub application draft version from different
         input
         sources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.import_resources_to_draft_app_version)
@@ -511,15 +511,15 @@
         appArn: str = ...,
         assessmentName: str = ...,
         assessmentStatus: Sequence[AssessmentStatusType] = ...,
         complianceStatus: ComplianceStatusType = ...,
         invoker: AssessmentInvokerType = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        reverseOrder: bool = ...
+        reverseOrder: bool = ...,
     ) -> ListAppAssessmentsResponseTypeDef:
         """
         Lists the assessments for an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_assessments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#list_app_assessments)
         """
@@ -577,15 +577,15 @@
     async def list_app_version_resources(
         self,
         *,
         appArn: str,
         appVersion: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        resolutionId: str = ...
+        resolutionId: str = ...,
     ) -> ListAppVersionResourcesResponseTypeDef:
         """
         Lists all the resources in an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_version_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#list_app_version_resources)
         """
@@ -593,15 +593,15 @@
     async def list_app_versions(
         self,
         *,
         appArn: str,
         endTime: TimestampTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        startTime: TimestampTypeDef = ...
+        startTime: TimestampTypeDef = ...,
     ) -> ListAppVersionsResponseTypeDef:
         """
         Lists the different versions for the Resilience Hub applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#list_app_versions)
         """
@@ -611,15 +611,15 @@
         *,
         appArn: str = ...,
         fromLastAssessmentTime: TimestampTypeDef = ...,
         maxResults: int = ...,
         name: str = ...,
         nextToken: str = ...,
         reverseOrder: bool = ...,
-        toLastAssessmentTime: TimestampTypeDef = ...
+        toLastAssessmentTime: TimestampTypeDef = ...,
     ) -> ListAppsResponseTypeDef:
         """
         Lists your Resilience Hub applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_apps)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#list_apps)
         """
@@ -629,15 +629,15 @@
         *,
         assessmentArn: str,
         maxResults: int = ...,
         name: str = ...,
         nextToken: str = ...,
         recommendationTemplateArn: str = ...,
         reverseOrder: bool = ...,
-        status: Sequence[RecommendationTemplateStatusType] = ...
+        status: Sequence[RecommendationTemplateStatusType] = ...,
     ) -> ListRecommendationTemplatesResponseTypeDef:
         """
         Lists the recommendation templates for the Resilience Hub applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_recommendation_templates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#list_recommendation_templates)
         """
@@ -697,15 +697,15 @@
     async def list_unsupported_app_version_resources(
         self,
         *,
         appArn: str,
         appVersion: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        resolutionId: str = ...
+        resolutionId: str = ...,
     ) -> ListUnsupportedAppVersionResourcesResponseTypeDef:
         """
         Lists the resources that are not currently supported in Resilience Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_unsupported_app_version_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#list_unsupported_app_version_resources)
         """
@@ -736,15 +736,15 @@
         *,
         appArn: str,
         appRegistryAppNames: Sequence[str] = ...,
         eksSourceNames: Sequence[str] = ...,
         logicalStackNames: Sequence[str] = ...,
         resourceGroupNames: Sequence[str] = ...,
         resourceNames: Sequence[str] = ...,
-        terraformSourceNames: Sequence[str] = ...
+        terraformSourceNames: Sequence[str] = ...,
     ) -> RemoveDraftAppVersionResourceMappingsResponseTypeDef:
         """
         Removes resource mappings from a draft application version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.remove_draft_app_version_resource_mappings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#remove_draft_app_version_resource_mappings)
         """
@@ -762,15 +762,15 @@
     async def start_app_assessment(
         self,
         *,
         appArn: str,
         appVersion: str,
         assessmentName: str,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> StartAppAssessmentResponseTypeDef:
         """
         Creates a new application assessment for an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.start_app_assessment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#start_app_assessment)
         """
@@ -796,15 +796,15 @@
         *,
         appArn: str,
         assessmentSchedule: AppAssessmentScheduleTypeType = ...,
         clearResiliencyPolicyArn: bool = ...,
         description: str = ...,
         eventSubscriptions: Sequence[EventSubscriptionTypeDef] = ...,
         permissionModel: PermissionModelTypeDef = ...,
-        policyArn: str = ...
+        policyArn: str = ...,
     ) -> UpdateAppResponseTypeDef:
         """
         Updates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#update_app)
         """
@@ -822,15 +822,15 @@
     async def update_app_version_app_component(
         self,
         *,
         appArn: str,
         id: str,
         additionalInfo: Mapping[str, Sequence[str]] = ...,
         name: str = ...,
-        type: str = ...
+        type: str = ...,
     ) -> UpdateAppVersionAppComponentResponseTypeDef:
         """
         Updates an existing Application Component in the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_app_version_app_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#update_app_version_app_component)
         """
@@ -843,15 +843,15 @@
         appComponents: Sequence[str] = ...,
         awsAccountId: str = ...,
         awsRegion: str = ...,
         excluded: bool = ...,
         logicalResourceId: LogicalResourceIdTypeDef = ...,
         physicalResourceId: str = ...,
         resourceName: str = ...,
-        resourceType: str = ...
+        resourceType: str = ...,
     ) -> UpdateAppVersionResourceResponseTypeDef:
         """
         Updates the resource details in the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_app_version_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#update_app_version_resource)
         """
@@ -860,15 +860,15 @@
         self,
         *,
         policyArn: str,
         dataLocationConstraint: DataLocationConstraintType = ...,
         policy: Mapping[DisruptionTypeType, FailurePolicyTypeDef] = ...,
         policyDescription: str = ...,
         policyName: str = ...,
-        tier: ResiliencyPolicyTierType = ...
+        tier: ResiliencyPolicyTierType = ...,
     ) -> UpdateResiliencyPolicyResponseTypeDef:
         """
         Updates a resiliency policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_resiliency_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#update_resiliency_policy)
         """
```

### Comparing `types-aiobotocore-resiliencehub-2.9.0/types_aiobotocore_resiliencehub/literals.py` & `types-aiobotocore-resiliencehub-2.9.1/types_aiobotocore_resiliencehub/literals.py`

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
     "AlarmTypeType",
     "AppAssessmentScheduleTypeType",
     "AppComplianceStatusTypeType",
     "AppDriftStatusTypeType",
     "AppStatusTypeType",
     "AssessmentInvokerType",
@@ -59,15 +58,14 @@
     "TestTypeType",
     "ResilienceHubServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AlarmTypeType = Literal["Canary", "Composite", "Event", "Logs", "Metric"]
 AppAssessmentScheduleTypeType = Literal["Daily", "Disabled"]
 AppComplianceStatusTypeType = Literal[
     "ChangesDetected", "NotAssessed", "PolicyBreached", "PolicyMet"
 ]
 AppDriftStatusTypeType = Literal["Detected", "NotChecked", "NotDetected"]
 AppStatusTypeType = Literal["Active", "Deleting"]
```

### Comparing `types-aiobotocore-resiliencehub-2.9.0/types_aiobotocore_resiliencehub/literals.pyi` & `types-aiobotocore-resiliencehub-2.9.1/types_aiobotocore_resiliencehub/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resiliencehub-2.9.0/types_aiobotocore_resiliencehub/type_defs.py` & `types-aiobotocore-resiliencehub-2.9.1/types_aiobotocore_resiliencehub/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ResponseMetadataTypeDef",
     "RecommendationItemTypeDef",
     "CostTypeDef",
     "DisruptionComplianceTypeDef",
     "AppComponentTypeDef",
     "EksSourceClusterNamespaceTypeDef",
```

### Comparing `types-aiobotocore-resiliencehub-2.9.0/types_aiobotocore_resiliencehub/type_defs.pyi` & `types-aiobotocore-resiliencehub-2.9.1/types_aiobotocore_resiliencehub/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resiliencehub-2.9.0/types_aiobotocore_resiliencehub.egg-info/PKG-INFO` & `types-aiobotocore-resiliencehub-2.9.1/types_aiobotocore_resiliencehub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-resiliencehub
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ResilienceHub 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ResilienceHub 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/
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
 
 <a id="types-aiobotocore-resiliencehub"></a>
 
 # types-aiobotocore-resiliencehub
 
 [![PyPI - types-aiobotocore-resiliencehub](https://img.shields.io/pypi/v/types-aiobotocore-resiliencehub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resiliencehub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resiliencehub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resiliencehub)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-resiliencehub)](https://pepy.tech/project/types-aiobotocore-resiliencehub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ResilienceHub 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
+[aiobotocore.ResilienceHub 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
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
 [types-aiobotocore-resiliencehub docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-resiliencehub-2.9.0/types_aiobotocore_resiliencehub.egg-info/SOURCES.txt` & `types-aiobotocore-resiliencehub-2.9.1/types_aiobotocore_resiliencehub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

