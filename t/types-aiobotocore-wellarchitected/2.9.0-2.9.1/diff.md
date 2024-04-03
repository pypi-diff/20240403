# Comparing `tmp/types-aiobotocore-wellarchitected-2.9.0.tar.gz` & `tmp/types-aiobotocore-wellarchitected-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-wellarchitected-2.9.0.tar", last modified: Wed Dec 13 20:00:45 2023, max compression
+gzip compressed data, was "types-aiobotocore-wellarchitected-2.9.1.tar", last modified: Thu Jan 18 01:22:02 2024, max compression
```

## Comparing `types-aiobotocore-wellarchitected-2.9.0.tar` & `types-aiobotocore-wellarchitected-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:45.625008 types-aiobotocore-wellarchitected-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:57:51.000000 types-aiobotocore-wellarchitected-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12667 2023-12-13 20:00:45.625008 types-aiobotocore-wellarchitected-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11072 2023-12-13 19:57:51.000000 types-aiobotocore-wellarchitected-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:45.625008 types-aiobotocore-wellarchitected-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2023-12-13 19:57:51.000000 types-aiobotocore-wellarchitected-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:45.625008 types-aiobotocore-wellarchitected-2.9.0/types_aiobotocore_wellarchitected/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2023-12-13 19:57:51.000000 types-aiobotocore-wellarchitected-2.9.0/types_aiobotocore_wellarchitected/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2023-12-13 19:57:51.000000 types-aiobotocore-wellarchitected-2.9.0/types_aiobotocore_wellarchitected/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      964 2023-12-13 19:57:51.000000 types-aiobotocore-wellarchitected-2.9.0/types_aiobotocore_wellarchitected/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49800 2023-12-13 19:57:51.000000 types-aiobotocore-wellarchitected-2.9.0/types_aiobotocore_wellarchitected/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    49797 2023-12-13 19:57:51.000000 types-aiobotocore-wellarchitected-2.9.0/types_aiobotocore_wellarchitected/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11896 2023-12-13 19:57:51.000000 types-aiobotocore-wellarchitected-2.9.0/types_aiobotocore_wellarchitected/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11894 2023-12-13 19:57:51.000000 types-aiobotocore-wellarchitected-2.9.0/types_aiobotocore_wellarchitected/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:57:51.000000 types-aiobotocore-wellarchitected-2.9.0/types_aiobotocore_wellarchitected/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    60434 2023-12-13 19:57:52.000000 types-aiobotocore-wellarchitected-2.9.0/types_aiobotocore_wellarchitected/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    60433 2023-12-13 19:57:52.000000 types-aiobotocore-wellarchitected-2.9.0/types_aiobotocore_wellarchitected/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:57:51.000000 types-aiobotocore-wellarchitected-2.9.0/types_aiobotocore_wellarchitected/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:45.625008 types-aiobotocore-wellarchitected-2.9.0/types_aiobotocore_wellarchitected.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12667 2023-12-13 20:00:45.000000 types-aiobotocore-wellarchitected-2.9.0/types_aiobotocore_wellarchitected.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      870 2023-12-13 20:00:45.000000 types-aiobotocore-wellarchitected-2.9.0/types_aiobotocore_wellarchitected.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:45.000000 types-aiobotocore-wellarchitected-2.9.0/types_aiobotocore_wellarchitected.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:45.000000 types-aiobotocore-wellarchitected-2.9.0/types_aiobotocore_wellarchitected.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:45.000000 types-aiobotocore-wellarchitected-2.9.0/types_aiobotocore_wellarchitected.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-13 20:00:45.000000 types-aiobotocore-wellarchitected-2.9.0/types_aiobotocore_wellarchitected.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:02.616972 types-aiobotocore-wellarchitected-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:19:18.000000 types-aiobotocore-wellarchitected-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12687 2024-01-18 01:22:02.612972 types-aiobotocore-wellarchitected-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11072 2024-01-18 01:19:18.000000 types-aiobotocore-wellarchitected-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:22:02.616972 types-aiobotocore-wellarchitected-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-01-18 01:19:18.000000 types-aiobotocore-wellarchitected-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:02.612972 types-aiobotocore-wellarchitected-2.9.1/types_aiobotocore_wellarchitected/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-01-18 01:19:18.000000 types-aiobotocore-wellarchitected-2.9.1/types_aiobotocore_wellarchitected/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-01-18 01:19:18.000000 types-aiobotocore-wellarchitected-2.9.1/types_aiobotocore_wellarchitected/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-01-18 01:19:18.000000 types-aiobotocore-wellarchitected-2.9.1/types_aiobotocore_wellarchitected/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49830 2024-01-18 01:19:19.000000 types-aiobotocore-wellarchitected-2.9.1/types_aiobotocore_wellarchitected/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49827 2024-01-18 01:19:18.000000 types-aiobotocore-wellarchitected-2.9.1/types_aiobotocore_wellarchitected/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11894 2024-01-18 01:19:19.000000 types-aiobotocore-wellarchitected-2.9.1/types_aiobotocore_wellarchitected/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11894 2024-01-18 01:19:19.000000 types-aiobotocore-wellarchitected-2.9.1/types_aiobotocore_wellarchitected/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:18.000000 types-aiobotocore-wellarchitected-2.9.1/types_aiobotocore_wellarchitected/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    60433 2024-01-18 01:19:20.000000 types-aiobotocore-wellarchitected-2.9.1/types_aiobotocore_wellarchitected/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60433 2024-01-18 01:19:19.000000 types-aiobotocore-wellarchitected-2.9.1/types_aiobotocore_wellarchitected/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:19:18.000000 types-aiobotocore-wellarchitected-2.9.1/types_aiobotocore_wellarchitected/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:02.612972 types-aiobotocore-wellarchitected-2.9.1/types_aiobotocore_wellarchitected.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12687 2024-01-18 01:22:02.000000 types-aiobotocore-wellarchitected-2.9.1/types_aiobotocore_wellarchitected.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-01-18 01:22:02.000000 types-aiobotocore-wellarchitected-2.9.1/types_aiobotocore_wellarchitected.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:22:02.000000 types-aiobotocore-wellarchitected-2.9.1/types_aiobotocore_wellarchitected.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:22:02.000000 types-aiobotocore-wellarchitected-2.9.1/types_aiobotocore_wellarchitected.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:22:02.000000 types-aiobotocore-wellarchitected-2.9.1/types_aiobotocore_wellarchitected.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-01-18 01:22:02.000000 types-aiobotocore-wellarchitected-2.9.1/types_aiobotocore_wellarchitected.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-wellarchitected-2.9.0/LICENSE` & `types-aiobotocore-wellarchitected-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-wellarchitected-2.9.0/PKG-INFO` & `types-aiobotocore-wellarchitected-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-wellarchitected
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.WellArchitected 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.WellArchitected 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/
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
 
 <a id="types-aiobotocore-wellarchitected"></a>
 
 # types-aiobotocore-wellarchitected
 
 [![PyPI - types-aiobotocore-wellarchitected](https://img.shields.io/pypi/v/types-aiobotocore-wellarchitected.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wellarchitected)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-wellarchitected.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wellarchitected)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-wellarchitected)](https://pepy.tech/project/types-aiobotocore-wellarchitected)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WellArchitected 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
+[aiobotocore.WellArchitected 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
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
 [types-aiobotocore-wellarchitected docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-wellarchitected-2.9.0/README.md` & `types-aiobotocore-wellarchitected-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-wellarchitected.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wellarchitected)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-wellarchitected)](https://pepy.tech/project/types-aiobotocore-wellarchitected)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WellArchitected 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
+[aiobotocore.WellArchitected 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
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
 [types-aiobotocore-wellarchitected docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-wellarchitected-2.9.0/setup.py` & `types-aiobotocore-wellarchitected-2.9.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-wellarchitected",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_wellarchitected"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.WellArchitected 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.WellArchitected 2.9.1 service generated with"
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
     keywords="aiobotocore wellarchitected type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_wellarchitected": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-wellarchitected-2.9.0/types_aiobotocore_wellarchitected/__main__.py` & `types-aiobotocore-wellarchitected-2.9.1/types_aiobotocore_wellarchitected/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.WellArchitected 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.WellArchitected 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected\nOther"
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

### Comparing `types-aiobotocore-wellarchitected-2.9.0/types_aiobotocore_wellarchitected/client.py` & `types-aiobotocore-wellarchitected-2.9.1/types_aiobotocore_wellarchitected/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
 
     async def create_lens_version(
         self,
         *,
         LensAlias: str,
         LensVersion: str,
         ClientRequestToken: str,
-        IsMajorVersion: bool = ...
+        IsMajorVersion: bool = ...,
     ) -> CreateLensVersionOutputTypeDef:
         """
         Create a new lens version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_lens_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#create_lens_version)
         """
@@ -208,15 +208,15 @@
     async def create_profile(
         self,
         *,
         ProfileName: str,
         ProfileDescription: str,
         ProfileQuestions: Sequence[ProfileQuestionUpdateTypeDef],
         ClientRequestToken: str,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateProfileOutputTypeDef:
         """
         Create a profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#create_profile)
         """
@@ -235,15 +235,15 @@
         self,
         *,
         TemplateName: str,
         Description: str,
         Lenses: Sequence[str],
         ClientRequestToken: str,
         Notes: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateReviewTemplateOutputTypeDef:
         """
         Create a review template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_review_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#create_review_template)
         """
@@ -275,30 +275,30 @@
         IndustryType: str = ...,
         Industry: str = ...,
         Notes: str = ...,
         Tags: Mapping[str, str] = ...,
         DiscoveryConfig: WorkloadDiscoveryConfigTypeDef = ...,
         Applications: Sequence[str] = ...,
         ProfileArns: Sequence[str] = ...,
-        ReviewTemplateArns: Sequence[str] = ...
+        ReviewTemplateArns: Sequence[str] = ...,
     ) -> CreateWorkloadOutputTypeDef:
         """
         Create a new workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_workload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#create_workload)
         """
 
     async def create_workload_share(
         self,
         *,
         WorkloadId: str,
         SharedWith: str,
         PermissionType: PermissionTypeType,
-        ClientRequestToken: str
+        ClientRequestToken: str,
     ) -> CreateWorkloadShareOutputTypeDef:
         """
         Create a workload share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_workload_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#create_workload_share)
         """
@@ -439,15 +439,15 @@
 
     async def get_consolidated_report(
         self,
         *,
         Format: ReportFormatType,
         IncludeSharedResources: bool = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetConsolidatedReportOutputTypeDef:
         """
         Get a consolidated report of your workloads.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_consolidated_report)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#get_consolidated_report)
         """
@@ -556,15 +556,15 @@
 
     async def import_lens(
         self,
         *,
         JSONString: str,
         ClientRequestToken: str,
         LensAlias: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> ImportLensOutputTypeDef:
         """
         Import a new custom lens or update an existing custom lens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.import_lens)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#import_lens)
         """
@@ -574,15 +574,15 @@
         *,
         WorkloadId: str,
         LensAlias: str,
         PillarId: str = ...,
         MilestoneNumber: int = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        QuestionPriority: QuestionPriorityType = ...
+        QuestionPriority: QuestionPriorityType = ...,
     ) -> ListAnswersOutputTypeDef:
         """
         List of answers for a particular workload and lens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_answers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#list_answers)
         """
@@ -592,15 +592,15 @@
         *,
         WorkloadId: str,
         LensArn: str,
         PillarId: str,
         QuestionId: str,
         ChoiceId: str,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListCheckDetailsOutputTypeDef:
         """
         List of Trusted Advisor check details by account related to the workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_check_details)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#list_check_details)
         """
@@ -610,15 +610,15 @@
         *,
         WorkloadId: str,
         LensArn: str,
         PillarId: str,
         QuestionId: str,
         ChoiceId: str,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListCheckSummariesOutputTypeDef:
         """
         List of Trusted Advisor checks summarized for all accounts related to the
         workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_check_summaries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#list_check_summaries)
@@ -629,30 +629,30 @@
         *,
         WorkloadId: str,
         LensAlias: str,
         PillarId: str = ...,
         MilestoneNumber: int = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        QuestionPriority: QuestionPriorityType = ...
+        QuestionPriority: QuestionPriorityType = ...,
     ) -> ListLensReviewImprovementsOutputTypeDef:
         """
         List lens review improvements.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_lens_review_improvements)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#list_lens_review_improvements)
         """
 
     async def list_lens_reviews(
         self,
         *,
         WorkloadId: str,
         MilestoneNumber: int = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListLensReviewsOutputTypeDef:
         """
         List lens reviews for a particular workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_lens_reviews)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#list_lens_reviews)
         """
@@ -660,15 +660,15 @@
     async def list_lens_shares(
         self,
         *,
         LensAlias: str,
         SharedWithPrefix: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Status: ShareStatusType = ...
+        Status: ShareStatusType = ...,
     ) -> ListLensSharesOutputTypeDef:
         """
         List the lens shares associated with the lens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_lens_shares)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#list_lens_shares)
         """
@@ -676,15 +676,15 @@
     async def list_lenses(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         LensType: LensTypeType = ...,
         LensStatus: LensStatusTypeType = ...,
-        LensName: str = ...
+        LensName: str = ...,
     ) -> ListLensesOutputTypeDef:
         """
         List the available lenses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_lenses)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#list_lenses)
         """
@@ -701,15 +701,15 @@
 
     async def list_notifications(
         self,
         *,
         WorkloadId: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        ResourceArn: str = ...
+        ResourceArn: str = ...,
     ) -> ListNotificationsOutputTypeDef:
         """
         List lens notifications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_notifications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#list_notifications)
         """
@@ -727,30 +727,30 @@
     async def list_profile_shares(
         self,
         *,
         ProfileArn: str,
         SharedWithPrefix: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Status: ShareStatusType = ...
+        Status: ShareStatusType = ...,
     ) -> ListProfileSharesOutputTypeDef:
         """
         List profile shares.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_profile_shares)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#list_profile_shares)
         """
 
     async def list_profiles(
         self,
         *,
         ProfileNamePrefix: str = ...,
         ProfileOwnerType: ProfileOwnerTypeType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListProfilesOutputTypeDef:
         """
         List profiles.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#list_profiles)
         """
@@ -758,15 +758,15 @@
     async def list_review_template_answers(
         self,
         *,
         TemplateArn: str,
         LensAlias: str,
         PillarId: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListReviewTemplateAnswersOutputTypeDef:
         """
         List the answers of a review template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_review_template_answers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#list_review_template_answers)
         """
@@ -786,15 +786,15 @@
         *,
         WorkloadNamePrefix: str = ...,
         LensNamePrefix: str = ...,
         ShareResourceType: ShareResourceTypeType = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         ProfileNamePrefix: str = ...,
-        TemplateNamePrefix: str = ...
+        TemplateNamePrefix: str = ...,
     ) -> ListShareInvitationsOutputTypeDef:
         """
         List the share invitations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_share_invitations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#list_share_invitations)
         """
@@ -810,15 +810,15 @@
     async def list_template_shares(
         self,
         *,
         TemplateArn: str,
         SharedWithPrefix: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Status: ShareStatusType = ...
+        Status: ShareStatusType = ...,
     ) -> ListTemplateSharesOutputTypeDef:
         """
         List review template shares.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_template_shares)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#list_template_shares)
         """
@@ -826,15 +826,15 @@
     async def list_workload_shares(
         self,
         *,
         WorkloadId: str,
         SharedWithPrefix: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Status: ShareStatusType = ...
+        Status: ShareStatusType = ...,
     ) -> ListWorkloadSharesOutputTypeDef:
         """
         List the workload shares associated with the workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_workload_shares)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#list_workload_shares)
         """
@@ -871,28 +871,28 @@
         WorkloadId: str,
         LensAlias: str,
         QuestionId: str,
         SelectedChoices: Sequence[str] = ...,
         ChoiceUpdates: Mapping[str, ChoiceUpdateTypeDef] = ...,
         Notes: str = ...,
         IsApplicable: bool = ...,
-        Reason: AnswerReasonType = ...
+        Reason: AnswerReasonType = ...,
     ) -> UpdateAnswerOutputTypeDef:
         """
         Update the answer to a specific question in a workload review.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_answer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#update_answer)
         """
 
     async def update_global_settings(
         self,
         *,
         OrganizationSharingStatus: OrganizationSharingStatusType = ...,
-        DiscoveryIntegrationStatus: DiscoveryIntegrationStatusType = ...
+        DiscoveryIntegrationStatus: DiscoveryIntegrationStatusType = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates whether the Amazon Web Services account is opted into organization
         sharing and discovery integration
         features.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_global_settings)
@@ -901,29 +901,29 @@
 
     async def update_lens_review(
         self,
         *,
         WorkloadId: str,
         LensAlias: str,
         LensNotes: str = ...,
-        PillarNotes: Mapping[str, str] = ...
+        PillarNotes: Mapping[str, str] = ...,
     ) -> UpdateLensReviewOutputTypeDef:
         """
         Update lens review for a particular workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_lens_review)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#update_lens_review)
         """
 
     async def update_profile(
         self,
         *,
         ProfileArn: str,
         ProfileDescription: str = ...,
-        ProfileQuestions: Sequence[ProfileQuestionUpdateTypeDef] = ...
+        ProfileQuestions: Sequence[ProfileQuestionUpdateTypeDef] = ...,
     ) -> UpdateProfileOutputTypeDef:
         """
         Update a profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#update_profile)
         """
@@ -932,15 +932,15 @@
         self,
         *,
         TemplateArn: str,
         TemplateName: str = ...,
         Description: str = ...,
         Notes: str = ...,
         LensesToAssociate: Sequence[str] = ...,
-        LensesToDisassociate: Sequence[str] = ...
+        LensesToDisassociate: Sequence[str] = ...,
     ) -> UpdateReviewTemplateOutputTypeDef:
         """
         Update a review template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_review_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#update_review_template)
         """
@@ -951,30 +951,30 @@
         TemplateArn: str,
         LensAlias: str,
         QuestionId: str,
         SelectedChoices: Sequence[str] = ...,
         ChoiceUpdates: Mapping[str, ChoiceUpdateTypeDef] = ...,
         Notes: str = ...,
         IsApplicable: bool = ...,
-        Reason: AnswerReasonType = ...
+        Reason: AnswerReasonType = ...,
     ) -> UpdateReviewTemplateAnswerOutputTypeDef:
         """
         Update a review template answer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_review_template_answer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#update_review_template_answer)
         """
 
     async def update_review_template_lens_review(
         self,
         *,
         TemplateArn: str,
         LensAlias: str,
         LensNotes: str = ...,
-        PillarNotes: Mapping[str, str] = ...
+        PillarNotes: Mapping[str, str] = ...,
     ) -> UpdateReviewTemplateLensReviewOutputTypeDef:
         """
         Update a lens review associated with a review template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_review_template_lens_review)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#update_review_template_lens_review)
         """
@@ -1004,15 +1004,15 @@
         ReviewOwner: str = ...,
         IsReviewOwnerUpdateAcknowledged: bool = ...,
         IndustryType: str = ...,
         Industry: str = ...,
         Notes: str = ...,
         ImprovementStatus: WorkloadImprovementStatusType = ...,
         DiscoveryConfig: WorkloadDiscoveryConfigTypeDef = ...,
-        Applications: Sequence[str] = ...
+        Applications: Sequence[str] = ...,
     ) -> UpdateWorkloadOutputTypeDef:
         """
         Update an existing workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_workload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#update_workload)
         """
@@ -1039,15 +1039,15 @@
 
     async def upgrade_profile_version(
         self,
         *,
         WorkloadId: str,
         ProfileArn: str,
         MilestoneName: str = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Upgrade a profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.upgrade_profile_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#upgrade_profile_version)
         """
```

### Comparing `types-aiobotocore-wellarchitected-2.9.0/types_aiobotocore_wellarchitected/client.pyi` & `types-aiobotocore-wellarchitected-2.9.1/types_aiobotocore_wellarchitected/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
 
     async def create_lens_version(
         self,
         *,
         LensAlias: str,
         LensVersion: str,
         ClientRequestToken: str,
-        IsMajorVersion: bool = ...
+        IsMajorVersion: bool = ...,
     ) -> CreateLensVersionOutputTypeDef:
         """
         Create a new lens version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_lens_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#create_lens_version)
         """
@@ -205,15 +205,15 @@
     async def create_profile(
         self,
         *,
         ProfileName: str,
         ProfileDescription: str,
         ProfileQuestions: Sequence[ProfileQuestionUpdateTypeDef],
         ClientRequestToken: str,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateProfileOutputTypeDef:
         """
         Create a profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#create_profile)
         """
@@ -232,15 +232,15 @@
         self,
         *,
         TemplateName: str,
         Description: str,
         Lenses: Sequence[str],
         ClientRequestToken: str,
         Notes: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateReviewTemplateOutputTypeDef:
         """
         Create a review template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_review_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#create_review_template)
         """
@@ -272,30 +272,30 @@
         IndustryType: str = ...,
         Industry: str = ...,
         Notes: str = ...,
         Tags: Mapping[str, str] = ...,
         DiscoveryConfig: WorkloadDiscoveryConfigTypeDef = ...,
         Applications: Sequence[str] = ...,
         ProfileArns: Sequence[str] = ...,
-        ReviewTemplateArns: Sequence[str] = ...
+        ReviewTemplateArns: Sequence[str] = ...,
     ) -> CreateWorkloadOutputTypeDef:
         """
         Create a new workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_workload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#create_workload)
         """
 
     async def create_workload_share(
         self,
         *,
         WorkloadId: str,
         SharedWith: str,
         PermissionType: PermissionTypeType,
-        ClientRequestToken: str
+        ClientRequestToken: str,
     ) -> CreateWorkloadShareOutputTypeDef:
         """
         Create a workload share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_workload_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#create_workload_share)
         """
@@ -436,15 +436,15 @@
 
     async def get_consolidated_report(
         self,
         *,
         Format: ReportFormatType,
         IncludeSharedResources: bool = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetConsolidatedReportOutputTypeDef:
         """
         Get a consolidated report of your workloads.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_consolidated_report)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#get_consolidated_report)
         """
@@ -553,15 +553,15 @@
 
     async def import_lens(
         self,
         *,
         JSONString: str,
         ClientRequestToken: str,
         LensAlias: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> ImportLensOutputTypeDef:
         """
         Import a new custom lens or update an existing custom lens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.import_lens)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#import_lens)
         """
@@ -571,15 +571,15 @@
         *,
         WorkloadId: str,
         LensAlias: str,
         PillarId: str = ...,
         MilestoneNumber: int = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        QuestionPriority: QuestionPriorityType = ...
+        QuestionPriority: QuestionPriorityType = ...,
     ) -> ListAnswersOutputTypeDef:
         """
         List of answers for a particular workload and lens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_answers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#list_answers)
         """
@@ -589,15 +589,15 @@
         *,
         WorkloadId: str,
         LensArn: str,
         PillarId: str,
         QuestionId: str,
         ChoiceId: str,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListCheckDetailsOutputTypeDef:
         """
         List of Trusted Advisor check details by account related to the workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_check_details)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#list_check_details)
         """
@@ -607,15 +607,15 @@
         *,
         WorkloadId: str,
         LensArn: str,
         PillarId: str,
         QuestionId: str,
         ChoiceId: str,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListCheckSummariesOutputTypeDef:
         """
         List of Trusted Advisor checks summarized for all accounts related to the
         workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_check_summaries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#list_check_summaries)
@@ -626,30 +626,30 @@
         *,
         WorkloadId: str,
         LensAlias: str,
         PillarId: str = ...,
         MilestoneNumber: int = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        QuestionPriority: QuestionPriorityType = ...
+        QuestionPriority: QuestionPriorityType = ...,
     ) -> ListLensReviewImprovementsOutputTypeDef:
         """
         List lens review improvements.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_lens_review_improvements)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#list_lens_review_improvements)
         """
 
     async def list_lens_reviews(
         self,
         *,
         WorkloadId: str,
         MilestoneNumber: int = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListLensReviewsOutputTypeDef:
         """
         List lens reviews for a particular workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_lens_reviews)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#list_lens_reviews)
         """
@@ -657,15 +657,15 @@
     async def list_lens_shares(
         self,
         *,
         LensAlias: str,
         SharedWithPrefix: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Status: ShareStatusType = ...
+        Status: ShareStatusType = ...,
     ) -> ListLensSharesOutputTypeDef:
         """
         List the lens shares associated with the lens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_lens_shares)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#list_lens_shares)
         """
@@ -673,15 +673,15 @@
     async def list_lenses(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         LensType: LensTypeType = ...,
         LensStatus: LensStatusTypeType = ...,
-        LensName: str = ...
+        LensName: str = ...,
     ) -> ListLensesOutputTypeDef:
         """
         List the available lenses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_lenses)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#list_lenses)
         """
@@ -698,15 +698,15 @@
 
     async def list_notifications(
         self,
         *,
         WorkloadId: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        ResourceArn: str = ...
+        ResourceArn: str = ...,
     ) -> ListNotificationsOutputTypeDef:
         """
         List lens notifications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_notifications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#list_notifications)
         """
@@ -724,30 +724,30 @@
     async def list_profile_shares(
         self,
         *,
         ProfileArn: str,
         SharedWithPrefix: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Status: ShareStatusType = ...
+        Status: ShareStatusType = ...,
     ) -> ListProfileSharesOutputTypeDef:
         """
         List profile shares.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_profile_shares)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#list_profile_shares)
         """
 
     async def list_profiles(
         self,
         *,
         ProfileNamePrefix: str = ...,
         ProfileOwnerType: ProfileOwnerTypeType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListProfilesOutputTypeDef:
         """
         List profiles.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#list_profiles)
         """
@@ -755,15 +755,15 @@
     async def list_review_template_answers(
         self,
         *,
         TemplateArn: str,
         LensAlias: str,
         PillarId: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListReviewTemplateAnswersOutputTypeDef:
         """
         List the answers of a review template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_review_template_answers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#list_review_template_answers)
         """
@@ -783,15 +783,15 @@
         *,
         WorkloadNamePrefix: str = ...,
         LensNamePrefix: str = ...,
         ShareResourceType: ShareResourceTypeType = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         ProfileNamePrefix: str = ...,
-        TemplateNamePrefix: str = ...
+        TemplateNamePrefix: str = ...,
     ) -> ListShareInvitationsOutputTypeDef:
         """
         List the share invitations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_share_invitations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#list_share_invitations)
         """
@@ -807,15 +807,15 @@
     async def list_template_shares(
         self,
         *,
         TemplateArn: str,
         SharedWithPrefix: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Status: ShareStatusType = ...
+        Status: ShareStatusType = ...,
     ) -> ListTemplateSharesOutputTypeDef:
         """
         List review template shares.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_template_shares)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#list_template_shares)
         """
@@ -823,15 +823,15 @@
     async def list_workload_shares(
         self,
         *,
         WorkloadId: str,
         SharedWithPrefix: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Status: ShareStatusType = ...
+        Status: ShareStatusType = ...,
     ) -> ListWorkloadSharesOutputTypeDef:
         """
         List the workload shares associated with the workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_workload_shares)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#list_workload_shares)
         """
@@ -868,28 +868,28 @@
         WorkloadId: str,
         LensAlias: str,
         QuestionId: str,
         SelectedChoices: Sequence[str] = ...,
         ChoiceUpdates: Mapping[str, ChoiceUpdateTypeDef] = ...,
         Notes: str = ...,
         IsApplicable: bool = ...,
-        Reason: AnswerReasonType = ...
+        Reason: AnswerReasonType = ...,
     ) -> UpdateAnswerOutputTypeDef:
         """
         Update the answer to a specific question in a workload review.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_answer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#update_answer)
         """
 
     async def update_global_settings(
         self,
         *,
         OrganizationSharingStatus: OrganizationSharingStatusType = ...,
-        DiscoveryIntegrationStatus: DiscoveryIntegrationStatusType = ...
+        DiscoveryIntegrationStatus: DiscoveryIntegrationStatusType = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates whether the Amazon Web Services account is opted into organization
         sharing and discovery integration
         features.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_global_settings)
@@ -898,29 +898,29 @@
 
     async def update_lens_review(
         self,
         *,
         WorkloadId: str,
         LensAlias: str,
         LensNotes: str = ...,
-        PillarNotes: Mapping[str, str] = ...
+        PillarNotes: Mapping[str, str] = ...,
     ) -> UpdateLensReviewOutputTypeDef:
         """
         Update lens review for a particular workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_lens_review)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#update_lens_review)
         """
 
     async def update_profile(
         self,
         *,
         ProfileArn: str,
         ProfileDescription: str = ...,
-        ProfileQuestions: Sequence[ProfileQuestionUpdateTypeDef] = ...
+        ProfileQuestions: Sequence[ProfileQuestionUpdateTypeDef] = ...,
     ) -> UpdateProfileOutputTypeDef:
         """
         Update a profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#update_profile)
         """
@@ -929,15 +929,15 @@
         self,
         *,
         TemplateArn: str,
         TemplateName: str = ...,
         Description: str = ...,
         Notes: str = ...,
         LensesToAssociate: Sequence[str] = ...,
-        LensesToDisassociate: Sequence[str] = ...
+        LensesToDisassociate: Sequence[str] = ...,
     ) -> UpdateReviewTemplateOutputTypeDef:
         """
         Update a review template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_review_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#update_review_template)
         """
@@ -948,30 +948,30 @@
         TemplateArn: str,
         LensAlias: str,
         QuestionId: str,
         SelectedChoices: Sequence[str] = ...,
         ChoiceUpdates: Mapping[str, ChoiceUpdateTypeDef] = ...,
         Notes: str = ...,
         IsApplicable: bool = ...,
-        Reason: AnswerReasonType = ...
+        Reason: AnswerReasonType = ...,
     ) -> UpdateReviewTemplateAnswerOutputTypeDef:
         """
         Update a review template answer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_review_template_answer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#update_review_template_answer)
         """
 
     async def update_review_template_lens_review(
         self,
         *,
         TemplateArn: str,
         LensAlias: str,
         LensNotes: str = ...,
-        PillarNotes: Mapping[str, str] = ...
+        PillarNotes: Mapping[str, str] = ...,
     ) -> UpdateReviewTemplateLensReviewOutputTypeDef:
         """
         Update a lens review associated with a review template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_review_template_lens_review)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#update_review_template_lens_review)
         """
@@ -1001,15 +1001,15 @@
         ReviewOwner: str = ...,
         IsReviewOwnerUpdateAcknowledged: bool = ...,
         IndustryType: str = ...,
         Industry: str = ...,
         Notes: str = ...,
         ImprovementStatus: WorkloadImprovementStatusType = ...,
         DiscoveryConfig: WorkloadDiscoveryConfigTypeDef = ...,
-        Applications: Sequence[str] = ...
+        Applications: Sequence[str] = ...,
     ) -> UpdateWorkloadOutputTypeDef:
         """
         Update an existing workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_workload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#update_workload)
         """
@@ -1036,15 +1036,15 @@
 
     async def upgrade_profile_version(
         self,
         *,
         WorkloadId: str,
         ProfileArn: str,
         MilestoneName: str = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Upgrade a profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.upgrade_profile_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#upgrade_profile_version)
         """
```

### Comparing `types-aiobotocore-wellarchitected-2.9.0/types_aiobotocore_wellarchitected/literals.py` & `types-aiobotocore-wellarchitected-2.9.1/types_aiobotocore_wellarchitected/literals.py`

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
     "AdditionalResourceTypeType",
     "AnswerReasonType",
     "CheckFailureReasonType",
     "CheckProviderType",
     "CheckStatusType",
     "ChoiceReasonType",
@@ -56,15 +55,14 @@
     "WorkloadImprovementStatusType",
     "WellArchitectedServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AdditionalResourceTypeType = Literal["HELPFUL_RESOURCE", "IMPROVEMENT_PLAN"]
 AnswerReasonType = Literal[
     "ARCHITECTURE_CONSTRAINTS", "BUSINESS_PRIORITIES", "NONE", "OTHER", "OUT_OF_SCOPE"
 ]
 CheckFailureReasonType = Literal[
     "ACCESS_DENIED", "ASSUME_ROLE_ERROR", "PREMIUM_SUPPORT_REQUIRED", "UNKNOWN_ERROR"
 ]
```

### Comparing `types-aiobotocore-wellarchitected-2.9.0/types_aiobotocore_wellarchitected/literals.pyi` & `types-aiobotocore-wellarchitected-2.9.1/types_aiobotocore_wellarchitected/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wellarchitected-2.9.0/types_aiobotocore_wellarchitected/type_defs.py` & `types-aiobotocore-wellarchitected-2.9.1/types_aiobotocore_wellarchitected/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ChoiceContentTypeDef",
     "ChoiceAnswerSummaryTypeDef",
     "ChoiceAnswerTypeDef",
     "AssociateLensesInputRequestTypeDef",
     "AssociateProfilesInputRequestTypeDef",
     "BestPracticeTypeDef",
```

### Comparing `types-aiobotocore-wellarchitected-2.9.0/types_aiobotocore_wellarchitected/type_defs.pyi` & `types-aiobotocore-wellarchitected-2.9.1/types_aiobotocore_wellarchitected/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wellarchitected-2.9.0/types_aiobotocore_wellarchitected.egg-info/PKG-INFO` & `types-aiobotocore-wellarchitected-2.9.1/types_aiobotocore_wellarchitected.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-wellarchitected
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.WellArchitected 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.WellArchitected 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/
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
 
 <a id="types-aiobotocore-wellarchitected"></a>
 
 # types-aiobotocore-wellarchitected
 
 [![PyPI - types-aiobotocore-wellarchitected](https://img.shields.io/pypi/v/types-aiobotocore-wellarchitected.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wellarchitected)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-wellarchitected.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wellarchitected)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-wellarchitected)](https://pepy.tech/project/types-aiobotocore-wellarchitected)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WellArchitected 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
+[aiobotocore.WellArchitected 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
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
 [types-aiobotocore-wellarchitected docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-wellarchitected-2.9.0/types_aiobotocore_wellarchitected.egg-info/SOURCES.txt` & `types-aiobotocore-wellarchitected-2.9.1/types_aiobotocore_wellarchitected.egg-info/SOURCES.txt`

 * *Files identical despite different names*

